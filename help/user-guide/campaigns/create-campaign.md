---
title: Adobe GenStudio for Performance Marketing Campaigns
description: Lär dig hur du skapar och hanterar digitala marknadsföringskampanjer som utnyttjar resurser och upplevelser i form av generativ AI.
feature: Campaign Planning, Campaign Brief
badgeBeta: label="Beta" tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."
source-git-commit: edbeb7f0d08e2215a23f15cfeff77a5217cd264b
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---

# Skapa en kampanj

En GenStudio for Performance Marketing-kampanj definierar de viktigaste digitala kampanjegenskaperna och utvecklas allt eftersom faserna driftsätts och utvärderas. GenStudio for Performance Marketing stöder den dynamiska processen att lansera en kampanj, spåra resultatet för enskilda kampanjkomponenter och att fokusera om annonsupplevelserna baserat på resultatstatistik.

Nyckelelementen i kampanjen lagras i ett kampanjobjekt, vilket skapar en delad kontext för alla resurser och upplevelser som är märkta med samma unika kampanjnamn. Den här etiketten identifierar kampanjen i hela GenStudio for Performance Marketing.

GenStudio systemansvariga och Genstudio-redigerare kan skapa kampanjer.

## Definiera kampanjinformation

{{$include /help/_includes/campaign-details.md}}


**Ange kampanjinformation**:

1. Klicka på **[!UICONTROL Add campaign]** från [!DNL Campaigns]. Vyn _Skapa en kampanj_ öppnas.

   Detaljer omfattar både valfria och obligatoriska fält som definierar kampanjen. De här detaljerna sparas i [!DNL Campaigns] som metadataattribut för kampanjen.

1. Dubbelklicka på rubriken _Ny kampanj_ och ange ett informativt, unikt namn.

   Det här namnet blir en _kampanjetikett_ i GenStudio for Performance Marketing, vilket gör att du kan associera resurser och upplevelser med kampanjen när den överförs och skapas.

1. Ange värden i fälten _Detaljer_ som beskriver kampanjen. Se tabellen _Kampanjinformation_ för definitioner av kampanjfunktionerna.

## Tilldela kanaler och regioner

Kanal- och regioninställningarna avgör var kampanjen distribueras och dess distributionskanaler.

GenStudio for Performance Marketing använder fördefinierade mallar som kallas _records_ för att representera viktiga kampanjkomponenter, till exempel kanaler, regioner, profiler och produkter. När du skapar en kampanj associerar du den med relevanta poster för var och en av dessa komponenter.

* **Kanalinställningar** - Definierar de offentliga distributionskanalerna för din kampanj, inklusive betalda mediekonton, e-postmarknadsföringstjänster och displayannonsnätverk. Data om resultatet för kampanjer, resurser och upplevelser i dessa kanaler matas in i [[!DNL Insights]](/help/user-guide/insights/overview.md) för kanalspecifik analys.

* **Regioninställningar** - Anger de geografiska områden där du distribuerar kampanjen. Genom att ansluta till regionala datakällor kan GenStudio for Performance Marketing skräddarsy innehåll och strategi efter lokala målgruppsinställningar. Detta ger en mer korrekt målinriktning och resultatanalys baserad på regionala mätvärden.

**Så här väljer du distributionskanaler för kampanjen**:

1. Klicka på plustecknet (**[!UICONTROL Connect records +]**) bredvid **[!UICONTROL Channels]**.

   Popup-fönstret _Välj kanaler_ öppnas.

1. Välj de kanaler som kampanjen ska distribueras på. Giltiga värden är `Email`, `Paid media`, `Web` och `Display ads`.

   Du kan också välja **[!UICONTROL See all]** om du vill öppna en vy över alla kanaler som stöds.

**Så här tilldelar du regioner till din kampanj**:

1. Klicka på plustecknet (**[!UICONTROL Connect records +]**) bredvid **[!UICONTROL Regions]**.

   Popup-fönstret _Markera områden_ öppnas. Du kan söka efter ett specifikt område som stöds.

1. Välj regioner i en eller flera målregioner för kampanjen. Giltiga regioner är `AMER`, `LATAM`, `EMEA`, `APAC` och `Japan`.

   Du kan också välja **[!UICONTROL See all]** om du vill öppna en vy över alla områden som stöds.

## Tilldela profiler och produkter

[Personas](/help/user-guide/guidelines/personas.md) och [produkter](/help/user-guide/guidelines/products.md) sparas som poster. En personlig post definierar egenskaperna för ett specifikt kundsegment - målgruppen för genererat innehåll. Det kan omfatta demografisk information och en historik över kundinteraktioner.

Produktregister definierar viktiga produktspecifikationer och attribut i samband med varumärkesriktlinjerna. Attribut kan omfatta funktioner, tillhörande bilder och produktpositionering inom ert varumärke.

Alternativen i listrutorna _Personas_ och _Produkter_ definieras på organisationsnivå. När du skapar en kampanj väljer du bland dessa fördefinierade poster för att säkerställa en konsekvent produktrepresentation och ha stöd för korrekt målinriktning, meddelanden och resultatspårning.

**Så här tilldelar du profiler till kampanjen**:

1. Klicka på plustecknet (**[!UICONTROL Connect records +]**) bredvid **[!UICONTROL Personas]**.

   Popup-fönstret _Välj personer_ öppnas. Du kan söka efter en specifik person som stöds.

1. Välj de profiler som er kampanj riktar sig till. Giltiga profiler definieras av din organisation när [riktlinjer skapas](/help/user-guide/guidelines/personas.md).

   Du kan också välja **[!UICONTROL See all]** om du vill öppna en vy över alla tillgängliga profiler.

**Så här tilldelar du produkter till din kampanj**:

1. Klicka på plustecknet (**[!UICONTROL Connect records +]**) bredvid **[!UICONTROL Products]**.

   Popup-fönstret _Välj produkter_ öppnas. Du kan söka efter en viss produkt som stöds.

1. Välj en eller flera produkter. Produkter definieras av din organisation när [riktlinjer skapas](/help/user-guide/guidelines/products.md).

   Du kan också välja **[!UICONTROL See all]** om du vill öppna en vy över alla tillgängliga produkter.

## Skapa kampanjer fullständigt

Klicka på **[!UICONTROL Create]** om du vill spara de angivna värdena och skapa kampanjen.

Det nya kampanjnamnet är nu tillgängligt som kampanjetikett i [!DNL Content] och [!DNL Create]. Du kan lägga till godkända resurser och upplevelser till din kampanj via [!DNL Content] eller tilldela en resurs och upplevelse till en kampanj när innehåll skapas.

## Lägg till innehåll i kampanjen

GenStudio for Performance Marketing länkar innehåll till kampanjer med kampanjetiketter lagrade i [!DNL Content]-metadata. Ett enstaka innehåll kan kopplas till flera kampanjer.

Kampanjetiketter identifierar kampanjen och dess attribut. När du tilldelar en etikett till en resurs eller upplevelse kopplas den till motsvarande kampanj.

**Så här lägger du till resurser och upplevelser från[!DNL Content]**:

1. Välj den godkända upplevelsen eller resursen i galleriet [!DNL Content] _Experiences_ eller _Assets_.

1. I vyn _Detaljer_ väljer du kampanjens namn i listrutan _Kampanjer_ .

**Så här lägger du till resurser och upplevelser när innehåll skapas**:

När du skapar innehåll kan du publicera den nyligen skapade resursen eller upplevelsen till [!DNL Content].

1. Välj en kampanj i listrutan _Kampanjer_ i popup-menyn _Bekräfta information för ditt godkända innehåll_.

1. Klicka på **[!UICONTROL Publish]**.

Den här kampanjen är nu tillgänglig på kontrollpanelen _Kampanjer_.
