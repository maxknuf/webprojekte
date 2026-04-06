# Design-System — Mexicotto

## Wann laden
Bei visuellen Änderungen, neuen Komponenten, Layout-Anpassungen, CSS-Arbeit.

## Farbpalette (Hybrid: Dark Hero/Nav/Footer + Light Content)

### Dark-Bereiche (Hero, Nav, Footer)
```css
--bg-dark:      #0C0B09;
--bg-dark-2:    #131210;
--bg-dark-3:    #1A1917;
--text-light:   #F0EAE0;
--text-light-m: #9A9080;
```

### Light-Bereiche (Content-Sektionen)
```css
--bg:           #F5F0EB;   /* Warmes Leinen */
--bg-alt:       #FFFFFF;   /* Karten, Wechsel-Sektionen */
--bg-warm:      #EDE4D8;   /* Sandstein-Highlight */
--text:         #2C2420;   /* Dunkle Erde */
--text-muted:   #7A6E64;   /* Warm-Grau */
--line:         rgba(139,94,60,0.12);
```

### Akzentfarben (überall)
```css
--accent:       #8B5E3C;   /* Terrakotta-Braun */
--accent-light: #A0714F;   /* Hover */
--accent-dark:  #6B4526;   /* Text-Emphasis */
--gold:         #C4A265;   /* Gold für CTAs */
--gold-light:   #D4B87A;   /* Gold Hover */
--stone:        #4A4540;   /* Stein-Grau */
--radius:       6px;       /* Eckiger als italia (8px) — Fliesen-Ästhetik */
```

## Typografie
- **Display:** `'DM Serif Display', serif` — warm, organisch, Material-Charakter
- **Body:** `'DM Sans', sans-serif` — Gewichte 300/400/500
- **Fluid Sizing:**
  - H1: `clamp(2.5rem, 7vw, 4.2rem)`
  - H2: `clamp(2rem, 5vw, 3rem)`
  - H3: `clamp(1.4rem, 3vw, 1.8rem)`
  - Body: `1rem` / Line-height `1.7`
- **Label:** DM Sans, 0.72rem, 500, uppercase, `letter-spacing: 0.18em`, Farbe `--gold`

## Layout
- **Container:** `.wrap` = `min(1300px, calc(100% - 48px))`
- **Sektions-Padding:** `120px 0` (Desktop), `80px 0` (Mobil)
- **Breakpoint:** `900px` (einziger Breakpoint)

## Komponenten

### Basis (adaptiert von italia-strandliegen)
- `.btn` / `.btn.solid` / `.btn.gold` — Button-Varianten
- `.split` / `.split.reverse` — 2-Spalten-Layout
- `.feature-grid` — 3-Spalten Feature-Cards
- `.showcase-grid` — Asymmetrisches 6-Spalten-Grid
- `.product-grid` — `auto-fit` responsive Grid
- `.reveal` / `.visible` — Scroll-Animationen
- `nav` — Sticky, blur-backdrop, mobile burger
- `footer` — Dark-Mode, mehrspaltig

### Neu für Mexicotto
- `.collection-card` — Große Produktkarten mit Bild, Titel, Tags, Preis-Range
- `.spec-table` — Technische Daten (Format, Stärke, Preis/m²)
- `.sample-cta` — Musterpaket-CTA mit `--bg-warm` Hintergrund
- `.gallery-filter` — Filter-Buttons für Referenzen (JS-gesteuert)
- `.page-header` — Bild-Header mit Gradient-Overlay (Dark-Mode)
- `.tile-pattern-bg` — Subtiles CSS-Muster als Sektions-Hintergrund

## Animationen
- **Reveal:** `opacity 0 → 1`, `translateY(32px → 0)`, Dauer `0.75s`
- **Reveal-Delays:** `.reveal-delay-1` bis `.reveal-delay-4` (je +0.1s)
- **Hero:** Ken-Burns `slowMove` Keyframe (scale 1 → 1.08, 20s)
- **Hover:** `transform: scale(1.04)` auf Bilder, `0.4s ease`
- **Buttons:** `background/border/color 0.3s ease`

## Bilder
- Lazy Loading: `loading="lazy"` auf allen Bildern außer Hero
- Format: JPEG für Fotos, SVG für Icons/Logo, PNG nur Favicon
- Hero max 1600px breit, <200KB
- `object-fit: cover` auf allen Bild-Containern

## Responsive (≤900px)
- Nav: Burger-Menü, Full-Screen Mobile-Menu
- Grids: 1 Spalte
- Split: Stack vertikal
- Padding: 80px 0
- Font-Größen reduziert via clamp()
