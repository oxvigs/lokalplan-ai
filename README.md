# Lokalplan Finder

En webapplikation til at finde danske lokalplaner ved adresse og stille AI-drevne spørgsmål om dem.

## Features

- 🔍 Søg efter lokalplaner ved at indtaste en dansk adresse
- 🗺️ Integration med Plandata.dk's officielle data
- 🤖 Stil spørgsmål til AI om lokalplanens indhold
- 📄 Direkte links til plandokumenter (PDF)

## Teknologier

- DAWA API (Danmarks Adresse Web API) - adresse autocomplete og geokodning
- Plandata WFS - lokalplan data
- Claude AI - spørgsmål og svar om lokalplaner

## Deploy til Vercel

### Metode 1: Via Vercel CLI

```bash
# Installer Vercel CLI (hvis ikke allerede installeret)
npm i -g vercel

# Deploy
vercel

# For produktion
vercel --prod
```

### Metode 2: Via GitHub

1. Push dette repository til GitHub
2. Gå til [vercel.com](https://vercel.com)
3. Klik "Import Project"
4. Vælg dit GitHub repository
5. Vercel vil automatisk deploye

### Metode 3: Via Vercel Dashboard

1. Zip denne mappe
2. Gå til [vercel.com/new](https://vercel.com/new)
3. Træk og slip zip-filen
4. Klik "Deploy"

## Lokal udvikling

Åbn blot `index.html` i en browser, eller kør en lokal server:

```bash
# Python
python -m http.server 8000

# Node.js
npx serve

# PHP
php -S localhost:8000
```

Åbn derefter: http://localhost:8000

## Bemærk

DAWA API lukker 1. juli 2026. Efter denne dato skal adressen-delen af applikationen opdateres til at bruge den nye Dataforsyningen API.
