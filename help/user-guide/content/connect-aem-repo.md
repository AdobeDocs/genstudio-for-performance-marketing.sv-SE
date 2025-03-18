---
title: Anslut till en [!DNL AEM Assets Content Hub] databas
description: Lär dig hur du ansluter Adobe GenStudio for Performance Marketing till en Adobe Experience Manager (AEM) [!DNL Content Hub] -databas och utnyttjar befintligt godkänt innehåll.
level: Experienced
feature: Content Management
exl-id: abb587fd-593c-4b9f-baad-993d92400d9b
source-git-commit: 19d0b8b929e293179a091cc7b5a6a1268b0abbbd
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Anslut till en [!DNL AEM Assets Content Hub]-databas

Om du har resurser i Adobe Experience Manager (AEM) kan du följa de här stegen för att göra dem tillgängliga i GenStudio for Performance Marketing.

>[!BEGINSHADEBOX]

**Förutsättningar**:

Följande steg kräver administratörsbehörighet för Admin Console och AEM Assets as a Cloud Service.

>[!ENDSHADEBOX]

## Steg 1: Aktivera [!DNL AEM Assets Content Hub]

Följ självbetjäningsprocessen **Distribuera Content Hub** för att aktivera [!DNL Content Hub] för din befintliga AEM Assets i Cloud Manager. Se [Distribuera [!DNL Content Hub]](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub) i _AEM as a Cloud Service_ -dokumentationen.

När du har aktiverat [!DNL AEM Assets Content Hub] har du en ny instans med suffixet `contenthub` i [!DNL AEM Assets as a Cloud Service] på Admin Console.

>[!IMPORTANT]
>
>Administratörer bör verifiera att databasen [!DNL AEM Assets Content Hub] finns i samma organisation som GenStudio for Performance Marketing.

## Steg 2: Införliva GenStudio-användare

I [!DNL Admin Console] lägger du till en GenStudio for Performance Marketing-användare eller användargrupp i produktprofilen för [!DNL AEM Assets Content Hub]. Om en innehållsgranskare inte har tillgång till samma organisation som [!DNL AEM Assets Content Hub]-databasen kan de få problem med att granska och godkänna innehåll.

- [Inbyggt [!DNL Content Hub] administratör](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-administrator)
- [Anlita [!DNL Content Hub] användare](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-users)

## Steg 3: Godkänn tillgångar

Godkänn resurser som ska användas i [!DNL AEM Assets Content Hub], vilket gör dem tillgängliga i GenStudio for Performance Marketing.

Se [Godkänn resurser i Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/approve-assets) i _AEM as a Cloud Service_ -dokumentationen.

## Steg 4: Konfigurera synlighet för resurser

Granska varje uppsättning konfigurationsalternativ i konfigurationsalternativen för filter, resursinformation, sökning och branding i _[!DNL AEM Assets Content Hub]_.

Se [Konfigurera Content Hub-användargränssnitt](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/configure-content-hub-ui-options) i dokumentationen för _AEM as a Cloud Service_.

## Steg 5: Verifiera anslutningen

I GenStudio for Performance Marketing Content är listan _[!UICONTROL Location]_tillgänglig ovanför galleriet till höger. Listan är inte tillgänglig om du inte har åtkomst eller om din organisation inte har distribuerat och anslutit en [!DNL AEM Assets Content Hub]-databas.

Läs [Assets-plats](manage-assets.md#assets-location) om du vill läsa om platslistan och ändra databaser.
