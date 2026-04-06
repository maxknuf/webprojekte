# Deployment — Mexicotto

## Wann laden
Vor Upload, bei Hosting-Fragen, Performance-Checks, Pre-Launch-Checkliste.

## Hosting
- **Plattform:** Netlify (Static Hosting)
- **Domain:** www.mexicotto.de (eigenständig)
- **Build:** Kein Build-Step — statische HTML-Dateien direkt
- **SSL:** Automatisch via Netlify

## Lokale Entwicklung
- **Server:** Python3 http.server auf Port 8081
- **Befehl:** `cd mexicotto && python3 -m http.server 8081`
- **launch.json:** Eintrag in `.claude/launch.json` für Preview-Tools

## Pre-Upload Checkliste

### Links & Navigation
- [ ] Alle internen Links funktionieren
- [ ] Alle Bilder laden (keine 404)
- [ ] Navigation konsistent auf allen Seiten
- [ ] Mobile Burger-Menü funktioniert
- [ ] Breadcrumbs korrekt

### SEO & Meta
- [ ] Jede Seite: Title-Tag (max 60 Zeichen)
- [ ] Jede Seite: Meta Description (max 155 Zeichen)
- [ ] Jede Seite: Canonical URL
- [ ] Jede Seite: Open Graph Tags
- [ ] Jede Seite: 1 H1
- [ ] Schema.org JSON-LD validiert (schema.org/validator)
- [ ] sitemap.xml enthält alle Seiten
- [ ] robots.txt erlaubt Crawling

### Performance
- [ ] Bilder optimiert (<200KB Hero, <100KB Content)
- [ ] Fonts: font-display: swap
- [ ] Lazy Loading auf allen Bildern außer Hero
- [ ] Kein Render-Blocking JS
- [ ] CSS/JS minifiziert (optional)

### Responsive & Browser
- [ ] Mobile getestet (375px)
- [ ] Tablet getestet (768px)
- [ ] Desktop getestet (1280px)
- [ ] Chrome, Firefox, Safari getestet
- [ ] Touch-Targets mindestens 44×44px

### Rechtliches
- [ ] Impressum vollständig (§5 TMG)
- [ ] Datenschutzerklärung (DSGVO)
- [ ] AGB vorhanden
- [ ] Cookie-Banner falls nötig

## .htaccess (für Apache/Strato-Fallback)
```apache
# HTTPS Redirect
RewriteEngine On
RewriteCond %{HTTPS} !=on
RewriteRule ^(.*)$ https://%{HTTP_HOST}/$1 [R=301,L]

# www Redirect
RewriteCond %{HTTP_HOST} !^www\. [NC]
RewriteRule ^(.*)$ https://www.%{HTTP_HOST}/$1 [R=301,L]

# Security Headers
Header set X-Content-Type-Options "nosniff"
Header set X-Frame-Options "SAMEORIGIN"
Header set Referrer-Policy "strict-origin-when-cross-origin"
Header set X-XSS-Protection "1; mode=block"

# Caching
<IfModule mod_expires.c>
  ExpiresActive On
  ExpiresByType image/jpeg "access plus 1 year"
  ExpiresByType image/png "access plus 1 year"
  ExpiresByType image/svg+xml "access plus 1 year"
  ExpiresByType text/css "access plus 1 month"
  ExpiresByType application/javascript "access plus 1 month"
  ExpiresByType font/ttf "access plus 1 year"
</IfModule>

# Gzip
<IfModule mod_deflate.c>
  AddOutputFilterByType DEFLATE text/html text/css application/javascript image/svg+xml
</IfModule>

# Custom 404
ErrorDocument 404 /mexicotto/404.html
```

## Post-Launch
1. Google Search Console: Property anlegen, sitemap.xml einreichen
2. Google My Business: Eintrag aktualisieren mit neuer Website
3. DNS: Domain auf Netlify zeigen (CNAME/A-Record)
4. SSL-Zertifikat prüfen
5. Alle Seiten in verschiedenen Browsern testen
6. Core Web Vitals prüfen (PageSpeed Insights)
