---
title: Adobe GenStudio for Performance Marketing användarroller och behörigheter
description: Läs om GenStudio for Performance Marketing användarroller och behörigheter.
level: Beginner
feature: Generative AI, Guidelines
role: Admin
exl-id: 33ebcf9c-e5f8-4011-b449-5f73d151f221
source-git-commit: a7b1665f9d735dad9f33aa4f92c56088ae85a625
workflow-type: tm+mt
source-wordcount: '1123'
ht-degree: 0%

---

# Användarroller och behörigheter

Att skapa och driftsätta moderna marknadsföringskampanjer kräver samarbete mellan intressenter med varierande ansvarsområden och kompetenser. _Användarroller_ styr intressenternas åtkomst till GenStudio for Performance Marketing många funktioner. Din tilldelade användarroll avgör vilka uppgifter du kan utföra med den här plattformen. En Adobe-systemadministratör tilldelar dig en roll i GenStudio produktprofil i Adobe Admin Console. Ditt välkomstmeddelande identifierar din tilldelade roll.

>[!NOTE]
>
>Innan någon användare etableras i dessa roller måste en Adobe-systemadministratör utses i Adobe Admin Console för att kunna utföra engångsinstallationsåtgärder. Den här Adobe-administratörsrollen fungerar endast i Adobe Admin Console. Den har ingen roll i GenStudio for Performance Marketing plattformsgränssnitt. En Adobe-systemadministratör som behöver systemhanterarrättigheter måste etablera sig som GenStudio-systemadministratör i Adobe Admin Console. Se [Etablera GenStudio for Performance Marketing](product-provisioning.md).

## Adobe systemadministratör jämfört med GenStudio systemadministratör

Dessa användarrolltitlar kan se likadana ut, men de identifierar unika roller som ger berättiganden i olika miljöer.

**Adobe systemadministratörer** har avancerade användarbehörigheter i Adobe Admin Console och utför alla användarhanteringsåtgärder, som att lägga till eller ta bort användare. Den här systemadministratörsrollen ger inga privilegier i GenStudio for Performance Marketing-programmet, vilket förklarar varför Adobe systemadministratörer inte behöver någon licens för GenStudio. Adobe systemadministratörer använder vanligtvis Admin Console för att lägga till och ta bort användarkonton från GenStudio-distributioner och tilldela eller ta bort behörigheter, eller behörigheter, från enskilda användare eller användargrupper.

**GenStudio systemhanterare** är avancerade användare i GenStudio for Performance Marketing men har inte behörighet att utföra åtgärder i Adobe Admin Console. Den här systemhanterarrollen kräver en GenStudio-produktlicens och motsvarar en Power-användare i [Adobe GenStudio for Performance Marketing produktbeskrivning](https://helpx.adobe.com/se/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html). GenStudio systemhanterare har fullständig behörighet till GenStudio for Performance Marketing-funktioner, inklusive att [!DNL Brands], [!DNL Persona] och [!DNL Product] har skapats, tagits bort, uppdaterats och publicerats. [Adobe GenStudio for Performance Marketing produktbeskrivning](https://helpx.adobe.com/se/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) förklarar hur GenStudio användarroller relaterar till produktlicenser.

Se [Administrativa roller](https://helpx.adobe.com/se/enterprise/using/admin-roles.html#enterprise) i _Administrationsguide för Enterprise och Teams_.

## Berättiganden

_Tillstånd_ ger behörighet att utföra specifika uppgifter och få åtkomst till skyddade resurser. Tillstånd, eller behörigheter, definieras i användarrollen i produktprofilen och användarna får dessa rättigheter när de tilldelas till den rollen.

>[!IMPORTANT]
>
>Lägg inte till nya, eller redigera eller ta bort, befintliga produktprofiler. Om du ändrar standardproduktprofilerna kan det allvarligt störa driftsättningen av GenStudio for Performance Marketing.

## Användarroller

Tre typer av GenStudio for Performance Marketing användarroller stöder denna mångfald av organisationsroller. Berättigandet är skräddarsytt för var och en av dessa användartyper och stöder varje användares ansvar i marknadsföringsorganisationen. Följande tre användarrolltyper är:

* **GenStudio-redigerare** använder GenStudio for Performance Marketing generativa AI-funktioner för att skapa marknadsföringskampanjresurser, begära granskning och godkännande av innehåll och publicera godkända utkast av det här innehållet. Alla GenStudio for Performance Marketing-användare kan komma åt och använda en resurs när redigeraren har sparat den i [!DNL Content]. GenStudio redigerare är kraftfulla användare i GenStudio for Performance Marketing.

* **GenStudio-medarbetare** är ett stort antal GenStudio for Performance Marketing-användare. Medarbetare kan visa och godkänna innehåll och är en viktig del av arbetsflödet som säkerställer att det innehåll du genererar matchar organisationens behov och standarder. GenStudio medarbetare är _medarbetaranvändare_ i GenStudio for Performance Marketing.

* **GenStudio systemhanterare** har den bredaste uppsättningen behörigheter, eller behörigheter, inom GenStudio for Performance Marketing. Systemansvariga utför den grundläggande startuppgiften att skapa skyddsutkast för att skapa och driftsätta kampanjresurser. Systemansvariga implementerar skyddsprofilerna genom att överföra varumärkes- och organisationsspecifik information, till exempel [varumärkesriktlinjer](./guidelines/overview.md). Systemhanterare har behörighet att skapa och publicera [!DNL Brands], men inte behörighet för användaradministration. GenStudio systemansvariga är kraftfulla användare i GenStudio for Performance Marketing.

### GenStudio Editors

_Redigerare_, eller innehållsskapare, har de grundläggande behörigheter som krävs för att skapa GenStudio for Performance Marketing [!DNL Brands]-, [!DNL Campaigns]- och [!DNL Content]-resurser. Dessa avancerade användare kan också redigera och ta bort resurser som de har skapat. GenStudio for Performance Marketing har stöd för att snabbt skapa hundratals innehållsdelar. Dessa användare kan generera innehållsfragment eller hela upplevelser som orkestrerar separata delar av godkänt innehåll för specifika marknadsföringskampanjer.

Redigerare interagerar med GenStudio for Performance Marketing generativa AI-tekniker genom att _fråga_. Frågekursen på arbetsytan innehåller verktyg som du kan använda för att ställa frågor i samband med en viss kampanjs riktlinjer. Därför beror kvaliteten och framgången för det genererade innehållet delvis på kvaliteten på de varumärkesriktlinjer som organisationen har överfört och på hur specifik uppmaningen är. Se [Skriv aktuella uppmaningar](effective-prompts.md).

I följande tabell visas standardredigerarens behörigheter:

| Funktion | Skapa | Uppdatera | Ta bort | Visa |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | no | no | no | ja |
| [!DNL Campaigns] | ja | ja | ja | ja |
| [!DNL Content] | ja | ja | ja | ja |
| [!DNL Create] | ja | ja | ja | ja |
| [!DNL Insights] | kan bara konfigurera anslutningar |    |     | ja |
| [!DNL Personas] | ja | ja | ja | ja |
| [!DNL Products] | ja | ja | ja | ja |
| [!DNL Reviews and approvals] | ja | ja | ja | ja |
| [!DNL Templates] | no | no | no | ja |

GenStudio systemhanterare kan ge redigerare behörighet att redigera och ta bort en [!DNL Brand].

### GenStudio medarbetare

_Medarbetare_ kan visa resurser i GenStudio for Performance Marketing men inte skapa, redigera eller ta bort dessa resurser. Medarbetare ser till exempel ett *Du har inte åtkomst till det här innehållet* när de försöker komma åt [[!DNL Create]](/help/user-guide/create/overview.md).

Medarbetarna arbetar bland annat med intressenter som är viktiga för att gransknings- och godkännandeprocessen ska lyckas, men som inte behöver skapa eller redigera innehåll direkt. Juridiska experter och chefer för kreatörer är exempel på potentiella medarbetare. GenStudio for Performance Marketing medarbetare kan ha behörighet att skapa och visa resurser i andra Creative Cloud-produkter.

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
| [!DNL Templates] | no | no | no | ja |

### GenStudio systemansvariga

_GenStudio systemhanterare_ har den mest kraftfulla uppsättningen behörigheter i GenStudio for Performance Marketing. Dessa avancerade användare utför den grundläggande introduktionsuppgiften att skapa grundläggande skyddsmekanismer för att skapa och driftsätta kampanjresurser. Systemansvariga implementerar skyddsprofilerna genom att överföra varumärkes- och organisationsspecifik information, till exempel [varumärkesriktlinjer](./guidelines/overview.md). Systemhanterare har behörighet att skapa och publicera [!DNL Brands], men inte behörighet för användaradministration.

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
| [!DNL Templates] | ja | ja | ja | ja |

Systemansvariga kan även överföra mallar.

Se [Kom igång med Adobe GenStudio for Performance Marketing](get-started.md) för en översikt över preliminära konfigurationsuppgifter.
