---
title: Anslut till Meta Ads
description: Anslut ett Meta Ads-konto för att aktivera och övervaka annonser och media med Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
recommendations: noDisplay
feature: Reporting and Insights
exl-id: 78110edf-947b-4e05-a3f1-de4b1eabda44
source-git-commit: 40c7d2d40f1c4bea9794e706d8e1ce7bf92042e3
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Anslut till Meta Ads

På den här sidan beskrivs hur du ansluter och hanterar ditt Meta Ads-profilkonto till GenStudio for Performance Marketing för att hantera kampanjer, exportera innehåll och få tillgång till annonsdata för aktiva kampanjer.

>[!BEGINSHADEBOX]

**Förutsättningar**:

- Facebook/Meta-inloggning som kan få åtkomst till alla Meta-tjänster

- _Full kontroll_ över Meta Business Portfolio- och Ad-konton, inklusive:

   - Hantera kampanjer
   - Visa prestanda
   - Hantera Creative Hub-modeller
   - Avancerad analys

- Inaktivera alla popup-blockerare i webbläsaren

>[!ENDSHADEBOX]

## Anslut ett Meta Ads-konto

1. Klicka på **[!UICONTROL More]** > **[!UICONTROL Settings]**.

1. Klicka på _på_ Meta Ads **[!UICONTROL Connect]**-kortet i avsnittet _Dataanslutningar_.

1. Logga in på ditt Facebook-konto.

   Du kan behöva ta bort blockerarna och sedan använda **[!UICONTROL Refresh]** för att försöka igen.

1. Följ instruktionerna för Facebook-autentisering, verifiera kontoinformationen och klicka på **[!UICONTROL Continue as ...]**

1. I _[!UICONTROL Facebook Login for Business]_(Meta till Adobe-symbol) går du igenom följande val för att ge GenStudio for Performance Marketing åtkomst:

   - Markera en eller flera Meta Business-profiler och klicka på **[!UICONTROL Continue]**
   - Markera en eller flera Meta-sidor och klicka på **[!UICONTROL Continue]**
   - Välj ett eller flera Instagram-konton och klicka på **[!UICONTROL Continue]**
   - Granska markeringar och klicka på **[!UICONTROL Save]**

     ![Granska markeringar](/help/assets/meta/meta-review-selections.png "Granska markeringar"){width="400" zoomable="yes"}

1. När du har fått en bekräftelse på att ditt konto är anslutet klickar du på **[!UICONTROL Got it]**.

   Detta steg säkerställer att GenStudio for Performance Marketing får tillgång till alla annonser, metadata och mätvärden för optimala prestanda.

1. I _[!UICONTROL Meta Ads]_&#x200B;väljer du ett eller flera konton som ska inkluderas i [!DNL Insights] och klickar på&#x200B;**[!UICONTROL Select]**.

1. När du fått en bekräftelse från _Platform connected_ klickar du på **[!UICONTROL View accounts]**.

   I vyn _[!UICONTROL Meta Ads accounts]_&#x200B;visas `Account name`, `Added by`, `Date added` och `Status`.

   ![Meta-kontolista](/help/assets/meta/meta-accounts-list.png "Lista över anslutna Meta-konton"){zoomable="yes"}

Använd **[!UICONTROL Add account]** om du vill lägga till fler konton i listan. Behörighetsflödet kan variera något när du lägger till konton som är länkade till samma Meta Business-profil. Du väljer bara de nya Meta Ads-kontona under anslutningsprocessen.

## Koppla från och felsöka en Meta Ads-integrering

Ibland är en GenStudio for Performance Marketing-instans felaktigt ansluten till ett Meta Ads-konto. Vanliga inställningar som kan orsaka problem är:

- Ett Instagram-konto har valts utan att den associerade Facebook-sidan har markerats
- Återkallade behörigheter för en användare som utförde den ursprungliga anslutningen

I sådana fall är det bäst att koppla Meta Ad-kontot till GenStudio for Performance Marketing-instansen. Först måste användaren ta bort appintegreringen direkt från sin Meta Business Manager och skapa en ren skiva för att återställa behörigheter. Detta kräver administratörsåtkomst till Meta Business Manager.

De här stegen rensar cachelagrade behörigheter och återställer integreringsflödet:

1. Gå till [Meta Business Manager](https://business.facebook.com) genom att besöka Facebook-webbplatsen.
1. Logga in med ditt konto. Kontot måste ha administratörsåtkomst till Business Manager.
1. Klicka på ikonen **[!UICONTROL Settings]** i det nedre vänstra hörnet för att navigera till dina Business Portfolio-inställningar.
1. Klicka på **[!UICONTROL Integrations]** på den vänstra menyn.
1. Välj **[!UICONTROL Connected Apps]**. Adobe GenStudio visas i listan med anslutna appar.
   ![Anslutna appar för Meta Business Manager](./meta-connected-apps.png "Panelen Anslutna appar för Meta Business Manager")
1. Klicka på programnamnet.
1. Klicka på **[!UICONTROL Remove]**.
1. Bekräfta borttagningen när du uppmanas till det.

Nu kan du koppla dina Meta-annonskonton, Instagram-profiler och Facebook-sidor igen.
