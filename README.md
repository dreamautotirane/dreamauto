# Dream Auto Tirane

Një faqe statike e lehtë për një shitës automjetesh, e projektuar për deployim në Cloudflare Pages pa hap build.

## Struktura

- index.html — faqja kryesore me hero, automjete të preferuara, informacion rreth dhe CTA për kontakt
- inventory.html — rrjet për lista automjetesh me karta placeholder
- contact.html — markup për formë kontakti me validim në klient
- about.html — faqe informacioni për shitësin
- css/style.css — stilizim mobile-first me variabla CSS dhe layout të përgjegjshëm
- js/main.js — toggle për navigacionin në telefon dhe validim bazë të formularit
- images/ — dosje boshe për fotografi të ardhshme

Note: një logo SVG është vendosur si `image.jpeg` për paraqitje të menjëhershme.
Nëse preferoni versionin që dërguat (PNG/JPG), vendosni atë si `images/logo.svg` dhe ndryshoni emrin ose zëvendësoni `images/logo.svg`.

## Pamja lokale

Hap çdo faqe direkt në browser, ose shërbeje folderin me një server statik të thjeshtë:

```bash
cd /path/to/dreamauto
python3 -m http.server 8000
```

Më pas vizito http://localhost:8000.

## Deployimi në Cloudflare Pages

1. Shto këtë folder në një repository GitHub.
2. Në Cloudflare Pages, krijo një projekt të ri dhe lidh repository.
3. Vendos direktorinë e output-it të build-it si rrënja e repository.
4. Nuk kërkohet komandë build.
5. Deployo projektin.

Faqja është plotësisht statike dhe punon pa framework apo pipeline build.
