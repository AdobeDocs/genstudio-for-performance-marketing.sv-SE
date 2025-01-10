---
title: Datahantering
description: Läs mer om datahantering och lagring för insikter i GenStudio for Performance Marketing.
feature: Insights
level: Experienced
role: Admin
last-substantial-update: 2025-1-7
source-git-commit: 5dbe645f2ccf033f515da22ffdcce86edcb9fb24
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Datahantering

GenStudio for Performance Marketing använder Adobe Experience Platform (AEP) för datainmatning och lagring av mätvärden och metadata som används i [!DNL Insights]. AEP använder _scheman_ för att definiera datastrukturer och _datamängder_ för att lagra och hantera datainsamlingar.

## Dataanslutningar

GenStudio for Performance Marketing använder Customer Journey Analytics (CJA) för att samla in flera datakällor genom att skapa en anslutning till en eller flera AEP-datauppsättningar. CJA använder dessa dataanslutningar för att skapa datavyer för analys av mätvärden med [!DNL Insights].

>[!BEGINSHADEBOX]

**Viktig information om dataanslutningar**

Om du är [Adobe-systemadministratör](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager) kan du ha rättigheter som tillåter åtkomst till AEP-sandlådehantering och Data Lake-komponenter som stöder GenStudio for Performance Marketing.

>[!WARNING]
>
>Om du återställer produktionssandlådan i AEP tas alla dataanslutningar bort och [!DNL Insights] slutar att fungera.

Var försiktig och ta inte bort följande dataanslutningar som krävs för att GenStudio for Performance Marketing ska fungera tillförlitligt:

- AEP-datauppsättningar prefix med `GS Insights`
- AEP-scheman, klasser och fältgrupper har prefixats med `GS Insights`
- Anpassad fältgrupp `timestamp for metadata`
- AEP-anslutningar: dataflöden prefixerade med `GS Insights`
- AEP-anslutningar: GS Insights-konto

Se [Ta bort konsekvenser](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion) i guiden _Customer Journey Analytics_ innan du tar bort några datakomponenter i AEP.

>[!ENDSHADEBOX]

## Datalagringspolicy

GenStudio for Performance Marketing sparar kanaldata i 13 månader. Denna lagringspolicy omfattar sex månaders data som samlats in under den första anslutningen, vilket säkerställer en omfattande historisk dataanalys och rapportering.

Se [Ansluta kanalannonskonto](/help/user-guide/insights/connect-channel.md).
