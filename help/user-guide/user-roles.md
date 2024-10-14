---
title: Adobe GenStudio for Performance Marketing användarroller och behörigheter
description: Läs om GenStudio for Performance Marketing användarroller och behörigheter.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
source-git-commit: 3e9a2a4f42ba79389691705c571bf6bbd0b990c5
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Användarroller och behörigheter

Att skapa och driftsätta moderna marknadsföringskampanjer kräver samarbete mellan intressenter med varierande ansvarsområden och kompetenser. _Användarroller_ styr intressenternas åtkomst till GenStudio for Performance Marketing många funktioner. Din tilldelade användarroll avgör vilka uppgifter du kan utföra med den här plattformen. En Adobe-systemadministratör tilldelar dig en roll i GenStudio produktprofil i Adobe Admin Console. Ditt välkomstmeddelande identifierar din tilldelade roll.

>[!NOTE]
>
>Innan några användare etableras i de här rollerna måste en Adobe-systemadministratör utses i Adobe Admin Console för att kunna utföra engångsinstallationsuppgifter. Administratörsrollen för Adobe fungerar endast i Adobe Admin Console. Den har ingen roll i GenStudio for Performance Marketing plattformsgränssnitt. En systemadministratör i Adobe som behöver systemhanterarrättigheter måste etablera sig som GenStudio systemadministratör i Adobe Admin Console. Se [Etablera GenStudio for Performance Marketing](product-provisioning.md).

## Berättiganden

_Tillstånd_ ger behörighet att utföra specifika uppgifter och få åtkomst till skyddade resurser. Tillstånd definieras i användarrollen i produktprofilen och användarna får dessa rättigheter när de tilldelas till den rollen.

## Användarroller

Tre typer av GenStudio for Performance Marketing användarroller stöder denna mångfald av organisationsroller. Behörigheterna är skräddarsydda för var och en av dessa användartyper och stöder varje användares ansvar i marknadsföringsorganisationen. Följande tre användarrolltyper är:

* **GenStudio-redigerare** använder GenStudio for Performance Marketing generativa AI-funktioner för att skapa marknadsföringskampanjresurser, begära granskning och godkännande av innehåll och publicera godkända utkast av det här innehållet. Alla GenStudio for Performance Marketing-användare kan komma åt och använda en resurs när redigeraren har sparat den i [!DNL Content].

* **GenStudio-medarbetare** är ett stort antal GenStudio for Performance Marketing-användare. Medarbetare kan visa och godkänna innehåll och är en viktig del av arbetsflödet som säkerställer att det innehåll du genererar matchar organisationens behov och standarder.

* **GenStudio systemhanterare** har den bredaste uppsättningen behörigheter i GenStudio for Performance Marketing. Systemansvariga utför den grundläggande startuppgiften att skapa skyddsutkast för att skapa och driftsätta kampanjresurser. Systemansvariga implementerar skyddsprofilerna genom att överföra varumärkes- och organisationsspecifik information, till exempel [varumärkesriktlinjer](./guidelines/overview.md). Systemhanterare har behörighet att skapa och publicera [!DNL Brands], men inte behörighet för användaradministration.

### GenStudio Editors

_Redigerare_, eller innehållsskapare, har de grundläggande behörigheter som krävs för att skapa GenStudio for Performance Marketing [!DNL Brands]-, [!DNL Campaigns]- och [!DNL Content]-resurser. De kan också redigera och ta bort resurser som de har skapat. GenStudio for Performance Marketing har stöd för att snabbt skapa hundratals innehållsdelar. Dessa användare kan generera innehållsfragment eller hela upplevelser som orkestrerar separata delar av godkänt innehåll för specifika marknadsföringskampanjer.

Redigerare interagerar med GenStudio for Performance Marketing generativa AI-tekniker genom att _fråga_. Frågekursen på arbetsytan innehåller verktyg som du kan använda för att ställa frågor i samband med en viss kampanjs riktlinjer. Därför beror kvaliteten och framgången för det genererade innehållet delvis på kvaliteten på de varumärkesriktlinjer som organisationen har överfört och på hur specifik uppmaningen är. Se [Skriv aktuella uppmaningar](effective-prompts.md).

I följande tabell visas standardredigerarens behörigheter:

| Funktion | Skapa | Uppdatera | Ta bort | Visa |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | ja |
| [!DNL Campaigns] | ja | ja | ja | ja |
| [!DNL Content] | ja | ja | ja | ja |
| [!DNL Create] | ja | ja | ja | ja |
| [!DNL Insights] | kan bara konfigurera annonsanslutningar |    |     | ja |
| [!DNL Personas] | ja | ja* | ja* | ja |
| [!DNL Products] | ja | ja* | ja* | ja |
| [!DNL Reviews and approvals] | ja | ja | ja | ja |

Redigerare kan redigera och ta bort [!DNL Personas] och [!DNL Products] som de har skapat.

GenStudio systemhanterare kan ge redigerare behörighet att redigera och ta bort en [!DNL Brand].

### GenStudio medarbetare

_Medarbetare_ kan visa resurser i GenStudio for Performance Marketing men inte skapa, redigera eller ta bort dessa resurser. Medarbetarna arbetar bland annat med intressenter som är viktiga för att gransknings- och godkännandeprocessen ska lyckas, men som inte behöver skapa eller redigera innehåll direkt. Juridiska experter och chefer för kreatörer är exempel på potentiella medarbetare. GenStudio for Performance Marketing medarbetare kan ha behörighet att skapa och visa resurser i andra Creative Cloud-produkter.

I följande tabell visas standardbehörigheter för medarbetare:

| Funktion | Skapa | Uppdatera | Ta bort | Visa |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | ja |
| [!DNL Campaigns] | no | no | no | ja |
| [!DNL Content] | no | no | no | ja |
| [!DNL Create] | no | no | no | ja |
| [!DNL Insights] | no | no | no | ja |
| [!DNL Personas] | no | no | no | ja |
| [!DNL Products] | no | no | no | ja |
| [!DNL Reviews and approvals] | no | no | no | ja |

### GenStudio systemansvariga

_GenStudio systemhanterare_ har den mest kraftfulla uppsättningen behörigheter i GenStudio for Performance Marketing. Systemansvariga utför den grundläggande startuppgiften att skapa skyddsutkast för att skapa och driftsätta kampanjresurser. Systemansvariga implementerar skyddsprofilerna genom att överföra varumärkes- och organisationsspecifik information, till exempel [varumärkesriktlinjer](./guidelines/overview.md). Systemhanterare har behörighet att skapa och publicera [!DNL Brands], men inte behörighet för användaradministration.

I följande tabell visas standardbehörigheterna för systemhanteraren:

| Funktion | Skapa | Uppdatera | Ta bort | Visa |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | ja | ja | ja | ja |
| [!DNL Campaigns] | ja | ja | ja | ja |
| [!DNL Content] | ja | ja | ja | ja |
| [!DNL Insights] | ja | ja | ja | ja |
| [!DNL Personas] | ja | ja | ja | ja |
| [!DNL Products] | ja | ja | ja | ja |
| [!DNL Reviews and approvals] | ja | ja | ja | ja |

Se [Kom igång med Adobe GenStudio for Performance Marketing](get-started.md) för en översikt över preliminära konfigurationsuppgifter.
