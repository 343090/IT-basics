# Stappenplan — Projectenpagina

Op basis van `SPECIFICATIE.md` versie 1.1. Elke stap is klein genoeg om in één keer te doen en heeft één duidelijke reden.

## Wat er al staat

Stappen 1 t/m 6 hieronder zijn grotendeels al uitgevoerd tijdens het bouwen. Ze staan er om te controleren of er niets is vergeten. Nieuw werk begint bij stap 7.

## Stappen

| # | Wat er wordt gedaan | Welk bestand | Waarom |
|---|---|---|---|
| 1 | Controleer of `projecten.html` bestaat en drie kaarten bevat | `projecten.html` | De basis van de pagina; zonder dit is de rest zinloos |
| 2 | Controleer of het menu-item "Projecten" naar `projecten.html" linkt | `index.html` | Bezoekers moeten de pagina kunnen bereiken |
| 3 | Controleer of de knop "Bekijk alle projecten" op de homepage staat | `index.html` | Tweede manier om de pagina te bereiken, vanaf de plek waar het project genoemd wordt |
| 4 | Controleer of `.tags`, `.page-header`, `.section-actions` en `.nav-links a.current` bestaan | `css/style.css` | Zonder deze klassen zijn tags, koptekst en terugknop ongestyled |
| 5 | Controleer of er geen `href="#"` meer in staat | `index.html`, `projecten.html` | Dode links ogen als een niet-af werkende site |
| 6 | Open beide pagina's in een browser, ook op mobiel formaat | geen | Controleert of het grid, het hamburger-menu en de kleuren kloppen in de praktijk |
| 7 | Lees de drie omschrijvingen op `projecten.html` na en herschrijf wat niet jouw stem is | `projecten.html` | Openstaand punt 6.3 uit de spec; dit is het enige echte werk |
| 8 | Beslis wat er met de dubbele inhoud gebeurt: de homepage en `projecten.html` vertellen nu hetzelfde verhaal in verschillende woorden | `index.html` óf `SPECIFICATIE.md` | Een bezoeker die beide pagina's leest ziet tegenstrijdige teksten over hetzelfde project |
| 9 | Werk de gekozen omschrijvingen door naar de kaarten die nog de oude tekst hebben | `index.html` | Zorgt dat beide pagina's hetzelfde zeggen |
| 10 | Herzie de titels "Project" en "Project managment" | `index.html` | "Project" zegt niets, en "managment" is een spelfout op een openbare pagina |
| 11 | Zet de status van stap 7 en 10 op groen in de checklist | `SPECIFICATIE.md` | De spec blijft kloppen met wat er werkelijk staat |
| 12 | Zodra het eerste project op GitHub staat: zet de "Bekijk"-knoppen terug met een echte link | `projecten.html`, `index.html` | Nu staan er geen knoppen; een portfolio is sterker als je code kunt laten zien |

## Wat er bewust niet in staat

- **Een map `images/` aanmaken** — er worden geen afbeeldingen gebruikt, dus de map zou leeg en misleidend zijn
- **Projecten uit JSON of een databestand laden** — drie projecten hardcoded in de HTML is overzichtelijker
- **Filteren op categorie of een zoekfunctie** — staat buiten scope in de spec
- **De "Over mij"-tekst herschrijven** — staat buiten scope, is wel iets voor een volgende ronde

## Open vraag

Moet de website online komen, bijvoorbeeld via GitHub Pages? Een portfolio dat alleen op je eigen laptop staat kun je niet aan iemand laten zien. Dat staat nu nergens in de spec, en het bepaalt of je later nog een `.gitignore`, een `CNAME` of een eigen domein nodig hebt.