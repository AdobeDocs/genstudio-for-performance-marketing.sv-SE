---
title: Skapa en Meta Ad Experience
description: Lär dig skapa varumärkesanpassade annonsupplevelser för Meta - för Facebook eller Instagram - med Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 42111bbf-70cd-4fd2-a7a9-15abe072d720
source-git-commit: 4658a759f5a4e03c54f645cfa1d1bbcc84fe1d91
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 0%

---

# Skapa en annonsupplevelse från Meta

I den här självstudiekursen visas hur du skapar [annonsupplevelser i Meta](/help/user-guide/create/meta-experiences.md) med GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (penselikonen i det vänstra navigeringsområdet).

Innan du börjar generera en annonsupplevelse från Meta är det viktigt att [införliva riktlinjer](/help/user-guide/guidelines/add-guidelines.md) i GenStudio for Performance Marketing och bekanta dig med grunderna i [att skapa en uppmaning](/help/user-guide/effective-prompts.md).

## Välj en mall

Om du vill börja generera en ny annonsupplevelse från Meta använder du en tillgänglig mall för att skapa ramverket för ditt innehåll. Läs [Meta riktlinjer för annonsmallar](/help/user-guide/templates/meta-template.md) om du vill ha information om vilka Meta-proportioner som stöds.

När du väljer en mall kan du välja mellan att använda en av dina överförda mallar eller en startmall.

**Så här väljer du en Meta-annonsmall**:

1. Klicka på _[!DNL Create]_&#x200B;i **[!UICONTROL Meta ads]**.
1. Välj **[!UICONTROL Custom templates]** om du vill bläddra bland dina överförda mallar eller **[!UICONTROL Starter templates]** om du vill bläddra bland de fördefinierade mallarna.

   Om du tänker lägga till videoresurser i dina Meta-varianter måste du välja en startmall. De är förinlästa med systemdefinierade innehållsområden som underlättar användningen av videoklipp.

1. Klicka för att välja en mall och klicka på **[!UICONTROL Use]**.

   Den här åtgärden öppnar arbetsytan, som är navet för innehållsskapande.

## Lägg till parametrar

Genom att lägga till [riktlinjer](/help/user-guide/guidelines/overview.md) och resurser i _Parametrar_ i snabbredigeringsmodulen förbättras innehållsgenereringsprocessen och det är ett viktigt steg när det gäller att förbereda sig för att generera en Meta-annons.

Om du använder en mall med fördefinierade riktlinjer (som [!DNL Brands], [!DNL Personas] eller [!DNL Products]) gäller dessa riktlinjer för dina varianter. Du kan ändra dem om du vill.

**Så här lägger du till parametrar och resurser**:

1. Klicka på ikonen _Parametrar_ för att expandera promptlådan.
1. I avsnittet _Parametrar_ väljer du riktlinjer -[!DNL Brands], [!DNL Personas] och [!DNL Products] - för att informera om hur du skapar innehåll.

   ![Välj persona](/help/assets/persona-select.png){width="600" zoomable="yes"}

   Om det inte finns några varumärken, profiler eller produkter tillgängliga från dessa menyer [lägger du till riktlinjer i din GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Lägg till innehåll (bilder eller videoklipp) för användning i upplevelsen *och* för att påverka innehållsgenereringen:
   * Klicka på **[!UICONTROL Select from Content]** för att välja resurser från din [!DNL Content]-databas, filtrera och markera en eller flera bilder.

     Om du använder en mall som har ett avsnitt för videoklipp, markeras och filtreras videoinnehållet (.mp4) automatiskt. Hovra över en video för att se en automatiskt uppspelad förhandsvisning.

     ![Välj visuellt innehåll](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

     Om du vill använda resurser från en ansluten [!DNL AEM Assets Content Hub]-databas väljer du en databas i listrutan _Plats_ . Filtrera och markera en eller flera bilder.

   * Du kan också dra och släppa bilder i avsnittet **[!UICONTROL Select from Content]** för att överföra en eller flera nya resurser.

1. Klicka på **[!UICONTROL Use]**.

När du är klar med att lägga till parametrar kan du komprimera promptlådan genom att klicka på ikonen _Parametrar_ igen.

## Ange en uppmaning

När riktlinjerna har valts kan du snabbt skapa innehåll för din nya annonsupplevelse från Meta med hjälp av det naturliga språket. Detaljerade anvisningar ger högre kvalitet än otydliga eller tvetydiga instruktioner.

Läs [Skriv effektiva uppmaningar](/help/user-guide/effective-prompts.md) om du vill veta mer om hur du skriver uppmaningar.

**Så här skriver du en fråga**:

1. Ange en uppmaning i rutan _&quot;Beskriv de upplevelser du vill generera&quot;_ .
1. Klicka på **[!UICONTROL Generate]**.

   Se [Hantera videoklipp](#manage-videos) om du vill veta hur de genereras och hur du hanterar dem.

Som standard genereras och visas fyra varianter på arbetsytan, som alla föds av uppmaningen, riktlinjer och innehåll som du har lagt till.

Genererat innehåll läses in progressivt - allt eftersom varje avsnitt i Meta-upplevelsen genereras visas det på arbetsytan. Se [Meta-upplevelser](/help/user-guide/create/meta-experiences.md#progressive-loading) om du vill veta hur dessa ändringar läses in på arbetsytan.

## Välj Meta annonskanal

När du skapar en Meta-annons kan du välja mellan Facebook- eller Instagram-annonser.

Växla kanalalternativet Meta-annonser - mellan **Facebook** och **Instagram** - på den högra menyraden (Facebook- och Instagram-ikoner) för att visa och hantera varianter för varje kanal.

När du [ändrar Meta-annonser](#revise-generated-variants) kan du ändra proportionerna för Facebook- och Instagram-annonser.

## Ändra genererade varianter

Innan du väljer vad som ska skickas för godkännande eller publicering till [!DNL Content] kan du redigera Meta-annonserna eller ta bort en variant från uppsättningen med genererade annonser.

Om du vill markera ett enskilt lager som ska revideras klickar du på ett redigerbart fält eller bild och klickar på _[!UICONTROL View Layers]_.

**Så här granskar du genererade varianter**:

* **Om du vill [redigera namnet på Meta-annonsutkastet](/help/user-guide/create/manage-variants.md#change-draft-name)** klickar du i titeln _Namnlöst utkast_ längst upp på arbetsytan och anger en ny titel.
* **Om du vill [redigera en Meta-annons manuellt](/help/user-guide/create/manage-variants.md#manually-edit-text)** klickar du i något av annonsavsnitten (till exempel ämnesraden,
sidhuvud eller brödtext) och redigera efter behov.
* **Om du vill ändra eller markera call to action** klickar du på knappen call-to-action och väljer bland de tillgängliga knapptextalternativen. Ange en URL för call-to-action-texten i _Länk_.
* **Om du vill [använda textformatering](/help/user-guide/create/manage-variants.md#manually-edit-text)** i en variant klickar du på texten i bilden eller på den infogade länken för en variant och klickar på **[!UICONTROL Format text]**.
<!-- **To [change or select the Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, click the call-to-action button and select _[!UICONTROL Rephrase]_ or _[!UICONTROL Add link]_. -->
* **Om du vill [lägga till en länk till en bild i en variant](/help/user-guide/create/manage-variants.md#add-image-link)** klickar du på en bildresurs (eller bildresursområdet om det inte finns någon bild) och klickar på länkikonen.
* **Om du vill [ändra storlek och proportioner för annonsen](/help/user-guide/create/manage-variants.md#change-aspect-ratio)** klickar du på knappen _[!UICONTROL Resize]_(ruta med en knappikon till vänster om arbetsytan) och väljer en ny storlek och proportioner som ska användas för alla varianter. Varianterna dupliceras och storleksändras.
* **Om du vill [återskapa ett avsnitt av en variant](/help/user-guide/create/manage-variants.md#re-generate-sections)** klickar du på ett redigerbart textfält och använder _[!UICONTROL Suggested edits]_-alternativen eller anger en ny fråga och klickar på&#x200B;**[!UICONTROL Generate]**.
* **Om du vill [lägga till eller byta ut bilder i en variant](/help/user-guide/create/manage-variants.md#swap-image)** klickar du på en bildresurs (eller bildresursområdet om det inte finns någon bild) och sedan på ikonen **[!UICONTROL Swap from content]** .
* **Om du vill [beskära eller flytta bilder](/help/user-guide/create/manage-variants.md#crop-assets)** klickar du på en bild, klickar på **[!UICONTROL Edit]** (pennikonen) och sedan **[!UICONTROL Crop]**. Justera bildens storlek och placering.
* **Om du vill [använda Generativ utökning för att ändra storlek på och anpassa bilder](/help/user-guide/create/manage-variants.md#use-generative-expand) till din arbetsmall** klickar du på en bild, klickar på **[!UICONTROL Edit]** (pennikon) och sedan **[!UICONTROL Expand]**. Justera bilden så att den passar proportionerna och mallen.
* **Om du vill [lägga till alternativ text för bilder i en variant](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)** klickar du på en bildresurs och använder alternativet _Alt-text_ för att manuellt lägga till eller generera alternativ text per bild.
* **Om du vill [lägga till hjälpmedelsetiketter](/help/user-guide/create/manage-variants.md#add-accessibility-labels) till dina varianter** klickar du på en bild eller call-to-action-länk och anger sedan en kort beskrivning av vad länken eller knappen gör.
* **Om du vill [ta bort en Meta-annons](/help/user-guide/create/manage-variants.md#delete-variant)** klickar du på alternativmenyn för en variant och sedan på **[!UICONTROL Delete variant]**.

### Hantera videoklipp

Håll pekaren över videoklippen för att se automatisk uppspelning med slinga.

Videoklippen omformas så att de passar de valda proportionerna under genereringen. Återgå till den ursprungliga videon som inte omformats genom att klicka på **[!UICONTROL Reframe Video]** och stänga av den.

## Skicka feedback

Klicka på alternativikonen (tre punkter) och välj [&#x200B; eller &#x200B;](/help/user-guide/create/manage-variants.md#generation-feedback) om du vill **[!UICONTROL Good output]** skicka feedback **[!UICONTROL Poor output]** om kvaliteten på genereringsutdata.

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

1. [Starta en godkännandebegäran](/help/user-guide/approvals/request-review.md) för att begära ett [godkännande av Meta-annonsupplevelser](/help/user-guide/approvals/approve-content.md).

   ![Skicka utkast för granskning och godkännande](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [Ta bort eller lägg till granskare](/help/user-guide/approvals/review-and-edit.md#manage-approvals) under granskningsprocessen.
1. [Få åtkomst till innehållet för granskning](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) och visa begäranden om revision.
1. Redigera utkasten per granskningskommentarer och [publicera dina Meta-annonsupplevelser](#publish-and-export-experience).

Mer information finns i [Recensioner och godkännanden](/help/user-guide/approvals/overview.md).

## Publicera och exportera

Om du vill göra de genererade Meta-annonserna tillgängliga för aktuell och framtida användning publicerar du dem på [!UICONTROL Content] och exporterar dem för användning i dina marknadsföringskampanjer.

1. **Om du vill publicera dina nya annonsupplevelser från Meta** klickar du på **[!UICONTROL Publish]** i det övre verktygsfältet eller i godkännandeflödet.
1. **Om du vill exportera dina nya annonsupplevelser från Meta** klickar du på **[!UICONTROL Export]** i det övre verktygsfältet.
   1. Välj format - HTML och bilder eller CSV och bilder (JPG eller PNG) - klicka på **[!UICONTROL Export]**.

Mer information finns i [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).

## Connect Meta

Du kan ansluta GenStudio for Performance Marketing till Meta för att få avancerade analyser och insikter om innehållets prestanda.

Se [Meta-annonser, anslut](/help/user-guide/connectors/meta-ads.md).
