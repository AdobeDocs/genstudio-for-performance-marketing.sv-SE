---
title: Begär granskningar och godkännanden
description: Begär en granskning av genererat innehåll med Adobe GenStudio for Performance Marketing.
feature: Content Review, Content Management
exl-id: 4d5cb23c-457f-47b6-a265-a283afbc54d4
source-git-commit: ec6b226745ba5b093f9c33246be3a8ed20c84381
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 0%

---

# Begär granskning och godkännande

Vill du bjuda in dina medarbetare att granska en resurs eller upplevelse som du har skapat? Du kan bjuda in intressenter att ge feedback på ett utkast av ditt innehåll med det slutliga målet att godkänna. Endast utsedda godkännare kan godkänna innehållet, men alla granskare kan lägga till och komma åt granskningskommentarer.

Om du har skapat en resurs eller upplevelse kan du be andra i din organisations godkännandekedja att granska och kommentera ditt arbete. Även om en medlem i en GenStudio for Performance Marketing-organisation kan granska ett utkast, är det bara den som är utsedd som kan kommentera eller godkänna utkastet.

## Starta en godkännandebegäran

När du har genererat en mediefil eller upplevelse kan du begära att den ska granskas och godkännas.

**Så här begär du en granskning**:

1. Klicka på knappen **[!UICONTROL Send for approval]** på den övre menyraden på arbetsytan.

   Popup-fönstret _Skicka för godkännande_ öppnas och identifierar det utkast som du begär en granskning för. Om du genererar flera varianter skickas hela arbetsytan för granskning.

1. (Valfritt) Markera fältet _Titel_ om du vill ändra utkastsrubriken. Förslagen ska vara beskrivande, informativa och fokusera på granskningsmålet.

   Om du ändrar titeln här ändras även den underliggande titeln för utkastupplevelsen.

1. Välj godkännare och granskare. När du börjar skriva fyller fältet **[!UICONTROL Approver]** automatiskt i användarnamnet för godkännaren i listan över användare med GenStudio for Performance Marketing-vy och godkännandebehörigheter.

   Knappen **[!UICONTROL Send]** aktiveras när du har angett minst ett godkännarnamn.

1. (Valfritt) Använd kommentarer för att förmedla ytterligare kontext om de resurser som granskas och rikta uppmärksamheten mot specifika detaljer och hänvisningar. Använd `@mentions` för att tagga medarbetare och meddela dem om specifik feedback.

1. Klicka på **[!UICONTROL Send]**.

   I produkt- och e-postmeddelanden aviseras varje utsedd godkännare om att de har innehåll att granska.

## Godkännandepanel

Panelen _Godkännande_ innehåller aktuell statusinformation om granskningsarbetsflödet så snart du startar en godkännandebegäran. Från den här panelen kan du:

* Lägg till eller ta bort granskningsdeltagare.
* Lägg till eller ändra ett meddelande för granskarna.
* Redigera granskningsrubriken.
* Ändra det valfria förfallodatumet.

Om Workfront Proof-integreringen är aktiverad visas statusen för varje godkännandefas i arbetsflöden med flera steg. Om du vill visa kommentarer klickar du på **[!UICONTROL View comments in Workfront]** för att öppna dem i [!DNL Proofing Viewer].

## Starta en godkännandebegäran med Workfront Proof

Workfront Proof förser innehållsredigerare med två primära alternativ för att starta en granskning:

* **Manuella inbjudningar**: Bjud in enskilda godkännare och granskare direkt för att delta i korrekturläsningsprocessen. Den här metoden ger flexibilitet vid arbete med engångsgranskningar.

* **Mallar för godkännande**: Använd fördefinierade mallar som innehåller en lista med granskare och, eventuellt, strukturerade godkännandesteg. Mallarna skapas och hanteras av Workfront Proof-administratören i ett särskilt Workfront-projekt. Mallar hjälper till att standardisera granskningsprocessen och säkerställa enhetlighet mellan team och innehållstyper.

**Så här startar du en granskningscykel genom att bjuda in deltagare manuellt**:

1. Klicka på **[!UICONTROL Request approval]** på arbetsytan.

   Popup-fönstret _Begär godkännande_ öppnas.

1. (Valfritt) Lägg till en titel för din granskningsförfrågan i fältet **[!UICONTROL Title]**.

1. Välj **[!UICONTROL Invite people]**.

1. Ange antingen deltagarens användarnamn eller e-postadress i fältet **[!UICONTROL Add names or emails]**.

   Organisationsmedlemsnamnen visas när du anger text.

1. Välj ett deltagarnamn och välj sedan deras roll: godkännare eller granskare. Som standard tilldelas deltagarna rollen som godkännare.

1. (Valfritt) Under **[!UICONTROL Settings]** tilldelar du ett förfallodatum för ett granskningsbeslut. Det här datumet används inte, men påminner granskarna om den förväntade tidsramen.

1. (Valfritt) Lägg till ett informativt meddelande som ger kontext för granskarna.

1. Klicka på **[!UICONTROL Send]** när du är redo att starta godkännandebegäran.

   Alla granskningsdeltagare meddelas via e-post om att de har tilldelats en granskningsuppgift.

**Så här startar du en granskning med en godkännandemall**:

1. Klicka på **[!UICONTROL Request approval]** på arbetsytan.

   Popup-fönstret _Begär godkännande_ öppnas.

1. (Valfritt) Lägg till en titel för din granskningsförfrågan i fältet **[!UICONTROL Title]**.

1. Välj ett Workfront Proof-projekt i listrutan **[!UICONTROL Project]**.

1. Välj en mall i listrutan **[!UICONTROL Use template]**.

   Popup-fönstret _Begär godkännande_ öppnas med förbestämda deltagare och granskningsfaser. Workfront Proof-administratörer skapar godkännandemallar och tilldelar dem till Workfront-projekt. Det projekt du väljer avgör både mallalternativen och fälten som visas på popup-menyn _Begär godkännande_.

1. (Valfritt) Du kan redigera mallen för användning i det här arbetsflödet för godkännande.

1. (Valfritt) Under **[!UICONTROL Settings]** tilldelar du ett förfallodatum för ett granskningsbeslut. Det här datumet används inte, men påminner granskarna om den förväntade tidsramen.

1. (Valfritt) Lägg till ett informativt meddelande som ger kontext för granskarna. Använd `@mentions` för att tagga medarbetare och meddela dem om specifik feedback.

1. Klicka på **[!UICONTROL Send]** när du är redo att starta godkännandebegäran.

## Få granskningskommentarer

* Klicka på **[!UICONTROL View comments in Workfront]**.

  [!DNL Proofing Viewer] visar korrekturet med alla kommentarer listade till höger om korrekturinnehållet. Om det finns flera kommentarer kan du navigera i listan genom att klicka på navigeringspilarna längst upp till höger. Klicka på en kommentar för att navigera till relevant avsnitt i korrekturet.

## Begär nytt godkännande

Gransknings- och godkännandecyklerna är iterativa. Granskarna föreslår ändringar, och de som skapar innehållet ser över utifrån feedback. Granskarna kan sedan begära en ny granskning innan materialet går vidare till slutligt godkännande och godkännande.

**Så här begär du ett nytt godkännande**:

1. Klicka på knappen **[!UICONTROL Request new approval]** längst upp till höger på arbetsytan.

   Popup-fönstret _Begär nytt godkännande_ öppnas och visar samma fält som popup-fönstret _Begär godkännande_. Statusen för varje fas visas (väntande eller ännu inte startat).

1. (Valfritt) Bjud in nya granskare eller ta bort just nu tilldelade granskare.

1. (Valfritt) Redigera förfallodatumet under _Inställningar_ eller lägg till ett meddelande.

1. Klicka på **[!UICONTROL Send]**.

   I produkt- och e-postmeddelanden aviseras varje utsedd godkännare om att de har innehåll att granska.
