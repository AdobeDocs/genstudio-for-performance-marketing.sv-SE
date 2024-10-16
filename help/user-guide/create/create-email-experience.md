---
title: Skapa en e-postupplevelse
description: Lär dig hur du skapar e-postupplevelser i Adobe GenStudio för Performance Marketing.
feature: Content, Brands Service, Guidelines, Content Generation, Create, Experiences, Variant Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 34446202-da98-45ff-869a-b43496a477f8
source-git-commit: cb309cbaa81807644ff8ba4a5e8ed4403b935315
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 0%

---

# Skapa en e-postupplevelse

I den här självstudiekursen visas hur du skapar [varumärkesprofilerade e-postupplevelser](/help/user-guide/create/email-experiences.md) med GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (penselikonen i det vänstra navigeringsområdet).

Om du vill skapa en effektiv e-postupplevelse rekommenderar vi att du [lägger till riktlinjer i GenStudio för Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) och penselredigerar [grunderna för att skapa en fråga](/help/user-guide/effective-prompts.md) innan du börjar.

## Välj en mall

Om du vill skapa en ny e-postupplevelse kan du använda en tillgänglig mall för att tillhandahålla ramverket för ditt innehåll.

**Så här väljer du en e-postmall**:

1. I _[!DNL Create]_klickar du på&#x200B;**[!UICONTROL Email]**i_&quot;Vad vill du skapa idag?&quot;avsnittet _.
1. Använd sökalternativet bredvid _Filter_ för att hitta en viss e-postmall.
1. Klicka för att välja en e-postmall och klicka på **[!UICONTROL Use]**.

   Arbetsytan, innehållscenter, visas.

## Lägg till parametrar

Om du lägger till [riktlinjer](/help/user-guide/guidelines/overview.md) och resurser i _Parametrar_ i snabbredigeringsmodulen läggs innehållsgenereringsprocessen ovanpå och det är ett viktigt förberedelsesteg för att skapa en e-postupplevelse.

**Så här lägger du till parametrar och resurser**:

1. Klicka på ikonen _Parametrar_ för att expandera promptlådan.
1. I avsnittet _Parametrar_ väljer du riktlinjer -[!DNL Brands], [!DNL Personas] och [!DNL Products] - för att informera om hur du skapar innehåll.

   Om det inte finns några varumärken, profiler eller produkter tillgängliga från dessa menyer [lägger du till riktlinjer i din GenStudio för Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Lägg till innehåll som ska användas i upplevelsen *och* för att påverka innehållsgenereringen:
   * Klicka på **[!UICONTROL Select from Content]** om du vill välja resurser (bilder) från din [!DNL Content]-databas, filtrera och markera en eller flera bilder.

     Om du vill använda resurser från en ansluten [!DNL AEM Assets Content Hub]-databas väljer du en databas i listrutan _Plats_ . Filtrera och markera en eller flera bilder.

   * Du kan också dra och släppa resurser i avsnittet **[!UICONTROL Select from Content]** för att överföra en eller flera nya resurser.
1. Klicka på **[!UICONTROL Use]**.

>[!NOTE]
>
>Om din e-postmall har flera avsnitt väljer du [!DNL Products] och innehåll (visuella resurser) för varje e-postavsnitt i _Fleravsnittsmeddelanden_. E-postmeddelanden med flera avsnitt har stöd för en visuell resurs per avsnitt. Du kan bara lägga till visuella resurser i e-postmeddelanden med flera avsnitt från [!DNL Content]. Du kan inte dra och släppa eller överföra resurser från den lokala källan.

När du är klar med att lägga till parametrar kan du komprimera promptlådan genom att klicka på ikonen _Parametrar_ igen.

## Ange en uppmaning

När du har valt riktlinjer kan du snabbt börja generera innehåll för din nya e-postupplevelse med det naturliga språket. Detaljerade uppmaningar ger högre kvalitet än otydliga eller obeskrivliga uppmaningar.

Läs [Skriv effektiva uppmaningar](/help/user-guide/effective-prompts.md) om du vill veta mer om hur du skriver uppmaningar.

**Så här skriver du en fråga**:

1. Ange en uppmaning i rutan _&quot;Beskriv de upplevelser du vill generera&quot;_ .
1. Klicka på **[!UICONTROL Generate]**.

Som standard genereras och visas fyra varianter på arbetsytan, som alla föds av uppmaningen, riktlinjer och innehåll som du har lagt till.

Genererat innehåll läses in stegvis - allt eftersom varje avsnitt i e-postupplevelsen genereras visas det på arbetsytan. Se [E-postupplevelser](/help/user-guide/create/meta-experiences.md#progressive-loading) om du vill veta hur ändringarna läses in på arbetsytan.

## Granska genererade e-postmeddelanden

Innan du väljer vad som ska skickas för godkännande eller publicering till [!DNL Content] kan du redigera e-postavsnitt eller ta bort en variant från uppsättningen genererade e-postmeddelanden.

**Så här granskar du genererade varianter**:

* **Om du vill [redigera namnet på e-postutkastet](/help/user-guide/create/manage-variants.md#change-draft-name)** klickar du på rubriken _Namnlöst utkast_ längst upp på arbetsytan och anger en ny titel.
* **Om du vill [redigera ett e-postmeddelande manuellt](/help/user-guide/create/manage-variants.md#manually-edit-text)** dubbelklickar du i något av de redigerbara textfälten (till exempel ämnesraden, huvudet eller kopian) och redigerar efter behov
* **Om du vill [återskapa ett avsnitt av en variant](/help/user-guide/create/manage-variants.md#re-generate-sections)** klickar du på ett redigerbart textfält och använder _[!UICONTROL Suggested edits]_-alternativen eller anger en ny fråga och klickar på&#x200B;**[!UICONTROL Generate]**.
* **Om du vill [lägga till eller byta ut bilder i en variant](/help/user-guide/create/manage-variants.md#swap-image)** klickar du på en bildresurs (eller bildresursområdet om det inte finns någon bild) och sedan på **[!UICONTROL Select/swap from content]** eller **[!UICONTROL Upload New Image]** för att lägga till eller byta ut en bild i en enskild variant.
* **Om du vill [ta bort ett e-postmeddelande](/help/user-guide/create/manage-variants.md#delete-variant)** klickar du för att markera e-posttiteln (till exempel&quot;E-post 1/4&quot;) och klickar på **[!UICONTROL Delete variant]**.

## Skicka feedback

Klicka på alternativikonen (tre punkter) och välj **[!UICONTROL Good output]** eller **[!UICONTROL Poor output]** om du vill [skicka feedback](/help/user-guide/create/manage-variants.md#generation-feedback) om kvaliteten på genereringsutdata.

## Förhandsgranska för enhet

När du granskar och förbereder e-postupplevelser kan du [växla mellan förhandsgranskningar för datorer och mobiler](/help/user-guide/create/manage-variants.md#preview-for-device) för att säkerställa att utkastvarianterna är konsekventa och visuella.

## Verifiera varumärkesjustering

Om du vill optimera de genererade e-postmeddelandena och säkerställa strikt efterlevnad av varumärkesidentiteten kan du utnyttja kraften i kontrollen [_Varumärkesriktlinjer_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) - som ger en sammanfattning av varumärkeskontraktionen för en variant - och [_Varumärkesvalidering_ ](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) - som visar omfattande information om varumärkesvalidering och belysande förbättringsområden.

**Så här verifierar du varumärkesjustering**:

1. Klicka på ikonen [**[!UICONTROL [!DNL Brand] guidelines check]**](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) för en variant och se en sammanfattning av hur varianten fungerar när den kontrolleras mot ditt varumärke.
1. Klicka **[!UICONTROL Review]** _eller_ på valideringsikonen för varumärket i den övre menyraden för att öppna [_Varumärkesvalideringspanelen_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) om du vill ha information om de avsnitt och riktlinjer som behöver förbättras.

1. Växla mellan e-postmeddelanden för att se hur ni kan förbättra det genererade innehållet så att det blir mer varumärkesanpassat.
1. [Granska e-postmeddelanden manuellt](#revise-generated-emails) för att säkerställa att dina e-postmeddelanden är i linje med ditt varumärke.

Se [Varumärkesvalidering](/help/user-guide/guidelines/brand-validation.md).

## Få recensioner och godkännanden

Använd panelen Godkännanden, som finns på den övre menyraden på arbetsytan, för att få granskningskommentarer, spåra granskningskommentarer och få godkännanden från intressenter.

**Så här får du granskningar och godkännanden**:

1. [Starta en godkännandebegäran](/help/user-guide/approvals/request-review.md) för att begära ett [godkännande av utkast till e-postupplevelser](/help/user-guide/approvals/approve-content.md).
1. [Ta bort eller lägg till granskare](/help/user-guide/approvals/review-and-edit.md#manage-approvals) under granskningsprocessen.
1. [Få åtkomst till innehållet för granskning](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) och visa begäranden om revision.
1. Redigera utkasten per granskningskommentarer och [publicera dina e-postupplevelser](#publish-and-export-experience).

Mer information finns i [Recensioner och godkännanden](/help/user-guide/approvals/overview.md).

## Publish och exportupplevelser

Om du vill göra de genererade e-postmeddelandena tillgängliga för aktuell och framtida användning publicerar du dem på [!UICONTROL Content] och exporterar dem för användning i dina marknadsföringskampanjer.

1. **Om du vill publicera dina nya e-postupplevelser** klickar du på **[!UICONTROL Publish]** i det övre verktygsfältet eller i godkännandeflödet.
1. **Om du vill exportera dina nya e-postupplevelser** klickar du på **[!UICONTROL Export]** i det övre verktygsfältet.
   1. Markera formatet (endast CSV och bilder eller HTML) och klicka på **[!UICONTROL Export]**.

Mer information finns i [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
