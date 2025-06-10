---
title: Integrering av Workfront Proof med granskning och godkännande
description: Workfront Proof-integrering med Adobe GenStudio for Performance Marketing.
feature: Content Review, Content Management
source-git-commit: f8508ee9440714137141e933cfe0f5761a510c7a
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---

# Workfront Proof-integrering med GenStudio for Performance Marketing

Integrering med Workfront Proof förbättrar GenStudio for Performance Marketing livscykel för granskning och godkännande med avancerade funktioner, inklusive godkännandemallar, arbetsflöden i flera steg och möjligheten att [jämföra korrekturversioner](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs). Denna strukturerade versionshantering säkerställer transparens, spårbarhet och smidigt samarbete under hela granskningens livscykel.

>[!BEGINSHADEBOX]

**Förutsättningar**:

Installera [Adobe Workfront Web Viewer-tillägget](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/review-proofs-in-workfront/review-a-proof/review-proof-in-web-viewer-extension)

>[!ENDSHADEBOX]

Workfront Proof [!DNL Proofing Viewer] är en avancerad arbetsyta för att visa, kommentera och jämföra korrektur. Från [!DNL Proofing Viewer] kan du

* Jämför olika versioner av innehållet
* Lägga till kommentarer och ritmarkeringar i ett korrektur
* Godkänn korrekturet

[!DNL Proofing Viewer] läses in när du klickar på korrektur-URL:en i ditt e-postmeddelande om godkännandebegäran eller i produktmeddelandet. Vyn [!DNL Proofing Viewer] _Mitt nya godkännande_ öppnas. Från den här vyn kan du granska innehåll och ge kommentarer med de viktigaste [!DNL Proofing Viewer] anteckningsverktygen.

Om du vill avsluta [!DNL Proofing Viewer] klickar du på **[!UICONTROL Return to GenStudio]**.

## Genstudio for Performance Marketing and Workfront Proof: feature comparison

I tabellen nedan jämförs GenStudio for Performance Marketing standardfunktioner för granskning och godkännande med de mer avancerade funktioner som är tillgängliga genom Workfront Proof-integreringen.

| Funktion        | GenStudio for Performance Marketing                                                                 | Workfront Proof                                                                 |
|-------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| **Livscykel för utkast/korrektur**        | Utkastinnehållet upphör att gälla vid publicering. | Rollbaserade godkännandekedjor i flera steg med tidsstämplade, beständiga loggar.<br> Alla versioner behålls i oändlighet. |
| **Kommentarer**                | Kommentarerna är kopplade till utkast-ID och tas bort efter publiceringen.                                           | Permanenta kommentarer och kommentarer bevaras för granskning och regelefterlevnad.     |
| **Versioner**           | Utkast behandlas som unika instanser.<br>Ingen jämförelse sida vid sida.                                      | Full versionskontroll med jämförelseverktyg för sida vid sida och övertäckning.        |
| **Projekthantering** | Grundläggande kampanjhantering. | Full livscykelhantering för kampanjer, inklusive anpassning, mallar, rapportering och detaljerade revisioner. |

### Licenser och användarroller

Licenser identifierar uppsättningen användarrättigheter i en produkt. Workfront Proof har fler licenstyper eller användarroller än GenStudio for Performance Marketing. [Proof roles overview](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles) introducerar användarroller som är kopplade till arbetsflödet för granskning och godkännande av Workfront Proof.

| GenStudio for Performance Marketing-licens       | Workfront-licens                 | Beskrivning                                                                                                                                                      |
|---------------------------------------------------|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| GenStudio System Manager                          | Workfront Administrator/Power User | Fullständig tillgång till GenStudio Performance Marketing-funktioner som varumärke, persona och produkthantering. Hanterar arbetsflöden och inställningar. Skapar godkännandemallar. |
| Skapare och redigerare av innehåll (Power user license)   | Korrekturskapare (standardlicens)  | Genererar och skickar innehållsutkast. I språkgranskaren överför resurser och initierar korrektur. Kräver en Workfront Proof-licens.                              |
| Granskare/godkännare (medarbetarlicens)        | Granskare/godkännare                 | Deltar i granskningar i flera steg, lägger till kommentarer och godkänner eller avvisar innehåll.                                                                             |

Adobe systemadministratörer hanterar användaretablering och berättiganden för båda produkterna i Adobe Admin Console.

>[!NOTE]
>
> Workfront Proof tillhandahåller [ytterligare användarroller](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles). Alla roller syns inte i Performance Marketing. Systemet uppfyller dock alla roller som anges i en Workfront Proof-mall.

### Utkast och korrektur

Workfront [!DNL Proofing Viewer] utökar GenStudio for Performance Marketing grundläggande gransknings- och godkännandeprocess med mer strukturerade gransknings- och godkännandefunktioner. De korrektur som granskas i den här integreringen är begränsade till de format som stöds av GenStudio for Performance Marketing.

### Versionskontroll

GenStudio for Performance Marketing stöder inte godkännandemallar, men det gör Workfront Proof. Korrekturens versionsfunktioner förbättrar granskningsprocessen och godkännandeprocessen för GenStudio innehåll avsevärt. Varje inskickat material i korrekturarbetsflödet behandlas som en separat version av innehållsutkastet eller _korrektur_. Korrektur sparas automatiskt och kan jämföras sida vid sida med tidigare versioner. Intressenter kan spåra ändringar, ge exakt feedback och upprätthålla en enhetlig nivå under hela granskningsprocessen. Beviset bevarar en komplett historik över alla kommentarer, beslut och versioner som stöder kraven på revisionsberedskap och regelefterlevnad. Varje version har också stöd för rollbaserade arbetsflöden för godkännande i flera steg, där varje åtgärd - godkännande, avvisning eller kommentarer - är tydligt loggad och tidsstämplad.

### Godkännandemallar

Workfront Proof godkännandemallar innehåller förformaterade steg som kan effektivisera arbetsflödet för korrekturgodkännande. Mallarna innehåller valda granskare och godkännare, korrekturroller och deadlines, vilket ger enhetlighet och effektivitet. Den som skapar en granskning kan välja bland en uppsättning fördefinierade mallar för både enfas- och flerfas-arbetsflöden för godkännande.

Varje steg i arbetsflödesmallen identifierar tilldelade granskare. Alla statusuppdateringar och kommentarer från Workfront Proof-arbetsflödet visas i korrekturläsaren, vilket förbättrar genomskinligheten och samarbetet.

Godkännandemallar har stöd för godkännanden i flera steg, vilket stöder samordning av granskningar från olika grupper av intressenter.

### Kommentar

Granskarna kan klicka direkt på specifika delar av korrekturet för att lämna exakta, kontextuella kommentarer. Alla kommentarer är tidsstämplade och sparade som en del av korrekturens versionshistorik. Kommentarshistorik är inte tillgänglig i GenStudio for Performance Marketing.

Du kan [jämföra två versioner av ett korrektur](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs) för att utvärdera granskningskommentarer och innehåll.

## Meddelanden och påminnelser

Granskare och godkännare får e-postmeddelanden när ett nytt korrektur finns tillgängligt för granskning eller när en pågående granskning har ändrat status.
[Korrekturmeddelanden och påminnelser](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/proof-notifications-and-reminders/proof-notifications-and-reminders/proof-notifications-and-reminders) innehåller en personlig länk till korrekturet, information om korrekturet och dess förlopp genom godkännandeprocessen samt versionsinformation.
