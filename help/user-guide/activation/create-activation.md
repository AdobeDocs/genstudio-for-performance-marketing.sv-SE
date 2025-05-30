---
title: Aktiveringsarbetsflöde
description: Läs mer om aktiveringsarbetsflödet för annonsupplevelser.
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
source-git-commit: c622b86ae2977026207edb8919102620ef582d39
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Aktiveringsarbetsflöde

_[!DNL Activate]_&#x200B;har stöd för aktivering av annonsupplevelser i kanalspecifika format, som Meta eller Google Campaign Manager 360.

En GenStudio for Performance Marketing-upplevelse är en marknadsföringskampanjkomponent, till exempel en annons, som förbereds som en annonsupplevelse till en viss målgrupp via en betald annonskanal eller ett e-postmeddelande. Upplevelser för aktivering innehåller tre huvudkomponenter:

* **Medieresurser**: Medieresurser är de bilder (GIF, PNG, JPEG) som ingår i annonsupplevelsen. Aktiveringen stöder för närvarande statiska bilder.

  Om du vill välja en bildresurs för annonsupplevelsen måste du välja rätt proportioner. Proportionerna definierar det proportionella förhållandet mellan en bilds bredd och höjd, och de är avgörande för att annonsplaceringen ska bli effektiv. Betalda mediekanaler anger noggrant giltiga proportioner för varje annonsplacering på deras plattform. När du lägger till bildresurser i aktiveringen måste du välja proportioner baserat på de slutliga annonsplaceringarna för din upplevelse. Filtyper är begränsade till JPEG, PNG och GIF.

* **Text**: Texten består av alla former av kopior som ingår i din annons, inklusive rubriker, brödtext och element för uppmaning till handling.

* **Metadata**: Användardefinierade attribut som du kan tilldela innehåll. Metadata förbättrar prestandaanalys, filtrering och spårning. Den är vanligtvis inte synlig för användarna.

Att skapa en aktivering innebär att förfina var och en av dessa annonskomponenter för en särskild kanalplacering och marknadsföringskampanj. GenStudio for Performance Marketing stöder aktivering av en upplevelse till en betalkanal.

## Arbetsflödesfaser

Även om unika placeringskrav definierar varje betald kanal, har alla annonseringsaktiveringar samma högnivåsteg. Att aktivera en upplevelse för en betald kanal har tre kärnfaser:

1. **Anslut GenStudio for Performance Marketing till målkanalen**. En GenStudio-systemadministratör måste ansluta dina kanalkonton innan du kan aktivera en upplevelse.

1. **Förbered för aktivering**. Ni kan förbereda upplevelserna för aktivering på två sätt:

   * Aktivera en godkänd upplevelse med fördefinierade inställningar direkt från _[!DNL Content]_. Detta smidiga sätt att aktivera en eller flera annonsupplevelser i en enda kanal. När du har valt en upplevelse i galleriet&#x200B;_[!DNL Content]_ kan du inte redigera eller lägga till resurser i din annonsupplevelse. Aktivera från _[!DNL Content]_&#x200B;är tillgängligt för annonsupplevelserna Meta och Google Campaign Manager 360.

   * Sammanställ annonsupplevelsen genom att välja visuella resurser från _[!DNL Content]_, lägga till textelement och välja proportioner. Den här metoden omfattar fler steg men ger större kreativ flexibilitet. Förberedelsen innefattar att välja medieresurser i rätt proportioner för din specifika annonsplacering och att tilldela text till call-to-action-element och brödtext. Du kan lägga till informativa metadata som gör det lättare för användare att söka efter upplevelsen efter aktiveringen. Varje annonskanalplacering anger giltiga proportioner för visuella resurser som ingår i placeringen.

1. **Granska och publicera din upplevelse till målkanalen**. Använd panelen _Förhandsgranska_ under upplevelseinställningen för att utvärdera ditt val av annonsplacering och textelement innan du slutför aktiveringen. Den slutliga förhandsgranskningen görs i målkanalens annonshanteringsapp. När du till exempel har aktiverat en annonsupplevelse i Meta i GenStudio for Performance Marketing måste du logga in i Meta Ads Manager, granska annonsupplevelsen och sedan välja specifika attribut innan du publicerar den.

När en annonsupplevelse finns i målmediekanalen kan _[!DNL Insights]_&#x200B;spåra och analysera dess prestandadata.

## Kanaler som stöds

Varje betald mediekanal har ett unikt aktiveringsarbetsflöde. Välj den betalda kanalen för aktiveringsriktlinjer:

* [Meta](/help/user-guide/activation/activate-meta-ad.md)
* [Google Campaign Manager 360](/help/user-guide/activation/activate-cm360-ad.md)
