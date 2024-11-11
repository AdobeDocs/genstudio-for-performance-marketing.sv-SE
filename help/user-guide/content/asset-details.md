---
title: Resursinformation
description: Adobe GenStudio for Performance Marketing lagrar godkänt material med omfattande metadata för sökbarhet och prestandaspårning.
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: edd27a6151cb81213ee27813beb4ecee835a1229
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Resursinformation

Adobe GenStudio for Performance Marketing lagrar godkänt material med omfattande metadata för upptäckt och prestandaspårning.

Varje resurs (inklusive upplevelser och mallar) har associerad _information_ (metadata) som hjälper till att identifiera, spåra, använda och lära sig av innehållsprestanda.

**Så här visar du resursinformation**:

1. I _[!DNL Content]_väljer du en resurs, upplevelse eller mall. När du klickar på en resurs öppnas en fokuserad vy över resursen.

1. Granska avsnittet _[!UICONTROL Details]_till höger i resursvyn.

   >[!TIP]
   >
   >Om avsnittet _[!UICONTROL Details]_inte visas klickar du på ikonen **[!UICONTROL Information]**(i).

   Resursinformationen innehåller metadata som används vid skapande eller överföring. Metadatatyperna för resurser omfattar [systemmetadata](#system-metadata) och [användardefinierade metadata](#user-defined-metadata).

>[!NOTE]
>
>Assets från AEM visar olika metadata. Mer information om hur du konfigurerar [!DNL AEM Assets Content Hub]-resursinformation finns i [Konfigurera resurssynlighet](connect-aem-repo.md#step-4-configure-asset-visibility).

## Redigera i Express

Du kan redigera bildresurser (JPG eller PNG) direkt i GenStudio for Performance Marketing med hjälp av Adobe Express. Arbetsytan i _[!UICONTROL Powered by Adobe Express]_har praktiska funktioner för att förbättra dina bilder utan att behöva lämna GenStudio-programmet. Du kan enkelt ta bort bakgrunder, använda generativa fyllningar, justera effekter och beskära bilder.

1. Välj en bildresurs i _[!DNL Content]_. När du klickar på en resurs öppnas en fokuserad vy över resursen.

1. I resursvyn klickar du på ikonen **[!UICONTROL Edit in Adobe Express]** i det övre högra hörnet.

1. Använd Express-kontrollerna på den vänstra panelen för att förbättra bilden på arbetsytan i _[!UICONTROL Powered by Adobe Express]_.

1. När du är nöjd med den uppdaterade bilden klickar du på **[!UICONTROL Save a copy]** uppe till höger.

1. Markera filformatet - JPG eller PNG - och klicka på **[!UICONTROL Save a copy]**.

1. Uppdatera **[!UICONTROL Asset name]** på popup-menyn _[!UICONTROL Save a copy of asset]_.

   - Välj **[!UICONTROL Same details as original asset]** om du vill överföra resursinformationen till den nya bilden.

   - Expandera avsnittet **[!UICONTROL More details]** för att uppdatera kampanjen, riktlinjerna och andra metadata.

   >[!TIP]
   >
   >Ju mer information du ger, desto mer upplever du GenStudio for Performance Marketing robusta funktioner. Välj en eller flera detaljer i listan eller ange en ny där det är tillämpligt, t.ex. med nyckelord. Varje detalj som du lägger till visas under listan. Klicka på **`x`** om du vill ta bort en detalj.

1. Klicka på **[!UICONTROL Save]**.

## Systemmetadata

Vissa metadata för resurser samlas in automatiskt när en resurs överförs. Du kan inte redigera standardsystemmetadata.

Standardmetadata som lagras och hämtas för en resurs är filens namn, dimensioner, källa med mera.

### Genererade taggar

När du lagrar en godkänd resurs i [!DNL Content] använder GenStudio for Performance Marketing Adobe AI och maskininlärningsfunktioner för att studera resursen och tillämpa taggar baserat på resursfunktionerna. En bild på en katt kan till exempel resultera i attributtaggar som `pet photography` eller `cat`, och färgtaggar som identifierar dominerande färger i bilden. Du kan inte redigera taggar som identifieras och används automatiskt.

Se [!DNL Insights] [Attributkategorier](/help/user-guide/insights/attribute-category.md) för detaljerade listor över bild-, video- och textfunktioner.

### Metadata för genererat innehåll

Den information som används för att generera en ny resurs eller upplevelse blir metadata, till exempel den fråga som användes. Du kan inte redigera frågan när innehållet har godkänts, men du kan använda den som startpunkt för att generera något nytt.

## Användardefinierade metadata

Användardefinierade metadata lägger till marknadsföringssammanhang till resursens innehåll, vilket gör att marknadsförarna kan förstå hur de ska använda och interagera med resursen.

När du [överför en resurs](/help/user-guide/content/manage-assets.md#add-assets) kan du definiera en uppsättning med valfri resursinformation som finns i GenStudio for Performance Marketing som metadata. Om du tar med mer information kan det bli enklare att identifiera resurser i sökningar och filtrering.

### Metadatainformation

Följande tabell visar vilka metadata (resursinformation) du kan definiera när du skapar en resurs.

| Fält | Beskrivning |
| ------------- | ----------- |
| Kampanjer (projektnamn) | Standardmetadata som hämtas och lagras med resursen |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) har lagts till i GenStudio for Performance Marketing och publicerats för användning |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md) har lagts till i GenStudio for Performance Marketing för användning |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) har lagts till i GenStudio for Performance Marketing för användning |
| Kanaler | Innehållstyper i GenStudio for Performance Marketing som resursen används för, till exempel e-post- och metaannonser |
| Tidsram | Tidsram som resursen användes för, t.ex. kvartal, årstid, år. Exempel: `Winter 2023` |
| Län | Områden som tillgången används för. Exempel: `North America`, `APAC`, `Italy` |
| Språk | Språk som resursen används för. Exempel: `Spanish` |
| Nyckelord | Nyckelord som används för ytterligare identifiering av tillgångars egenskaper och syfte |

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
