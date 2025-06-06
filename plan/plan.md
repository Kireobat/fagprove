# plan

## Innholdsfortegnelse

- [plan](#plan)
  - [Innholdsfortegnelse](#innholdsfortegnelse)
  - [Mål med oppgaven](#mål-med-oppgaven)
  - [Krav til systemet](#krav-til-systemet)
    - [Ekstra funksjonalitet (hvis tid)](#ekstra-funksjonalitet-hvis-tid)
    - [Notater (krav til systemet)](#notater-krav-til-systemet)
  - [Fremgangsmåte](#fremgangsmåte)
  - [Avgrensninger](#avgrensninger)
  - [Skisser](#skisser)
  - [Tids- og kostnadsestimat](#tids--og-kostnadsestimat)
    - [Lønnskostnader (kan være feil)](#lønnskostnader-kan-være-feil)
    - [Programmer, verktøy og utstyr (ekskl. MVA)](#programmer-verktøy-og-utstyr-ekskl-mva)
    - [Tidsestimat](#tidsestimat)
      - [Notater (tidsestimat)](#notater-tidsestimat)
  - [Nødvendige programmer, verktøy og utstyr](#nødvendige-programmer-verktøy-og-utstyr)
  - [Informasjonsskilder og sparringspartnere](#informasjonsskilder-og-sparringspartnere)

---

## Mål med oppgaven

- Utvikle et system for VerktøyPartner AS som gir bedre kontroll over verktøy og utlån.

---

## Krav til systemet

- Registrere verktøy med navn, serienummer, tilstand og type.
- Registrere skader på verktøy.
- Registrere utlån med forventet returdato.
- Registrere når verktøy blir returnert.
- Opprette gebyr hvis verktøy ikke er returnert innen forventet tid.
- Søke på verktøy/utstyr basert på status (tilgjengelig, utleid eller til service).
- Søke i aktive og historiske utlån.
- Kunder skal kun kunne se om et verktøy er tilgjengelig.
- Ansatte skal ha tilgang på alt annet.

### Ekstra funksjonalitet (hvis tid)

- Mulighet for kunden å spørre om utlån av verktøy og kreve godkjenning fra ansatt.

### Notater (krav til systemet)

Systemet bør lages slik at det kan tilpasses for eventuelle endrings ønsker fra kunden

---

## Fremgangsmåte

---

## Avgrensninger

Jeg kommmer til å prioritete backend delen av denne oppgaven. Jeg tenker det er viktigst å få på plass et fungerende API som kan håndetere administrasjon av verktøy og utlån.

Hvis jeg får tid til å lagen en frontend, så blir det en SvelteKit applikasjon som lar deg kommunisere med API-et på en enkel måte. Jeg er usikker på hvor vidt jeg rekker å utforme frontenden universelt. Med tailwind skal man egentlig designe for mobil først, men ettersom tidsrammen er kort vil jeg fokusere på å lage en desktopversjon først siden det mest sannsynlig er det som vil bli brukt. (kan spørre kunden om dette)

---

## Skisser

Skisser er tilgjengelig i `/plan/diagrams/` mappen.

Jeg har brukt [draw.io](https://app.diagrams.net/) for å lage skissene, men de er eksportert som PNG for enkelhets skyld.

---

## Tids- og kostnadsestimat

### Lønnskostnader (kan være feil)

- Tidsbegrensing: 7 arbeidsdager
- Tid per dag: 7,5 timer
- Totalt: 52,5 timer
- Timeslønn: 172 NOK
- Kostnad lønn: 9030 NOK
- Arbeidsgiver avgift: 14,1%
Total kostnad lønn: **10303 NOK**

### Programmer, verktøy og utstyr (ekskl. MVA)

- Visual Studio Code: gratis
- Copilot Pro: 100 USD per år
- IntelliJ IDEA: 599 EURO per år
- Docker: gratis
- PostgreSQL: gratis
- Jenkins: gratis
- Nginx: gratis
- Draw.io: gratis
- Driftskostnader: ? NOK per år

USD kostnad i NOK: `100 * 10,09 = 1009 NOK`
EURO kostnad i NOK: `599 * 11,52 = 6901 NOK`
Total kostnad programmer, verktøy og utstyr: **? + 7910 NOK**

### Tidsestimat

- Planlegging: dag 1
- Backend utvikling: dager 2,3, 4 og kanskje 5
- Frontend utvikling: dager 5 og 6
- Annen dokumentasjon og presenatsjon: dag 7

#### Notater (tidsestimat)

- Hvis nødvendig kommer jeg til å bruke dagene originalt satt av til frontend utvikling til å forbedre backend.

---

## Nødvendige programmer, verktøy og utstyr

- Utvikling
  - Visual Studio Code
    - SvelteKit + TS + tailwind for frontend
      - valgt fordi jeg er mer komfortabel med SvelteKit enn React
    - Markdown for dokumentasjon
      - valgt fordi det er standard innen utvikling
  - IntelliJ IDEA
    - Kotlin med Spring Boot
      - valgt fordi jeg har erfaring med det fra jobben
  - PostgreSQL
    - valgt fordi jeg har erfaring med det fra jobben
  - git-idm-npm
    - git identity manager
    - [https://www.npmjs.com/package/git-idm-npm](https://www.npmjs.com/package/git-idm-npm)
    - valgt fordi jeg ikke vil committe med jobb git til privat git sitt repo
  - draw.io
    - for skisser
    - valgt fordi det er enkelt å bruke og gratis
  
- Bygg og distribusjon
  - GitHub
    - valgt fordi det er standard innen utvikling
  - Jenkins
    - kontinuerlig integrasjon og distribusjon
    - valgt fordi jeg har satt det opp hjemme fra før av
  - Docker
    - containerisering av applikasjonen
    - valgt fordi det er standard innen utvikling
  - Nginx
    - reverse proxy
    - valgt fordi jeg har satt det opp hjemme fra før av

---

## Informasjonsskilder og sparringspartnere

- Oppgavetekst (tilgjengelig [her](/task/task.md))
- Samtaler med kunden (tilgjengelig i [loggene](/logs/logs.md))
- AI-chatter og andre kilder som er dokumentert i [loggene](/logs/logs.md)
- Kolleger
  - Rasmus
