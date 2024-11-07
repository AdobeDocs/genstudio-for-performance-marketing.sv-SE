---
title: Versionsinformation för Adobe GenStudio for Performance Marketing
description: Läs om de senaste funktionerna och förbättringarna i Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
source-git-commit: b502e0a558cbc26c70d813938734a2f6f230dc8e
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Versionsinformation för GenStudio for Performance Marketing

Den här versionsinformationen innehåller information om de senaste uppdateringarna av GenStudio for Performance Marketing-programmet.

## 2024.11.07 {#latest}

### Korrigeringar

* Rotationsrutan _Spara i arbete_ visas inte längre när en användare klickar på **[!UICONTROL Upload New Image]** och sedan avbryter åtgärden innan överföringen har slutförts. <!-- GS-6780 -->

* Upplevelsetitlar skapas nu korrekt vid upplevelsegenerering. <!-- GS-7006 -->

* Problem med flimrade rullningslister vid inläsning av utkast har lösts. <!-- GS-5587 -->

* Länken `View documentation` i popup-fönstret [!DNL Content] _Lägg till den godkända mallen_ fungerar nu som förväntat. <!-- GS-6881 -->

* Om du tar bort en bild från promptlådan under en storleksändring uppstår inte längre något fel. <!-- GS-7115 7009 -->

* Markering av **[!UICONTROL Delete]** från åtgärdsmenyn [!DNL Create] (..) fungerar nu som förväntat. <!-- GS-6871 -->

* Användarna kan nu styra alla interaktiva element i Meta- och mallarna enbart med tangentbordet. <!-- GS-4066 -->

* Hämtning av bilddimensioner från mallbildfält har lagts till för att visa annonsmallar. Begäran om smart beskärning skickas nu för den faktiska dimensionen av bilden och inte för hela mallen. <!-- GS-6926 -->

* Strängen `Zoom to fit to screen` har lokaliserats i genererade e-post- och Meta-annonser. <!-- GS-5063 -->

* Frågekassen [!DNL Create] stängs nu som förväntat när en användare klickar bort. <!-- GS-5254 -->

* Export av metaannonser innehåller nu den valda etiketten för att ringa upp till åtgärd som förväntat. <!-- GS-6504 -->

* Varumärkespoängen uppdateras nu och behålls som förväntat för återskapade upplevelser. <!-- GS-6535 -->

* HTML-export av Meta-annonser och visningsannonser innehåller inte längre wrapper `div`- och `chrome`-element. <!-- GS-7116 -->

* Problem med återgivning av utkast via e-post vid publicering har nu lösts. <!-- GS-6394 -->

* Knappen Canvas **[!UICONTROL Brand]** är nu inaktiverad när ingen varumärkespoäng genereras. <!-- GS-6429 -->

* Växlingen Facebook/Instagram i åtgärdsfältet för arbetsytan uppdaterar nu den rendering som du förväntade dig när inställningen för arbetsytan `ReadOnly` är aktiverad. <!-- GS-7039 -->

#### Omgenerering av bilder

* Att ändra storlek på flera Meta ad-varianter fungerar nu som väntat. Tidigare visades inte regenererade varianter på arbetsytan, men de förblev tomma. <!-- GS-7010 -->

* Fragmentomgenerering fungerar nu som förväntat för upplevelser med ändrad storlek. <!-- GS-6836 -->

* Återskapande av Meta-annonser efter att de har ändrat storlek resulterar inte längre i ett fel. Tidigare ändrades kanalens metadata från `meta` till `facebook` när bilder ändrades före omgenerering. <!-- GS-7042 -->

## 2024.10.31

### Nya funktioner

* Sökfiltret **[!DNL Content]** har nu stöd för sökning efter färgtagg. <!-- GS-5501 -->

* Arbetsytan **[!DNL Create]** visar nu teckenantal för e-postfragment. <!-- GS-5819 -->

### Korrigeringar

* Etiketter för skärmläsare som saknas har lagts till i `view`-element för mobiler och datorer. <!-- GS-5624 4729 -->

* Ämnesraden och textområdena före sidhuvudet på **[!DNL Create]**-arbetsytan är nu dynamiska i höjdled. <!-- GS-6258 -->

* Layoutproblem med e-postkanter har lösts. <!-- GS-6631 -->

* Tangentbordsfokus fungerar nu som väntat på knappen **[!DNL Content]** **[!UICONTROL Delete]**. Tidigare gick det inte att nå eller använda den här knappen med tangentbordet.  <!-- GS-4065 -->

## 2024.10.14 General Availability release

I den här versionen presenteras Adobe GenStudio for Performance Marketing, en generativ AI-baserad applikation som snabbar upp planering, utveckling och analys av marknadsföringskampanjer. GenStudio for Performance Marketing ger marknadsföringsteamen möjlighet att skapa varumärkesanpassat flerkanalsinnehåll för annonser, e-post och kampanjer samtidigt som ni får realtidsinsikter för att optimera innehållets prestanda.

### Funktioner

Några viktiga funktioner:

I **[!DNL Create]** introduceras arbetsytan, som erbjuder en strukturerad frågeupplevelse som gör det möjligt för innehållsredigerare att snabbt generera innehåll och varianter. Systemansvariga utbildar produkten enligt riktlinjer för varumärken. [!DNL Create] ser till att allt AI-genererat innehåll följer varumärkesriktlinjerna - branding, kundprofiler och produktbeskrivningar - och effektiviserar produktionen av slagkraftigt, varumärkesenhetligt marknadsföringsmaterial.

**[!DNL Content]** lagrar förvaltade, varumärkeskompatibla, godkända resurser och upplevelser. GenStudio for Performance Marketing-användare kan enkelt hitta, redigera, återanvända och dela godkända mediefiler, vilket minskar behovet av att återskapa innehåll från grunden för varje kampanj.

**[!DNL Reviews and Approvals]** skapar ett ramverk för intressenter som kan granska och godkänna genererade varianter innan de sparar till **[!DNL Content]** eller exporterar.

**[!DNL Campaigns]** organiserar och hanterar marknadsföringskampanjer och säkerställer smidig körning och spårning. Medarbetarna kan visualisera, planera och spåra kampanjer för att hantera flera initiativ effektivt och säkerställa att de levereras i rätt tid.

**[!DNL Insights]** erbjuder realtidsutvärdering av innehållsprestanda, vilket hjälper marknadsförarna att optimera sina strategier och fatta datadrivna beslut.

GenStudio for Performance Marketing kan integreras med andra Adobe Experience Cloud-produkter, inklusive Adobe Express och Adobe AEM Assets.

### Ytterligare information

Se följande resurser:

* [Adobe GenStudio for Performance Marketing Användarhandbok](https://experienceleague.adobe.com/en/docs/genstudio/user-guide/home)

* [Adobe GenStudio Academy](genstudioacademy.md), Adobe onlineutbildningsplattform för att använda generativa AI-tekniker i den kreativa processen. [Registrera dig för GenStudio Academy](http://adobe.ly/genstudioacademyregistration).
