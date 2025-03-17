# Teknisk dokumentation for Tema 8 gruppeprojekt

Når man er flere der bidrager til en kodebase, lærer man hurtigt, at ens sædvanlige måder at gøre tingene på ikke nødvendigvis er logisk for alle.
Skriv derfor jeres fælles retningslinjer for punkterne herunder(tilføj gerne flere selv), sådan som det giver bedst mening for jer som gruppe. Dokumentationen sikre, at jeres fælles kodebase forbliver overskuelig, er let at arbejde med og til at forstå for alle, og at I undgå konflikter, og har nemmere ved at hjælpe hinanden undervejs.

Vi har aftalt, at vi følger kode-måden, som vi blev undervist i, med hensyn til at bruge nye brances for hvert component, og vi laver nye astro-sider for hvert component. Samtidig har vi opdelt og bestemt os for, hvilke sider vi laver hver især, så vi ikke kommer til at få errors/komplikationer i github/visuel studio code.

## Projektstruktur:

Beslut, hvordan I vil organisere jeres projekt – struktur for mapper og filer.

- Hvordan organiserer I billeder, fonte og andre ressourcer?
  Vi importerer google font links til fonte i head-elementet, som skal være ens på alle sider. Samme med favicon. Dog forholder vi alle billeder både svg og webp inde i assets mappen.

- Hvor placerer I boilerplate?(fx CSS- og JavaScript-filer, der bruges på tværs af projektet)
  Vi har en CSS generel mappe, som er vores boilerplate for css styles variabler fx farver og fonte. Så har vi javaScript fil for elementer, der er det samme for alle sider, netop header, nav og footer. Så de elementer vil forholdes i egne javaScript filer, som linkes til alle pages. Vi linker til <script src="js/page-name.astro"></script> nede i bunden af body lige under main og over footer.

- Hvor placerer I HTML, CSS- og JavaScript-filer til fx detaljevisning og listevisning?
  Vi følger den generelle struktur Astro har tilberedt i forvejen. Så HTML/astro pages ligger under pages og hvert enkelt component.astro har sine egne filer under components mappen.

## Navngivning:

Beslutte hvordan i vil navngive filer og mapper for at sikre en ensartet struktur og undgå forvirring.>

- Hvordan navngiver I filnavne? (fx små bogstaver, ingen mellemrum, brug af - eller \_)
  pages/sider skal forholdes små bogstaver, ingen mellemrum og brug af - og \_

Men med components, så SKAL de åbenbart have Stort første bogstav.

- Hvordan sikre I at det er til at forstå hvilke HTML-, CSS- og JavaScript-filer der høre sammen?
  Hvis de direkte hænger sammen, så hedder det nøjagtig det samme bortset fra .astro, .css og .js.

## Link til scripts:

- Hvor placerer I script referencer i HTML'en? (fx i <head> med defer attribute, eller sidst i <body>)
  sidst i body.

## Git branches:

- Hvordan navngiver I branches, så alle kan forstår hvem der arbejder i branchen og på hvad?(fx feature-lotte-formular)
  Vi sørger for, at alle brances hedder følgende: feature-element/component-navn. Så hvis Sebastian laver footer, så vil brancen for denne component være feature-footer-seb

## Arbejdsflow:

- Hvordan fordeler I arbejdet, så I undgår at flere arbejder i de samme filer samtidigt?
  Vi har lavet en orden inde i figma-to do page, hvor vi kan se, hvem der skal arbejde på hvilke sider.

- Hvordan sikrer I, at commit-beskeder er beskrivende?
  Aktionen skal være det første ord og det skal være i bydeform, og så forholdes det kort i stikord form, så fx hvis Sebastian har lavet noget css på footeren, så vil commit beskeden være: add css ændringer på footer component

- Hvordan kommunikerer i om ændringer i main branchen når feature merges?
  Hvis dette sker, så sørger vi for, at der er kun 1, som ændrer på dette feature i main, og andre venter med at merge deres ting til main før personen, som arbejder på main er færdig. Men dette burde undgås ved at vente med at merge ting til main branch til man er helt færdig.

## Kode:

- Hvordan skriver i funktioner i JavaScript?(fx med function keyword eller som arrow functions)
  Vi er blevet bekendt nok med arrow functions, så vi bruger bare den originale måde, som vi har lært.

- Beslut hvilken CSS selector i benytter til referencer i henholdsvis CSS og JavaScript(fx. id'er til JavaScript og Classes til CSS)
  Vi bruger mest classes, fordi det kan bruges flere gange/mere frit.

- Skal filer have korte forklaringer som kommentarer?
  Egentlig ikke. Det håber vi på, ikke behøves. Og hvis vi til sidst ikke forstår hinandens kode, så kan vi bruge chatGPT til at give kommentare til koden. Ellers forklare vi det til hinanden.

# Funktionalitet

Dette afsnit skal forklare hvad I konkret har arbejde med, for at udvikle websitet. Tænk over hvilke interaktioner brugeren kan foretage på sitet? Eller hvordan websitet håndterer og præsenterer data? Eksempler på funktionalitet, der kan beskrives:

- Hentning af events fra API.
  Vi bruger ikke et API i dette Tema
- Filtrering af events baseret på brugerens valg.
  Vi har tydelige filtrerings knapper, som fører brugeren ned til det rette sted på siden.
- Dynamisk visning af events i HTML.
  Ingen dynamisk visning, fordi vi ikke henter data fra API i dette tema.

Brug korte beskrivelser, som i eksemplerne herover

# API endpoints

Dette afsnit skal liste de endpoints fra API'et i har benyttet:

- (fx. https://dummyjson.com/products)

intet brug af API

# Dokumentation af Funktion

Dette afsnit skal beskrive en funktion I selv har udviklet. Det kunne eksempelvis være en funktion der generere en listen over fx. produkter:

- Beskrivelse: Hvad gør funktionen? Hvordan spiller den sammen med resten af koden?
- Parametre: Hvilke input forventes (fx en værdi fra en dropdown eller URL'en)?
- Returnerer: Beskriv, om funktionen returnerer en værdi eller blot manipulerer DOM’en.
- Eksempel på brug: Indsæt funktions-koden herunder(der hvor koden er i eksemplet) og vis, hvordan funktionen kaldes:

```javascript
//funktionens kode:
function voresFunktion(sprog) {
  console.log(`${sprog} syntax highlighting`);
}
//hvordan funktionen kaldes:
voresFunktion("JavaScript");
```

Vi har ikke kodet endnu.
