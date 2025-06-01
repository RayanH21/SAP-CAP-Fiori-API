# SAP CAP Project – Externe Service Integratie

Dit project gebruikt het SAP Cloud Application Programming Model (CAP) om data op te halen uit een externe service en read-only weer te geven in een Fiori Elements-app.

## Installatie en starten

```bash
npm install
npm install axios dotenv
npm run dev
```

## Structuur

- `/srv`, `/app`, `/db`: standaard CAP-structuur
- `.cds`-bestanden definiëren het datamodel en de services
- `external-service.js`: bevat de handler-logica
- `.env`: bevat geen gevoelige data – pas zelf endpoints aan indien nodig

## Environment Variables

Maak een `.env` bestand aan in de `cap-api-fiori` map en voeg toe:

```env
TOKEN_URL=https://41208216trial.it-cpitrial05-rt.cfapps.us10-001.hana.ondemand.com/http/CP012IF002
IFLOW_URL=...
CLIENT_ID=...
CLIENT_SECRET=...
```

Vervang de waarden door je eigen API-gegevens en iFlow URL.
