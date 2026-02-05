# Portfolio - One Pager

Ein modernes, responsives One-Pager Portfolio mit Tailwind CSS, Dark Mode & GitHub Pages ready.

## 🚀 Features

- ✨ **Dark Mode mit Toggle** - Eleganter Dark/Light Wechsel
- 📱 **Mobile First Design** - Perfekt auf allen Screens (2–6 Spalten Grid für Skills)
- 🎨 **Moderne Ästhetik** - Gradient, Shadows, Hover Effects
- ⚡ **Performance Optimiert** - Keine Frameworks, nur reines CSS/HTML/JS
- 🔍 **SEO Ready** - Meta Tags, semantisches HTML
- 🌐 **GitHub Pages Ready** - Direkt deploybar
- ♿ **Accessible** - ARIA Labels, Focus States
- 📦 **Tailwind CSS** - Utility-First CSS Framework

## 📂 Projektstruktur

```
portfolio/
├── index.html             # Komplette One-Pager Seite
├── package.json           # Dependencies
├── tailwind.config.js     # Tailwind Config (mit Dark Mode)
├── .gitignore
├── src/
│   └── input.css         # Custom CSS & Tailwind Directives
├── dist/
│   └── styles.css        # Kompilierte CSS (Auto-generated)
├── assets/
│   ├── images/           # Dein Profilbild (1:1 Format → rund)
│   └── fonts/            # Custom Fonts (optional)
└── README.md
```

## 🎯 Design-Highlights

### Responsive Grid für Skills
```
📱 Mobile:  2 Spalten
📊 Tablet:  3 Spalten (sm:)
💻 Desktop: 4-6 Spalten (md: lg:)
```

### Dark Mode Toggle
Kostenlos im Navbar:
- Automatisches Speichern (localStorage)
- Smooth Transitions
- System-Einstellung Fallback

### Profilbild
- 1:1 Format mit `rounded-full` für Kreis-Form
- Ort: `./assets/images/profile.jpg`
- Größen: Mobile 256px → Desktop 320px

## 📦 Installation & Setup

### 1. Dependencies installieren
```bash
npm install
```

### 2. Development Server
```bash
npm run dev
```
Die CSS wird im Watch-Modus kompiliert und aktualisiert sich automatisch.

### 3. Production Build
```bash
npm run build
```
Minifizierte CSS wird in `/dist` generiert.

### 4. Lokal testen
```bash
npm run preview
```
Öffnet die Seite auf `http://localhost:8000`

## 🌐 GitHub Pages Deployment

### Schritt 1: Profilbild einfügen
Speichere dein 1:1 Bild unter:
```
assets/images/profile.jpg
```

### Schritt 2: CSS kompilieren
```bash
npm run build
```

### Schritt 3: GitHub Setup
1. Repository Settings → **Pages**
2. Wähle: **Deploy from a branch**
3. Branch: `main` / Folder: `/ (root)`
4. Die `index.html` wird automatisch erkannt

### Schritt 4: Custom Domain (optional)
In Settings → Pages → Custom domain eintragen

## ✏️ Inhalte anpassen

### Name & Bio
In `index.html` suchen:
- `"Dein Name"` → Dein echter Name
- `"Dein Name"` im Footer

### Farben
In `tailwind.config.js`:
```javascript
colors: {
  primary: '#DEINE_HEX',
  secondary: '#DEINE_HEX',
}
```

### Kontakt & Social Links
In `index.html` Hero und Contact Section:
```html
<a href="mailto:DEINE_EMAIL">
<a href="GITHUB_URL">
<a href="LINKEDIN_URL">
...
```

### Skills hinzufügen/ändern
Im HTML `<section id="skills">`:
- SVG Icons austauschen
- Kategorien umbenennen
- Neue Tools hinzufügen

## 📱 Responsive Breakpoints

| Device | Breakpoint | Grid Skills |
|--------|-----------|---------|
| Mobile | 0-640px | 2 Spalten |
| Tablet | 640px+ (sm:) | 3 Spalten |
| Laptop | 768px+ (md:) | 4 Spalten |
| Desktop | 1024px+ (lg:) | 6 Spalten |

## 🎨 Dark Mode Technik

```javascript
// Automatischer Toggle
<button onclick="toggleDarkMode()">
  <!-- Icon wechselt je nach Mode -->
</button>

// Gespeichert in localStorage
```

CSS mit Dark Mode Utilities:
```html
<div class="bg-white dark:bg-slate-900">
  <!-- Dark Variante wird automatisch applied -->
</div>
```

## 🔧 Kustomisierung Beispiele

### Andere Farben für Hero
```html
<!-- In: section class="...from-blue-50...to-purple-50..." -->
from-green-50 to-emerald-50
```

### Social Icons in Footer entfernen
```html
<!-- Die ganze <div class="flex justify-center gap-4..."> entfernen -->
```

### Sticky Navigation entfernen
```css
<!-- In <nav> die Klasse "sticky top-0" entfernen -->
```

## 📊 Build & Performance

- **HTML**: 1 Datei, ~8KB
- **CSS**: ~15KB (unkomprimiert) → ~3KB (gquipped + minified)
- **JS**: ~0.5KB (nur Dark Mode Toggle)
- **Total**: ~20KB (komprimiert)

Geladen in **<500ms** auch auf langsamen Verbindungen ✨

## 🚀 Weitere Tipps

1. **Favicon hinzufügen**
   ```html
   <link rel="icon" href="/favicon.ico">
   ```

2. **Google Analytics**
   ```html
   <!-- Am Ende vor </body> -->
   <script async src="https://www.googletagmanager.com/gtag/js?id=..."></script>
   ```

3. **Open Graph für Social Sharing**
   ```html
   <meta property="og:image" content="/assets/images/profile.jpg">
   ```

## 📝 Lizenz

MIT

---

**Viel Erfolg beim Portfolio! 🎉**

Fragen? Brauchst du Anpassungen? Lass es mich wissen!
