---
title: Aktiveringsarbetsflöde
description: Läs mer om aktiveringsarbetsflödet för annonsupplevelser.
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
source-git-commit: 09090a57a0f41c23e8787bfb267e74427d9b7356
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# Aktiveringsarbetsflöde

_[!DNL Activate]_har stöd för aktivering av annonsupplevelser i form av en kreativ i kanalspecifika format, som en Meta- eller Google Campaign Manager 360-annonsupplevelse.

En GenStudio for Performance Marketing-upplevelse är en marknadsföringskampanjkomponent, till exempel en annons, som förbereds som en kreativ produkt för en viss målgrupp på en betald annonskanal eller via e-post. Kreatörerna består av tre huvudkomponenter:

* **Medieresurser**: Medieresurser är de bilder (GIF, PNG, JPEG) som ingår i annonsupplevelsen. Aktiveringen stöder för närvarande statiska bilder.

  Om du vill välja en bildresurs för annonsupplevelsen måste du välja rätt proportioner. Proportionerna definierar det proportionella förhållandet mellan en bilds bredd och höjd, och de är avgörande för att annonsplaceringen ska bli effektiv. Betalda mediekanaler anger noggrant giltiga proportioner för varje annonsplacering på deras plattform. När du lägger till bildresurser i aktiveringen måste du välja proportioner baserat på de slutliga annonsplaceringarna för din upplevelse. Filtyper är begränsade till JPEG, PNG och GIF.

* **Text**: Texten består av alla former av kopior som ingår i din annons, inklusive rubriker, brödtext och element för uppmaning till handling.

* **Metadata**: Användardefinierade attribut som du kan tilldela innehåll. Metadata förbättrar prestandaanalys, filtrering och spårning. Den är vanligtvis inte synlig för användarna.

Att skapa en aktivering innebär att förfina var och en av dessa annonskomponenter för en särskild kanalplacering och marknadsföringskampanj. GenStudio for Performance Marketing stöder aktivering av en upplevelse till en betalkanal.

## Arbetsflödesfaser

Även om unika placeringskrav definierar varje betald kanal, har alla annonseringsaktiveringar samma högnivåsteg. Att aktivera en upplevelse för en betald kanal har tre kärnfaser:

* **Anslut GenStudio for Performance Marketing till målkanalen**. En GenStudio-systemadministratör måste ansluta dina kanalkonton innan du kan aktivera en upplevelse.

* **Förbered för aktivering**. Förberedelsen innefattar att välja medieresurser i rätt proportioner för din specifika annonsplacering och att tilldela text till call-to-action-element och brödtext. Du kan också lägga till informativa metadata som gör det lättare för användare att söka efter upplevelsen efter aktiveringen. Varje annonskanalplacering anger giltiga proportioner för visuella resurser som ingår i placeringen.

  >[!TIP]
  >
  >Du kan välja godkända annonsupplevelser direkt från _[!DNL Content]_Experience Gallery som ska förberedas som Google Campaign Manager 360-kreatörer. När du har valt en upplevelse i galleriet_[!DNL Content]_ kan du inte redigera eller lägga till resurser i din kreativitet.

* **Granska och publicera din upplevelse till målkanalen**. Använd panelen _Förhandsgranska_ under den kreativa konfigurationen för att utvärdera ditt val av annonsplacering och textelement innan du slutför aktiveringen. Den slutliga förhandsgranskningen görs i målkanalens annonshanteringsapp. När du till exempel har aktiverat en annonsupplevelse i Meta i GenStudio for Performance Marketing måste du logga in i Meta Ads Manager, granska din kreativitet och sedan välja specifika attribut innan du publicerar den.

När en kreatör väl har publicerat sin målbetalda mediekanal kan _[!DNL Insights]_spåra och analysera dess prestandadata.

## Kanaler som stöds

Varje betald mediekanal har ett unikt aktiveringsarbetsflöde. Välj den betalda kanalen för aktiveringsriktlinjer:

* [Meta](activate-meta-ad.md)
* [Google Campaign Manager 360](activate-cm360-ad.md)
