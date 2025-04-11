---
title: Datahantering
description: Läs mer om datainhämtning och lagring för  [!DNL Insights] i GenStudio for Performance Marketing.
feature: Reporting and Insights
level: Experienced
role: Admin, Data Architect
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
source-git-commit: 8e61fa5c08102c5dd9905e693d7f129105d9f633
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Datahantering

GenStudio for Performance Marketing använder Adobe Experience Platform (AEP) för datainmatning och lagring av mätvärden och metadata som används i [!DNL Insights]. AEP använder _scheman_ för att definiera datastrukturerna och _datauppsättningarna_ för att lagra och hantera datainsamlingar.

## Dataanslutningar

GenStudio for Performance Marketing använder Customer Journey Analytics (CJA) för att samla in flera datakällor genom att skapa en anslutning till en eller flera AEP-datauppsättningar. CJA använder dessa dataanslutningar för att skapa datavyer för analys av mätvärden med [!DNL Insights].

>[!BEGINSHADEBOX]

**Viktig information om dataanslutningar**

Om du är [Adobe-systemadministratör](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager) kan du ha rättigheter som tillåter åtkomst till AEP sandlådehantering och Data Lake-komponenter som stöder GenStudio for Performance Marketing.

>[!WARNING]
>
>Om du återställer produktionssandlådan i AEP tas alla dataanslutningar bort och [!DNL Insights] slutar att fungera.

Var försiktig och ta inte bort följande dataanslutningar som krävs för att GenStudio for Performance Marketing ska fungera tillförlitligt:

- AEP-datauppsättningar prefix med `GS Insights`
- AEP-scheman, klasser och fältgrupper har prefixats med `GS Insights`
- Anpassad fältgrupp `timestamp for metadata`
- AEP-anslutningar: dataflöden prefix med `GS Insights`
- AEP Connections: GS Insights-konto

Se [Ta bort konsekvenser](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion) i _Customer Journey Analytics_-handboken innan du tar bort några datakomponenter i AEP.

>[!ENDSHADEBOX]

## Datalagringspolicy

GenStudio for Performance Marketing sparar kanaldata i 13 månader. Denna lagringspolicy omfattar sex månaders data som samlats in under den första anslutningen, vilket säkerställer en omfattande historisk dataanalys och rapportering.

Se [Ansluta kanalannonskonto](/help/user-guide/connectors/connect-channel.md).
