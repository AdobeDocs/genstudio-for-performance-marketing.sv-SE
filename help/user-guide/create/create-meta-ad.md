---
title: Skapa en Meta-annonsupplevelse
description: Lär dig skapa varumärkesanpassade annonsupplevelser i Meta - för Facebook eller Instagram - med Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 42111bbf-70cd-4fd2-a7a9-15abe072d720
source-git-commit: 9d7d607b52c232612f5920fc4a6d4ccd8dff93c9
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---

# Skapa en Meta-annonsupplevelse

I den här självstudiekursen visas hur du skapar [varumärkesanpassade annonsupplevelser](/help/user-guide/create/meta-experiences.md) med GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (penselikonen i det vänstra navigeringsområdet).

Innan du börjar generera en annonsupplevelse med Meta är det viktigt att [införliva riktlinjer](/help/user-guide/guidelines/add-guidelines.md) i GenStudio for Performance Marketing och bekanta dig med grunderna i [att skapa en uppmaning](/help/user-guide/effective-prompts.md).

## Välj en mall

Om du vill börja generera en ny annonsupplevelse med Meta använder du en tillgänglig mall för att tillhandahålla ramverket för ditt innehåll. Mer information om vilka metadataproportioner som stöds finns i [Bästa tillvägagångssätt för mallar](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines).

**Så här väljer du en mall för Meta-annons**:

1. I _[!DNL Create]_klickar du på&#x200B;**[!UICONTROL Meta ads]**i_&quot;Vad vill du skapa idag?&quot;avsnittet _.
1. Använd sökalternativet bredvid _Filter_ för att hitta en specifik mall för metaannonser.
1. Klicka för att välja en mall och klicka på **[!UICONTROL Use]**.

   Den här åtgärden öppnar arbetsytan, som är navet för innehållsskapande.

## Lägg till parametrar

Genom att lägga till [riktlinjer](/help/user-guide/guidelines/overview.md) och resurser i _Parametrar_ i promptlådan förbättras innehållsgenereringsprocessen och det är ett viktigt steg när det gäller att förbereda sig för att generera en Meta-annons.

Om du använder en mall med fördefinierade riktlinjer - [!DNL Brands], [!DNL Personas] eller [!DNL Products] - gäller dessa riktlinjer för dina varianter. Du kan ändra dem om du vill.

**Så här lägger du till parametrar och resurser**:

1. Klicka på ikonen _Parametrar_ för att expandera promptlådan.
1. I avsnittet _Parametrar_ väljer du riktlinjer -[!DNL Brands], [!DNL Personas] och [!DNL Products] - för att informera om hur du skapar innehåll.

   ![Välj persona](/help/assets/persona-select.png){width="600" zoomable="yes"}

   Om det inte finns några varumärken, profiler eller produkter tillgängliga från dessa menyer [lägger du till riktlinjer i din GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Lägg till innehåll som ska användas i upplevelsen *och* för att påverka innehållsgenereringen:
   * Klicka på **[!UICONTROL Select from Content]** om du vill välja resurser (bilder) från din [!DNL Content]-databas, filtrera och markera en eller flera bilder.

     ![Välj visuellt innehåll](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

     Om du vill använda resurser från en ansluten [!DNL AEM Assets Content Hub]-databas väljer du en databas i listrutan _Plats_ . Filtrera och markera en eller flera bilder.

   * Du kan också dra och släppa resurser i avsnittet **[!UICONTROL Select from Content]** för att överföra en eller flera nya resurser.
1. Klicka på **[!UICONTROL Use]**.

När du är klar med att lägga till parametrar kan du komprimera promptlådan genom att klicka på ikonen _Parametrar_ igen.

## Ange en uppmaning

När riktlinjer har valts kan du snabbt skapa innehåll för din nya Meta-annonsupplevelse med hjälp av det naturliga språket. Detaljerade anvisningar ger högre kvalitet än otydliga eller tvetydiga instruktioner.

Läs [Skriv effektiva uppmaningar](/help/user-guide/effective-prompts.md) om du vill veta mer om hur du skriver uppmaningar.

**Så här skriver du en fråga**:

1. Ange en uppmaning i rutan _&quot;Beskriv de upplevelser du vill generera&quot;_ .
1. Klicka på **[!UICONTROL Generate]**.

Som standard genereras och visas fyra varianter på arbetsytan, som alla föds av uppmaningen, riktlinjer och innehåll som du har lagt till.

Genererat innehåll läses in stegvis - allt eftersom varje avsnitt i metaupplevelsen genereras visas det på arbetsytan. Se [Metaupplevelser](/help/user-guide/create/meta-experiences.md#progressive-loading) om du vill veta hur ändringarna läses in på arbetsytan.

## Välj kanal för Meta-annonser

När du genererar en Meta-annons kan du välja mellan Facebook- eller Instagram-annonser.

Växla kanalalternativet Meta-annonser - mellan **Facebook** och **Instagram** - på den högra menyraden (Facebook- och Instagram-ikoner) för att visa och hantera varianter för varje kanal.

När du [ändrar metadataannonserna](#revise-generated-variants) kan du ändra proportionerna för Facebook- och Instagram-annonser.

## Ändra genererade varianter

Innan du väljer vad som ska skickas för godkännande eller publicering till [!DNL Content] kan du redigera Meta-annonserna eller ta bort en variant från uppsättningen med genererade annonser.

**Så här granskar du genererade varianter**:

* **Om du vill [redigera namnet på metadatautkastet](/help/user-guide/create/manage-variants.md#change-draft-name)** klickar du i titeln _Namnlöst utkast_ längst upp på arbetsytan och anger en ny titel.
* **Om du vill [redigera en Meta-annons manuellt](/help/user-guide/create/manage-variants.md#manually-edit-text)** klickar du i något av annonsavsnitten (till exempel ämnesraden,
sidhuvud eller brödtext) och redigera efter behov.
* **Om du vill ändra eller markera anropet till åtgärden** klickar du på knappen för att ringa till åtgärd och väljer bland de tillgängliga textalternativen för knappen. I _Länk_ anger du en URL för texten som anropar till åtgärd.
<!-- **To [change or select the Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, click the call-to-action button and select _[!UICONTROL Rephrase]_ or _[!UICONTROL Add link]_. -->
* **Om du vill [lägga till en länk till en bild i en variant](/help/user-guide/create/manage-variants.md#add-image-link)** klickar du på en bildresurs (eller bildresursområdet om det inte finns någon bild) och klickar på länkikonen.
* **Om du vill [återskapa ett avsnitt av en variant](/help/user-guide/create/manage-variants.md#re-generate-sections)** klickar du på ett redigerbart textfält och använder _[!UICONTROL Suggested edits]_-alternativen eller anger en ny fråga och klickar på&#x200B;**[!UICONTROL Generate]**.
* **Om du vill [lägga till eller byta ut bilder i en variant](/help/user-guide/create/manage-variants.md#swap-image)** klickar du på en bildresurs (eller bildresursområdet om det inte finns någon bild) och sedan på ikonen **[!UICONTROL Swap from content]** .
* **Om du vill [beskära eller flytta bilder](/help/user-guide/create/manage-variants.md#crop-assets)** håller du pekaren över en bild, klickar på beskärningsikonen som visas och justerar bildens storlek och placering.
* **Om du vill [ta bort en metaannons](/help/user-guide/create/manage-variants.md#delete-variant)** klickar du på alternativmenyn för en variant och sedan på **[!UICONTROL Delete variant]**.

## Skicka feedback

Klicka på alternativikonen (tre punkter) och välj **[!UICONTROL Good output]** eller **[!UICONTROL Poor output]** om du vill [skicka feedback](/help/user-guide/create/manage-variants.md#generation-feedback) om kvaliteten på genereringsutdata.

## Verifiera justering av innehållskontroll

Om du vill optimera de genererade varianterna och säkerställa strikt efterlevnad av varumärkesidentitet, plattformsriktlinjer och tillgänglighetsstandarder, kan du utnyttja kraften i [_innehållskontrollpanelen_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Den här panelen visar omfattande detaljer för innehållskontroll och lyser upp förbättringsområden.

**Så här utför du innehållskontroller på en variant**:

1. Klicka på panelikonen _Innehållskontroll_ i det högra åtgärdsfältet för att öppna panelen [_Innehållskontroll_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Visa en sammanfattning av kontrollerna *Behöver granskas* och *Godkänd* för att se vilka avsnitt och riktlinjer som behöver förbättras.

   ![_Innehållskontroll_ panel](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [Granska varianter](#revise-generated-variants) manuellt för att se till att dina varianter är nära justerade med de utförda innehållskontrollerna.

Se [Varumärkesvalidering](/help/user-guide/guidelines/brand-validation.md).

## Få recensioner och godkännanden

Använd panelen Godkännanden, som finns som en ikon i det högra åtgärdsfältet på arbetsytan, för att få granskningar, spåra granskningskommentarer och få godkännanden från intressenter.

**Så här får du granskningar och godkännanden**:

1. [Starta en godkännandebegäran](/help/user-guide/approvals/request-review.md) för att begära ett [godkännande av förberedda Meta-annonsupplevelser](/help/user-guide/approvals/approve-content.md).

   ![Skicka utkast för granskning och godkännande](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [Ta bort eller lägg till granskare](/help/user-guide/approvals/review-and-edit.md#manage-approvals) under granskningsprocessen.
1. [Få åtkomst till innehållet för granskning](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) och visa begäranden om revision.
1. Redigera utkasten per granskningskommentarer och [publicera dina Meta-annonsupplevelser](#publish-and-export-experience).

Mer information finns i [Recensioner och godkännanden](/help/user-guide/approvals/overview.md).

## Publicera och exportera

Om du vill göra de genererade Meta-annonserna tillgängliga för aktuell och framtida användning publicerar du dem på [!UICONTROL Content] och exporterar dem för användning i dina marknadsföringskampanjer.

1. **Om du vill publicera dina nya Meta-annonsupplevelser** klickar du på **[!UICONTROL Publish]** i det övre verktygsfältet eller i godkännandeflödet.
1. **Om du vill exportera dina nya Meta-annonsupplevelser** klickar du på **[!UICONTROL Export]** i det övre verktygsfältet.
   1. Välj format - HTML och bilder eller CSV och bilder (JPG eller PNG) - klicka på **[!UICONTROL Export]**.

Mer information finns i [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).

## Connect Meta

Du kan ansluta GenStudio for Performance Marketing till Meta för att få avancerade analyser och [insikter](/help/user-guide/insights/overview.md) om innehållsprestanda.

Mer information finns i [Anslut kanalkonto](/help/user-guide/insights/connect-channel.md).
