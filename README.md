# SAP CAP Project – Externe Service Integratie

Dit project gebruikt het SAP Cloud Application Programming Model (CAP) om data op te halen uit een externe service en read-only weer te geven in een Fiori Elements-app.

## Installatie en starten

```bash
npm install
npm run dev
```

## Structuur

- `/srv`, `/app`, `/db`: standaard CAP-structuur
- `.cds`-bestanden definiëren het datamodel en de services
- `external-service.js`: bevat de handler-logica
- `.env`: bevat geen gevoelige data – pas zelf endpoints aan indien nodig