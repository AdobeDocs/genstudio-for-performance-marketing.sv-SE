---
title: Aktivera en Meta-annons
description: Lär dig hur du aktiverar en annonsupplevelse i Meta.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
source-git-commit: 09450c99dfc6bc283519b068a3b34c0551e45fc8
workflow-type: tm+mt
source-wordcount: '1642'
ht-degree: 0%

---

# Aktivera en Meta-annons

Adobe GenStudio for Performance Marketing stöder aktivering av Meta-annonsupplevelser för Instagram och Facebook.

Du kan [skapa en metaupplevelse](/help/user-guide/create/create-meta-ad.md) i GenStudio for Performance Marketing och välja den för aktivering, eller skapa en ny upplevelse från godkända resurser i [!DNL Activate].

När du aktiverar en Meta-annons följer [samma allmänna steg](create-activation.md) som krävs för aktivering till andra betalda kanaler. Aktiveringsprocessen har stöd för att förbereda er annonsupplevelse för Metas specifika krav. När du har aktiverat en metaupplevelse i GenStudio for Performance Marketing använder du [Metaannonshanteraren](https://adsmanager.facebook.com/) för att finjustera upplevelsen för specifika metaannonsplaceringar före den slutliga publiceringen.

GenStudio systemansvariga och redaktörer kan aktivera annonsupplevelser.

## Steg 1: Konfigurera dina Meta-konton

[Logga in på Meta](https://adsmanager.facebook.com/) för att komma åt ditt Meta Ads Manager-konto innan du startar en aktivering.

>[!BEGINSHADEBOX]

**Förutsättningar**:

Bekräfta att dina anslutna Meta-annonskonton har fullständig behörighet att hantera annonser i de här komponenterna i Meta-annonsplattformen:

* Facebook-sida
* Meta-kampanj
* Meta ad set
* Instagramprofil (valfritt)

>[!ENDSHADEBOX]

## Steg 2: Anslut till dina Meta-konton

Innan din organisation kan aktivera upplevelser måste en GenStudio-systemadministratör ansluta dina Meta-konton till GenStudio for Performance Marketing. Med den här anslutningen kan data flöda mellan GenStudio och externa marknadsföringsverktyg som Meta, vilket möjliggör aktiveringsprocessen.

Se [Ansluta till metaannonser](/help/user-guide/connectors/meta-ads.md).

När synkroniseringen har slutförts kan du visa de tillagda kontona. Stora mängder data tar längre tid att synkronisera.

## Steg 3: Förbered din upplevelse för aktivering

Du kan starta en aktivering på två sätt:

* **Aktivera direkt från [!DNL Content]_**. Att välja en godkänd upplevelse med fördefinierade inställningar är det mest effektiva sättet att starta en aktivering i en enda kanal.

* **Sammanställ din annonsupplevelse från [!DNL Activate] > _Upplevelsekonfiguration_**&#x200B;Du kan skapa en upplevelse genom att välja visuella resurser från&#x200B;_[!DNL Content]_, lägga till textelement och välja proportioner. Den här metoden har fler steg men ger större flexibilitet när du skapar en kreativ upplevelse.

### Aktivera en godkänd upplevelse från innehåll

Ni kan välja mer än en upplevelse att aktivera till en enda betalkanal. Du kan behöva välja en plattform innan du fortsätter med aktiveringen.

Om du har markerat mer än en upplevelse som ska aktiveras som en grupp använder du det vänstra sidofältet för att fokusera vyn _Experience setup_ på informationen för den valda upplevelsen.

1. Använd söknings- och filterverktygen i _[!DNL Content]_-galleriet för att identifiera den upplevelse som du vill aktivera och klicka sedan på&#x200B;**[!UICONTROL Activate]**.

   Sidan Metaannonser _Experience setup_ öppnas för den här upplevelsen. Den är förifylld med information från den valda upplevelsen. Du kan redigera fälten **[!UICONTROL Call-to-action]**, **[!UICONTROL Website URL]** och **[!UICONTROL Display link]**. Om du väljer mer än en upplevelse att aktivera, innehåller vyn _Upplevelsekonfiguration_ en vänster sidospalt som visar miniatyrbilder av alla valda upplevelser. Använd den här vänstra sidofältet för att fokusera vyn _Experience setup_ på informationen för den valda upplevelsen.

1. Välj en kampanj i listrutan **[!UICONTROL Campaigns]**.

   Om du arbetar med flera upplevelser kan du växla mellan upplevelserna i det vänstra sidofältet tills du har färdigställt varje upplevelse.

1. Klicka på **[!UICONTROL Next]** för att bekräfta dina inställningar för Meta-annonser.

1. Ge varje upplevelse ett namn. Efter aktiveringen kan du använda det här namnet för att söka efter den här upplevelsen i tabellen _Aktiverade upplevelser_.

### Sammanställ upplevelsekomponenter

Om du väljer att inte direkt aktivera en godkänd upplevelse från _[!DNL Content]_&#x200B;kan du välja resurser, tilldela proportioner och utkasttextelement.

**Så här förbereder du din upplevelse för aktivering**:

1. Från _[!DNL Activate]_&#x200B;klickar du på&#x200B;**[!UICONTROL New]**&#x200B;på ikonen som representerar din valda betalda kanal. Vyn_ Experience Setup _öppnas.

   Sidan _Experience setup_ är en central plats för att förbereda er annonsaktivering. Förbereda din annons innehåller följande tre uppgifter:

1. Ge upplevelsen ett namn. Efter aktiveringen kan du använda det här namnet för att söka efter den här upplevelsen i tabellen _Aktiverade upplevelser_.
1. Välj medieresurser. Du kan använda resurser från _[!DNL Content]_&#x200B;eller överföra externa resurser (till exempel från OneDrive eller Dropbox).
1. [Lägg till text](#add-ad-text).
1. [Lägg till metadata](#assign-metadata).

   _Förhandsgranskningspanelen_ har stöd för en interaktiv vy av text och resurser i en specifik annonsplacering. Använd listrutan _Välj placering_ för att växla mellan annonsplaceringar som stöds. Med förhandsgranskningar kan du slutföra beslut om annonselement för specifika placeringar. När du väljer en placering på panelen _Förhandsgranska_ påverkas bara annonsvyn. Ditt placeringsval på panelen _Förhandsgranska_ sparas inte.

### Välj medieresurser

Använd avsnittet _Media_ för att välja minst en bildresurs som ska ingå i din upplevelse. Annonsplaceringar är associerade med bildproportioner som stöds, som visas som alternativ i listrutan _Placeringar_ . Den här menyn visar vilka annonsplaceringar som stöds för Facebook-inlägg eller Instagram-artiklar, ordnade efter proportioner.

Efter överföring sparas resurserna i _[!DNL Content]_. I området_ Media _visas bilden som standard med bildförhållandet 1:1. Alternativa proportioner inkluderar bara de värden som stöds av den betalda annonskanalen. De grupperas efter lodrät och vågrät orientering. GenStudio for Performance Marketing stöder användning av upp till sex bildproportioner per aktiverad upplevelse.

**Så här överför du en resurs från innehåll**:

_[!DNL Content]_&#x200B;ger en central vy för din organisations godkända resurser och upplevelser. Du kan fokusera det[_[!DNL Content]_-galleriet](/help/user-guide/content/manage-assets.md) som visar lager med resurser med menyalternativen **[!UICONTROL Search]** (förstoringsglas) och _Filter_ .

1. Klicka på **[!UICONTROL New]** på kanalkortet från _[!DNL Activate]_. Vyn_ Experience Setup _öppnas.

1. Klicka på **[!UICONTROL Select]** och välj sedan **[!UICONTROL Select from Content]**. Vyn _Välj innehåll_ öppnas och ett galleri med bildresurser som du söker igenom eller filtrerar visas.

1. Använd _[!DNL Content]_-galleriets sök- och filterverktyg för att välja minst en resurs som ska överföras.

1. Klicka på **[!UICONTROL Use]** om du vill inkludera den valda resursen i annonsupplevelsen. Fönstret _Experience Setup_ innehåller resursen i standardproportionen i området _Media_. Panelen _Förhandsvisa_ förhandsvisar resursen i annonsplaceringen som stöder den här proportionen.

Om överföringen inte lyckas visas ett informativt felmeddelande som innehåller en länk till resursen i _[!DNL Content]_.

**Så här överför du en extern resurs**:

Du kan överföra upp till sex statiska bilder utanför galleriet _[!DNL Content]_&#x200B;från antingen Microsoft OneDrive eller Dropbox.

1. Klicka på **[!UICONTROL New]** på panelen Meta i _[!DNL Activate]_. Fönstret_ Experience Setup _öppnas.

1. Klicka på **[!UICONTROL Select]** i avsnittet _Media_. I en nedrullningsbar meny visas alternativ för att _välja från innehåll_ eller _överföra_.

1. Klicka på **[!UICONTROL Upload]**. Fönstret _Lägg till proportioner_ öppnas.

1. Välj bilder i de proportioner som stöds genom att dra och släppa bildfiler i bildens överföringsområde. Du kan även söka efter resurser på enheten.

1. (Valfritt) Om du vill överföra resurser från din enhet klickar du på **[!UICONTROL Browse]** och väljer sedan _Bläddra bland filer_ eller _Bläddra bland mappar_ för att identifiera resurser som ska överföras.

1. I området _Lägg till information_ lägger du till informativ information till dina överförda resurser för att underlätta sökning och filtrering i _[!DNL Content]_. Dessa uppgifter sparas som metadata.

1. När du har överfört dina resurser och tilldelad information klickar du på **[!UICONTROL Add Assets]** längst ned till höger.

### Lägga till text

Använd avsnittet _Text_ på sidan _Aktivera meta-annons_ för att lägga till övertygande, varumärkesanpassad text i obligatoriska textfält. Texten innehåller den primära (brödtexten) texten för annonsen och texten för uppmaning att ringa in. Du kan inte redigera fälten _Primär text_, _Rubriker_ och _Beskrivning_. Du kan redigera fälten _Call-to-action_, _Visningslänk_ och _URL-adress för webbplats_.

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

GenStudio for Performance Marketing kräver _primär text_ och _rubrik_, inte metadata.

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

När du har sammanställt eller valt din upplevelse klickar du på **[!UICONTROL Next]** för att bekräfta metainställningen.

## Steg 4: Bekräfta konfigurationen av meta-kontot

När ni har förberett era annonsupplevelser måste ni bekräfta era Meta-kontouppgifter. Vyn _Meta och konfiguration_ har fyllts i med alternativ som härleds från de konfigurerade Meta-kontona.

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

På sidan _Granska_ visas din annonsupplevelse som den är sammansatt i _Experience setup_ och du får en sista möjlighet att visa och redigera din upplevelse. Klicka på **[!UICONTROL Edit section]** bredvid etiketten _Experience setup_ för att göra ändringarna. Du kan också klicka på **[!UICONTROL Back]** i det övre högra hörnet för att gå tillbaka till sidan _Experience setup_ .

### Steg 6: Fullständig aktivering av annonsupplevelsen

1. Klicka på **[!UICONTROL Publish]**.

   Den fullständiga annonsupplevelsen för Meta och tillhörande metadata överförs direkt till den valda annonsuppsättningen för Meta Ads Manager. Upplevelserna levereras till Meta Ads Manager i ett inaktivt tillstånd. Från Meta Ads Manager kan ni hantera de sista stegen i distributionen av annonsupplevelsen och Meta-kampanjen.

1. [Logga in på Meta Ads Manager](https://adsmanager.facebook.com/) för att granska annonsupplevelsen och slutföra publiceringen i specifika Meta-kanaler.
