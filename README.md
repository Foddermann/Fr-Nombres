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
