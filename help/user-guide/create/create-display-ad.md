---
title: Skapa en annonsvisning
description: Lär dig hur du skapar webbannonsupplevelser i Adobe [!DNL GenStudio] för Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 7d5e777b-7a30-48f4-b253-9823e38eecce
source-git-commit: 81923bf493ec6fa2ed1a2fa655a76b01d7c87bc7
workflow-type: tm+mt
source-wordcount: '1094'
ht-degree: 0%

---

# Skapa en webbannonsupplevelse

I den här självstudiekursen visas hur du skapar profilerade [displayannonsupplevelser](display-ad-experiences.md) med GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (penselikonen i det vänstra navigeringsområdet).

Om du vill skapa en övertygande webbannonsupplevelse rekommenderar vi att du [lägger till riktlinjer i GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) och läser [grunderna för skrivfrågor](/help/user-guide/effective-prompts.md) innan du börjar.

## Välj en mall

Om du vill skapa en webbannonsupplevelse använder du en tillgänglig mall för att tillhandahålla ramverket för ditt innehåll. Se [Riktlinjer för visningsannonsmallar](/help/user-guide/templates/display-template.md) för mer information om visningsannonsdimensioner som stöds.

**Så här väljer du en visningsannonsmall**:

1. Klicka på _[!DNL Create]_&#x200B;i **[!UICONTROL Display ads]**.
1. Använd sökalternativet, bredvid _Filter_, för att hitta en specifik mall för visningsannons.
1. I vyn _Välj mall_ klickar du på en mall för visningsannons.
1. Klicka på **[!UICONTROL Use]**.

   Arbetsytan, som fungerar som nav för att skapa innehåll, visas.

## Lägg till parametrar

Om du lägger till [riktlinjer](/help/user-guide/guidelines/overview.md) och resurser i _Parametrar_ i snabbredigeraren läggs innehållsgenereringsprocessen ovanpå och det är ett viktigt förberedelsesteg för att generera en visningsupplevelse.

Om du använder en mall med fördefinierade riktlinjer (som [!DNL Brands], [!DNL Personas] eller [!DNL Products]) gäller dessa riktlinjer för dina varianter. Du kan ändra dem om du vill.

![Ange parametrar i promptlådan](/help/assets/prompt-displayad2.png){width="300" align="center"}

**Så här lägger du till parametrar och resurser**:

1. Klicka på ikonen _Parametrar_ för att expandera promptlådan.
1. I avsnittet _Parametrar_ väljer du riktlinjer -[!DNL Brands], [!DNL Personas] och [!DNL Products] - för att informera om hur du skapar innehåll.

   Om det inte finns några varumärken, profiler eller produkter tillgängliga från dessa menyer [lägger du till riktlinjer i din GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Så här lägger du till innehåll som ska användas i upplevelsen *och* för att påverka innehållsgenereringen:
   * Klicka på **[!UICONTROL Select from Content]** om du vill välja resurser (bilder) från din [!DNL Content]-databas, filtrera och markera en eller flera bilder.

     Om du vill använda resurser från en ansluten [!DNL AEM Assets Content Hub]-databas väljer du en databas i listrutan _Plats_ . Filtrera och markera en eller flera bilder.

   * Du kan också dra och släppa resurser i avsnittet **[!UICONTROL Select from Content]** för att överföra en eller flera nya resurser.
1. Klicka på **[!UICONTROL Use]**.

När du är klar med att lägga till parametrar komprimerar du promptlådan genom att klicka på ikonen _Parametrar_ igen.

## Ange en uppmaning

När du har valt riktlinjer kan du snabbt skapa innehåll för den nya webbannonsupplevelsen med hjälp av det naturliga språket. För att förbättra kvaliteten på den genererade webbannonsupplevelsen är det viktigt att skapa detaljerade och beskrivande uppmaningar.

Läs [Skriv effektiva uppmaningar](/help/user-guide/effective-prompts.md) om du vill veta mer om hur du skriver uppmaningar.

**Så här skriver du en fråga**:

1. Ange en uppmaning i rutan _&quot;Beskriv de upplevelser du vill generera&quot;_ .
2. Klicka på **[!UICONTROL Generate]**.

Som standard genereras och visas fyra varianter på arbetsytan, som följs av uppmaningen, riktlinjer och innehåll som du har lagt till.

## Ändra genererade varianter

Innan du väljer vad som ska skickas för godkännande eller publicering till [!DNL Content] kan du redigera visnings- och textavsnitt eller ta bort en genererad variant.

Om du vill markera ett enskilt lager som ska revideras klickar du på ett redigerbart fält eller bild och klickar på _[!UICONTROL View Layers]_.

**Så här granskar du genererade varianter**:

* **Om du vill [redigera namnet för visning och utkast](/help/user-guide/create/manage-variants.md#change-draft-name)** klickar du i titeln _Namnlöst utkast_ längst upp på arbetsytan och anger en ny titel.
* **Om du vill [redigera en visningsannons manuellt](/help/user-guide/create/manage-variants.md#manually-edit-text)** dubbelklickar du i något av avsnitten eller fälten i displayannonsen (t.ex. ämnesraden, huvudet eller brödtexten) och redigerar efter behov.
* **Om du vill [använda textformatering](/help/user-guide/create/manage-variants.md#manually-edit-text)** i en variant klickar du på texten i bilden eller på den infogade länken för en variant och klickar på **[!UICONTROL Format text]**.
* **Om du vill [återskapa ett avsnitt av en variant](/help/user-guide/create/manage-variants.md#re-generate-sections)** klickar du på ett redigerbart textfält och använder _[!UICONTROL Suggested edits]_-alternativen eller anger en ny uppmaning i [!UICONTROL Generate new text_ section] och klickar på&#x200B;**[!UICONTROL Generate]**.
* **Om du vill [lägga till eller byta ut bilder i en variant](/help/user-guide/create/manage-variants.md#swap-image)** klickar du på en bildresurs (eller bildresursområdet om det inte finns någon bild) och sedan på ikonen **[!UICONTROL Swap from content]** .
* **Om du vill [lägga till en länk till en bild i en variant](/help/user-guide/create/manage-variants.md#add-image-link)** klickar du på en bildresurs (eller bildresursområdet om det inte finns någon bild) och klickar på länkikonen.
* **Om du vill [lägga till alternativ text för bilder i en variant](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)** klickar du på en bildresurs och använder alternativet _Alt-text_ för att manuellt lägga till eller generera alternativ text per bild.
* **Om du vill [lägga till hjälpmedelsetiketter](/help/user-guide/create/manage-variants.md#add-accessibility-labels) till dina varianter** klickar du på en bild eller call-to-action-länk och anger sedan en kort beskrivning av vad länken eller knappen gör.
* **Om du vill [ändra storlek och proportioner för annonsen](/help/user-guide/create/manage-variants.md#change-aspect-ratio)** klickar du på knappen _[!UICONTROL Resize]_(ruta med en knappikon till vänster om arbetsytan) och väljer en ny storlek och proportioner som ska användas för alla varianter. Varianterna dupliceras och storleksändras.
* **Om du vill [beskära eller flytta bilder](/help/user-guide/create/manage-variants.md#crop-assets)** klickar du på en bild, klickar på **[!UICONTROL Edit]** (pennikonen) och sedan **[!UICONTROL Crop]**. Justera bildens storlek och placering.
* **Om du vill [använda Generativ utökning för att ändra storlek på och anpassa bilder](/help/user-guide/create/manage-variants.md#use-generative-expand) till din arbetsmall** klickar du på en bild, klickar på **[!UICONTROL Edit]** (pennikon) och sedan **[!UICONTROL Expand]**. Justera bilden så att den passar proportionerna och mallen.

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## Skicka feedback

Klicka på alternativikonen (tre punkter) och välj [&#x200B; eller &#x200B;](/help/user-guide/create/manage-variants.md#generation-feedback) om du vill **[!UICONTROL Good output]** skicka feedback **[!UICONTROL Poor output]** om kvaliteten på genereringsutdata.

## Verifiera justering av innehållskontroll

Om du vill optimera de genererade varianterna och säkerställa strikt efterlevnad av varumärkesidentitet, plattformsriktlinjer och tillgänglighetsstandarder, kan du utnyttja kraften i [_innehållskontrollpanelen_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Den här panelen visar omfattande detaljer för innehållskontroll och lyser upp förbättringsområden.

**Så här utför du innehållskontroller på en variant**:

1. Klicka på panelikonen _Innehållskontroll_ i det högra åtgärdsfältet för att öppna panelen [_Innehållskontroll_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Visa en sammanfattning av kontrollerna *Behöver granskas* och *Godkänd* för att se vilka avsnitt och riktlinjer som behöver förbättras.

   ![_Innehållskontroll_ panel](/help/assets/content-check-panel.png){width="300"}

2. [Granska varianter](#revise-generated-variants) manuellt för att se till att dina varianter är nära justerade med de utförda innehållskontrollerna.

Se [Varumärkesvalidering](/help/user-guide/guidelines/brand-validation.md).

## Få recensioner och godkännanden

Använd panelen Godkännanden, som finns som en ikon i det högra åtgärdsfältet på arbetsytan, för att få granskningar, spåra granskningskommentarer och få godkännanden från intressenter.

**Så här får du granskningar och godkännanden**:

1. [Starta en godkännandebegäran](/help/user-guide/approvals/request-review.md) för att begära ett [godkännande av utkast till displayannonsupplevelser](/help/user-guide/approvals/approve-content.md).
1. [Ta bort eller lägg till granskare](/help/user-guide/approvals/review-and-edit.md#manage-approvals) under granskningsprocessen.
1. [Få åtkomst till innehållet för granskning](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) och visa begäranden om revision.
1. Redigera utkasten per granskningskommentarer och [publicera dina webbannonsupplevelser](#publish-and-export-experience).

Se [Recensioner och godkännanden](/help/user-guide/approvals/overview.md).

## Publicera och exportera

Om du vill göra de genererade webbannonserna tillgängliga för aktuell och framtida användning publicerar du dem på [!UICONTROL Content] och exporterar dem för användning i dina marknadsföringskampanjer.

1. **Om du vill publicera dina nya visningsupplevelser** klickar du på **[!UICONTROL Publish]** i det övre verktygsfältet eller i godkännandeflödet.
   1. Välj _[!UICONTROL [!DNL Campaigns]]_&#x200B;och lägg till&#x200B;_[!UICONTROL More details]_ om du vill.
   1. Klicka på **[!UICONTROL Publish]**.

      ![Publicera en displayannons](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **Klicka** i det övre verktygsfältet om du vill exportera dina nya visnings- och annonsupplevelser **[!UICONTROL Export]**.
   1. Markera formatet - HTML och bilder, PNG eller JPG - och klicka på **[!UICONTROL Export]**.

      Exporterad HTML ska placeras i en fördefinierad webbegenskap, som en mall eller en `div`-behållare. Utan dessa angivna mått kan bilderna se förvrängda ut när de visas oberoende av varandra.

Se [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
