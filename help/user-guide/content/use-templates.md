---
title: Arbeta med mallar
description: Upptäck hur du använder mallar effektivt för att effektivisera din kreativa process i Adobe GenStudio for Performance Marketing.
feature: Templates, Content
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: 62ab3849296195ca4d9525cb5688f74ce8bede54
workflow-type: tm+mt
source-wordcount: '935'
ht-degree: 0%

---

# Arbeta med mallar

GenStudio for Performance Marketing gör det möjligt för innehållsskapare att snabbt producera enhetligt marknadsföringsinnehåll med hjälp av _mallar_. En mall minskar tiden och arbetet som krävs för att generera nytt innehåll avsevärt genom att tillhandahålla en startpunkt som inkluderar förkonfigurerade layouter och designelement.

GenStudio for Performance Marketing stöder inte direkt framtagning av mallar i programmet, men du kan enkelt utforma och förbereda mallar med vanliga designverktyg som Adobe InDesign, Illustrator eller Express. När designen är klar kan du anpassa den för användning i GenStudio for Performance Marketing. Börja använda mallar genom att följa de här stegen:

1. **Designa din mall**: Använd det designverktyg du föredrar för att skapa den visuella layouten för din [mall med element](#template-elements) som förrubrik, rubrik, brödtext, CTA, bilder och sidfot.

2. **Koda din mall**: Konvertera din design till HTML och infogad CSS för att säkerställa att den är ren och responsiv på olika enheter. Ta en titt på [hjälpmedelsriktlinjerna](accessibility-for-templates.md) som kan hjälpa dig att nå ut till din avsedda målgrupp.

3. **Förbered för GenStudio for Performance Marketing**: Anpassa mallen HTML med hjälp av mallspråket Handlebars. Infoga platshållare för att ange var GenStudio for Performance Marketing ska generera innehåll dynamiskt. Se hur du [anpassar en mall](customize-template.md) för GenStudio for Performance Marketing.

Med de här stegen kan du skapa professionella och effektiva mallar som är klara att användas i GenStudio for Performance Marketing, så att du snabbt och effektivt kan producera varumärkesinnehåll.

## Mallelement

En mall är en uppsättning instruktioner som definieras med HTML och infogad CSS som kan användas för att skapa en e-post, en social annons eller en webbannonsupplevelse. Mallelement tillhandahåller strukturen för att skapa innehåll.

Nedan följer en lista över element som används i mallar och en del detaljer om deras egenskaper:

- **Förrubrik**

   - Fungerar som en sekundär ämnesrad i ett e-postmeddelande och förbättrar ämnesraden
   - Mellan 40 och 50 tecken
   - Visas i inkorgen bredvid motivet innan e-postmeddelandet öppnas
   - Används i e-postmallar

- **Sidhuvud**

   - Övre delen av e-postmeddelandet som mottagaren ser när han/hon öppnar e-postmeddelandet
   - Anger tonen och ger sammanhang för det inkluderade innehållet
   - Används i e-postmallar

- **Rubrik**

   - Första innehållet som mottagaren ser
   - Bör vara lockande att fånga intresset
   - Används i metadatamallar

- **Brödtext**

   - Huvudsakligt innehållsområde där det primära meddelandet överförs
   - Möjlighet att inkludera text, bilder och andra medier
   - Används i mallar för e-post och metaannonser

- **CTA**

   - Knappen Call-to-action använder en fras och en länk
   - Uppmuntrade mottagaren att utföra en viss åtgärd, som att klicka på en länk eller göra ett köp
   - Används i mallar för e-post och metaannonser

- **Bilder**

   - Förbättrar den visuella effekten
   - Dela upp text
   - Stöd meddelandet
   - Bör vara högkvalitativ och uppseendeväckande
   - Används i mallar för e-post och metaannonser

- **Sidfot**

   - Avsnittet längst ned som innehåller ytterligare innehåll, t.ex. kontaktinformation, länkar till sociala medier, ansvarsfriskrivningar och alternativ för att avbryta prenumerationen
   - Används i e-postmallar

- **Textövertäckning**

   - Text på en bild
   - Använd för att stödja och förbättra rubriken och brödtexten
   - Används i metadatamallar

>[!TIP]
>
>Se de [identifierade fältnamnen](customize-template.md#recognized-field-names) som GenStudio for Performance Marketing stöder för mallar av varje kanaltyp.

## Anpassa mall

Du [anpassar mallen](customize-template.md) för användning i GenStudio for Performance Marketing genom att infoga platshållare för innehåll, eller fält, som den generativa AI-filen använder för att infoga innehåll. GenStudio for Performance Marketing känner igen vissa fält, till exempel fältet `body`, och följer kanalriktlinjerna som konfigurerats för det valda varumärket.

>[!TIP]
>
>Följ [hjälpmedelsriktlinjerna](accessibility-for-templates.md) och [bästa praxis](/help/user-guide/content/best-practices-for-templates.md) så att du kan nå ut till fler av din publik och skapa en optimal upplevelse.

## Hantera mallar

Galleriet [!DNL Templates] visar din lista med mallar som är anpassade för att generera upplevelser i GenStudio for Performance Marketing. Du kan filtrera mallar efter kanaltyp, till exempel e-post, webbannonser och Meta-annonser.

![Listan Innehållsmall](/help/assets/content-templates.png){width="650" zoomable="yes"}

### Lägga till en mall

Innan du överför en mall måste du se till att den är helt förberedd och klar att användas i GenStudio for Performance Marketing genom att följa vägledningen för [Anpassa mallar](customize-template.md) .

**Så här lägger du till en mall**:

1. I _[!DNL Content]_väljer du avsnittet **[!UICONTROL Templates]**.

1. Klicka på **[!UICONTROL Add template]**.

1. I rutan _[!UICONTROL Add your approved template]_bläddrar du efter mallfilen HTML eller drar HTML-mallfilen till släppområdet. Klicka på&#x200B;**[!UICONTROL Next]**.

1. Granska de identifierade fälten i rutan _[!UICONTROL Review discovered fields]_. Kontrollera att du använder rätt mall och att all information är som förväntat. Klicka på&#x200B;**[!UICONTROL Next]**.

   Exempel på Förhandsgranska för en e-postmall:

   ![Förhandsgranskningsfält har identifierats](/help/assets/template-detected-fields.png){width="650"}

   >[!TIP]
   >
   >Om mallen inte är korrekt klickar du på **[!UICONTROL Back]** och går tillbaka till föregående steg. Överför den korrigerade mallfilen.

1. I rutan _[!UICONTROL Provide template details and upload]_ger du mallen ett namn och väljer en **[!UICONTROL Channel]**-typ.

   Mallnamn och kanaltyp krävs. Ytterligare krav kan vara:

   - **Meta**: kräver proportioner
   - **Visningsannonser**: kräver Dimensioner

1. Lägg till så många detaljer du kan för att förbättra identifiering av mallar i sökningar och filtrering.

1. Klicka på **[!UICONTROL Done]**.

### Uppdatera mall

Mallar kan innehålla statiska filer, till exempel ikoner eller logotyper. [Statiskt innehåll](/help/user-guide/content/customize-template.md#static-content) lagras inte när mallförhandsvisningen har skapats. GenStudio for Performance Marketing fortsätter att referera till källlänken som finns i mallen. Använd Uppdatera för att uppdatera mallförhandsvisningen med de senaste versionerna av dessa resurser.

**Så här uppdaterar du mallen**:

1. I _[!DNL Content]_väljer du avsnittet **[!UICONTROL Templates]**.

1. Klicka på en mall för en fullständig vy och en lista med detaljer.

1. Klicka på **[!UICONTROL Refresh]** (cirklingspilar) i det övre högra hörnet för att uppdatera alla resurser som används i mallen.

### Skapa en upplevelse med en mall

Hitta och använd en befintlig mall i GenStudio for Performance Marketing för att skapa fler upplevelser.

**Så här skapar du en upplevelse med en mall**:

1. I _[!DNL Content]_väljer du avsnittet **[!UICONTROL Templates]**.

1. Klicka på en mall för en fullständig vy och en lista med detaljer.

1. Klicka på **[!UICONTROL Create Experience]** (penselverktyget) i det övre högra hörnet om du vill använda mallen.

1. Fortsätt till [Skapa](/help/user-guide/create/overview.md#create-use-cases) en upplevelse.
