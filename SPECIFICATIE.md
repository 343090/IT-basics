# Specificatie — Projectenpagina

Versie: 1.1 · Status: afgerond, op één punt na te bevestigen

## 1. Doel

Een eigen pagina waarop bezoekers in één oogopslag zien waar Eymen aan heeft gewerkt en waarmee. De pagina is de uitgebreide versie van de huidige "Mijn Vakken"-sectie op de homepage.

Doelgroep: docenten, stagebegeleiders en werkgevers die snel willen beoordelen wat hij gedaan heeft.

## 2. Wat een bezoeker kan zien en doen

**Zien**
- De drie projecten: IT-basics, Local WP en Project management
- Per project: titel, korte omschrijving, en bij twee projecten de gebruikte technologieën
- Dat hij een Software Developer student is (navbar, koptekst, footer)

**Doen**
- Vanuit het menu naar de projectenpagina navigeren, op desktop én mobiel
- Met "Terug naar home" weer terug naar de homepage
- Vanaf de homepage met één knop naar de pagina

**Bewust niet mogelijk**
- Een project openen. De "Bekijk"-knoppen zijn verwijderd omdat ze nergens heen gingen. Ze komen terug zodra er een echte link is (zie 6.1).

## 3. Te bouwen onderdelen

| Onderdeel | Beschrijving |
|---|---|
| Navbar | Zelfde als homepage; item "Projecten" gemarkeerd als huidige pagina |
| Koptekst | "Mijn projecten" + korte intro, in hetzelfde blauwe thema |
| Projectgrid | 3 kaarten naast elkaar op desktop, onder elkaar op mobiel |
| Projectkaart | Titel, omschrijving en optioneel tags. Geen knop |
| Terugknop | "Terug naar home" onder de grid |
| Knop op homepage | "Bekijk alle projecten" onder de bestaande vakkensectie |
| Footer | Zelfde als homepage |

Uitstraling: bestaande blauwe kleuren (`#3498db`, `#2c3e50`, `#34495e`). Geen nieuwe themakleuren, geen animaties.

## 4. Bestaande bestanden die veranderen

| Bestand | Wijziging |
|---|---|
| `index.html` | Menu-item "Vakken" → "Projecten", linkt naar `projecten.html`; knop "Bekijk alle projecten" onder de vakkensectie; drie dode "Bekijk"-knoppen verwijderd |
| `css/style.css` | Nieuwe klassen: `.tags`, `.page-header`, `.section-actions`, `.nav-links a.current` |
| `README.md` | Projectenpagina en `projecten.html` in structuur en functielijst |
| `js/main.js` | Geen wijziging nodig — navbar en formulier werken al op beide pagina's |

## 5. Nieuwe bestanden

| Bestand | Inhoud |
|---|---|
| `projecten.html` | De projectenpagina zelf |
| `SPECIFICATIE.md` | Dit document |

Niet nodig en daarom niet aangemaakt: aparte CSS- of JS-bestanden, een databestand met projecten, detailpagina's per project, de map `images/` (bij deze pagina worden geen afbeeldingen gebruikt).

## 6. Beslissingen

1. **"Bekijk"-knoppen** — besloten: verwijderd tot er een echte bestemming is. Zodra het eerste project op GitHub staat, komen ze terug met een link naar de repository. Dat is een uitbreiding, geen afwerking.
2. **Tags** — besloten: alleen echte technologieën, en alleen waar ze iets toevoegen. IT-basics toont `HTML, CSS`; Local WP toont `WordPress, HTML`; Project management toont geen tags, omdat `Planning` een vaardigheid is en geen technologie.
3. **Omschrijvingen** — nog open: geschreven door OpenCode en ingekort tot ongeveer twee zinnen. Eymen leest ze na en herschrijft wat niet zijn stem is.

## 7. Wanneer is de pagina klaar

De pagina is klaar wanneer:

- [x] Vanuit het menu van beide pagina's te bereiken is, en terug
- [x] Kaarten naast elkaar staan op desktop en onder elkaar op een telefoon
- [x] Het hamburger-menu op beide pagina's werkt
- [x] "Bekijk alle projecten" op de homepage naar de nieuwe pagina leidt
- [x] Kleuren en knoppen hetzelfde zijn als op de homepage
- [x] Geen dode `#`-links meer op beide pagina's
- [ ] Teksten zijn goedgekeurd (punt 6.3)

Zes van de zeven punten staan op groen. Het laatste punt is een kwestie van nalezen, niet van bouwen.

## 8. Buiten scope

Detailpagina per project, zoekfunctie, filteren op categorie, projecten uit JSON laden, animaties, screenshots, en de "Over mij"-tekst op de homepage.