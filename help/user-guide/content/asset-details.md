---
title: Resursinformation
description: Adobe GenStudio for Performance Marketing lagrar godkänt material med omfattande metadata för sökbarhet och prestandaspårning.
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: 088bc6df481fb1e961a7df3c79515642ec39767d
workflow-type: tm+mt
source-wordcount: '505'
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

Följande bildresurs innehåller systemmetadata som beskriver filtyp, storlek och andra egenskaper, ett användardefinierat nyckelord samt flera AI-identifierade attribut och färger.

![information om en resurs med flera taggar](/help/assets/content-asset-details.png)

>[!NOTE]
>
>Assets från AEM visar olika metadata. Mer information om hur du konfigurerar [!DNL AEM Assets Content Hub]-resursinformation finns i [Konfigurera resurssynlighet](connect-aem-repo.md#step-4-configure-asset-visibility).

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
| [!UICONTROL Timeframe] | Tidsram som tillgången används för, t.ex. kvartal, årstid, år. Exempel: `Winter 2023` |
| Län | Områden som tillgången används för. Exempel: `North America`, `APAC`, `Italy` |
| Språk | Språk som resursen används för. Exempel: `Spanish` |
| Nyckelord | Användardefinierade nyckelord som används för att ytterligare identifiera egenskaper och syften för tillgångar |

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
