# LO Rana og Omegn – Nettside

Offisiell nettside for LO Rana og Omegn samorganisasjon.

🌐 **[lo-rana.no](https://lo-rana.no)**

---

## Om nettsiden

Enkeltside-nettside (HTML/CSS/JS) for LO Rana og Omegn, som representerer de lokale fagforeningene i Rana, Hemnes, Nesna og Lurøy.

## Innhold

- Om oss med statistikk
- Våre kjernesaker (ekspanderbare kort)
- Siste nytt fra Facebook (Facebook Page Plugin)
- Nyttige lenker for LO-medlemmer
- Styret med kontaktinformasjon
- Kontaktside med Google Maps
- Footer med navigasjon

## Filer

```
/
├── index.html        # Hele nettsiden
├── assets/           # Bilder og logoer
│   ├── logo_kvadrat_1.png
│   ├── logo_horisontal.png
│   ├── img_event1.jpg
│   ├── img_event2.jpg
│   └── [styrebilder].jpg
├── CNAME             # Domenekobling til lo-rana.no
└── .gitignore
```

## Oppdatere innhold

### Endre tekst eller lenker
Åpne `index.html` i en teksteditor. Seksjoner er merket med kommentarer som `<!-- REDIGER: ... -->`.

### Legge til styrebilde
Legg bildefilen i `assets/`-mappen og oppdater den aktuelle `styre-portrait`-blokken i `index.html`:
```html
<div class="styre-portrait">
  <img src="assets/FILNAVN.jpg" alt="Navn" loading="lazy" />
</div>
```

### Publisere endringer
```bash
git add .
git commit -m "Beskrivelse av endringen"
git push
```

Siden oppdateres automatisk på [lo-rana.no](https://lo-rana.no) innen 1–2 minutter.

## Teknisk

- Ren HTML/CSS/JavaScript – ingen rammeverk eller byggeprosess
- Hostet på GitHub Pages
- Domene: `lo-rana.no` (DNS via Telenor)
- Font: Open Sans (Google Fonts)
- Facebook Page Plugin for automatisk nyhetsfeed

## Kontakt

**LO Rana og Omegn**  
Søndre gate 13, 8624 Mo i Rana  
lo-rana@lo-rana.no
