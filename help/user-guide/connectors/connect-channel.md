---
title: Anslut betalmedia
description: Anslut ett kanalkonto för att aktivera och övervaka annonser och media med Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: cf4be61925761c9630cb8ea5c995d017b3938a31
workflow-type: tm+mt
source-wordcount: '644'
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

### Google Campaign Manager 360-anslutning

>[!BEGINSHADEBOX]

**Förutsättningar**:

- Google Campaign Manager 360-konto
- Ta bort alla popup-blockerare i webbläsaren

>[!ENDSHADEBOX]

**Så här ansluter du ett Google Campaign Manager 360-konto**:

1. Klicka på **[!UICONTROL Connect]** på _Google Campaign Manager 360_-kortet i avsnittet _Dataanslutningar_.

1. Logga in på ditt Google Campaign Manager 360-konto.

   Du kan behöva ta bort blockerarna och sedan använda **[!UICONTROL Refresh]** för att försöka igen.

1. Läs villkoren och klicka på **[!UICONTROL Allow]** för att bevilja åtkomst.

1. I vyn _[!UICONTROL Google Campaign Manager 360]_väljer du en eller flera annonsörer och klickar på&#x200B;**[!UICONTROL Select]**.

I vyn _[!UICONTROL Google Campaign Manager 360 accounts]_visas `Account name`, `Added by`, `Date added` och `Status`. Använd **[!UICONTROL Add account]**om du vill lägga till fler konton i listan.

### Koppla metaannonser

När du ansluter din _Meta Business_-profil till GenStudio for Performance Marketing säkerställer den sömlös åtkomst till annonsdata för dina företagssidor, Meta Ads-konton och andra Meta-resurser.

>[!BEGINSHADEBOX]

**Förutsättningar**:

- Facebook-/Meta-inloggning som kan komma åt alla metatjänster, som Meta Ads-konto och Facebook Business Profile
- Åtkomst till Meta-annonskonto med behörigheten `View performance` för åtkomst till rapporter och visning av annonser, inklusive följande
   - Behörigheter krävs för användning med [!DNL Insights]:

      - `pages_show_list`
      - `ads_read`
      - `ads_management`
      - `pages_read_engagement`

   - Behörigheter krävs för användning med [!DNL Activate]:

      - `ads_management`
      - `ads_read`
      - `business_management`
      - `instagram_basic`
      - `instagram_content_publish`
      - `pages_manage_ads`
      - `pages_manage_posts`
      - `pages_show_list`

- Ta bort alla popup-blockerare i webbläsaren

>[!ENDSHADEBOX]

**Så här ansluter du ett Meta ads-konto**:

1. Klicka på **[!UICONTROL Connect]** på _Meta Ads_-kortet i avsnittet _Dataanslutningar_.

1. Logga in på ditt Facebook-konto.

   Du kan behöva ta bort blockerarna och sedan använda **[!UICONTROL Refresh]** för att försöka igen.

1. Följ instruktionerna för Facebook-autentisering, verifiera kontoinformationen och klicka på **[!UICONTROL Continue as ...]**

1. I _[!UICONTROL Facebook Login for Business]_(Meta till Adobe-symbol) går du igenom följande val för att ge GenStudio for Performance Marketing åtkomst:

   - Välj en eller flera Meta Business-profiler och klicka på **[!UICONTROL Continue]**
   - Markera en eller flera metasidor och klicka på **[!UICONTROL Continue]**
   - Välj ett eller flera Instagram-konton och klicka på **[!UICONTROL Continue]**
   - Granska markeringar och klicka på **[!UICONTROL Save]**

1. När du har fått en bekräftelse på att ditt konto är anslutet klickar du på **[!UICONTROL Got it]**.

   Detta steg säkerställer att GenStudio for Performance Marketing får tillgång till alla annonser, metadata och mätvärden för optimala prestanda.

1. I _[!UICONTROL Meta Ads]_väljer du ett eller flera konton som ska inkluderas i [!DNL Insights] och klickar på&#x200B;**[!UICONTROL Select]**.

1. När du fått en bekräftelse från _Platform connected_ klickar du på **[!UICONTROL View accounts]**.

   I vyn _[!UICONTROL Meta Ads accounts]_visas `Account name`, `Added by`, `Date added` och `Status`.

Använd **[!UICONTROL Add account]** om du vill lägga till fler konton i listan. Auktoriseringsflödet kan variera något när du lägger till konton som är länkade till samma Meta Business-profil. Du väljer bara de nya Meta Ads-kontona under anslutningsprocessen.

## Intag av data

Till att börja med importerar GenStudio for Performance Marketing de senaste sex månaderna med historiska data. Med den här metoden får ni omedelbar tillgång till relevanta insikter för att analysera trender, utvärdera resultatet och fatta välgrundade beslut. Injektionsprocessen kan ta en till fem dagar beroende på mängden data på ditt konto.

>[!BEGINSHADEBOX]

**Princip för datainmatning och lagring**

GenStudio for Performance Marketing sparar kanaldata i 13 månader. Denna lagringspolicy omfattar sex månaders data som samlats in under den första anslutningen, vilket säkerställer en omfattande historisk dataanalys och rapportering.

>[!ENDSHADEBOX]
