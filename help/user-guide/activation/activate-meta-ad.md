---
title: Aktivera en Meta-annons
description: Lär dig hur du aktiverar en annonsupplevelse i Meta.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
source-git-commit: 6ee58b22761be357bb9ff753cf9e5bd5b431c513
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 0%

---

# Aktivera en Meta-annons

Adobe GenStudio for Performance Marketing stöder aktivering av Meta-annonser, eller kreatörer, för Instagram och Facebook.

Du kan [skapa en metaupplevelse](/help/user-guide/create/create-meta-ad.md) i GenStudio for Performance Marketing och välja den för aktivering, eller skapa en ny upplevelse från godkända resurser i [!DNL Activate].

När du aktiverar en Meta-annons följer [samma allmänna steg](create-activation.md) som krävs för aktivering till andra betalda kanaler. Aktiveringsprocessen har stöd för att förbereda era annonsupplevelser för Metas specifika krav. När du har aktiverat en metaupplevelse, eller en kreativ upplevelse i GenStudio for Performance Marketing, använder du [Meta Ads Manager](https://adsmanager.facebook.com/) för att finjustera upplevelsen för specifika Meta-annonsplaceringar före den slutliga publiceringen.

## Steg 1: Konfigurera dina Meta-konton

[Logga in på Meta](https://adsmanager.facebook.com/) för att komma åt ditt Meta Ads Manager-konto innan du startar en aktivering. Bekräfta att dina anslutna Meta-annonskonton innehåller:

* Facebook-sida
* Meta-kampanj
* Meta ad set
* Instagramprofil (valfritt)

Du måste ha behörighet att publicera innehåll i Meta Ads Manager.

## Steg 2: Anslut till dina Meta-konton

Innan din organisation kan aktivera upplevelser måste en GenStudio-systemadministratör ansluta dina Meta-konton till GenStudio for Performance Marketing. Tack vare den här anslutningen kan data flöda mellan GenStudio och externa marknadsföringsverktyg som Meta, vilket möjliggör aktiveringsprocesser.

**Så här ansluter du GenStudio for Performance Marketing till dina Meta-konton**:

1. Klicka på **[!UICONTROL Connect]** på panelen Meta Ads i _Inställningar_. Vyn _Meta ads_ öppnas.

1. Välj **[!UICONTROL Allow pop-ups]** i webbläsaren om du uppmanas till det.

1. Välj ett eller flera av dina annonskonton att ansluta och klicka sedan på **[!UICONTROL Select]**.

När synkroniseringen har slutförts kan du visa de tillagda kontona. Stora mängder data tar längre tid att synkronisera.

## Steg 3: Förbered din upplevelse för aktivering

GenStudio systemansvariga och redaktörer kan aktivera annonsupplevelser.

**Så här förbereder du din upplevelse för aktivering**:

1. Klicka på **[!UICONTROL New]** på produktpanelen Meta i _[!DNL Activate]_._ Installationsvyn för Creative _öppnas.

   På Creative installationssida finns en central plats där du kan förbereda aktiveringen av din Meta-annons. Förbereda din annons innehåller följande tre uppgifter:

1. Ge upplevelsen ett namn. Efter aktiveringen kan du använda det här namnet för att söka efter den här upplevelsen i tabellen _Aktiverade upplevelser_.
1. Välj medieresurser. Du kan använda resurser från Innehåll eller överföra externa resurser (till exempel från OneDrive eller Dropbox).
1. [Lägg till text](#add-ad-text).
1. [Lägg till metadata](#assign-metadata).

   _Förhandsgranskningspanelen_ har stöd för en interaktiv vy av text och resurser i en specifik annonsplacering. Använd listrutan _Välj placering_ för att växla mellan annonsplaceringar som stöds. Med förhandsgranskningar kan du slutföra beslut om annonselement för specifika placeringar. När du väljer en placering på panelen _Förhandsgranska_ påverkas bara annonsvyn. Ditt placeringsval på panelen _Förhandsgranska_ sparas inte.

### Välj medieresurser

Använd avsnittet _Media_ för att välja minst en bildresurs som ska ingå i din upplevelse. Annonsplaceringar är associerade med bildproportioner som stöds, som visas som alternativ i listrutan _Placeringar_ . Den här menyn visar vilka annonsplaceringar som stöds för Facebook-inlägg eller Instagram-artiklar, ordnade efter proportioner.

Efter överföring sparas resurserna i _[!DNL Content]_. I området_ Media _visas bilden som standard med bildförhållandet 1:1. Alternativa proportioner inkluderar bara de värden som stöds av den betalda annonskanalen. De grupperas efter lodrät och vågrät orientering. GenStudio for Performance Marketing stöder användning av upp till sex bildproportioner per aktiverad upplevelse.

**Så här överför du en resurs från innehåll**:

_[!DNL Content]_ger en central vy för din organisations godkända resurser och upplevelser. Du kan fokusera det[_[!DNL Content]_-galleriet](/help/user-guide/content/manage-assets.md) som visar lager med resurser med menyalternativen **[!UICONTROL Search]** (förstoringsglas) och _Filter_ .

1. Klicka på **[!UICONTROL New]** på panelen Meta Ads i _[!DNL Activate]_._ Installationsvyn för Creative _öppnas.

1. Klicka på **[!UICONTROL Select]** och välj sedan **[!UICONTROL Select from Content]**. Vyn _Välj innehåll_ öppnas och ett galleri med bildresurser som du söker igenom eller filtrerar visas.

1. Använd _[!DNL Content]_-galleriets sök- och filterverktyg för att välja minst en resurs som ska överföras.

1. Klicka på **[!UICONTROL Use]** om du vill inkludera den valda resursen i din kreativitet. Fönstret _Creative-inställningar_ innehåller resursen i standardproportionen i området _Media_. Panelen _Förhandsvisa_ förhandsvisar resursen i annonsplaceringen som stöder den här proportionen.

Om överföringen misslyckas öppnas ett informativt felmeddelande som innehåller en länk till resursen i _[!DNL Content]_.

**Så här överför du en extern resurs**:

Du kan överföra upp till sex statiska bilder utanför galleriet _[!DNL Content]_från antingen Microsoft OneDrive eller Dropbox.

1. Klicka på **[!UICONTROL New]** på panelen Meta i _[!DNL Activate]_. Fönstret_ Creative-inställningar _öppnas.

1. Klicka på **[!UICONTROL Select]** i avsnittet _Media_. I en nedrullningsbar meny visas alternativ för att _välja från innehåll_ eller _överföra_.

1. Klicka på **[!UICONTROL Upload]**. Fönstret _Lägg till proportioner_ öppnas.

1. Välj bilder i de proportioner som stöds genom att dra och släppa bildfiler i bildens överföringsområde. Du kan även söka efter resurser på enheten.

1. (Valfritt) Om du vill överföra resurser från din enhet klickar du på **[!UICONTROL Browse]** och väljer sedan _Bläddra bland filer_ eller _Bläddra bland mappar_ för att identifiera resurser som ska överföras.

1. I området _Lägg till information_ lägger du till informativ information till dina överförda resurser för att underlätta sökning och filtrering i _[!DNL Content]_. Dessa uppgifter sparas som metadata.

1. När du har överfört dina resurser och tilldelad information klickar du på **[!UICONTROL Add Assets]** längst ned till höger.

### Lägga till text

Använd avsnittet _Text_ på sidan _Aktivera meta-annons_ för att lägga till övertygande, varumärkesanpassad text i obligatoriska textfält. Texten innehåller den primära (brödtexten) texten för annonsen och texten för uppmaning att ringa in.

| Fält | Obligatoriskt | Teckengräns (max) |
|-----------------|---------------------------|---------------------------------|
| Annonsnamn | ja | 500 |
| Primär text | ja | 500 |
| Headline | ja | 255 |
| Beskrivning | no | 125 |
| Uppmaning | ja | endast alternativ i listrutor |
| Visa URL | no | 1000 |
| Webbplatsens URL | ja | 1000 |
| Bild | minst en |                                 |

_Primär text_ och _rubrik_ krävs endast av GenStudio for Performance Marketing, inte av Meta.

### Tilldela metadata

Upplevelseinformation sparas som metadata och hjälp när användaren söker efter en upplevelse. Den här detaljen gör upplevelsen mer synlig i [!DNL Content]. Använd de här valfria, användardefinierade detaljerna för att identifiera upplevelsens syfte och sammanhang, eller kampanjer, i vilka den distribueras.

| Detalj | Beskrivning |
|------------|-------------|
| Kampanjer | Alla GenStudio for Performance Marketing-kampanjer som annonsupplevelsen tillhör |
| Varumärke | Riktlinjer, användardefinierade eller standard, som gör det möjligt för användare att fastställa riktlinjer för varumärket som fångar det väsentliga i ett varumärkes identitet. |
| Produkter | Produkter som är kopplade till din organisation och som identifieras i GenStudio for Performance Marketing |
| Personas | Personer som är kopplade till din organisation och som identifieras i GenStudio for Performance Marketing |
| Tidsram | Kvartal, säsong, år eller annan organisatoriskt definierad tidsenhet under vilken annonsupplevelsen är aktiv |
| Län | Det geografiska område där upplevelsen lanseras |
| Språk | Språk som annonsupplevelsen används för |
| Nyckelord | Användardefinierade nyckelord som underlättar sökning och kategorisering av annonsupplevelsen |

När du har monterat din kreativitet klickar du på **[!UICONTROL Next]** för att bekräfta Meta-konfigurationen.

## Steg 4: Bekräfta konfigurationen av meta-kontot

När du har förberett din kreativitet måste du bekräfta din Meta-kontoinformation och tilldela annonsfunktionen ett spårnings-ID. Vyn _Meta och konfiguration_ har fyllts i med alternativ som härleds från de konfigurerade Meta-kontona.

| Detalj | Beskrivning |
|------------|-------------|
| Konton | Meta-konton som har anslutits till GenStudio for Performance Marketing |
| Facebook-sida | Facebook-sida där upplevelsen publiceras |
| Instagram-konto | Instagramkonton som har anslutits till GenStudio for Performance Marketing |
| Kampanjer | Metakampanjer som annonsupplevelsen tillhör |
| Annonsuppsättningar | Meta ad sets som den aktiverade annonsupplevelsen tillhör. Inställningarna bestämmer den slutliga placeringen av annonsen. |

### Spårnings-ID

Spårnings-ID:n (annonsnamn) tillhandahåller en mekanism för att samla in mätvärden som är länkade till upplevelseresultatet. Ange annonsnamnet i det här fältet.

Klicka på **[!UICONTROL Next]** i det övre högra hörnet för att förhandsgranska din annonsupplevelse och slutföra aktiveringen.

## Steg 5: Förhandsgranska och aktivera annonsen

På sidan _Granska_ visas din annonsupplevelse som den är sammansatt i _Creative-konfigurationen_ och du har en sista möjlighet att visa och redigera din upplevelse. Klicka på **[!UICONTROL Edit section]** bredvid etiketten _Creative-konfiguration_ för att göra ändringarna. Du kan också klicka på **[!UICONTROL Back]** i det övre högra hörnet för att gå tillbaka till _Creative-konfigurationssidan_.

### Fullständig aktivering av annonsupplevelsen

Klicka på **[!UICONTROL Publish]**. Den fullständiga annonsupplevelsen för Meta och tillhörande metadata överförs direkt till den valda annonsuppsättningen för Meta Ads Manager. Upplevelserna levereras till Meta Ads Manager inaktiverat. Från Meta Ads Manager kan ni hantera de sista stegen i distributionen av annonsupplevelsen och Meta-kampanjen.

### Logga in på Meta Ads Manager för att slutföra aktiveringen

När aktiveringen är klar måste du logga in på Meta Ads Manager. Från [Meta Ads Manager](https://adsmanager.facebook.com/) kan du granska annonsupplevelsen och slutföra publiceringen i specifika Meta-kanaler.
