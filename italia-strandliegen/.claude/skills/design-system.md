# Design-System — Italia Strandliegen

## Wann laden
Bei jeder neuen Seite, Komponente oder visuellen Änderung.

## Farbschema (hell/mediterran)
```
--bg: #F9F7F3           Sandfarbig (Hintergrund)
--bg-alt: #FFFFFF       Weiß (Karten, alternierend)
--accent: #2C5F7A       Mittelmeer-Blau (Primary)
--accent-light: #3A7A9B Helles Blau (Hover)
--accent-dim: #D7A768   Sonnengold (Akzente, CTAs)
--text: #2D3748         Dunkelgrau (Text)
--text-muted: #718096   Gedämpft (Subtext)
--line: rgba(44,95,122,0.15)  Trennlinien
```

## Typografie
- **Display:** `'Cinzel', serif` — Headlines, Logo, Navigation. Uppercase + letter-spacing: 0.05-0.15em
- **Body:** `'Outfit', sans-serif` — Fließtext, Buttons, UI. Weights: 200-600
- **Fluid:** `clamp()` für alle Schriftgrößen. H1: clamp(2.5rem, 8vw, 4.5rem)

## Komponenten
- **`.wrap`**: `width: min(1300px, calc(100% - 48px)); margin: 0 auto;`
- **`.btn`**: Outline-Style, uppercase Cinzel, hover → filled. `.btn.solid` für Primary-CTA
- **`.split`**: 2-Spalten-Grid mit 80px gap, collapst bei 900px
- **`.drink-card`** (→ umbenennen zu `.feature-card`): Weiße Box, Border, Hover-Lift
- **`.showcase-grid`**: 6-Spalten asymmetrisches Galerie-Grid
- **`nav`**: Fixed, blur-backdrop bei scroll, Logo links, Links rechts
- **`section`**: padding: 120px 0 (80px mobile)

## Responsive Breakpoints
- **Desktop:** > 900px — Volle Grid-Layouts
- **Mobile:** <= 900px — Single-Column, Nav-Links hidden (Burger), section padding 80px

## Animationen
- Ken-Burns Hero (40s infinite)
- Hover-Lifts: translateY(-5px) + box-shadow
- Smooth scroll behavior
- Transition: 0.4s cubic-bezier(0.16, 1, 0.3, 1)

## Regeln
- Kein Dark Mode
- Alle Bilder: `loading="lazy"` außer Hero
- Bilder: object-fit: cover, border-radius: 8px
- Maximale Bildbreite in `assets/images/` speichern
- SVG für Icons und Logo
- Keine externen CSS-Frameworks
