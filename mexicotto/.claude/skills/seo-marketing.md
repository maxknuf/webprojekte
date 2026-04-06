# SEO & Marketing — Mexicotto

## Wann laden
Bei neuen Seiten, Content-Erstellung, Meta-Tags, Schema.org-Markup, Conversion-Optimierung.

## Keyword-Strategie

### Primär (hohes Suchvolumen)
- Mexicotto Fliesen
- Terrakotta Fliesen kaufen
- Feinsteinzeug Natursteinoptik
- Cotto Fliesen handgefertigt
- Cotto Bodenfliesen

### Sekundär
- Verde 1999 Feinsteinzeug
- Solnhofener Naturstein Imitat
- Outdoor Feinsteinzeug 2cm
- Terrassenplatten Feinsteinzeug
- Italienische Fliesen Deutschland

### Long-Tail
- handgefertigte italienische Terrakotta Fliesen kaufen
- Feinsteinzeug Natursteinoptik Großformat kaufen
- Musterpaket Cotto Fliesen bestellen
- Cotto Fliesen Pflege und Imprägnierung
- Solnhofener Platten Alternative Feinsteinzeug

### Lokal
- Fliesen Übersee
- Fliesen Chiemsee
- Fliesenleger Bayern
- Fliesen kaufen Rosenheim

## Meta-Tag Template
```html
<title>[Keyword] | Mexicotto — Fliesen & Naturstein</title>
<meta name="description" content="[155 Zeichen max, Keyword vorne, CTA am Ende]" />
<link rel="canonical" href="https://www.mexicotto.de/[seite].html" />
```

## Open Graph Template
```html
<meta property="og:title" content="[Seitentitel]" />
<meta property="og:description" content="[Kurzbeschreibung]" />
<meta property="og:type" content="website" />
<meta property="og:url" content="https://www.mexicotto.de/[seite].html" />
<meta property="og:image" content="https://www.mexicotto.de/assets/images/og/[seite].jpg" />
<meta property="og:locale" content="de_DE" />
<meta property="og:site_name" content="Mexicotto" />
```

## Schema.org

### LocalBusiness (Homepage, Über uns)
```json
{
  "@context": "https://schema.org",
  "@type": "LocalBusiness",
  "name": "Mexicotto — ATB IMPORT",
  "description": "Exklusive italienische Fliesen: Cotto, Feinsteinzeug, Naturstein",
  "url": "https://www.mexicotto.de",
  "telephone": "+49-176-30368575",
  "email": "info@mexicotto.de",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "Greimelstr. 1",
    "addressLocality": "Übersee",
    "postalCode": "83236",
    "addressCountry": "DE"
  },
  "areaServed": "DE",
  "priceRange": "€€-€€€"
}
```

### Product + Offer (Produktseiten)
```json
{
  "@type": "Product",
  "name": "[Produktname]",
  "description": "[Beschreibung]",
  "brand": { "@type": "Brand", "name": "Mexicotto" },
  "offers": {
    "@type": "Offer",
    "priceCurrency": "EUR",
    "price": "[Preis]",
    "priceValidUntil": "[Datum]",
    "availability": "https://schema.org/InStock"
  }
}
```

### Weitere Schema-Typen
- **BreadcrumbList** — Alle Unterseiten
- **FAQPage** — Pflege-Seite, Produktseiten mit FAQ
- **ImageGallery** — Referenzen-Seite

## Conversion-Regeln
- **Jede Seite:** mindestens 1 CTA (Beratung anfragen / Musterpaket bestellen)
- **Musterpaket (10€):** Low-Barrier-Entry, prominent auf Cotto-Seite + Homepage
- **Telefonnummer:** Immer sichtbar in Nav (klickbar auf Mobil: `tel:+498642...`)
- **Trust-Signals:** "Exklusivvertrieb Verde 1999", "Beratung · Planung · Verkauf · Montage"
- **Kontakt-Teaser:** Auf jeder Seite vor dem Footer

## Technisches SEO
- Alt-Tags auf allen Bildern (beschreibend, Keyword wenn passend)
- Interne Verlinkung zwischen verwandten Seiten
- 1 H1 pro Seite mit primärem Keyword
- URL-Struktur: `mexicotto-cotto.html`, `feinsteinzeug.html` (sprechend, flach)
- `sitemap.xml` mit allen Seiten
- `robots.txt` erlaubt Crawling
- Canonical-URLs auf jeder Seite
- Breadcrumb-Navigation auf Unterseiten
