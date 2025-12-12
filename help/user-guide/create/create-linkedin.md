---
title: Skapa en länkad upplevelse
description: Lär dig skapa varumärkeskompatibla LinkedIn-upplevelser med Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
badgeBeta: label="Beta" tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."
recommendations: noDisplay
exl-id: abe10fc8-d6d5-4cad-9273-400b622f22b7
source-git-commit: 6c2a8ca1fd981bc4f6eb15f1487b304c0c8f67b4
workflow-type: tm+mt
source-wordcount: '1183'
ht-degree: 0%

---

# Skapa en länkad upplevelse

I den här självstudien visas hur du skapar [LinkedIn-upplevelser](/help/user-guide/create/meta-experiences.md) som följer varumärkesriktlinjerna med GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (penselikonen i det vänstra navigeringsområdet).

Innan du börjar generera en LinkedIn-annons är det viktigt att [lägga till riktlinjer](/help/user-guide/guidelines/add-guidelines.md) i GenStudio for Performance Marketing och lära dig grunderna i [att skapa en uppmaning](/help/user-guide/effective-prompts.md).

## Välj en mall

Om du vill generera en ny LinkedIn-upplevelse behöver du en mall som anger ramverket för ditt innehåll. Mer information om LinkedIn-proportioner som stöds finns i [LinkedIn-mallriktlinjer](/help/user-guide/templates/linkedin-template.md).

Du kan välja i listan över egna mallar eller välja en startmall.

**Så här väljer du en LinkedIn-mall**:

1. Klicka på _[!DNL Create]_i **[!UICONTROL LinkedIn]**.
1. Välj **[!UICONTROL Custom templates]** om du vill bläddra bland dina överförda mallar eller **[!UICONTROL Starter templates]** om du vill bläddra bland de fördefinierade mallarna.

   Om du tänker lägga till videoresurser i dina Meta-varianter måste du välja en startmall. De är förinlästa med systemdefinierade innehållsområden som underlättar användningen av videoklipp.

1. Klicka för att välja en mall och klicka sedan på **[!UICONTROL Use]**.

   Den här åtgärden öppnar arbetsytan, som är navet för innehållsskapande.

## Lägg till parametrar

Genom att lägga till [riktlinjer](/help/user-guide/guidelines/overview.md) och resurser i _Parametrar_ i snabbredigeringsmodulen förbättras innehållsgenereringsprocessen och det är ett viktigt steg när det gäller att förbereda sig för att generera en LinkedIn-upplevelse.

**Så här lägger du till parametrar och resurser**:

1. Klicka på ikonen _Parametrar_ för att expandera promptlådan.
1. I avsnittet _Parametrar_ väljer du riktlinjer -[!DNL Brands], [!DNL Personas] och [!DNL Products] - för att informera om hur du skapar innehåll.

   ![Välj persona](/help/assets/persona-select.png){width="600" zoomable="yes"}

   Om det inte finns några varumärken, profiler eller produkter tillgängliga från dessa menyer [lägger du till riktlinjer i din GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Lägg till innehåll (bilder eller videoklipp) för användning i upplevelsen *och* för att påverka innehållsgenereringen genom att klicka på **[!UICONTROL Select from Content]**. Du kan också dra och släppa bilder i avsnittet **[!UICONTROL Select from Content]** för att överföra en eller flera nya resurser.

   Använd filtret för att söka efter innehåll och markera en eller flera bilder.

   Om du använder en mall som har ett avsnitt för videoklipp, markeras och filtreras videoinnehållet (.mp4) automatiskt. Hovra över en video för att se en automatiskt uppspelad förhandsvisning.

   ![Välj visuellt innehåll](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

   Om du vill använda resurser från en ansluten [!DNL AEM Assets Content Hub]-databas väljer du en databas i listrutan _Plats_ . Filtrera och markera en eller flera bilder.

1. Klicka på **[!UICONTROL Use]**.

När du är klar med att lägga till parametrar kan du komprimera promptlådan genom att klicka på ikonen _Parametrar_ igen.

## Ange en uppmaning

När du har valt riktlinjer kan du snabbt skapa innehåll för din nya LinkedIn-upplevelse med ett naturligt språk. Detaljerade anvisningar säkerställer att du får bra kvalitet och användbara resultat.

Läs [Skriv effektiva uppmaningar](/help/user-guide/effective-prompts.md) om du vill veta mer om hur du skriver uppmaningar.

**Så här skriver du en fråga**:

1. Ange en uppmaning i rutan _&quot;Beskriv de upplevelser du vill generera&quot;_ .
1. Klicka på **[!UICONTROL Generate]**.

   Se [Hantera videoklipp](#manage-videos) om du vill veta hur de genereras och hur du hanterar dem.

Som standard genereras och visas fyra varianter på arbetsytan, som alla föds av uppmaningen, riktlinjer och innehåll som du har lagt till.

Genererat innehåll läses in progressivt - allt eftersom varje avsnitt i LinkedIn-upplevelsen genereras visas det på arbetsytan. Mer information om hur ändringarna läses in på arbetsytan finns i [LinkedIn-upplevelser](/help/user-guide/create/linkedin-experiences.md#progressive-loading) .

## Granska genererade LinkedIn-annonser

Innan du skickar varianter för godkännande eller publicering till [!DNL Content] kan du redigera LinkedIn-annonserna eller ta bort en variant från uppsättningen med genererade annonser.

**Så här granskar du genererade varianter**:

* **Om du vill [redigera namnet på LinkedIn och utkastet](/help/user-guide/create/manage-variants.md#change-draft-name)** klickar du i titeln _Namnlöst utkast_ högst upp på arbetsytan och anger en ny titel.
* **Om du vill [redigera en LinkedIn-annons manuellt](/help/user-guide/create/manage-variants.md#manually-edit-text)** klickar du i något av annonsavsnitten (till exempel ämnesraden, huvudet eller brödtexten) och redigerar efter behov.
* **Om du vill ändra eller markera call to action** klickar du på knappen call-to-action och väljer bland de tillgängliga knapptextalternativen. Ange en URL för call-to-action-texten i _Länk_.
* **Om du vill [använda textformatering](/help/user-guide/create/manage-variants.md#manually-edit-text)** i en variant klickar du på texten i bilden för en variant och sedan på **[!UICONTROL Format text]**.
* **Om du vill [återskapa ett avsnitt av en variant](/help/user-guide/create/manage-variants.md#re-generate-sections)** klickar du på ett redigerbart textfält och använder _[!UICONTROL Suggested edits]_-alternativen eller anger en ny uppmaning i [!UICONTROL Generate new text_ section] och klickar på&#x200B;**[!UICONTROL Generate]**.
* **Om du vill [använda Generativ utökning för att ändra storlek på och anpassa bilder](/help/user-guide/create/manage-variants.md#use-generative-expand) till din arbetsmall** klickar du på en bild, klickar på **[!UICONTROL Edit]** (pennikon) och sedan **[!UICONTROL Expand]**. Justera bilden så att den passar proportionerna och mallen.
* **Om du vill [beskära eller flytta bilder](/help/user-guide/create/manage-variants.md#crop-assets)** håller du pekaren över en bild, klickar på beskärningsikonen som visas och justerar bildens storlek och placering.
* **Om du vill [ändra storlek och proportioner för annonsen](/help/user-guide/create/manage-variants.md#change-aspect-ratio)** klickar du på knappen _[!UICONTROL Resize]_(ruta med en knappikon till vänster om arbetsytan) och väljer en ny storlek och proportioner som ska användas för alla varianter. Varianterna dupliceras och storleksändras.
* **Om du vill [lägga till eller byta ut resurser (bild eller video) i en variant](/help/user-guide/create/manage-variants.md#swap-image)** klickar du på en resurs (eller resursområdet) och sedan på ikonen **[!UICONTROL Swap from content]** .
* **Om du vill [lägga till alternativ text för bilder i en variant](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)** klickar du på en bildresurs och använder alternativet _Alt-text_ för att manuellt lägga till eller generera alternativ text per bild.
* **Om du vill [lägga till hjälpmedelsetiketter](/help/user-guide/create/manage-variants.md#add-accessibility-labels) till dina varianter** klickar du på en bild eller call-to-action-länk och anger sedan en kort beskrivning av vad länken eller knappen gör.
* **Om du vill [ta bort en LinkedIn-annons](/help/user-guide/create/manage-variants.md#delete-variant)** klickar du på alternativmenyn för en variant och sedan på **[!UICONTROL Delete variant]**.

### Hantera videoklipp

Håll pekaren över videoklippen för att se automatisk uppspelning med slinga.

Videoklippen omformas så att de passar de valda proportionerna under genereringen. Återgå till den ursprungliga videon som inte omformats genom att klicka på **[!UICONTROL Reframe Video]** och stänga av den.

## Skicka feedback

Klicka på alternativikonen (tre punkter) och välj [ eller ](/help/user-guide/create/manage-variants.md#generation-feedback) om du vill **[!UICONTROL Good output]** skicka feedback **[!UICONTROL Poor output]** om kvaliteten på genereringsutdata.

## Verifiera justering av innehållskontroll

Om du vill optimera de genererade varianterna och säkerställa strikt efterlevnad av varumärkesidentitet, plattformsriktlinjer och tillgänglighetsstandarder, kan du utnyttja kraften i [_innehållskontrollpanelen_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Den här panelen visar omfattande detaljer för innehållskontroll och lyser upp förbättringsområden.

**Så här utför du innehållskontroller på en variant**:

1. Klicka på panelikonen _Innehållskontroll_ i det högra åtgärdsfältet för att öppna panelen [_Innehållskontroll_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Visa en sammanfattning av kontrollerna *Behöver granskas* och *Godkänd* för att se vilka avsnitt och riktlinjer som behöver förbättras.

   ![_Innehållskontroll_ panel](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [Granska varianter](#revise-generated-linkedin-ads) manuellt för att se till att dina varianter är nära justerade med de slutförda innehållskontrollerna.

Se [Varumärkesvalidering](/help/user-guide/guidelines/brand-validation.md).

## Få recensioner och godkännanden

Använd panelen Godkännanden, som finns på den övre menyraden på arbetsytan, för att få granskningskommentarer, spåra granskningskommentarer och få godkännanden från intressenter.

**Så här får du granskningar och godkännanden**:

1. [Starta en godkännandebegäran](/help/user-guide/approvals/request-review.md) för att begära ett [godkännande av Meta-annonsupplevelser](/help/user-guide/approvals/approve-content.md).

   ![Skicka utkast för granskning och godkännande](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [Ta bort eller lägg till granskare](/help/user-guide/approvals/review-and-edit.md#manage-approvals) under granskningsprocessen.
1. [Få åtkomst till innehållet för granskning](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) och visa begäranden om revision.
1. Redigera utkasten per granskningskommentarer och [publicera dina Meta-annonsupplevelser](#publish-and-export-experience).

Mer information finns i [Recensioner och godkännanden](/help/user-guide/approvals/overview.md).

## Publicera och exportera

Om du vill göra de genererade LinkedIn-annonserna tillgängliga för aktuell och framtida användning publicerar du dem på [!UICONTROL Content] och exporterar dem för användning i dina marknadsföringskampanjer.

1. **Om du vill publicera dina nya upplevelser** klickar du på **[!UICONTROL Publish]** i det övre verktygsfältet eller i godkännandeflödet.
1. **Om du vill exportera dina nya upplevelser** klickar du på **[!UICONTROL Export]** i det övre verktygsfältet.
   1. Markera formatet - JPG, PNG eller GIF - och klicka på **[!UICONTROL Export]**.

Mer information finns i [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
