---
title: GenStudio Experience Selector MFE
description: Förstå och implementera Experience Selector Micro FrontEnd för dina GenStudio-appar och tillägg.
feature: Extensibility, Extensions, Experiences
source-git-commit: d6e580763d85df6d9d295d4e87501af4b022f57b
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# GenStudio Experience Selector MFE

Experience Selector är en Micro Frontend (MFE) som tillhandahåller en `ExperienceSelectorDialog`-komponent för att välja GenStudio-upplevelser. Använd komponenten i ditt program genom att importera funktionen `renderExperienceSelectorWithSUSI` från det fristående JavaScript-paketet, som automatiskt läser in den senaste distribuerade Micro FrontEnd och visar ett naturligt komponentgränssnitt.

Med GenStudio Experience Selector MFE kan man

- Bläddra bland och välj ut GenStudio-upplevelser
- Filtrera upplevelser efter olika kriterier
- Stöd för både ett och flera markeringslägen
- Hantera autentisering via integrering med SUSI (Sign-Up Sign-In)
- Skapa ett enhetligt gränssnitt för olika ramverk

## Integreringsalternativ

MFE kan integreras med två olika metoder:

### ESM (ES-moduler) - rekommenderas

```javascript
import { renderExperienceSelectorWithSUSI } from 'https://experience-stage.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/esm/standalone.js';
```

### UMD (Universal Module Definition)

```html
<script src="https://experience-stage.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/umd/standalone.js"></script>
```

## Konfigurationsegenskaper

Funktionen `renderExperienceSelectorWithSUSI` accepterar ett konfigurationsobjekt med följande egenskaper:

| Egenskap | Typ | Obligatoriskt | Beskrivning |
|----------|------|----------|-------------|
| `apiKey` | string | Ja | API-nyckel för GenStudio-tjänster |
| `imsOrg` | string | Ja | IMS-organisations-ID |
| `env` | string | Ja | Miljö (`stage`, `prod`) |
| `susiConfig` | object | Ja | [SUSI-autentiseringskonfiguration](#susi-configuration) |
| `onSelectionConfirmed` | function | Ja | Återanrop när markeringen har bekräftats |
| `onDismiss` | function | Ja | Återanrop när dialogrutan stängs |
| `locale` | string | Nej | Språkinställning (till exempel `en-US`) |
| `isOpen` | boolesk | Nej | Inledande dialogstatus |
| `selectionType` | string | Nej | Markeringsläget (`single` eller `multiple`) |
| `customFilters` | array | Nej | Egna filtervillkor |
| `dialogTitle` | string | Nej | Anpassad dialogrutans titel |

### SUSI-konfiguration

Objektet `susiConfig` kan innehålla:

```javascript
{
  clientId: 'genstudio',
  environment: 'stg1', // or 'prod'
  scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
  locale: 'en_US',
  modalSettings: {
    width: 500,
    height: 700
  }
}
```

## QuickStart

1. **Välj ramverk** bland de tillgängliga exemplen nedan
1. **Navigera till exempelkatalogen**
1. **Installera beroenden** (för React-/Vue-exempel)
1. **Uppdatera konfigurationen** med API-nycklar och IMS-organisation:

   ```javascript
   const experienceSelectorProps = {
     locale: 'en-US',
     apiKey: 'exc_app',           
     imsOrg: 'your-ims-org@AdobeOrg',  // Replace with your IMS Org
     env: 'stage', // or 'prod'
     susiConfig: {
        clientId: 'genstudio',
        environment: 'stg1', // or 'prod'
        scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
        locale: 'en_US',
        modalSettings: {
          width: 500,
          height: 700,
        },
     },
     customFilters: ['genstudio-channel:email'],
     selectionType: 'single', // or 'multiple'
     dialogTitle: 'Select Email Templates'
   };
   ```

1. **Kör utvecklingsservern**

### Exempel på implementeringar

Den här databasen innehåller fungerande exempel för olika ramverk:

- [Ett komplett React-program som demonstrerar integrationen med Vite-byggsystemet](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/react-js).

- [Ett Vue 3-program med API-integrering för disposition](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vue-js).

- [Två vanilj-JavaScript-implementeringar](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js):

- [Den här Vanilla ESM-versionen använder ES6-moduler och moderna JavaScript](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-esm).

- [Denna Vanilla UMD-version använder UMD-paket som läses in via skripttaggen ](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-umd-global-var).

## Autentiseringsflöde

Experience Selector hanterar autentisering automatiskt via SUSI:

1. När dialogrutan öppnas kontrollerar den om det finns någon autentisering.
1. Om den inte är autentiserad öppnas ett SUSI-inloggningsflöde.
1. När autentiseringen är klar visas upplevelseväljaren.
1. Användare kan bläddra bland och välja upplevelser.
1. De valda upplevelserna returneras via motringningen `onSelectionConfirmed`.
