---
title: Distribuera din app
description: Distribuera din app, eller din add-on, för GenStudio for Performance Marketing.
feature: Extensibility
exl-id: 4935356b-08df-402c-b1a2-b89627afc188
source-git-commit: 2df93292f456cc952f72faea3d25ca0503a4e2db
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Distribuera din app

Genom att distribuera din add-on blir den tillgänglig för användning av din organisation och andra. Ditt distributionsarbetsflöde beror på om din add-on är avsedd för offentlig eller privat distribution.

I det här avsnittet diskuteras privat distribution. Privat distribution begränsar distributionen av tillägget till organisationen, som identifieras av IMS-organisationen, som den har utvecklats för.

Offentlig distribution gör tillägget tillgängligt som ett program på Adobe Exchange. [Offentlig distribution](https://developer.adobe.com/app-builder/docs/guides/distribution/public/) i utvecklardokumentationen för _App Builder_ beskriver hur du gör din app tillgänglig för alla Adobe-organisationer.

>[!BEGINSHADEBOX]

**Förutsättningar**:

Bekräfta följande behörigheter:

* Utvecklarbehörigheter i organisationen som du skickar appen från för godkännande

* Systemadministratörsbehörighet för att godkänna appen

Ditt App Builder-program måste distribueras i ett App Builder-projekt.

>[!ENDSHADEBOX]

**Så här distribuerar du din app privat**:

Privat distribution gör din app tillgänglig endast för medlemmar i din organisation.

1. I [Adobe Developer Console](https://developer.adobe.com/console/) väljer du den organisation, det projekt och den arbetsyta där appen distribueras.

1. Välj **[!UICONTROL Approval]** i området _Workspace overview_. Fönstret _App Approval_ (Appgodkännande) öppnas.

1. I området _Information om appöverföringar_ lägger du till informativ information om ditt tillägg. Informationen innehåller programnamn, beskrivning och e-postadress för kontakt.

1. När du har fyllt i alla fält klickar du på **[!UICONTROL Submit]**.

1. Logga in på [Adobe Exchange](https://exchange.adobe.com/) med samma Adobe ID som du använde för att logga in på Developer Console. Om du inte har systemadministratörsbehörighet i den här organisationen begär du godkännande från en systemadministratör för organisationen.

1. Välj **[!UICONTROL Manage]** > **[!UICONTROL App Builder applications]** för att få åtkomst till en begäran om att granska appen.

1. När du har granskat appen väljer du **[!UICONTROL Approve]**. Du kan även lägga till informativa anteckningar.

Din add-on visas nu i din organisations GenStudio for Performance Marketing-instans.
