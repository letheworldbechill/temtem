# ⏱️ FokusPause - Bildschirmzeit Manager

Eine elegante Progressive Web App (PWA) zur Verwaltung deiner Bildschirmzeit mit automatischem Timer und Sperrbildschirm.

## ✨ Features

- 🚀 **Automatischer Timer-Start** - Startet automatisch wenn du den Tab öffnest
- ⏰ **Anpassbare Zeiten** - Arbeitszeit (1-480 Min) und Pausenzeit (1-60 Min)
- 🔒 **Vollbild-Sperrbildschirm** - Visueller Block nach Ablauf der Arbeitszeit
- 🔔 **Benachrichtigungen** - Sound, Vibration und Desktop-Notifications
- 📱 **Installierbar** - Als App auf Handy/Desktop installierbar (PWA)
- 💾 **Offline-fähig** - Funktioniert auch ohne Internetverbindung
- 🌙 **Dark Mode** - Schonend für die Augen
- 📏 **Responsive** - Perfekt auf Mobile und Desktop

## 🚀 GitHub Pages Hosting

### Schnell-Anleitung (2 Minuten)

1. **Repository erstellen**
   - Gehe zu [github.com/new](https://github.com/new)
   - Name: z.B. `fokuspause` oder `screen-timer`
   - ✅ "Add a README file" NICHT ankreuzen
   - Klicke "Create repository"

2. **Dateien hochladen**
   - Klicke "uploading an existing file"
   - Ziehe ALLE Dateien aus diesem Ordner hinein:
     - `index.html`
     - `manifest.json`
     - `sw.js`
     - `.nojekyll`
     - `icon-192.png`
     - `icon-512.png`
   - Commit message: "Initial commit"
   - Klicke "Commit changes"

3. **GitHub Pages aktivieren**
   - Gehe zu **Settings** → **Pages** (linke Sidebar)
   - Source: **Deploy from a branch**
   - Branch: **main** / **/ (root)**
   - Klicke **Save**

4. **Fertig!** 🎉
   - Warte 1-2 Minuten
   - Deine App ist live unter: `https://DEIN-USERNAME.github.io/REPO-NAME/`

### Alternative: Git Command Line

```bash
# Repository klonen (ersetze URL mit deiner)
git clone https://github.com/DEIN-USERNAME/fokuspause.git
cd fokuspause

# Dateien kopieren
cp -r /pfad/zu/diesen/dateien/* .

# Pushen
git add .
git commit -m "Add FokusPause app"
git push origin main

# Dann GitHub Pages in Settings aktivieren
```

## 📱 Als App installieren

### Android
1. Öffne die Seite in Chrome
2. Tippe auf "Zum Startbildschirm hinzufügen" oder das Install-Banner

### iOS
1. Öffne die Seite in Safari
2. Tippe auf Teilen → "Zum Home-Bildschirm"

### Desktop (Chrome/Edge)
1. Klicke auf das Install-Symbol in der Adressleiste
2. Oder: Menü → "FokusPause installieren"

## ⚙️ Einstellungen

| Option | Standard | Beschreibung |
|--------|----------|--------------|
| Arbeitszeit | 90 Min | Zeit bis zur Pause |
| Pausenzeit | 10 Min | Dauer des Sperrbildschirms |
| Auto-Start | ✅ An | Timer startet bei Tab-Fokus |
| Sound | ✅ An | Akustische Benachrichtigung |

## 🔓 Notfall-Entsperrung

Falls du den Sperrbildschirm vorzeitig verlassen musst:
- **3× schnell auf "Notfall-Entsperrung" tippen**

## 📁 Dateien

```
fokuspause/
├── index.html      # Haupt-App (alles in einer Datei)
├── manifest.json   # PWA-Konfiguration
├── sw.js          # Service Worker für Offline-Support
├── .nojekyll      # GitHub Pages Konfiguration
├── icon-192.png   # App-Icon klein
├── icon-512.png   # App-Icon groß
└── README.md      # Diese Datei
```

## 🛠️ Technologien

- Vanilla HTML/CSS/JavaScript (keine Dependencies!)
- Progressive Web App (PWA)
- Service Worker für Offline-Nutzung
- Page Visibility API
- Web Notifications API
- Wake Lock API
- LocalStorage

## ⚠️ Hinweis

Web-Apps können den Bildschirm nicht wirklich sperren (OS-Einschränkung). Die App zeigt einen Vollbild-Overlay im Browser. Für echte Systemsperren wäre eine native App nötig.

## 📄 Lizenz

MIT License - Frei verwendbar!

---

Made with ☕ für bessere Bildschirmzeit-Balance
