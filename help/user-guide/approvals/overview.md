---
title: Adobe GenStudio for Performance Marketing granskningar och godkännanden
description: Läs mer om GenStudio for Performance Marketing granskning och godkännande.
level: Beginner
feature: Content Review, Content Management
exl-id: c83f47c0-e8ae-4c54-84b3-c50f67d6b3c2
source-git-commit: 7955796949c17f7cd877b115cba45c58cdd614a7
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Adobe GenStudio for Performance Marketing granskningar och godkännanden

Arbetsflödet för granskning och godkännande säkerställer att alla intressenter - från kreativa team till juridiska experter - effektivt kan granska och godkänna kampanjresurser och upplevelser, inklusive generativa AI-producerade varumärkesresurser.

>[!NOTE]
>
> Den här funktionen är också tillgänglig som en [integrering med Adobe Workfront Proof](/help/user-guide/approvals/proof-integration.md). Integrationen ger dig tillgång till provfunktioner i GenStudio for Performance Marketing Canvas. Tack vare integreringen med Workfront Proof får GenStudio for Performance Marketing en mer strukturerad, transparent och samverkansbaserad granskningsprocess, som hjälper teamen att gå från utkast till slutversion med större självförtroende och tydlighet.

## Fördelar med arbetsflödet för granskning och godkännande

* **Stöd för robust, iterativt generativt AI-innehåll**. Att skapa och distribuera varumärkesanpassat innehåll i en organisation är en mycket iterativ process. GenStudio for Performance Marketing generativa AI-funktioner gör det enkelt att snabbt skapa hundratals tillgångsvarianter. Varje granskare kan begära flera ändringar av ett tillgångsutkast innan han eller hon godkänner det. Ju fler granskare, desto fler möjliga iterationer innan alla intressenter kommer överens om en slutgiltig variant.

* **Stöd för kreativ integritet**. Godkännanden skyddar ert varumärkes kreativa integritet genom att de som skapar materialet deltar i godkännandeprocessen. Genom att involvera kreativa intressenter (till exempel innehållsskapare och creative directors) i gransknings- och godkännandeprocessen ser du till att slutresultatet överensstämmer med din vision och varumärkesidentitet.

* **Uppfyller kampanjmålen och de juridiska kraven**. Godkännandeprocessen hjälper till att verifiera att innehållet stöder kampanjmål. Det säkerställer att allt marknadsföringsmaterial följer lagar och förordningar, vilket minimerar riskerna och potentiella rättsliga problem.

* **Integrering med Adobe Workfront Proof**. Användare har tillgång till Workfront Proof kraftfulla gransknings- och godkännandefunktioner inifrån GenStudio for Performance Marketing. Innehåll som granskas i GenStudio for Performance Marketing synkroniseras med Workfront Proof och kommentarer och status bevaras. [Integrationen visar](/help/user-guide/approvals/proof-integration.md) hur Korrektur utökar GenStudio for Performance Marketing arbetsflöde för godkännande.

## Livscykel för granskning och godkännande

De huvudsakliga faserna i arbetsflödet för granskning och godkännande omfattar:

* [Begär granskning och godkännande av innehållet som du har skapat](/help/user-guide/approvals/request-review.md). GenStudio for Performance Marketing effektiviserar processen att begära godkännanden och hantera godkännare. Workfront Proof godkännandemallar kan förenkla detta ännu mer.

* [Granska och redigera innehåll](/help/user-guide/approvals/review-and-edit.md). Meddelanden håller innehållsskaparna i slingan om begärda ändringar och godkännanden. Granskning av innehåll utlöser en automatisk ny godkännandecykel.

* [Godkänn innehåll](/help/user-guide/approvals/approve-content.md). Utsedda godkännare märker innehållet som godkänt eller klart för publicering.

* [Publicera innehåll](/help/user-guide/approvals/publish-content.md). Om du publicerar godkänt innehåll till [!DNL Content] blir det tillgängligt för andra i organisationen att använda eller referera till det.

## Om innehållsutkast

_Utkast_ är preliminära versioner av resurser eller upplevelser som inte har slutfört gransknings- och godkännandeprocessen. Utkaststatus identifierar var utkastet befinner sig i gransknings- och godkännandeprocessen. Ett unikt utkast-ID identifierar varje utkast. Detta ID är giltigt tills ett utkast har godkänts och publicerats till [!DNL Content]. Granskningskommentarer och godkännanden för ett utkast är kopplade till detta enskilda utkast-ID. Det finns ingen versionshantering för GenStudio-innehållsutkast.

När ett utkast slutför gransknings- och godkännandeprocessen och publiceras till [!DNL Content], går utkast-ID ut. GenStudio for Performance Marketing sparar inte tillhörande kommentarer och godkännandestatus. Utkast-URL:en är inte längre giltig.

Utkaststatus fångar statusen för innehållsutkastet när det går igenom gransknings- och godkännandeprocessen. Den GenStudio for Performance Marketing-redigerare som skapade den granskade resursen får ett meddelande om alla begärda ändringar av utkastet eller godkännandena. Godkännare ändrar utkaststatus för att ange om ett utkast behöver ändras ytterligare eller kan godkännas. Alla utsedda godkännare måste godkänna en mediefil eller upplevelse innan den kan publiceras.

Tillgängliga statusvärden för utkast:

**Meddelande**: Innehållsredigeraren har startat gransknings- och godkännandeprocessen genom att meddela godkännarna att ett utkast är klart för granskning.
**Behöver arbete**: Anger att en eller flera godkännare har begärt ändringar av innehållsutkastet. Innehåll med den här statusen kan inte sparas till [!DNL Content].
**Godkänd**: Alla utsedda godkännare har godkänt resursen eller upplevelsen. Innehållsredigeraren kan nu lägga till metadata till resursen eller upplevelsen och spara den i [!DNL Content].

>[!NOTE]
>
> Utkasten motsvarar _korrektur_ för användare av Workfront Proof-integreringen. [Utkast och korrektur](/help/user-guide/approvals/proof-integration.md#drafts-and-proofs) skiljer sig åt när det gäller beständighet och versionshantering.

## Godkännanderoller

_Granskare_ kan lägga till kommentarer men inte godkänna innehåll. Deltagande i granskare är praktiskt men inte nödvändigt. _Godkännare_ måste godkänna innehållet innan det kan gå igenom godkännandeprocessen. Integreringen med Workfront Proof har stöd för ett större antal användarroller.

## Meddelanden

GenStudio for Performance Marketing produktmeddelanden uppdaterar godkännare och innehållsredigerare i realtid om resursstatusändringar och `@mention` kommentarer. Aviseringar ger snabb redigering genom flera gransknings-, redigerings- och godkännandecykler.

Redigerare och godkännare kan registrera sig för att få dessa meddelanden i Slack. Se [Prenumerera på tjänster i Experience Cloud](https://experienceleague.adobe.com/sv/docs/core-services/interface/services/customer-attributes/subscription).

Åtgärder som vidtas av godkännandedeltagare utlöser automatiska meddelanden i produkten och e-postmeddelanden. När du startar en godkännandeprocess får utsedda godkännare meddelanden både via e-post och i produkten. Du hålls kvar i slingan med meddelanden i produkten och e-post när en godkännare lägger till `@mention` kommentarer eller fattar ett beslut. Meddelanden innehåller länkar till innehållsutkastet.

Om du initierade gransknings- och godkännandeprocessen för innehåll meddelas du om alla godkännanden och granskningskommentarer. Godkännare meddelas dock endast om kommentarer som innehåller dem med en `@mention`.
