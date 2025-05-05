---
title: Versionsinformation för Adobe GenStudio for Performance Marketing Beta
description: Läs om de senaste funktionerna och förbättringarna i Adobe GenStudio for Performance Marketing.
hidefromtoc: true
hide: true
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: ad532813338a7506483c2ab5892a61d7dc4785d4
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# Versionsinformation för Adobe GenStudio for Performance Marketing Beta

I dessa anmärkningar beskrivs viktiga Adobe GenStudio for Performance Marketing-korrigeringar och förbättringar för den vecka som slutar den 4 oktober.

## Nya funktioner och förbättringar

* Filtreringsmöjligheterna i hela produkten har förbättrats. Problem med filtrering efter ålder och kön i [!DNL Insights] har lösts.  <!-- GS-1198 -->

* Du kan redigera bildresurser (JPG eller PNG) direkt med Adobe Express. Innehållsredigerare kan använda arbetsytan i _[!UICONTROL Powered by Adobe Express]_&#x200B;för att ta bort bakgrunder, använda generativa fyllningar, justera effekter och beskära bilder utan att lämna GenStudio for Performance Marketing. <!-- GS-4615 -->

* Förbättrade upplevelsen av progressiv inläsning av genererade varianter, genererad e-post och sammanhangsbaserade meddelanden. <!-- GS-4651 3062-->

* Innehållsredigerare kan nu använda funktionen för att justera beskärning för att beskära återgivna bilder i varianter. <!-- GS-2342 -->

* Problem med att ändra storlek och duplicera mallar har lösts. <!-- GS-4895 -->

* Märkesvalidering förklarar nu orsaken till fel som inträffar under valideringen.

* I mallförhandsvisningar visas nu text i bilden som förväntat. <!-- GS-5917 -->

## Ytterligare förbättringar och åtgärdade problem

* Arbetsytan [!DNL Create] återger nu anpassade teckensnitt från mallar som förväntat. <!-- GS-3415 -->

* Det rätta teckensnittet används nu vid export av Meta-annonser. <!-- GS-5875 -->

* Problem med mallöverföring som resulterade i slutförd överföring men som inte syns i produktgränssnittet har åtgärdats. <!-- GS-4815 5650-->

* Användarna kan nu beskära Meta-annonser manuellt efter att de har ändrat storlek. <!-- GS-5871 -->

* Användare behöver inte längre logga in två gånger på ett Meta-annonskonto i en kanal när de också är inloggade på Facebook. <!-- GS-3009 -->

* Arbetsytans vy av resurser och upplevelser är nu konsekvent när det gäller att skapa, granska och godkänna innehåll. <!-- GS-5877 -->

* På arbetsytan visas nu endast fyra varianter när du återskapar efter en storleksändring. <!-- GS-5869 -->

* Webbläsarbaserad stavningskontroll fungerar nu som förväntat på arbetsytan i [!DNL Create]. <!-- GS-5760 -->

* Visningsannonser exporteras nu som PNG-filer när **[!UICONTROL Export as PNG]** är markerat. Tidigare exporterades visningsannonser som JPEG när PNG-formatet valdes. <!-- GS-5545 -->

* Utfyllnaden har ökat mellan knappen **[!UICONTROL Manual crop]** och knappen **[!UICONTROL Generate]**. Tidigare var knappen **[!UICONTROL Manual crop]** delvis dold. <!-- GS-6084 -->

* I mallförhandsvisningar visas nu Google-teckensnitt som förväntat. <!-- GS-5946 -->

* Importerade TypeKit- och Google-teckensnitt läses nu in som förväntat under exporten. <!-- GS-5948 -->

* Löste problem med att generera innehåll med anpassade mallar. Tidigare visades inte popup-fönstret när en innehållsredigerare försökte generera en resurs med en anpassad mall och konsolen visade fel. <!-- GS-5262 -->

* DisplayAds-utkastet av arbetsytan behåller nu sin position när en användare högerklickar på arbetsytan innan han/hon vänsterklickar utanför snabbmenyn. Tidigare flyttades arbetsytan när användaren vänsterklickade, vilket gjorde att utkastinnehållet inte var delvis tillgängligt.  <!-- GS-5687 -->

* Inläsningen av skuggningseffekter kvarstår tills bildomformningen är klar.  <!-- GS-5811 -->

* Poängen för varumärkesvalidering ogiltigförklaras inte längre efter att en användare har redigerat genererade e-postmeddelanden, Meta-annonser eller visningsannonser. Tidigare var poängen dold. <!-- GS-5379 -->

* Mallar som har CSS-format kopplade till sitt `body`-element används nu som förväntat vid export av upplevelser. <!-- GS-5947 -->

* Problem med manuell beskärning av stora dimensionsbilder har korrigerats. <!-- GS-6039 -->

* Endast ett popup-meddelande visas nu när en användare lägger till en ny resurs i [!DNL Content]. <!-- GS-5020 -->

* Förbättrade arbetsyteprestanda vid textredigering.  <!-- GS-5118 -->

* Lagt till blanksteg mellan strängar i e-postmeddelandet [!DNL Create] eller i Meta och Canvas. <!-- GS-5019 -->

* Redigerare kan nu spara en fil med namn som innehåller specialtecken efter redigering i Express. <!-- GS-6131 -->

### Lokalisering

Den här versionen innehåller förbättringar av lokaliseringen i hela produktgränssnittet, bland annat följande gränssnittsområden:

* URL:en för målet för alternativet **[!UICONTROL Learn more]** på snabbmenyn [!DNL Create]. <!-- GS-5029 -->

* Nummerformat intill [!DNL Insights] > [!DNL Experience] sökindatafält. <!-- GS-4494 -->

## Känt fel

* Återskapade e-postfragment visas inte i varianten efter markeringen. (Varianter visas dock efter att utkastet har öppnats på nytt.) <!-- GS-5913 -->
