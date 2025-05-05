---
title: Generera bilder
description: Skapa en bild som matchar stilen för en referensbild i Adobe [!DNL GenStudio] för Performance Marketing (Prestandamarknadsföring).
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."
role: User
level: Beginner
recommendations: noDisplay
source-git-commit: 277731aeea966da3cbd1fdabf015bfab3b907d39
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 0%

---

# Generera bilder

Med GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (penselikon) kan du generera _[!DNL On-brand images]_- genererade resurser som hämtar inspiration från en vald bild och fångar upp den visuella effekten och den övergripande estetiken.<!-- [two types of images](#image-types) using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon)—_[!DNL On-brand images]_ and _[!DNL Similar images]_. -->

Om du vill skapa en effektfull och effektfull bild rekommenderar vi att du [lägger till riktlinjer i GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) och läser [grunderna för skrivfrågor](/help/user-guide/effective-prompts.md).

## Bildtyper

_[!DNL On-brand images]_&#x200B;är genererade resurser som hämtar inspiration från en vald bild och fångar upp den visuella effekten och den övergripande estetiken. De här bilderna skapas med bilder som redan finns i [!DNL Content] och en noggrant skapad prompt som guidar designen. De följer strikt både varumärkesriktlinjerna och de parametrar som valts under produktionsprocessen.

_[!DNL On-brand images]_<!-- and _[!DNL Similar images]_ --> innehåller angivna riktlinjer, parametrar och en [genomtänkt fråga](/help/user-guide/effective-prompts.md) för att leverera tilltalande bildresurser.

<!-- * _[!DNL Similar images]_—Image assets created with strong similarity to an existing selected image available in [!DNL Content]. When generating similar images, GenStudio for Performance Marketing redesigns the selected image, giving slight variations on the content to provide variety and nuance. -->

## Generera varumärkesbilder

Du kan generera [!DNL On-brand images] med hjälp av definierade riktlinjer, parametrar och en vald referensbild. Dessa element, tillsammans med din fråga, vägleder genereringen av konsekventa [!DNL On-brand image]-variationer.

### Välj en referensbild

Om du vill skapa en _[!DNL On-brand images]_&#x200B;väljer du en befintlig bild som sparats i [!DNL Content]. Mer information om [!DNL on-brand image]-dimensioner som stöds finns i [Bästa tillvägagångssätt för mallar](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines).

**Välj en referensbild**:

1. Klicka på **[!UICONTROL On-brand image]** i _[!DNL Create]_.
1. Använd sökalternativet bredvid _Filter_ för att hitta en viss bild.

   ![Välj referensbild](/help/assets/select-img.png){width="400" zoomable="yes"}

   Om du vill använda resurser från en ansluten [!DNL AEM Assets Content Hub]-databas väljer du en databas i listrutan _Plats_ . Filtrera och markera en bild.

1. Klicka på en bild i vyn _Markera bild_.

   Den markerade bilden kan vara upp till 10 MB stor.

1. Klicka på **[!UICONTROL Use]**.

   Arbetsytan, som fungerar som nav för att skapa innehåll, visas.

### Lägg till parametrar

Genom att ta med [riktlinjer](/help/user-guide/guidelines/overview.md) och parametrar förbättras innehållsgenereringsprocessen och det är ett viktigt förberedelsesteg för att skapa en [!DNL on-brand image].

**Så här lägger du till riktlinjer och parametrar**:

1. På fliken _Grundläggande_ väljer du en [!DNL Brand] som informerar innehållsskapandet.

   Om det inte finns några varumärken tillgängliga på den här menyn [lägger du till riktlinjer i din GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Välj en bildkategori som bäst passar det önskade resultatet från _[!UICONTROL Image category]_.

   Bildkategorier är tillgängliga om en [!DNL Brand] har valts. Alternativen avgörs av de valda [!DNL Brand].

<!-- 1. _(Optional)_ Select a custom model from _[!UICONTROL Model]_.

   Models are available if you access to [custom models in Firefly](https://adobedx.slack.com/archives/CMF1JGMLY/p1743534402774569). The _Models_ list will be blank if you do not have access. -->

1. Välj önskat proportioner från _[!UICONTROL Aspect ratio]_.
1. Klicka på **[!UICONTROL Select from Content]** i _[!UICONTROL Style reference]_&#x200B;för att lägga till en referensbild. Bilden du väljer påverkar den visuella estetiken och djupet i de bilder du genererar.

   Om du vill använda resurser från en ansluten [!DNL AEM Assets Content Hub]-databas väljer du en databas i listrutan _Plats_ . Filtrera och markera en bild.

1. På fliken _Avancerat_ väljer du _innehållstypen_.

   Detta är förvalt baserat på bildkategorin som finns för den valda [!DNL Brand]-_bilden_ eller _fotot_ - och kan inte redigeras.

1. Justera den övergripande intensiteten för bildens befintliga visuella egenskaper i _[!UICONTROL Visual intensity]_.

### Ange en uppmaning

När du har valt parametrar kan du snabbt börja generera varumärkesbilder med det naturliga språket.

Se [Skriv aktuella uppmaningar](/help/user-guide/effective-prompts.md).

**Så här skriver du en fråga**:

1. Skriv en uppmaning i rutan.
1. Klicka på **[!UICONTROL Generate]**.

Som standard genereras och visas fyra varianter på arbetsytan, som följs av uppmaningen, parametrarna och det innehåll som du har lagt till.

### Redigera i Adobe Express

När du har genererat bildvarianter kan du redigera dem direkt i Adobe GenStudio for Performance Marketing med Adobe Express.

**Så här redigerar du en enskild bild med Adobe Express**:

1. Håll pekaren över en genererad bildvariant och klicka på _[!UICONTROL Edit in Adobe Express]_.

   Ett _Powered by Adobe Express_-fönster visas.

1. Utför bildredigering, till exempel [beskära en bild](https://helpx.adobe.com/express/create-and-edit-images/edit-images/crop-images.html), [ta bort ett objekt](https://helpx.adobe.com/express/create-and-edit-images/create-and-modify-with-generative-ai/remove-objects-generative-fill.html) och använda effekter.

   Läs [Adobe Express-dokumentation](https://helpx.adobe.com/express/user-guide.html) om du vill veta mer om hur du ändrar bilder i GenStudio for Performance Marketing med Adobe Express.

1. Klicka på _[!UICONTROL Apply changes]_&#x200B;om du vill spara ändringarna.
1. Fortsätt redigera enskilda bildvarianter efter behov och tillämpa ändringarna för att spara förloppet.

### Verifiera justering av innehållskontroll

Om du vill optimera de genererade varianterna och säkerställa strikt efterlevnad av varumärkesidentitet, plattformsriktlinjer och tillgänglighetsstandarder, kan du utnyttja kraften i [_innehållskontrollpanelen_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Den här panelen visar omfattande detaljer för innehållskontroll och lyser upp förbättringsområden.

**Så här utför du innehållskontroller**:

1. Klicka på panelikonen _Innehållskontroll_ i det högra åtgärdsfältet för att öppna panelen [_Innehållskontroll_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Visa en sammanfattning av kontrollerna *Behöver granskas* och *Godkänd* för att se vilka avsnitt och riktlinjer som behöver förbättras.

   ![_Innehållskontroll_ panel](/help/assets/content-check-img.png){width="500" zoomable="yes"}

1. Granska bildvarianter för att säkerställa att dina varianter är nära anpassade till de utförda innehållskontrollerna.

Se [Varumärkesvalidering](/help/user-guide/guidelines/brand-validation.md).

<!-- ## Generate Similar images

You can quickly generate images similar to a selected image within [!DNL Content] from the [!DNL Create] home.

**To create _[!DNL Similar images]_**:

1. In _[!DNL Create]_, click **[!UICONTROL Similar images]**.
1. Use the search option, adjacent to _Filter_, to find a specific image.

   To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ drop-down menu. Filter and select one image.

1. In the _Select image_ view, click on an image.
1. Click **[!UICONTROL Use]**.

   The Canvas, which serves as the central hub for content creation, is displayed. Four image variations similar to the original selected image appear.

   ![Generate similar images](/help/assets/generate-similar.png){width="400" zoomable="yes"} -->

## Publicera och exportera bilder

Genererade bildutkast visas i avsnittet _Senaste_ på startsidan för [!DNL Create].

Om du vill göra de genererade bilderna tillgängliga för aktuell och framtida användning publicerar du dem till [!UICONTROL Content] och exporterar dem för användning i dina marknadsföringskampanjer.

1. **Om du vill publicera dina nya bilder** klickar du på **[!UICONTROL Publish]** i det övre verktygsfältet.
   1. _[!UICONTROL Add details]_, till exempel&#x200B;_[!UICONTROL Campaigns]_ eller _[!UICONTROL Channels]_, om du vill.
   1. Klicka på **[!UICONTROL Publish]**.

1. **Om du vill exportera dina nya bilder** klickar du på **[!UICONTROL Export]** i det övre verktygsfältet.
   1. Markera formatet (JPG eller PNG) och klicka på **[!UICONTROL Export]**.

Se [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
