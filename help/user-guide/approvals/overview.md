---
title: Adobe GenStudio for Performance Marketing granskningar och godkännanden
description: Läs mer om GenStudio for Performance Marketing granskning och godkännande.
feature: Approval
exl-id: c83f47c0-e8ae-4c54-84b3-c50f67d6b3c2
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# Adobe GenStudio for Performance Marketing granskningar och godkännanden

Arbetsflödet för granskning och godkännande säkerställer att alla intressenter - från kreativa team till juridiska experter - effektivt kan granska och godkänna kampanjresurser och upplevelser, inklusive generativa AI-producerade varumärkesresurser.

## [!DNL Review and Approval] fördelar med arbetsflödet

* **Stöd för robust, iterativt generativt AI-innehåll**. Att skapa och distribuera varumärkesanpassat innehåll i en organisation är en mycket iterativ process. GenStudio for Performance Marketing generativa AI-funktioner gör det enkelt att snabbt skapa hundratals tillgångsvarianter. Varje granskare kan begära flera ändringar av ett tillgångsutkast innan han eller hon godkänner det. Ju fler granskare, desto fler möjliga iterationer innan alla intressenter kommer överens om en slutgiltig variant.

* **Stöd för kreativ integritet**. Godkännanden skyddar ert varumärkes kreativa integritet genom att de som skapar materialet deltar i godkännandeprocessen. Genom att involvera kreativa intressenter (till exempel innehållsskapare och creative directors) i gransknings- och godkännandeprocessen ser du till att slutresultatet överensstämmer med din vision och varumärkesidentitet.

* **Följer Campaign-målen och de juridiska kraven**. Godkännandeprocessen hjälper till att verifiera att innehållet stöder kampanjmål. Det säkerställer att allt marknadsföringsmaterial följer lagar och förordningar, vilket minimerar riskerna och potentiella rättsliga problem.

## Livscykel för granskning och godkännande

De huvudsakliga faserna i arbetsflödet för granskning och godkännande omfattar:

* [Begär granskning och godkännande av innehåll som du har skapat](./request-review.md)
* [Granska och redigera innehåll](./review-and-edit.md)
* [Godkänn innehåll](./approve-content.md)
* [Publish-innehåll](./publish-content.md)

## Vem kan begära en granskning eller godkänna innehåll?

Om du har skapat en resurs eller upplevelse kan du be andra i din organisations godkännandekedja att formellt granska och kommentera ditt arbete. Även om en medlem i en GenStudio for Performance Marketing-organisation kan granska ett utkast, är det bara den som är utsedd som kan kommentera eller godkänna utkastet.

## Om [!DNL Content] utkast

_Utkast_ är preliminära versioner av resurser eller upplevelser som inte har genomgått gransknings- och godkännandeprocessen. Utkaststatus identifierar var utkastet befinner sig i gransknings- och godkännandeprocessen. Ett unikt utkast-ID identifierar varje utkast. Det här ID:t är giltigt tills ett utkast har godkänts och publicerats till [!DNL Content]. Granskningskommentarer och godkännanden för ett utkast är kopplade till detta enskilda utkast-ID.

När ett utkast slutför gransknings- och godkännandeprocessen och publiceras till [!DNL Content], förfaller utkast-ID:t och GenStudio for Performance Marketing sparar inte associerade kommentarer och godkännandestatus. Utkast-URL:en är inte längre giltig.

Utkaststatus fångar statusen för innehållsutkastet när det går igenom gransknings- och godkännandeprocessen. Den GenStudio for Performance Marketing-redigerare som skapade den granskade resursen får ett meddelande om alla begärda ändringar av utkastet eller godkännandena. Godkännare ändrar utkaststatus för att ange om ett utkast behöver ändras ytterligare eller kan godkännas. Alla utsedda godkännare måste godkänna en mediefil eller upplevelse innan den kan publiceras.

Tillgängliga statusvärden för utkast:

**Meddelande**: Innehållsredigeraren har startat gransknings- och godkännandeprocessen genom att meddela godkännarna att ett utkast är klart för granskning.
**Behöver arbete**: Anger att en eller flera godkännare har begärt ändringar av innehållsutkastet. Innehåll med den här statusen kan inte sparas till [!DNL Content].
**Godkänd**: Alla utsedda godkännare har godkänt resursen eller upplevelsen. Innehållsredigeraren kan nu lägga till metadata till resursen eller upplevelsen och spara den i [!DNL Content].

## Meddelanden

GenStudio for Performance Marketing produktmeddelanden uppdaterar godkännare och innehållsredigerare i realtid om resursstatusändringar och `@mention` kommentarer. Aviseringar ger snabb redigering genom flera gransknings-, redigerings- och godkännandecykler.

Innehållsredigerare och godkännare kan registrera sig för att få dessa meddelanden i Slack. Se [Prenumerera på tjänster i Experience Cloud](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences#slack).

Åtgärder som vidtas av godkännandedeltagare utlöser automatiska meddelanden i produkten och e-postmeddelanden. När du startar en godkännandeprocess får utsedda godkännare meddelanden både via e-post och i produkten. Du hålls kvar i slingan med meddelanden i produkten och e-post när en godkännare lägger till `@mention` kommentarer eller fattar ett beslut. Meddelanden innehåller länkar till innehållsutkastet.

Om du initierade gransknings- och godkännandeprocessen för innehåll meddelas du om alla godkännanden och granskningskommentarer. Godkännare meddelas dock endast om kommentarer som innehåller dem med en `@mention`.
