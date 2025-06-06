# Plan

## Innholdsfortegnelse

- [Plan](#plan)
  - [Innholdsfortegnelse](#innholdsfortegnelse)
  - [🎯 Mål med oppgaven](#-mål-med-oppgaven)
  - [📋 Krav til systemet](#-krav-til-systemet)
    - [Hovedfunksjonalitet](#hovedfunksjonalitet)
    - [Ekstra funksjonalitet (hvis tid)](#ekstra-funksjonalitet-hvis-tid)
  - [🚀 Fremgangsmåte](#-fremgangsmåte)
    - [Ting som gjøres hver dag](#ting-som-gjøres-hver-dag)
    - [06.06.2025 - Dag 1](#06062025---dag-1)
    - [10.06.2025 - Dag 2](#10062025---dag-2)
    - [11.06.2025 - Dag 3](#11062025---dag-3)
    - [12.06.2025 - Dag 4](#12062025---dag-4)
    - [13.06.2025 - Dag 5](#13062025---dag-5)
    - [16.06.2025 - Dag 6](#16062025---dag-6)
    - [17.06.2025 - Dag 7](#17062025---dag-7)
  - [⚠️ Avgrensninger](#️-avgrensninger)
  - [📊 Skisser](#-skisser)
  - [💰 Tids- og kostnadsestimat](#-tids--og-kostnadsestimat)
    - [Lønnskostnader](#lønnskostnader)
    - [Programmer, verktøy og utstyr (ekskl. MVA)](#programmer-verktøy-og-utstyr-ekskl-mva)
    - [Tidsestimat](#tidsestimat)
  - [🛠️ Nødvendige programmer, verktøy og utstyr](#️-nødvendige-programmer-verktøy-og-utstyr)
    - [Utvikling](#utvikling)
      - [Visual Studio Code](#visual-studio-code)
      - [IntelliJ IDEA](#intellij-idea)
      - [Database](#database)
      - [Andre verktøy](#andre-verktøy)
    - [Bygg og distribusjon](#bygg-og-distribusjon)
  - [📚 Informasjonskilder og sparringspartnere](#-informasjonskilder-og-sparringspartnere)

---

## 🎯 Mål med oppgaven

Utvikle et system for VerktøyPartner AS som gir bedre kontroll over verktøy og utlån.

---

## 📋 Krav til systemet

### Hovedfunksjonalitet

- ✅ Registrere verktøy med navn, serienummer, tilstand og type
- ✅ Registrere skader på verktøy
- ✅ Registrere utlån med forventet returdato
- ✅ Registrere når verktøy blir returnert
- ✅ Opprette gebyr hvis verktøy ikke er returnert innen forventet tid
- ✅ Søke på verktøy/utstyr basert på status (tilgjengelig, utleid eller til service)
- ✅ Søke i aktive og historiske utlån
- ✅ Kunder skal kun kunne se om et verktøy er tilgjengelig
- ✅ Ansatte skal ha tilgang på alt annet

> **Note:** Systemet bør lages slik at det kan tilpasses for eventuelle endringsønsker fra kunden.

### Ekstra funksjonalitet (hvis tid)

- 🔄 Mulighet for kunden å spørre om utlån av verktøy og kreve godkjenning fra ansatt

---

## 🚀 Fremgangsmåte

### Ting som gjøres hver dag

- **Daglig oppdatering av logg:** Oppdatere loggen med hva som er gjort hver dag
- **Oppdatere dokumentasjon:** Oppdatere dokumentasjonen hvis nødvendig

### 06.06.2025 - Dag 1

**Hovedfokus:** Planlegging og oppstart

- **Oppstartsmøte med kunden:** Gå gjennom oppgaveteksten og kravene, avklare eventuelle uklarheter
- **Opprettelse av repo:** Opprette et nytt repo for fagprøven
- **Planlegging:**
  - Lage en grov plan for utviklingen
    - Skriv ned verktøy og teknologier som skal brukes, samt lage skisser for systemet
    - Lage et tidsestimat for hver fase av utviklingen
  - Estimer kostnader for lønn og verktøy
  - Prøv å finne ut hva man får tid til å lage

### 10.06.2025 - Dag 2

**Hovedfokus:** Backend-utvikling (grunnlag)

- **Backend-utvikling:**
  - Oppsett av Spring Boot-prosjekt med Kotlin
  - Opprette funksjonalitet for registrering av verktøy, skader, utlån og service
  - Opprette funksjonalitet for søk på verktøy, utlån og service
  - Opprette tester for funksjonaliteten
  - Oppsett av PostgreSQL-database for lagring av data
  - Opprette nødvendige filer for Jenkins og Docker *(kan nok kopiere fra tidligere prosjekter)*

### 11.06.2025 - Dag 3

**Hovedfokus:** Backend-utvikling (sikkerhet og avansert funksjonalitet)

- **Backend-utvikling:**
  - Fortsette med oppgavene fra forrige dag hvis de ikke er ferdig
  - Implementering av autentisering og autorisering for ansatte og kunder *(se på tidligere prosjekter for referanse og ers-tester)*
  - Implementering av gebyrhåndtering *(CRON jobb?)*
  - Kanskje en liten demo av systemet for kunden for å få tilbakemeldinger

- **Mulige endringsforslag:**
  - Være forberedt på å gjøre endringer i systemet basert på tilbakemeldinger fra kunden

### 12.06.2025 - Dag 4

**Hovedfokus:** Backend ferdigstillelse og frontend-oppstart

- **Backend-utvikling:**
  - Fortsette med oppgavene fra forrige dag hvis de ikke er ferdig

- **Frontend-utvikling:**
  - Oppsett av SvelteKit-prosjekt med TypeScript, Tailwind og Flowbite
  - Kanskje bruke [Google Stich](https://stitch.withgoogle.com/) for å gi meg ideer om designet
  - Lage en enkel frontend som lar ansatte og kunder kommunisere med API-et
    - Kunder skal kunne se om verktøy er tilgjengelig, mens ansatte skal ha tilgang til alt annet
  - Opprette sider for å se verktøy, skader, utlån og service

- **Mulige endringsforslag:**
  - Være forberedt på å gjøre endringer i systemet basert på tilbakemeldinger fra kunden

### 13.06.2025 - Dag 5

**Hovedfokus:** Frontend-utvikling og dokumentasjon

- **Frontend-utvikling:**
  - Fortsette med oppgavene fra forrige dag hvis de ikke er ferdig
  - Implementere funksjonalitet for å registrere verktøy, skader, utlån og service
  - Implementere søkefunksjonalitet for verktøy og utlån

- **Dokumentasjon:**
  - Lage en presentasjon av systemet for kunden
  - Skrive noe om relevante lovverk (UU, GDPR, etc.) i dokumentasjonen
  - Forklare kort hvilke tiltak innenfor demokrati og medborgerskap, og bærekraft, har bedriften du har hatt læretiden i, gjennomført, eventuelt burde ha gjennomført

### 16.06.2025 - Dag 6

**Hovedfokus:** Ferdigstillelse og testing

- **Frontend-utvikling:**
  - Fortsette med oppgavene fra forrige dag hvis de ikke er ferdig

- **Reservert tid:**
  - Reservert tid til bugs og andre uforutsette hendelser

### 17.06.2025 - Dag 7

**Hovedfokus:** Egenvurdering og presentasjon

- **Egenvurdering:**
  - Oppsummering av gjennomført oppgave
  - Begrunnelse av valg du har gjort
  - Avvik i løsning i forhold til plan eller oppgavetekst?
  - Utfordringer
  - Bruk av hjelpemidler (AI, kolleger, etc.)
  - Hva kunne vært gjort annerledes eller bedre (prosess og resultat)?

- **Framføring av fagprøve:**
  - Presentere systemet for kunden
  - Gå gjennom dokumentasjonen og svare på eventuelle spørsmål
  - Få tilbakemeldinger fra kunden

---

## ⚠️ Avgrensninger

**Prioritering:** Backend-delen av denne oppgaven prioriteres høyest. Det er viktigst å få på plass et fungerende API som kan håndtere administrasjon av verktøy og utlån.

**Frontend-utvikling:** Hvis jeg får tid til å lage en frontend, blir det en SvelteKit-applikasjon som lar deg kommunisere med API-et på en enkel måte.

> **Note:** Jeg er usikker på hvor vidt jeg rekker å utforme frontenden universelt. Med Tailwind skal man egentlig designe for mobil først, men ettersom tidsrammen er kort vil jeg fokusere på å lage en desktop-versjon først siden det mest sannsynlig er det som vil bli brukt. *(kan spørre kunden om dette)*

---

## 📊 Skisser

Skisser er tilgjengelig i [/plan/diagrams/](diagrams/) mappen.

**Verktøy brukt:** [draw.io](https://app.diagrams.net/) - eksportert som PNG for enkelhets skyld.

---

## 💰 Tids- og kostnadsestimat

### Lønnskostnader

| Element | Verdi |
|---------|-------|
| **Tidsbegrensning** | 7 arbeidsdager |
| **Tid per dag** | 7,5 timer |
| **Totalt** | 52,5 timer |
| **Timeslønn** | 172 NOK |
| **Kostnad lønn** | 9 030 NOK |
| **Arbeidsgiveravgift** | 14,1% |
| **Total kostnad lønn** | **10 303 NOK** |

### Programmer, verktøy og utstyr (ekskl. MVA)

| Verktøy | Kostnad |
|---------|---------|
| Visual Studio Code | Gratis |
| Copilot Pro | 100 USD/år *(1 009 NOK)* |
| IntelliJ IDEA | 599 EUR/år *(6 901 NOK)* |
| Docker | Gratis |
| PostgreSQL | Gratis |
| Jenkins | Gratis |
| Nginx | Gratis |
| Draw.io | Gratis |
| Driftskostnader | ? NOK/år |
| **Total** | **? + 7 910 NOK** |

> *Valutakurser: USD = 10,09 NOK, EUR = 11,52 NOK*

### Tidsestimat

| Fase | Tidsperiode |
|------|-------------|
| **Planlegging** | Dag 1 |
| **Backend-utvikling** | Dag 2-4 (mulig dag 5) |
| **Frontend-utvikling** | Dag 5-6 |
| **Dokumentasjon og presentasjon** | Dag 7 |

> **Note:** Hvis nødvendig kommer jeg til å bruke dagene opprinnelig satt av til frontend-utvikling til å forbedre backend.

---

## 🛠️ Nødvendige programmer, verktøy og utstyr

### Utvikling

#### Visual Studio Code

- **Frontend:** SvelteKit + TypeScript + Tailwind + Flowbite
  - *Valgt fordi jeg er mer komfortabel med SvelteKit enn React*
- **Dokumentasjon:** Markdown
  - *Valgt fordi det er standard innen utvikling*

#### IntelliJ IDEA

- **Backend:** Kotlin med Spring Boot
  - *Valgt fordi jeg har erfaring med det fra jobben*

#### Database

- **PostgreSQL**
  - *Valgt fordi jeg har erfaring med det fra jobben*

#### Andre verktøy

- **git-idm-npm** - Git identity manager
  - [npmjs.com/package/git-idm-npm](https://www.npmjs.com/package/git-idm-npm)
  - *Valgt fordi jeg ikke vil committe med jobb-git til privat-git sitt repo*
- **draw.io** - For skisser
  - *Valgt fordi det er enkelt å bruke og gratis*

### Bygg og distribusjon

- **GitHub** - *Standard innen utvikling*
- **Jenkins** - Kontinuerlig integrasjon og distribusjon
  - *Valgt fordi jeg har satt det opp hjemme fra før av*
- **Docker** - Containerisering av applikasjonen
  - *Standard innen utvikling*
- **Nginx** - Reverse proxy
  - *Valgt fordi jeg har satt det opp hjemme fra før av*

---

## 📚 Informasjonskilder og sparringspartnere

- **Oppgavetekst:** [task.md](../task/task.md)
- **Samtaler med kunden:** Tilgjengelig i [loggene](../logs/logs.md)
- **AI-chatter og andre kilder:** Dokumentert i [loggene](../logs/logs.md)
- **Kolleger:**
  - Rasmus
