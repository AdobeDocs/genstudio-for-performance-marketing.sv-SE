---
title: Resursinformation
description: Adobe GenStudio for Performance Marketing lagrar godkänt material med omfattande metadata för sökbarhet och prestandaspårning.
feature: Generative AI, Content Attributes, Content Management
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: 19d0b8b929e293179a091cc7b5a6a1268b0abbbd
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# Resursinformation

Adobe GenStudio for Performance Marketing lagrar godkänt material med omfattande metadata för upptäckt och prestandaspårning.

Varje resurs (inklusive upplevelser och mallar) har associerad _information_ (metadata) som hjälper till att identifiera, spåra, använda och lära sig av innehållsprestanda.

**Så här visar du resursinformation**:

1. I _[!DNL Content]_&#x200B;väljer du en resurs, upplevelse eller mall. När du klickar på en resurs öppnas en fokuserad vy över resursen.

1. Granska avsnittet _[!UICONTROL Details]_&#x200B;till höger i resursvyn.

1. Om avsnittet _[!UICONTROL Details]_&#x200B;inte visas klickar du på ikonen **[!UICONTROL Information]**(i).

Resursinformationen innehåller metadata som används under skaps- eller överföringsprocessen. Metadatatyperna för resurser omfattar [systemmetadata](#system-metadata) och [användardefinierade metadata](#user-defined-metadata).

Följande bildresurs innehåller systemmetadata som beskriver filtyp, storlek och andra egenskaper, ett användardefinierat nyckelord samt flera AI-identifierade attribut och färger.

![information om en resurs med flera taggar](/help/assets/content-asset-details.png)

>[!NOTE]
>
>Assets från AEM databaser visar olika metadata. Mer information om hur du konfigurerar [!DNL AEM Assets Content Hub]-resursinformation finns i [Konfigurera resurssynlighet](connect-aem-repo.md#step-4-configure-asset-visibility).

## Systemmetadata

Vissa metadata för resurser samlas automatiskt in när en resurs överförs, till exempel filtyp, storlek, dimensioner, källa och annat. Förutom filnamnet kan du inte redigera standardsystemmetadata.

### Genererade taggar

När du lagrar en godkänd resurs i [!DNL Content] använder GenStudio for Performance Marketing Adobe AI och maskininlärningsfunktioner för att studera resursen och tillämpa taggar baserat på resursfunktionerna. En bild på en katt kan till exempel resultera i attributtaggar som `pet photography` eller `cat`, och färgtaggar som identifierar dominerande färger i bilden. Du kan inte redigera taggar som identifieras och används automatiskt.

Se [!DNL Insights] [Attributkategorier](/help/user-guide/insights/attributes.md#categories) för detaljerade listor över bild-, video- och textfunktioner.

### Metadata för genererat innehåll

Den information som används för att generera en ny resurs eller upplevelse blir metadata, till exempel den fråga som användes. Du kan inte redigera frågan när innehållet har godkänts, men du kan använda den som startpunkt för att generera något nytt.

## Användardefinierade metadata

Användardefinierade metadata lägger till marknadsföringssammanhang till resursens innehåll, vilket gör att marknadsförarna kan förstå hur de ska använda och interagera med resursen.

När du [överför en resurs](/help/user-guide/content/manage-assets.md#add-assets) kan du definiera en uppsättning med valfri resursinformation som finns i GenStudio for Performance Marketing som metadata. Om du tar med mer information kan det bli enklare att identifiera resurser i sökningar och filtrering.

**Så här redigerar du användardefinierade metadata**:

1. I _[!DNL Content]_&#x200B;väljer du en resurs, upplevelse eller mall. När du klickar på en resurs öppnas en fokuserad vy över resursen.

1. Granska avsnittet _[!UICONTROL Details]_&#x200B;till höger i resursvyn.

1. Klicka på **[!UICONTROL Edit details]** (penna) för att redigera tillgång, upplevelse eller mallmetadata.

   Ju mer information du ger, desto mer upplever du GenStudio for Performance Marketing robusta funktioner. Välj en eller flera detaljer i listan eller ange en ny där det är tillämpligt, t.ex. med nyckelord. Varje detalj som du lägger till visas under listan. Klicka på **`x`** om du vill ta bort en detalj.

### Metadatainformation

I följande tabell visas de metadata (resursinformation) som du kan definiera när du skapar en resurs.

| Fält | Beskrivning |
| -------------- | ----------- |
| Titel | Namnet på resursen; standardtiteln kan vara det ursprungliga filnamnet |
| [!DNL Campaigns] | [[!DNL Campaigns]](/help/user-guide/campaigns/overview.md) innehåller kampanjinnehåll med konsekvent meddelandehantering för att uppnå ett affärsmål<br>Om du klickar på en kampanjlänk visas kampanjens översiktssida |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) har lagts till i GenStudio for Performance Marketing och publicerats för användning |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md) har lagts till i GenStudio for Performance Marketing för användning |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) har lagts till i GenStudio for Performance Marketing för användning |
| Kanaler | Plattformar för distribution av vissa innehållstyper, t.ex. e-post, banderoll och displayannonsering |
| [!UICONTROL Timeframe] | Tidsram som tillgången används för, t.ex. kvartal, årstid, år. Exempel: `Winter 2023` |
| Län | Områden som tillgången används för. Exempel: `North America`, `APAC`, `Italy` |
| Språk | Språk som resursen används för. Exempel: `Spanish` |
| Nyckelord | Användardefinierade nyckelord används för ytterligare identifiering av tillgångsegenskaper och syfte |

>[!TIP]
>
>Klicka på **[!UICONTROL Edit details]** (penna) om du vill redigera metadata för resursen. Du kan till exempel ändra resursnamnet eller lägga till eller ta bort nyckelord.

## Generativ kontext

Avsnittet [!UICONTROL Generative Context] visar vilken information som användes för att generera upplevelsen, till exempel `Prompt` som användes under [!DNL Create]-processen. Denna insikt kan hjälpa er att skapa ännu fler framgångsrika varianter.

Informationen kan omfatta:

- Parametrarna `Brand`, `Product` och `Persona` har valts under [!DNL Create]-processen
- `Subject line` och `Preheader` för e-postupplevelser
- `Headline` och `Body` för Metaannonser

## Historik

Expandera avsnittet _[!UICONTROL History]_&#x200B;i en upplevelse för att visa en tidslinje med godkännanden och aktiviteter. En godkänd upplevelse visar till exempel datum, tid och godkännare:

```
Approved

December 10, 2024 at 6:00 PM by Username
```
