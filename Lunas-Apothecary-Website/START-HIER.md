# Luna’s Apothecary – Website veröffentlichen

## 1. Eigenes Website-Repository

Erstelle ein neues **öffentliches** GitHub-Repository, zum Beispiel `Lunas-Apothecary-Website`, mit Branch `main`. Nutze ein eigenes Repository nur für diese Website, damit weder dein App-Quellcode noch deine Schnellen-Website betroffen sind.

## 2. Dateien hochladen

Entpacke das ZIP. Lade die Website-Dateien und den Ordner `assets` über **Code → Add file → Upload files** hoch. Du darfst auch den kompletten entpackten Ordner hochladen: Die Veröffentlichung findet ihn automatisch. Wichtig: `luna-site.json` muss neben `index.html` liegen. Lade die Website nur einmal hoch.

## 3. Veröffentlichung einrichten

Der versteckte Ordner `.github` wird beim Hochladen manchmal ausgelassen. Deshalb gibt es eine sichtbare Kopie des vollständigen Workflows: `GITHUB-PAGES.yml`.

- Öffne im Repository **Code → Add file → Create new file**.
- Gib exakt `.github/workflows/pages.yml` als Dateinamen ein. Dieser Pfad muss im Hauptverzeichnis des Repositorys liegen.
- Kopiere den gesamten Inhalt von `GITHUB-PAGES.yml` in die neue Datei.
- Speichere mit **Commit changes** direkt auf `main`.
- Falls `.github/workflows/pages.yml` bereits im Hauptverzeichnis existiert, ist dieser Schritt erledigt.
- Wähle **Settings → Pages → Source → GitHub Actions**.
- Öffne **Actions → Publish Lunas Apothecary website → Run workflow**.

Nach einem grünen Lauf findest du den echten Website-Link unter **Settings → Pages**. Ab dann veröffentlichen Änderungen auf `main` die Website automatisch neu.

Es wird kein zusätzliches `prepare-site.py` benötigt. Der Workflow enthält alle Schritte und findet die Website sowohl im Hauptverzeichnis als auch in einem Unterordner. Nur HTML, CSS, Bilder und erzeugte SEO-Dateien werden veröffentlicht.

## Vorschau ohne Veröffentlichung

Öffne `index.html` direkt im Browser. Die Website benötigt kein JavaScript und keine Installation.

## Google

Bei Veröffentlichung werden die tatsächliche Website-Adresse, Canonical-Tags, `sitemap.xml` und `robots.txt` automatisch ergänzt. Reiche die fertige Sitemap bei Bedarf in Google Search Console ein. Veröffentlichung bedeutet nicht sofortige Google-Indexierung und garantiert keine Platzierung. Bei einem GitHub-Projekt-Unterpfad wird dessen robots.txt nicht als domainweite Richtlinie verwendet; die Sitemap kann trotzdem direkt eingereicht werden.

## Inhalt und Pflege

- Texte: `index.html`
- Farben und Layout: `styles.css`
- Website-Datenschutz: `datenschutz.html`
- Originalbilder: `assets/`
- `luna-site.json`: Erkennungsdatei für die Veröffentlichung, bitte mit hochladen.

Die Website ist deutsch. Das Spiel ist laut App Store Englisch und für iPhone ab iOS 18.6. Stand: 27. September 2026, App-Version 1.0.

Support-Adresse und Name stammen aus deinen öffentlichen App-/Support-Angaben. Es wurde keine Anschrift erfunden. Die Website-Datenschutzseite beschreibt die Umsetzung und verlinkt deine bestehende App-Datenschutzerklärung; individuelle rechtliche Betreiberangaben und Datenschutzerklärung bitte vor öffentlichem Einsatz prüfen und bei Bedarf ergänzen. Keine juristische Vollständigkeitsprüfung.

## Quellen

- https://apps.apple.com/de/app/lunas-apothecary/id6802070602
- https://itunes.apple.com/lookup?id=6802070602&country=de
- https://github.com/Jillri/LunasApothecary-Privacy
- https://github.com/Jillri/LunasApothecary-Support
- https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages

Icon und Screenshots sind Originale des App-Store-Eintrags und werden lokal mitgeliefert. Für die Website der App-Inhaberin übernommen, keine separate Lizenz zur Nutzung in fremden Projekten. Keine externen Schriftarten, keine Tracking-Dienste, keine kostenpflichtigen Laufzeitabhängigkeiten.
