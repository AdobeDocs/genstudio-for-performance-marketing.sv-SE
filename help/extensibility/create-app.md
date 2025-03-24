---
title: Skapa en App Builder-app för att utöka GenStudio for Performance Marketing
description: Börja bygga en app eller ett tillägg.
feature: Extensibility
exl-id: 4e757dd4-a02d-472c-bc13-6f27dffa48f2
source-git-commit: 52e8e078bc013fe686b5cc2105089f7098cce575
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# Utveckla en App Builder-app

Utvecklare som utökar GenStudio for Performance Marketing inbyggda funktioner använder [Adobe App Builder](https://developer.adobe.com/app-builder/) för att skapa, skicka och distribuera sina utbyggbara appar eller tillägg.

>[!BEGINSHADEBOX]

**Förutsättningar**:

* Node.js (version 20.x eller senare)

* npm (paketerat med Node.js)

* Adobe Developer kommandoradsgränssnitt. Installera: `npm install -g @adobe/aio-cli`

>[!ENDSHADEBOX]

## Appstruktur

GenStudio for Performance Marketing-tillägg är App Builder-program och innehåller samma grundläggande komponenter som andra App Builder-program.

### Bygg och konfigurera filer

Bland huvudkomponenterna i App Builder-programmen finns dessa bygg- och konfigurationsfiler. Den här listan innehåller inte alla bygg- och konfigurationsfiler.

* `README.md`: Innehåller allmän information om appen.

* TS-appfiler:

   * `package.json`
   * `package-lock.json`
   * `eslint`
   * `tsconfig`
   * `jest test up`

* App Builder konfigurationsfiler:

   * `app.config.yaml`
   * `ext.config.yaml`: konfigurationsfil för tillägget
   * `app.config.yaml`: konfigurationsfil för tillägget (omfattar definition av din app som ett GenStudio for Performance Marketing-tillägg)
   * `.aio`
   * `.env`: Verkställ inte filen `.env` till källkontrollen

### Source code

```
- src/
    - genstudiopem/
        - web-src/
            - src/
                - components/
                - utils/
                - Constants.ts
                - index.tsx
                - index.css
                - utils.ts
        - index.html
```

### Source-kodkomponenter

* `ExtensionRegistration.tsx`: Definierar de nödvändiga API:erna som värdappen (GenStudio for Performance Marketing) behöver för att läsa in och visa tillägget.

* `App.tsx`: Huvudprogramkomponent som definierar routning till andra komponenter.

* `AdditionalContextDialog.tsx`: Dialogrutekomponent för att visa ytterligare kontexttillägg.

* `RightPanel.tsx`: Dialogrutekomponent för ett valideringstillägg.

* `Helper`-komponenter: Inkluderar `ClaimsChecker`.

## Skapa en App Builder-app från en befintlig app

Du kan använda en exempelapp för att snabbt komma igång med att skapa din add-on.

**Så här skapar du en App Builder-app från en befintlig app**:

1. Hämta en exempelapp från databasen [GenStudio UIX Examples](https://github.com/adobe/genstudio-uix-examples).

1. Välj **[!UICONTROL Download All]** på arbetsytan för App Builder Project på [Adobe Developer Console](https://developer.adobe.com/console/) om du vill hämta projektinformation.

1. Öppna exempelappen lokalt i den integrerade utvecklingsmiljö du föredrar.

1. Autentisera med Adobe Developer kommandoradsgränssnitt:

   ```bash
   aio login
   ```

1. Ladda ned JSON-filen och skapa sedan din app:

   ```bash
   aio app use '/path/to/your/downloaded/app-builder/project/details/config.json'
   ```

## Lägg till egen kod i din add-on

Du definierar din tilläggskod i `AdditionalContextDialog.tsx`- och `RightPanel.tsx`-filer. Dessa två filer definierar popup-utseendet och beteendet när användarna öppnar tillägget.

* `AdditionalContextDialog.tsx`: Definiera den här komponenten om du tänker använda tillägget _Lägg till kontext_ . Användare interagerar med den här komponenten när de klickar på _Tillägg_ i frågerutan i [!DNL Create].

* `RightPanel.tsx`: Definiera den här komponenten om du tänker använda tillägget _Höger panel_ (upplevelsevalidering). Användare interagerar med den här komponenten när de klickar på valideringstillägget på den högra panelen i ett [!DNL Create]-upplevelseutkast.

Du är nu redo att [distribuera din app](deploy-app.md)

## Bästa tillvägagångssätt för apputveckling

Genom att underhålla utvecklingsmiljön kan du undvika programutvecklings- och distributionsfel:

* Om du använder en äldre version av ett exempelprogram uppgraderar du beroendena genom att installera om dem:

  ```bash
  rm -rf node_modules package-lock.json && npm i
  ```

* Uppgradera GenStudio UIX SDK. Bekräfta att du använder den senaste versionen av [GenStudio UIX SDK](https://github.com/adobe/genstudio-uix-sdk). Läs [GenStudio UIX-exempeldatabasen](https://github.com/adobe/genstudio-uix-examples) om du vill veta hur du använder de senaste SDK-ändringarna.
