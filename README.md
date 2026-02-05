# Portfolio - One Pager

Ein einfaches, modernes One-Pager Portfolio mit Tailwind CSS für GitHub Pages.

## 🚀 Features

- Clean und modernes Design
- Responsive Layout (Mobile-first)
- Tailwind CSS für schnelle Entwicklung
- Build-Prozess für Produktion
- GitHub Pages ready

## 📂 Projektstruktur

```
portfolio/
├── index.html           # Hauptseite
├── package.json         # Dependencies und Scripts
├── tailwind.config.js   # Tailwind Konfiguration
├── .gitignore          # Git Ignorieren
├── src/
│   └── input.css       # Tailwind CSS Input
├── dist/
│   └── styles.css      # Kompilierte CSS (Auto-generated)
└── assets/             # Bilder, Icons, etc.
    ├── images/
    └── fonts/
```

## 📦 Installation

1. Dependencies installieren:
```bash
npm install
```

2. Development-Server starten:
```bash
npm run dev
```

Die CSS wird automatisch kompiliert und bei Änderungen neu generiert.

3. CSS für Production minifizieren:
```bash
npm run build
```

## 🌐 GitHub Pages Deployment

### Option 1: Aus dem `/dist` Ordner deployen

1. Stelle sicher, dass `npm run build` erfolgreich lief
2. In GitHub Repository Settings gehe zu "Pages"
3. Wähle "Deploy from a branch"
4. Wähle Branch und setze den Folder auf `/dist`

### Option 2: Aus dem Root deployen
1. Verschiebe `dist/styles.css` zum Root und aktualisiere `index.html`
2. Setze Pages auf `/root` (Standard)

## ⚙️ Kustomisierung

### Farben & Design
Bearbeite `tailwind.config.js`:
```javascript
theme: {
  extend: {
    colors: {
      primary: '#0047AB',
      secondary: '#FF6B6B',
    }
  }
}
```

### Inhalte
Bearbeite `index.html` direkt - alle Standardelemente sind vorbereitet.

## 📄 Lizenz

MIT

---

**Viel Spaß beim Erstellen deines Portfolios! 🎉**
