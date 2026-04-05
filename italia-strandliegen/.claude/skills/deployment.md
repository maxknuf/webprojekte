# Deployment — Italia Strandliegen

## Hosting: Strato
- Statische HTML-Seite, kein Build-Step nötig
- Domain: italia-strandliegen.de (bereits bei Strato)

## Vor dem Upload prüfen
1. Alle internen Links funktionieren (keine toten Links)
2. Alle Bilder laden (keine 404er)
3. Mobile Ansicht getestet
4. Schema.org valide (Google Rich Results Test)
5. sitemap.xml und robots.txt aktuell

## .htaccess (wichtig für Strato)
- HTTPS-Redirect
- Security Headers (X-Frame-Options, X-Content-Type-Options)
- Caching für Bilder/CSS/JS (1 Jahr)
- Gzip-Komprimierung
- Custom 404-Seite
- www-Redirect (mit oder ohne www konsistent)

## Upload-Prozess
1. Per FTP/SFTP auf Strato-Webspace
2. Alle Dateien in Root des Webspace
3. SSL-Zertifikat aktiv? Prüfen
4. Nach Upload: alle Seiten im Browser testen
5. Google Search Console: Sitemap einreichen

## Nach dem Launch
- Google Search Console einrichten
- Sitemap einreichen
- Google My Business aktualisieren (falls vorhanden)
