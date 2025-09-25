---
title: Aktivera en Meta-annons
description: Lär dig hur du aktiverar en annonsupplevelse från Meta.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
source-git-commit: 0ccdeb2b3375e9ee72bfc4458eeaff11709768cb
workflow-type: tm+mt
source-wordcount: '1868'
ht-degree: 0%

---

# Aktivera en Meta-annons

Adobe GenStudio for Performance Marketing stöder aktivering av Meta annonsupplevelser för Instagram och Facebook.

Du kan [skapa en Meta-upplevelse](/help/user-guide/create/create-meta-ad.md) i GenStudio for Performance Marketing och välja den för aktivering, eller skapa en ny upplevelse från godkända resurser i [!DNL Activate].

När du aktiverar en Meta-annons följer [samma allmänna steg](create-activation.md) som krävs för aktivering i andra betalda kanaler. Aktiveringsprocessen har stöd för att förbereda er annonsupplevelse för Meta specifika krav. När du har aktiverat en Meta-upplevelse i GenStudio for Performance Marketing använder du [Meta Ads Manager](https://adsmanager.facebook.com/) för att finjustera upplevelsen för specifika Meta-annonsplaceringar innan den slutliga publiceringen.

GenStudio systemansvariga och redaktörer kan aktivera annonsupplevelser.

## Steg 1: Konfigurera dina Meta-konton

[Logga in på Meta](https://adsmanager.facebook.com/) för att få åtkomst till ditt Meta Ads Manager-konto innan du startar en aktivering.

>[!BEGINSHADEBOX]

**Förutsättningar**:

Bekräfta att dina anslutna Meta-annonskonton har fullständig behörighet att hantera annonser i de här komponenterna av Meta annonsplattform:

* Facebook-sida
* Meta-kampanj
* Meta ad set
* Instagramprofil (valfritt)

>[!ENDSHADEBOX]

## Steg 2: Anslut till dina Meta-konton

Innan ni kan aktivera upplevelser måste en GenStudio-systemadministratör koppla era Meta-konton till GenStudio for Performance Marketing. Tack vare den här anslutningen kan data flöda mellan GenStudio och externa marknadsföringsverktyg som Meta, vilket möjliggör aktiveringsprocessen.

Se [Ansluta till Meta Ads](/help/user-guide/connectors/meta-ads.md).

När synkroniseringen har slutförts kan du visa de tillagda kontona. Stora mängder data tar längre tid att synkronisera.

## Steg 3: Förbered din upplevelse för aktivering

Du kan starta en aktivering på två sätt:

* **Aktivera direkt från[!DNL Content]**. Att välja en godkänd upplevelse med fördefinierade inställningar är det mest effektiva sättet att starta en aktivering i en enda kanal.

* **Samla din annonsupplevelse från [!DNL Activate] > _Experience setup_**. Du kan skapa en upplevelse genom att välja visuella resurser från [!DNL Content], lägga till textelement och välja proportioner. Den här metoden har fler steg men ger större flexibilitet när du skapar en kreativ upplevelse.

### Aktivera en godkänd upplevelse från innehåll

Ni kan välja mer än en upplevelse att aktivera till en enda betalkanal. Du kan behöva välja en plattform innan du fortsätter med aktiveringen.

Om du har markerat mer än en upplevelse som ska aktiveras som en grupp använder du det vänstra sidofältet för att fokusera vyn _Experience setup_ på informationen för den valda upplevelsen.

1. Använd söknings- och filterverktygen i [!DNL Content]-galleriet för att identifiera den upplevelse som du vill aktivera och klicka sedan på **[!UICONTROL Activate]**.

   Sidan _Upplevelsekonfiguration_ visas för den här upplevelsen. Den är förifylld med information från den valda upplevelsen. Du kan redigera fälten **[!UICONTROL Call-to-action]**, **[!UICONTROL Website URL]** och **[!UICONTROL Display link]**. Om du väljer mer än en upplevelse att aktivera, innehåller vyn _Upplevelsekonfiguration_ en vänster sidospalt som visar miniatyrbilder av alla valda upplevelser. Använd den här vänstra sidofältet för att fokusera vyn _Experience setup_ på informationen för den valda upplevelsen.

1. Välj en kampanj i listrutan **[!UICONTROL Campaigns]**.

   Om du arbetar med flera upplevelser kan du växla mellan upplevelserna i det vänstra sidofältet tills du har färdigställt varje upplevelse.

1. Klicka på **[!UICONTROL Next]** för att bekräfta konfigurationen av dina Meta-annonser.

1. Ge varje upplevelse ett namn. Efter aktiveringen kan du använda det här namnet för att söka efter den här upplevelsen i tabellen _Aktiverade upplevelser_.

### Sammanställ upplevelsekomponenter

Om du väljer att inte direkt aktivera en godkänd upplevelse från [!DNL Content] kan du välja resurser, tilldela proportioner och utkasttextelement.

**Så här förbereder du din upplevelse för aktivering**:

1. Från [!DNL Activate] klickar du på **[!UICONTROL New]** på ikonen som representerar din valda betalda kanal. Vyn _Experience Setup_ öppnas.

   Sidan _Experience setup_ är en central plats för att förbereda er annonsaktivering. Förbereda din annons innehåller följande tre uppgifter:

1. Ge upplevelsen ett namn. Efter aktiveringen kan du använda det här namnet för att söka efter den här upplevelsen i tabellen _Aktiverade upplevelser_.
1. Välj medieresurser. Du kan använda resurser från [!DNL Content] eller överföra externa resurser (till exempel från OneDrive eller Dropbox).
1. [Lägg till text](#add-ad-text).
1. [Lägg till metadata](#assign-metadata).

   _Förhandsgranskningspanelen_ har stöd för en interaktiv vy av text och resurser i en specifik annonsplacering. Använd listrutan _Välj placering_ för att växla mellan annonsplaceringar som stöds. Med förhandsgranskningar kan du slutföra beslut om annonselement för specifika placeringar. När du väljer en placering på panelen _Förhandsgranska_ påverkas bara annonsvyn. Ditt placeringsval på panelen _Förhandsgranska_ sparas inte.

### Välj medieresurser

Använd avsnittet _Media_ för att välja minst en bildresurs som ska ingå i din upplevelse. Annonsplaceringar är associerade med bildproportioner som stöds, som visas som alternativ i listrutan _Placeringar_ . Den här menyn visar vilka annonsplaceringar som stöds för Facebook-inlägg eller Instagram-artiklar, ordnade efter proportioner.

Efter överföring sparas resurserna i [!DNL Content]. I området _Media_ visas bilden som standard med bildförhållandet 1:1. Alternativa proportioner inkluderar bara de värden som stöds av den betalda annonskanalen. De grupperas efter lodrät och vågrät orientering. GenStudio for Performance Marketing stöder användning av upp till sex bildproportioner per aktiverad upplevelse.

**Så här överför du en resurs från innehåll**:

[!DNL Content] ger en central vy för din organisations godkända resurser och upplevelser. Du kan fokusera det [[!DNL Content] galleri](/help/user-guide/content/manage-assets.md) som visas på resursen med menyalternativen **[!UICONTROL Search]** (förstoringsglas) och _Filter_ .

1. Klicka på [!DNL Activate] på kanalkortet från **[!UICONTROL New]**. Vyn _Experience Setup_ öppnas.

1. Klicka på **[!UICONTROL Select]** och välj sedan **[!UICONTROL Select from Content]**. Vyn _Välj innehåll_ öppnas och ett galleri med bildresurser som du söker igenom eller filtrerar visas.

1. Använd [!DNL Content]-galleriets sök- och filterverktyg för att välja minst en resurs som ska överföras.

1. Klicka på **[!UICONTROL Use]** om du vill inkludera den valda resursen i annonsupplevelsen. Fönstret _Experience Setup_ innehåller resursen i standardproportionen i området _Media_. Panelen _Förhandsvisa_ förhandsvisar resursen i annonsplaceringen som stöder den här proportionen.

Om överföringen inte lyckas visas ett informativt felmeddelande som innehåller en länk till resursen i _[!DNL Content]_.

**Så här överför du en extern resurs**:

Du kan överföra upp till sex statiska bilder utanför galleriet [!DNL Content] från antingen Microsoft OneDrive eller Dropbox.

1. Klicka på [!DNL Activate] på Meta-panelen i **[!UICONTROL New]**. Fönstret _Experience Setup_ öppnas.

1. Klicka på _i avsnittet_ Media **[!UICONTROL Select]**. I en nedrullningsbar meny visas alternativ för att _välja från innehåll_ eller _överföra_.

1. Klicka på **[!UICONTROL Upload]**. Fönstret _Lägg till proportioner_ öppnas.

1. Välj bilder i de proportioner som stöds genom att dra och släppa bildfiler i bildens överföringsområde. Du kan även söka efter resurser på enheten.

1. (Valfritt) Om du vill överföra resurser från din enhet klickar du på **[!UICONTROL Browse]** och väljer sedan _Bläddra bland filer_ eller _Bläddra bland mappar_ för att identifiera resurser som ska överföras.

1. I området _Lägg till information_ lägger du till informativ information till dina överförda resurser för att underlätta sökning och filtrering i _[!DNL Content]_. Dessa uppgifter sparas som metadata.

1. När du har överfört dina resurser och tilldelad information klickar du på **[!UICONTROL Add Assets]** längst ned till höger.

### Lägga till text

Använd avsnittet _Text_ på sidan _Aktivera Meta-annons_ för att lägga till övertygande, varumärkesanpassad text i obligatoriska textfält. Texten innehåller den primära (brödtexten) texten för annonsen och call-to-action-texten. Du kan inte redigera fälten _Primär text_, _Rubriker_ och _Beskrivning_. Du kan redigera fälten _Call-to-action_, _Visningslänk_ och _URL-adress för webbplats_.

| Fält | Obligatoriskt | Teckengräns (max) |
|-----------------|---------------------------|---------------------------------|
| Annonsnamn | ja | 500 |
| Primär text | ja | 500 |
| Headline | ja | 255 |
| Beskrivning | no | 125 |
| Call to action | ja | endast alternativ i listrutor |
| Visa URL | no | 1000 |
| Webbplatsens URL | ja | 1000 |
| Bild | minst en |                                 |

GenStudio for Performance Marketing kräver _primär text_ och _rubrik_, inte Meta.

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

När du har sammanställt eller valt din upplevelse klickar du på **[!UICONTROL Next]** för att bekräfta din Meta-konfiguration.

## Steg 4: Bekräfta konfigurationen av Meta-kontot

När ni har förberett era annonsupplevelser måste ni bekräfta er kontoinformation för Meta. Vyn _Meta-annonskonfiguration_ har fyllts i med alternativ som härleds från de konfigurerade Meta-kontona.

| Detalj | Beskrivning |
|------------|-------------|
| Konton | Meta-konton som är anslutna till GenStudio for Performance Marketing |
| Facebook-sida | Facebook-sida där upplevelsen publiceras |
| Instagram-konto | Instagramkonton som har anslutits till GenStudio for Performance Marketing |
| Kampanjer | Meta-kampanjer som annonsupplevelsen tillhör |
| Annonsuppsättningar | Meta annonsuppsättningar som den aktiverade annonsupplevelsen tillhör. Inställningarna bestämmer den slutliga placeringen av annonsen. |

### Skapa en ny annonsuppsättning

Du kan skapa en ny annonsuppsättning under plattformskonfigurationen genom att klona en befintlig annonsuppsättning under plattformskonfigurationen. Metaannonser definierar timing, kanalinformation och publik för en viss annons. En Meta-kampanj kan innehålla flera annonsuppsättningar, men en annonsuppsättning är exklusivt kopplad till en kampanj.

**Så här skapar du en ny annonsuppsättning**:

1. Välj en kampanj i listrutan _Meta-kampanjer_.

   Den valda kampanjen avgör vilka annonsuppsättningar som är tillgängliga som alternativ i den nedrullningsbara menyn _Annonsuppsättningar_.

1. Klicka på **[!UICONTROL + Create new ad set]**.

   Popup-fönstret _Skapa ny annonsuppsättning_ öppnas och identifierar den Meta-kampanj där den nya annonsuppsättningen skapas.

1. Välj den annonsuppsättning som du vill klona i listrutan _Använd konfiguration_.

   GenStudio for Performance Marketing tilldelar ett standardannonsmängdsnamn genom att lägga till `- Copy` till det valda annonsmängdsnamnet.

1. (Valfritt men rekommenderas) Ange ett unikt annonsnamn i fältet **[!UICONTROL New ad set name]** om du vill ersätta standardvärdet.

1. Klicka på **[!UICONTROL Create ad set]**.

   Du återgår till vyn _Plattformskonfiguration_ där den nya annonsuppsättningen är förvald. Ett meddelande visas med en länk till annonsuppsättningen i Meta Ads Manager. Den här annonsuppsättningen är tillgänglig för framtida aktiveringar.

>[!NOTE]
>
>Om annonsuppsättningen har skapats men det inte gick att spara annonsuppsättningsnamnet, sparas annonsuppsättningen i Meta Ads Manager med standardnamnet (_ursprungligt annonsuppsättningsnamn - Kopia_).

### Spårnings-ID

Spårnings-ID:n (annonsnamn) tillhandahåller en mekanism för att samla in mätvärden som är länkade till upplevelseresultatet. Ange annonsnamnet i det här fältet.

Klicka på **[!UICONTROL Next]** i det övre högra hörnet för att förhandsgranska din annonsupplevelse och slutföra aktiveringen.

## Steg 5: Förhandsgranska och aktivera annonsen

På sidan _Granska_ visas din annonsupplevelse som den är sammansatt i _Experience setup_ och du får en sista möjlighet att visa och redigera din upplevelse. Klicka på **[!UICONTROL Edit section]** bredvid etiketten _Experience setup_ för att göra ändringarna. Du kan också klicka på **[!UICONTROL Back]** i det övre högra hörnet för att gå tillbaka till sidan _Experience setup_ .

### Steg 6: Fullständig aktivering av annonsupplevelsen

1. Klicka på **[!UICONTROL Publish]**.

   Den kompletta annonsupplevelsen i Meta och tillhörande metadata överförs direkt till den valda annonsuppsättningen i Meta Ads Manager. Upplevelserna levereras till Meta Ads Manager i ett inaktivt tillstånd. Från Meta Ads Manager kan ni hantera de sista stegen i driftsättningen av annonsupplevelsen och Meta kampanj.

1. [Logga in på Meta Ads Manager](https://adsmanager.facebook.com/) för att granska annonsupplevelsen och slutföra publiceringen i specifika Meta-kanaler.
