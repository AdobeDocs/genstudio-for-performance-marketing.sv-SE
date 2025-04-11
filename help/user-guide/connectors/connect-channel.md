---
title: Anslut betalmedia
description: Anslut ett kanalkonto för att aktivera och övervaka annonser och media med Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: 2844914d25d9bc3a2be7f47d0cd7f26f7c921555
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Anslut betalmediekonton

_[!DNL Data connectors]_möjliggör sömlös integrering mellan GenStudio for Performance Marketing och dina betalda medienätverkskonton. Genom att ansluta till kanalkonton från tredje part kan du utbyta viktiga data, till exempel kampanjresultatstatistik i [[!DNL Insights]](/help/user-guide/insights/overview.md), och du kan leverera nya annonsplaceringar med [[!DNL Activate]](/help/user-guide/activation/overview.md). Tack vare den här integreringen kan GenStudio for Performance Marketing hantera era medier och annonser och samtidigt få värdefulla insikter, inklusive visningar, klickningar och konverteringar, från era aktiva kampanjer.

**Så här ansluter du till ett betalt mediekonto**:

1. Klicka på ellipsen **[!UICONTROL ... More]** i den nedre vänstra navigeringen.

1. Välj **[!UICONTROL Settings]** med kodikonen.

1. I _[!UICONTROL Settings]_väljer du en anslutningstyp i avsnittet_[!UICONTROL Data connectors]_ och klickar på **[!UICONTROL Connect]**.

   Om det finns anslutna konton kan du klicka på _anslutna konton_ för att visa en lista med kontonamn, detaljer och status.

1. Se den [anslutningstyp](#connector-types) du valt, granska förutsättningarna och fortsätt med anslutningsstegen.

## Betalda medieanslutningar

GenStudio for Performance Marketing har stöd för olika anslutningstyper som kan integreras med de marknadsföringsplattformar ni föredrar. Varje anslutningstyp har specifika förutsättningar och konfigurationssteg som ska slutföras för att anslutningen ska lyckas.

### Koppla metaannonser

>[!BEGINSHADEBOX]

**Förutsättningar**:

- Facebook-/Meta-annonskonto
- Åtkomst till Meta-annonskonto med behörigheten `View performance` för åtkomst till rapporter och visning av annonser
- Ta bort alla popup-blockerare i webbläsaren

>[!ENDSHADEBOX]

**Så här ansluter du ett Meta ads-konto**:

1. Klicka på **[!UICONTROL Connect]** på _Meta Ads_-kortet i avsnittet _Dataanslutningar_.

1. Logga in på ditt Facebook-konto.

   Du kan behöva ta bort blockerarna och sedan använda **[!UICONTROL Refresh]** för att försöka igen.

1. Följ instruktionerna för Facebook-autentisering.

1. Gå igenom följande markeringar i popup-fönstret _[!UICONTROL Facebook Login for Business]_(Meta till Adobe-symbol).

   - Verifiera kontoinformationen och klicka på **[!UICONTROL Continue as]**
   - Bevilja åtkomst för att välja sidor och klicka på **[!UICONTROL Continue]**
   - Bevilja åtkomst till utvalda företag och klicka på **[!UICONTROL Continue]**
   - Välj ett eller flera Instagram-konton och klicka på **[!UICONTROL Continue]**
   - Granska markeringar och klicka på **[!UICONTROL Save]**

1. I vyn _[!UICONTROL Meta Ads]_markerar du ett eller flera konton och klickar på&#x200B;**[!UICONTROL Select]**.

I vyn _[!UICONTROL Meta Ads accounts]_visas `Account name`, `Added by`, `Date added` och `Status`. Använd **[!UICONTROL Add account]**om du vill lägga till fler konton i listan.

## Intag av data

Till att börja med importerar GenStudio for Performance Marketing de senaste sex månaderna med historiska data. Med den här metoden får ni omedelbar tillgång till relevanta insikter för att analysera trender, utvärdera resultatet och fatta välgrundade beslut. Injektionsprocessen kan ta en till fem dagar beroende på mängden data på ditt konto.

>[!BEGINSHADEBOX]

**Princip för datainmatning och lagring**

GenStudio for Performance Marketing sparar kanaldata i 13 månader. Denna lagringspolicy omfattar sex månaders data som samlats in under den första anslutningen, vilket säkerställer en omfattande historisk dataanalys och rapportering.

>[!ENDSHADEBOX]
