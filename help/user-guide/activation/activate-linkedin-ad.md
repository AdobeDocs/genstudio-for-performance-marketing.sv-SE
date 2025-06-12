---
title: Aktivera en LinkedIn-annons
description: Lär dig hur du aktiverar en LinkedIn-annonsupplevelse.
feature: Ad Activation
source-git-commit: 5279caaf4651ed81c3cf3d8a4de2f17c3f151ec8
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 0%

---

# Aktivera en LinkedIn-annons

Adobe GenStudio for Performance Marketing stöder aktivering av LinkedIn-upplevelser med enstaka resurser på [LinkedIn Campaign Manager](https://business.linkedin.com/marketing-solutions)- och LinkedIn-sidor.

Du kan [skapa en LinkedIn-upplevelse](/help/user-guide/create/create-linkedin.md) i GenStudio for Performance Marketing och välja den för aktivering, eller skapa en ny upplevelse från godkända resurser i [!DNL Activate].

När du aktiverar en LinkedIn-annons följer [samma allmänna steg](create-activation.md) som krävs för aktivering till andra betalda kanaler. Aktiveringsprocessen har stöd för att förbereda annonsupplevelsen för LinkedIn:s specifika krav. När du har aktiverat en LinkedIn-upplevelse i GenStudio for Performance Marketing kan du använda LinkedIn Campaign Manager för att finjustera upplevelsen för specifika LinkedIn-annonsplaceringar före den slutliga publiceringen.

GenStudio systemansvariga och redaktörer kan aktivera annonsupplevelser.

## Steg 1: Konfigurera dina LinkedIn-konton

[Logga in på](https://www.linkedin.com/campaignmanager/login) ditt LinkedIn Campaign Manager-konto innan du startar en aktivering.

>[!BEGINSHADEBOX]

**Förutsättningar**:

* Ett LinkedIn Campaign Manager-konto med fullständig behörighet för att hantera kampanjgrupper, kampanjer och annonser. Det här kontot måste innehålla kampanjgrupper och kampanjer.

* LinkedIn-annonskonton med fullständig behörighet för att skapa annonser och publicera innehåll på LinkedIn-sidor.

>[!ENDSHADEBOX]

## Steg 2: Anslut till dina LinkedIn-konton

Innan din organisation kan aktivera upplevelser måste en GenStudio-systemadministratör ansluta dina LinkedIn-konton till GenStudio for Performance Marketing. Med den här anslutningen kan data flöda mellan GenStudio och externa marknadsföringsverktyg som LinkedIn, vilket möjliggör aktiveringsprocessen.

När synkroniseringen har slutförts kan du visa de tillagda kontona. Stora mängder data tar längre tid att synkronisera.

## Steg 3: Förbered din upplevelse

Du kan starta en aktivering genom att välja en eller flera godkända upplevelser med fördefinierade inställningar från [!DNL Content].

Vyn _Upplevelsekonfiguration_ är en arbetsyta för att justera och granska upplevelser före aktivering. Om du väljer mer än en upplevelse att aktivera, innehåller den här vyn en vänster sidospalt som visar miniatyrbilder av alla valda upplevelser. Använd den här vänstra sidofältet för att fokusera vyn _Experience setup_ på informationen för den valda upplevelsen.

_Förhandsgranskningspanelen_ har stöd för en interaktiv vy av text och resurser i en specifik annonsplacering. Använd listrutan _Välj placering_ för att växla mellan annonsplaceringar som stöds. Med förhandsgranskningar kan du slutföra beslut om annonselement för specifika placeringar. När du väljer en placering på panelen _Förhandsgranska_ påverkas bara annonsvyn. Ditt placeringsval på panelen _Förhandsgranska_ sparas inte.

### Aktivera en godkänd upplevelse från innehåll

Du kan välja en eller flera upplevelser som ska aktiveras till en enda betalkanal. Upplevelser kan bara innehålla en resurs. Information läses in från de valda godkända upplevelserna.

Information om redigerbar upplevelse:

* Call-to-action (CTA) text
* Webbplatsens URL
* Visa länk

**Så här väljer du upplevelser**:

1. Använd söknings- och filterverktygen i [!DNL Content]-galleriet för att identifiera den upplevelse som du vill aktivera och klicka sedan på **[!UICONTROL Activate]**. Du kan också välja en upplevelse och välja **[!UICONTROL Activate]** på menyn mer (..).

   Sidan för LinkedIn-annonser _Experience setup_ öppnas för den här upplevelsen. Den är förifylld med information från den valda upplevelsen. Du kan behöva välja en plattform innan du fortsätter med aktiveringen.

1. (Valfritt) Redigera värden i redigerbara fält (**[!UICONTROL Call to action]**, **[!UICONTROL Website URL]**, *[!UICONTROL Display link]**).

1. (Valfritt) Klicka på **[!UICONTROL Add experience]** om du vill lägga till upplevelser i den här aktiveringsgruppen.

1. Klicka på **[!UICONTROL Next]** för att bekräfta din upplevelseinställning.

## Steg 4: Bekräfta konfiguration av LinkedIn-konto

När ni har förberett era annonsupplevelser måste ni bekräfta er kontoinformation för LinkedIn. Vyn _LinkedIn och setup_ har fyllts i med alternativ som härleds från de konfigurerade LinkedIn-kontona.

_Kampanjgrupper_ är en viktig komponent i LinkedIn Campaign Manager. Kampanjgrupper organiserar diskreta kampanjer i enlighet med ett gemensamt mål. Kampanjer kan ärva budgetbegränsningar, mål och scheman från den kampanjgrupp som de tillhör.

**Så här bekräftar du kontokonfigurationen**:

1. Välj ett konto i listrutan **[!UICONTROL Account]**. Alternativen är LinkedIn-konton som har anslutits till GenStudio for Performance Marketing.

1. Välj en kampanjgrupp i listrutan **[!UICONTROL Campaign group]**. Detta är kampanjgruppen LinkedIn där upplevelsen publiceras.

1. Välj en kampanj i listrutan **[!UICONTROL Campaigns]**. Detta är den LinkedIn-kampanj som annonsupplevelsen levereras till.

1. Ange ett annonsnamn i fältet **[!UICONTROL Ad name]** för varje upplevelse. LinkedIn Campaign Manager identifierar upplevelsen med det här namnet.

1. Klicka på **[!UICONTROL Next]** för att bekräfta inställningarna för LinkedIn-annonser.

## Steg 5: Förhandsgranska och aktivera annonsen

Sidan _Review_ ger dig möjlighet att granska aktiveringen innan du publicerar den.

**Så här granskar och publicerar du din upplevelse**:

1. (Valfritt) Klicka på **[!UICONTROL Edit section]** bredvid upplevelsen eller plattformsinformationen som du vill redigera.
Beroende på vilket avsnitt du har valt öppnas vyn _Upplevelsetinställningar_ eller _Plattformskonfiguration_.

1. (Valfritt) Redigera informationen och klicka sedan på **[!UICONTROL Next]** för att återgå till _granskningsvyn_.

1. Klicka på **[!UICONTROL Publish]**.

   Den fullständiga annonsupplevelsen i LinkedIn och tillhörande metadata överförs direkt till den avsedda kampanjen för LinkedIn Campaigns Manager. Upplevelserna levereras i ett inaktivt läge. I LinkedIn Campaign Manager kan ni hantera de sista stegen i distributionen av annonsupplevelsen och LinkedIn-kampanjen.

## Steg 6: Slutför publiceringen av annonsupplevelsen

1. [Logga in på](https://www.linkedin.com/campaignmanager/login) ditt LinkedIn Campaign Manager-konto för att granska din annonsupplevelse och slutföra publiceringen på specifika LinkedIn-sidor.
