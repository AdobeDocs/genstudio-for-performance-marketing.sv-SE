---
title: Skapa en webbannonsupplevelse
description: Lär dig hur du skapar webbannonsupplevelser i Adobe [!DNL GenStudio] för Performance Marketing.
feature: Brands Service, Guidelines, Content Generation, Generative AI, Create, Experiences, Variant Generation
badgeBeta: label="Beta" tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."
role: User
level: Beginner
recommendations: noDisplay
exl-id: 7d5e777b-7a30-48f4-b253-9823e38eecce
source-git-commit: 9cc284cdb00a204baf6b0a2d9d7f67cf9bc9c81f
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 0%

---

# Skapa en webbannonsupplevelse

I den här självstudiekursen visas hur du skapar profilerade [displayannonsupplevelser](display-ad-experiences.md) med GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (penselikonen i det vänstra navigeringsområdet).

Om du vill skapa en övertygande webbannonsupplevelse rekommenderar vi att du [lägger till riktlinjer i GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) och läser [grunderna för skrivfrågor](/help/user-guide/effective-prompts.md) innan du börjar.

## Välj en mall

Om du vill skapa en webbannonsupplevelse använder du en tillgänglig mall för att tillhandahålla ramverket för ditt innehåll. Mer information om visningsannonsdimensioner som stöds finns i [Bästa tillvägagångssätt för mallar](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines).

**Så här väljer du en visningsannonsmall**:

1. I _[!DNL Create]_klickar du på&#x200B;**[!UICONTROL Display ads]**i_&quot;Vad vill du skapa idag?&quot;avsnittet _.
1. Använd sökalternativet, bredvid _Filter_, för att hitta en specifik mall för visningsannons.
1. I vyn _Välj mall_ klickar du på en mall för visningsannons.
1. Klicka på **[!UICONTROL Use]**.

   Arbetsytan, som fungerar som nav för att skapa innehåll, visas.

## Lägg till parametrar

Om du lägger till [riktlinjer](/help/user-guide/guidelines/overview.md) och resurser i _Parametrar_ i snabbredigeraren läggs innehållsgenereringsprocessen ovanpå och det är ett viktigt förberedelsesteg för att generera en visningsupplevelse.

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

![Ange en fråga](/help/assets/prompt-displayad.png){width="650" zoomable="yes"}

Läs [Skriv effektiva uppmaningar](/help/user-guide/effective-prompts.md) om du vill veta mer om hur du skriver uppmaningar.

**Så här skriver du en fråga**:

1. Ange en uppmaning i rutan _&quot;Beskriv de upplevelser du vill generera&quot;_ .
1. Klicka på **[!UICONTROL Generate]**.

Som standard genereras och visas fyra varianter på arbetsytan, som följs av uppmaningen, riktlinjer och innehåll som du har lagt till.

## Revidera genererade displayannonser

Innan du väljer vad som ska skickas för godkännande eller publicering till [!DNL Content] kan du redigera visnings- och textavsnitt eller ta bort en genererad variant.

**Så här granskar du genererade varianter**:

* **Om du vill [redigera namnet för visning och utkast](/help/user-guide/create/manage-variants.md#change-draft-name)** klickar du i titeln _Namnlöst utkast_ längst upp på arbetsytan och anger en ny titel.
* **Om du vill [redigera en visningsannons manuellt](/help/user-guide/create/manage-variants.md#manually-edit-text)** dubbelklickar du i något av avsnitten eller fälten i displayannonsen (t.ex. ämnesraden, huvudet eller brödtexten) och redigerar efter behov.
* **Om du vill [återskapa ett avsnitt av en variant](/help/user-guide/create/manage-variants.md#re-generate-sections)** klickar du på ett redigerbart textfält och använder de tillgängliga alternativen för att omformulera, förkorta, förlänga eller generera ny text.
* **Om du vill [ändra storlek och proportioner för annonsen](/help/user-guide/create/manage-variants.md#change-aspect-ratio)** klickar du på knappen _[!UICONTROL Resize]_(ruta med en knappikon till vänster om arbetsytan) och väljer en ny storlek och proportioner som ska användas för alla varianter. Varianterna dupliceras och storleksändras.
* **Om du vill [beskära eller flytta bilder](/help/user-guide/create/manage-variants.md#crop-assets)** håller du pekaren över bilden, klickar på beskärningsikonen som visas och justerar bildens storlek och placering. Klicka på **[!UICONTROL Apply]**.

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## Skicka feedback

Klicka på alternativikonen (tre punkter) och välj **[!UICONTROL Good output]** eller **[!UICONTROL Poor output]** om du vill [skicka feedback](/help/user-guide/create/manage-variants.md#generation-feedback) om kvaliteten på genereringsutdata.

## Verifiera varumärkesjustering

Om du vill optimera de annonser som skapas och säkerställa strikt efterlevnad av varumärkesidentiteten kan du utnyttja kraften i [_varumärkesvalideringspanelen_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) som visar omfattande information om varumärkesvalidering och lyser upp förbättringsområden.

**Så här verifierar du varumärkesjustering**:

1. Klicka på ikonen för varumärkesvalidering i det övre menyfältet för att öppna [_panelen för varumärkesvalidering_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel). Du kan se information om de fragment och riktlinjer som behöver förbättras.

1. Växla mellan annonserna för att se hur ni kan förbättra det genererade innehållet för att bli mer varumärkesanpassade.
1. [Granska annonser manuellt](#revise-generated-display-ads) för att säkerställa att dina e-postmeddelanden är i linje med ditt varumärke.

Se [Varumärkesvalidering](/help/user-guide/guidelines/brand-validation.md).

## Få recensioner och godkännanden

Använd panelen Godkännanden, som finns på den övre menyraden på arbetsytan, för att få granskningskommentarer, spåra granskningskommentarer och få godkännanden från intressenter.

**Så här får du granskningar och godkännanden**:

1. [Starta en godkännandebegäran](/help/user-guide/approvals/request-review.md) för att begära ett [godkännande av utkast till e-postupplevelser](/help/user-guide/approvals/approve-content.md).
1. [Ta bort eller lägg till granskare](/help/user-guide/approvals/review-and-edit.md#manage-approvals) under granskningsprocessen.
1. [Få åtkomst till innehållet för granskning](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) och visa begäranden om revision.
1. Redigera utkasten per granskningskommentarer och [publicera dina webbannonsupplevelser](#publish-and-export-experience).

Se [Recensioner och godkännanden](/help/user-guide/approvals/overview.md).

## Publish och exportupplevelser

Om du vill göra de genererade webbannonserna tillgängliga för aktuell och framtida användning publicerar du dem på [!UICONTROL Content] och exporterar dem för användning i dina marknadsföringskampanjer.

1. **Om du vill publicera dina nya visningsupplevelser** klickar du på **[!UICONTROL Publish]** i det övre verktygsfältet eller i godkännandeflödet.
   1. Välj _[!UICONTROL [!DNL Campaigns]]_och lägg till_[!UICONTROL More details]_ om du vill.
   1. Klicka på **[!UICONTROL Publish]**.

      ![Publish en displayannons](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **Klicka **[!UICONTROL Export]**i det övre verktygsfältet om du vill exportera dina nya visnings- och annonsupplevelser**.
   1. Markera formatet - HTML och bilder, PNG eller JPG - och klicka på **[!UICONTROL Export]**.

      Exporterad HTML ska placeras i en fördefinierad webbegenskap, som en mall eller `div`-behållare. Utan dessa angivna mått kan bilderna se förvrängda ut när de visas oberoende av varandra.

Se [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
