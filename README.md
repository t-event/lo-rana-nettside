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
├── index.html                    # Hele nettsiden
├── robots.txt                    # Tillater indeksering fra søkemotorer og sosiale medier
├── assets/                       # Bilder og logoer
│   ├── logo_kvadrat_1.png
│   ├── logo_horisontal.png
│   ├── img_event1.jpg
│   ├── img_event2.jpg
│   ├── Børge Masterdalshei.jpg
│   ├── Konrad Feyling Gruber.jpg
│   ├── Mathias Tustervatn.jpg
│   ├── Morten Lage Jacobsen.jpg
│   ├── Remi.jpg
│   └── Roger Ranfjordnes.jpg
├── CNAME                         # Domenekobling til lo-rana.no
└── .gitignore
```

## Oppdatere innhold

### Endre tekst eller lenker
Åpne `index.html` i en teksteditor. Seksjoner er merket med kommentarer som `<!-- REDIGER: ... -->`.

### Legge til eller bytte styrebilde

Styrebilder skal være 600×600 px JPEG. Komprimer bildet med `sips` i Terminal før det legges inn:

```bash
sips -Z 600 FILNAVN.jpg
```

Dette endrer størrelsen slik at lengste kant blir 600 px og beholder proporsjonene. Legg deretter bildefilen i `assets/`-mappen.

**Nytt styremedlem:** Legg til en ny `styre-portrait`-blokk i `index.html`:

```html
<div class="styre-portrait">
  <img src="assets/FILNAVN.jpg" alt="Navn" loading="lazy" />
</div>
```

**Bytte eksisterende bilde:** Erstatt den gamle bildefilen i `assets/` med den nye (behold samme filnavn), eller endre `src`-attributtet i den aktuelle `styre-portrait`-blokken til det nye filnavnet.

### Publisere endringer
```bash
git add .
git commit -m "Beskrivelse av endringen"
git push
```

Siden oppdateres automatisk på [lo-rana.no](https://lo-rana.no) innen 1–2 minutter.

## Sosiale medier

Nettsiden har Open Graph-tagger som styrer forhåndsvisningen når lenken deles på Facebook, Instagram, LinkedIn, Slack og andre plattformer (tittel, beskrivelse og bilde).

Hvis forhåndsvisningen på Facebook ser feil ut eller ikke oppdateres, bruk Facebooks Sharing Debugger til å tvinge en ny skanning:

1. Gå til [developers.facebook.com/tools/debug](https://developers.facebook.com/tools/debug)
2. Lim inn `https://lo-rana.no/`
3. Klikk **Scrape Again** 2–3 ganger med litt ventetid mellom hvert forsøk

## Teknisk

- Ren HTML/CSS/JavaScript – ingen rammeverk eller byggeprosess
- Hostet på GitHub Pages
- GitHub-repo: [github.com/t-event/lo-rana-nettside](https://github.com/t-event/lo-rana-nettside)
- Domene: `lo-rana.no` (DNS via Telenor)
- Font: Open Sans (Google Fonts)
- Facebook Page Plugin for automatisk nyhetsfeed

## Kontakt

**LO Rana og Omegn**  
Søndre gate 13, 8624 Mo i Rana  
lo-rana@lo-rana.no
