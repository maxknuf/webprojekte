# Projekt-Regeln — Mexicotto

## Wann laden
Bei Fragen zu Business-Kontext, Produkten, Preisen, Konventionen, Dateistruktur.

## Unternehmen
- **Firma:** ATB IMPORT (Fliesen-Import & Beratung)
- **Inhaber:** Tom Bölsterl
- **Partner:** Ofenbau Hogger (Bastian Hogger) — Montage & Verlegung
- **Adresse:** Greimelstr. 1, 83236 Übersee
- **Telefon:** +49 176 30368575
- **E-Mail:** info@mexicotto.de
- **Domain:** www.mexicotto.de
- **Branche:** Fliesen-Import, Beratung, Planung, Verkauf, Montage

## USP-Kommunikation
1. **Exklusivvertrieb Verde 1999** — Premium-Feinsteinzeug nicht überall erhältlich
2. **Alles aus einer Hand** — Beratung · Planung · Verkauf · Montage
3. **Handgefertigte Terrakotta** — Mexicotto Cotto, echtes italienisches Handwerk
4. **Persönliche Beratung** — Kleines Unternehmen, direkter Inhaberkontakt
5. **Bundesweiter Versand** — Lieferung deutschlandweit inklusive

## Produkte

### Mexicotto Cotto (Terrakotta)
- Handgefertigt, gebrannte Erde
- Format: ca. 29×29 cm
- Varianten: Cotto Regular 1–4, Cotto Antik
- Eigenschaften: atmungsaktiv, feuchtigkeitsregulierend, natürlich schadstoffrei
- **Musterpaket:** 3 Fliesen + Lithofin-Behandlung für 10€
- Pflege: Lithofin Imprägnierung empfohlen

### Feinsteinzeug (Verde 1999 / Campogalliano)
- **19 Kollektionen:** Dakota, Jurassic, Archaios, Panarea, I Marmi, Aquarius, Livingstone, Cosmopolitan, Stone Instinct, Lapis, Tufo, Aloft, Glassalike, Centuries, Matrix, Elementi, Retro, Artwood, Checkerboard
- Formate: 30×60, 40×60, 60×60, 90×90, 100×100, 60×120 cm
- Stärke: 1 cm (Innen), 2 cm (Outdoor), rektifiziert
- Oberflächen: Matt (Naturale) und Poliert (Lev)
- **Preis:** 38–48 €/m² zzgl. MwSt., Mindestbestellung 15 m²
- Naturstein-Optik (Marmor, Schiefer, Travertin, Kalkstein, Sandstein, Tuff)
- I Marmi: Statuario, Calacatta Oro, Carrara — Matt + Lev, inkl. Mosaik/Chevron-Dekore
- **UST-IdNr:** DE 163179614
- **PDF-Kataloge:** 19 Stück in assets/pdfs/ verfügbar

### Solnhofener Imitat
- Feinsteinzeug in Solnhofener Naturstein-Optik
- Günstiger als echter Solnhofener, gleiche Ästhetik
- Robuster und pflegeleichter

### Outdoor / 2cm
- Feinsteinzeug 2 cm Stärke
- Für Terrassen, Balkone, Außenbereiche
- Frostbeständig, rutschfest

## Datei-Konventionen
- **Seiten:** Flat im Root-Ordner (`mexicotto-cotto.html`, nicht `produkte/cotto.html`)
- **Bilder:** `assets/images/[kategorie]/[beschreibender-name].jpg`
  - Kategorien: hero, collections/cotto, collections/feinsteinzeug, collections/solnhofener, collections/outdoor, gallery, textures, icons, og
- **CSS:** Einzige Datei `css/style.css`
- **JS:** Einzige Datei `js/main.js`
- **Fonts:** Self-hosted in `assets/fonts/`

## Content-Regeln
- **Sprache:** Deutsch
- **Anrede:** Formell-freundlich (Sie-Form)
- **Preise:** Nur echte Preise angeben (38–48€/m² Feinsteinzeug, 10€ Musterpaket)
- **Unbekannte Preise:** "auf Anfrage" verwenden
- **Bilder:** AI-Platzhalter zunächst, beschreibende Dateinamen für späteren Austausch
- **Keine Übertreibungen:** Faktenbasiert, Qualität spricht für sich

## Tech-Stack
- Pure HTML5 / CSS3 / Vanilla JS
- Keine Frameworks, kein Build-Step
- Self-hosted Fonts (DM Serif Display + DM Sans)
- CSS Custom Properties für Design-System
- IntersectionObserver für Scroll-Reveal
- `loading="lazy"` für Bilder
- Schema.org JSON-LD für SEO
- Netlify Static Hosting
