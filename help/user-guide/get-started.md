---
title: Kom igång med Adobe GenStudio for Performance Marketing
description: Lär dig hur du kommer igång med GenStudio for Performance Marketing för att generera nytt varumärkesanpassat marknadsföringsinnehåll.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: bcb03198-bbcb-45ae-af01-25c1e834b563
source-git-commit: fd49abb491477b0a8ed5b1f646219458efc49365
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 2%

---

# Kom igång med Adobe GenStudio for Performance Marketing

Adobe GenStudio for Performance Marketing har en omfattande verktygslåda som effektiviserar framtagning, hantering och analys av innehåll. Den ger innehållsframtagningen en livscykel med generativa AI-funktioner som förändrar hur marknadsföringsmaterial skapas, granskas, delas och analyseras.

## Börja skapa, dela och granska innehåll

Om du är nybörjare på att skapa AI-baserade verktyg eller bara är nyfiken på GenStudio for Performance Marketing grundprinciper kan du läsa [Koncept](concepts.md) och [Skriv effektiva uppmaningar](effective-prompts.md). Du kan ta en titt på [Adobe GenStudio Academy](https://learningmanager.adobe.com/genstudioacademy), Adobe onlineutbildningsplattform om hur du använder generativa AI-tekniker i den kreativa processen.

## Tåg GenStudio for Performance Marketing

GenStudio for Performance Marketing använder information om ert varumärke och era marknader för att förbättra framtagningen av varumärkesanpassat innehåll. Utbildningsmaterialet innehåller exempel, beskrivningar av kundens [profiler](/help/user-guide/guidelines/personas.md) och [produkter](/help/user-guide/guidelines/products.md) samt [varumärkesriktlinjer](/help/user-guide/guidelines/overview.md).

Systemansvariga skapar Adobe GenStudio for Performance Marketing genom att ange eller överföra organisationsspecifik information. Förberedelsen säkerställer att redaktörer och samarbetspartners effektivt kan använda de generativa AI-funktionerna för att skapa och granska kampanjresurser. När systemadministratören i Adobe förser din organisations produktinstans med behörigheter för GenStudio systemhanterare kan GenStudio systemhanterare förbereda produktens underliggande generativa AI-ramverk med hjälp av riktlinjer.

### Steg 1: Lägg till riktlinjer

Att bygga upp de viktigaste byggstenarna i organisationens varumärkesidentitet är en nödvändig förutsättning för arbete som utförs av redaktörer och samarbetspartners. [Riktlinjer](./guidelines/overview.md) fångar varumärken som logotyper, röstton och färgpaletter. Du kan antingen överföra [[!DNL Brands] riktlinjer](./guidelines/brands.md)-dokument eller ange varumärkesinformation manuellt. [[!DNL Personas] riktlinjer](./guidelines/personas.md) och [[!DNL Products] riktlinjer](./guidelines/products.md) är också viktiga. GenStudio for Performance Marketing underliggande generativa AI-funktioner använder dessa riktlinjer för att skapa skyddsmekanismer som vägleder innehållsgenereringen.

#### Förbered dina riktlinjer

Omfattande och fokuserade riktlinjer för [[!DNL Brands]](./guidelines/brands.md), [[!DNL Products]](./guidelines/products.md) och [[!DNL Personas]](./guidelines/personas.md) definierar kärnaspekter av organisationens marknadsföringskampanjer. GenStudio for Performance Marketing extraherar information från dessa riktlinjer för att börja bygga upp ert varumärke.

Följ dessa metodtips när du förbereder riktlinjer:

* Använd specifikt språk.

* Ta med de bästa exemplen som du hittar om den stil och ton du vill att kampanjresurserna ska innehålla.

* Undvik redundans. Det kan vara frestande att upprepa ett direktiv flera gånger, men redundans i riktlinjerna hjälper inte till att fånga upp och genomföra varumärkesriktlinjerna.

* Identifiera element som du vill att LLM ska exkludera när innehåll genereras (till exempel utropstecken i text).

Du kan överföra stödlinedokument eller läsa dem när du anger information manuellt i GenStudio for Performance Marketing. Se [Lägg till riktlinjer](./guidelines/overview.md) för vägledning om hur du överför eller anger den här informationen.

#### Riktlinjer för ändringar

En GenStudio-systemadministratör kan förbereda produktens underliggande generativa AI-ramverk genom att manuellt ange eller överföra organisationens specifika varumärkeskrav. Även om det är en engångsåtgärd att upprätta en organisations varumärkesriktlinjer kan ni ändra och förbättra dessa riktlinjer baserat på organisationens volatilitet, tillväxt och förändrade marknadsförhållanden.

### Steg 2: Konfigurera ett Adobe Admin Console-projekt för GenStudio [!DNL Brands]

Systemadministratörer måste slutföra ytterligare konfigurationsuppgifter innan medarbetare kan redigera eller skapa [!DNL Brands]. Systemadministratörer i Adobe utför följande uppgifter i Adobe Admin Console:

* Skapa en ny användargrupp som innehåller alla användare som behöver redigera och skapa [!DNL Brands]-berättiganden.

* Skapa ett nytt projekt i Adobe Admin Console.

Se [Tilldela varumärkesbehörigheter](configure-brand-permissions.md).

### Steg 3: Överför mallar

Med mallar går det snabbare att skapa innehåll. En mall innehåller godkända funktioner, t.ex. sidhuvuden och sidfötter, och är optimerad för specifika kanaler. Systemansvariga överför och hanterar vanligtvis mallar för sin organisation. Med hjälp av mallar kan redaktörer snabbt komma igång med att skapa innehåll inom de fastställda gränserna för organisationens varumärke.

Se [Arbeta med mallar](./content/use-templates.md).

### Steg 4: Överför godkända tillgångar

Godkända resurser i [!DNL Content] är tillgängliga för alla GenStudio for Performance Marketing-redigerare. Du kan fylla i [!DNL Content] med resurser som innehållsredigerare kan använda när nya upplevelser eller resurser skapas.

Se [Överför godkända resurser](./content/manage-assets.md).

### Steg 5: Anslut till ett Meta-konto (Facebook)

Konfigurera en anslutning mellan GenStudio for Performance Marketing och företagets sociala konton för att ta emot data från era aktiva marknadsföringskampanjer, resurser och upplevelser. [[!DNL Insights]](./insights/overview.md) innehåller verktyg för att analysera kanalhärledda data. Se [Anslut till ett Meta-konto (Facebook)](./insights/connect-channel.md#meta-ads-connect).
