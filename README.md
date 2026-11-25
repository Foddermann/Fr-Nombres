# Nombres FR – iPhone-Zahlentrainer

## Installation über GitHub Pages

1. Neues GitHub-Repository anlegen, z. B. `nombres-fr`.
2. Alle Dateien aus diesem Ordner in den Root des Repositories hochladen.
3. **Settings → Pages → Build and deployment**.
4. **Deploy from a branch**, Branch **main**, Ordner **/(root)** wählen und speichern.
5. Die angezeigte `github.io`-Adresse in Safari auf dem iPhone öffnen.
6. **Teilen → Zum Home-Bildschirm**.
7. Die App einmal online öffnen. Danach steht der App-Shell über den Service Worker auch offline bereit.

## Dateien

- `index.html` – komplette App (HTML/CSS/JavaScript)
- `manifest.webmanifest` – PWA-Metadaten
- `sw.js` – Offline-Cache
- `apple-touch-icon.png` – iPhone-Homescreen-Icon (180×180)
- `icon-192.png`, `icon-512.png` – PWA-Icons

## Datenschutz

Trainingsfortschritt wird per `localStorage` lokal im Browser gespeichert. Export/Import ist in der App integriert.

## Version 1.1 – Qualitätskorrektur

- Multiple-Choice-Generator garantiert vier eindeutige Optionen mit genau einer richtigen Antwort.
- Französische Telefonnummern sprechen führende Nullen korrekt mit (z. B. 06 → zéro six).
- Integrierte Inhaltsprüfung validiert alle Aufgaben und erzeugte Auswahloptionen beim Start.
- Neuer Service-Worker-Cache `nombres-fr-v1.1.0`, damit Updates nach GitHub-Upload sauber übernommen werden.

## Update einer bestehenden GitHub-Pages-Installation

Beim Ersetzen einer älteren Version bitte **index.html und sw.js gemeinsam** hochladen. Danach die GitHub-Pages-URL einmal in Safari öffnen und neu laden. Der Service Worker verwendet in Version 1.1 einen neuen Cache-Namen, sodass die alte App-Shell verworfen wird.
