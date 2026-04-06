# Mexicotto — Premium-Website für ATB IMPORT

## Projekt
- **Domain:** www.mexicotto.de
- **Firma:** ATB IMPORT (Tom Bölsterl) + Ofenbau Hogger (Bastian Hogger)
- **Hosting:** Netlify (static) / eigenständige Domain
- **Fonts:** DM Serif Display (Display) + DM Sans (Body) — self-hosted in `assets/fonts/`
- **Stack:** Pure HTML5 · CSS3 · Vanilla JS — kein Framework, kein Build-Step

## Dateistruktur
```
mexicotto/
├── css/style.css          # Einzige CSS-Datei
├── css/fonts.css          # Font-Deklarationen
├── js/main.js             # Einzige JS-Datei
├── assets/images/         # Bilder nach Kategorie sortiert
├── assets/logo/           # Logo + Favicon
└── assets/fonts/          # TTF-Dateien
```

## Skills (bedarfsgesteuert laden)

| Skill | Datei | Wann laden |
|-------|-------|------------|
| Design-System | `.claude/skills/design-system.md` | Bei visuellen Änderungen, neuen Komponenten, CSS-Anpassungen |
| SEO & Marketing | `.claude/skills/seo-marketing.md` | Bei neuen Seiten, Content-Erstellung, Meta-Tags, Schema.org |
| Projekt-Regeln | `.claude/skills/project-rules.md` | Bei Fragen zu Business-Kontext, Preisen, Produkten, Konventionen |
| Deployment | `.claude/skills/deployment.md` | Vor Upload, bei Hosting-Fragen, Performance-Checks |

## Regeln
- Sprache: Deutsch, formell-freundlich (Sie-Form)
- Jede Seite: genau 1 H1 mit Keyword, mindestens 1 CTA, Schema.org-Markup
- Bilder: Lazy Loading (`loading="lazy"`), Alt-Tags, in `/assets/images/[kategorie]/`
- Design: Hybrid — dunkler Hero/Nav/Footer, helle Content-Sektionen
- Keine Preise ohne Quelle — "auf Anfrage" wenn unklar
