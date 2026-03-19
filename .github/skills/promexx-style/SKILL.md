---
name: promexx-style
description: Brand stijlgids voor PROMEXX (promexx.nl). Gebruik deze skill wanneer er documenten, presentaties, websites, e-mails, social media posts, of andere visuele materialen gemaakt moeten worden in de huisstijl van PROMEXX. Trigger ook bij vermeldingen van "PROMEXX stijl", "PROMEXX huisstijl", "PROMEXX branding", of wanneer output consistent moet zijn met de PROMEXX merkidentiteit.
---

# PROMEXX Huisstijl

Stijlbeschrijving gebaseerd op de website https://www.promexx.nl/ (geanalyseerd maart 2026).

PROMEXX is een technisch softwarebedrijf gespecialiseerd in software development voor complexe machines en mechatronica, gevestigd in de Brainportregio (Best, bij Eindhoven). De visuele identiteit straalt professionaliteit, technische diepgang en menselijke warmte uit.

---

## Kleurenpalet

### Primaire kleuren

| Naam               | HEX       | Gebruik                                                    |
|--------------------|-----------|-------------------------------------------------------------|
| **PROMEXX Donkerblauw** | `#0F1B2D` | Hoofdachtergrond, hero-secties, navigatie, footer            |
| **PROMEXX Marineblauw** | `#1A2A3A` | Secundaire achtergronden, kaarten, donkere panelen           |
| **PROMEXX Mintgroen**   | `#7ECEC2` | Primaire accentkleur, buttons, links, hover-states, iconen   |
| **Wit**                  | `#FFFFFF` | Tekst op donkere achtergrond, lichte secties                 |

### Secundaire / ondersteunende kleuren

| Naam                   | HEX       | Gebruik                                              |
|------------------------|-----------|-------------------------------------------------------|
| **Lichtgrijs**         | `#F5F5F5` | Lichte achtergrondpanelen, alternerende secties        |
| **Middegrijs**         | `#8A9BAE` | Subtekst, meta-informatie (datums, labels)             |
| **Donkergrijs tekst**  | `#2D3A4A` | Broodtekst op lichte achtergronden                     |
| **Mintgroen licht**    | `#A8DED5` | Hover-states, subtiele accenten, klantlogo's           |

### Kleurgebruik richtlijnen

- De website is overwegend **donker** (dark theme): diepe marineblauw/donkerblauw achtergronden met witte tekst en mintgroene accenten.
- Mintgroen (`#7ECEC2`) wordt gebruikt als **call-to-action kleur**: buttons, links, en interactieve elementen.
- Cursieve tekst in headings wordt soms in mintgroen weergegeven als accentuering.
- Lichte secties (wit/lichtgrijs) worden afgewisseld met donkere secties voor contrast en ritme.
- Klantlogo's worden weergegeven in een gedempte mintgrijs/groen tint, passend bij het kleurenpalet.

---

## Typografie

### Primair font: **Outfit**

PROMEXX gebruikt het Google Font **Outfit** als hoofdlettertype. Dit is een geometrisch sans-serif font met een moderne, schone uitstraling die past bij de technische identiteit van het bedrijf.

| Toepassing         | Font     | Gewicht           | Stijl     |
|--------------------|----------|-------------------|-----------|
| **H1 (hero)**      | Outfit   | 700 (Bold)        | Normaal   |
| **H2 (sectie)**    | Outfit   | 600 (SemiBold)    | Normaal   |
| **H3 (subsectie)** | Outfit   | 600 (SemiBold)    | Normaal   |
| **Broodtekst**     | Outfit   | 400 (Regular)     | Normaal   |
| **Accent / cursief**| Outfit  | 400–600           | *Italic*  |
| **Button-tekst**   | Outfit   | 500–600 (Medium)  | Normaal   |
| **Navigatie**      | Outfit   | 500 (Medium)      | Normaal   |
| **Meta / labels**  | Outfit   | 400 (Regular)     | Normaal   |

### Typografie richtlijnen

- **Hero headings** zijn groot en bold, met soms *cursieve woorden* als accentuering (bijv. "impact op de *echte* wereld").
- Broodtekst heeft een comfortabele regelafstand (line-height ~1.6–1.7) voor goede leesbaarheid.
- Tekst op donkere achtergronden is wit; tekst op lichte achtergronden is donkergrijs.
- Links en interactieve elementen zijn in mintgroen of onderstreept.
- Lettertypes worden via Google Fonts geladen:
  ```html
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700&display=swap" rel="stylesheet">
  ```

---

## Layout & Structuur

- **Full-width secties** die afwisselen tussen donkere en lichte achtergronden.
- **Maximale contentbreedte**: ~1200px, gecentreerd.
- **Ruime witruimte** (padding) rond secties, typisch 80–120px verticaal.
- **Twee-kolom layouts** voor content + afbeelding combinaties.
- **Kaart-gebaseerde layouts** voor nieuws, testimonials en cases.
- **Horizontale logo-carrousel** voor klantlogo's.

---

## Visuele elementen

### Buttons

- **Primaire button**: mintgroene achtergrond (`#7ECEC2`) met donkere tekst, afgeronde hoeken (border-radius ~6–8px).
- **Secundaire / ghost button**: transparant met mintgroene border en mintgroene tekst.
- Hover-state: lichte tint verschuiving of opacity-verandering.

### Afbeeldingen

- Foto's tonen echte medewerkers, teamactiviteiten en bedrijfsevenementen — authentiek en warm.
- Sfeerfoto's zonder overdreven stockfoto-achtige poses.
- Soms een lichte overlay of donker filter op hero-afbeeldingen voor tekst-leesbaarheid.

### Iconen

- Eenvoudige lijn-iconen (SVG), consistent in stijl.
- Kleur: mintgroen of wit, afhankelijk van achtergrond.

### Logo

- Het PROMEXX-logo is wit op donkere achtergronden.
- Er is een beeldmerk (geometrisch symbool) en een woordmerk.
- SVG-formaat beschikbaar via: `promexx-logo-white.svg` en `promexx-beeldmerk-white.svg`.

---

## Toon & Schrijfstijl

- **Professioneel maar toegankelijk**: technisch onderlegd, maar menselijk en warm.
- **Direct en helder**: geen wollige taal, recht op de man af.
- **Trots maar niet arrogant**: het bedrijf is trots op medewerkers en resultaten.
- **Inclusief en teamgericht**: nadruk op "wij", "samen", "onze mensen".
- **Nederlandstalig** als primaire taal, met technische termen in het Engels waar gebruikelijk in de branche (C++, real-time, embedded, etc.).

---

## CSS Variabelen (referentie)

```css
:root {
  /* Primaire kleuren */
  --promexx-dark: #0F1B2D;
  --promexx-navy: #1A2A3A;
  --promexx-mint: #7ECEC2;
  --promexx-white: #FFFFFF;

  /* Secundaire kleuren */
  --promexx-light-gray: #F5F5F5;
  --promexx-mid-gray: #8A9BAE;
  --promexx-text-dark: #2D3A4A;
  --promexx-mint-light: #A8DED5;

  /* Typografie */
  --promexx-font: 'Outfit', sans-serif;

  /* Spacing */
  --promexx-section-padding: 100px 0;
  --promexx-content-max-width: 1200px;
  --promexx-border-radius: 8px;
}
```

---

## Toepassing per medium

| Medium              | Richtlijn                                                                     |
|---------------------|-------------------------------------------------------------------------------|
| **Website / HTML**  | Dark theme als basis, Outfit font, mintgroene accenten                         |
| **Presentaties**    | Donkere slides met witte tekst, mintgroene highlights, ruime opmaak            |
| **Documenten**      | Wit papier met donkerblauwe headings en mintgroene accenten                    |
| **Social media**    | Donkere achtergronden, mintgroene tekstelementen, authentieke foto's           |
| **E-mail**          | Schone layout, donkerblauw header-blok, mintgroene CTA-buttons                |