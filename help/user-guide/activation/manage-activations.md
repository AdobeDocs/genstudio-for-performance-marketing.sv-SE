---
title: Hantera aktiveringar
description: Lär dig hantera aktiverade upplevelser med Adobe GenStudio for Performance Marketing.
feature: Ad Activation
exl-id: 7cf340d4-37ab-4906-9aad-088a26db0818
source-git-commit: 0ccdeb2b3375e9ee72bfc4458eeaff11709768cb
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---

# Hantera aktiveringar

[!DNL Activate] erbjuder en centraliserad vy över varje annonskanals aktiveringsstatus, inklusive aktiveringar av typen Publicerad (lyckades), Misslyckad (misslyckades) och Publicering (väntar). Vyn _Aktiverade upplevelser_ visar alla aktiveringar för ett anslutet kanal- och annonskonto.

[!DNL Activate] organiserar aktiverade upplevelser per annonskanal. Klicka på **[!UICONTROL View]** i kanalpanelen. Vyn _Aktiverade upplevelser_ för den valda kanalen öppnas. I den här vyn visas upplevelser per namn och beställningar per aktiveringsdatum. Om din organisation inte har aktiverat upplevelser för den kanalen, innehåller produktrutan inte knappen **[!UICONTROL View]**.

## Aktiverad upplevelsevy

I den här vyn visas aktiveringar efter upplevelsenamn i fallande kronologisk ordning (den senaste listan först).

I följande tabell visas de attribut som definierar varje upplevelse.

| Attribut | Värde |
|------------------|---------------------------------------------------------------------------------------------|
| Experience name | Namnet på upplevelsen i GenStudio for Performance Marketing<br>Det här namnet identifierar upplevelsen i _[!DNL Content]_ |
| Annonsnamn | Annonsens namn i annonskanalen |
| Publiceringsdatum | Datum när annonsupplevelsen publicerades<br>Använder månadsdagens format |
| Publicerat av | Namn på den GenStudio for Performance Marketing-användare som aktiverade upplevelsen |
| Regioner | Det geografiska område där upplevelsen lanseras |
| Status | Status för den valda annonsupplevelsen<br>Värdena omfattar Misslyckad, Publicerad och Publicering |

Använd **[!UICONTROL Search]** (förstoringsglas) eller bläddra i upplevelselistan för att hitta en aktivering efter upplevelsenamn.

Klicka på aktiveringen för att öppna en fokuserad översikt över aktiveringsinformationen.

## Detaljvy

Klicka på en aktivering i vyn _Aktiverade upplevelser_. Den skrivskyddade vyn _Aktiveringsinformation_ innehåller definieringsinformationen för en aktiverad upplevelse, inklusive misslyckade aktiveringar. Vyn innehåller information som hämtats från både GenStudio for Performance Marketing och annonskanalen.

* **Publiceringstid och publiceringsdatum**: Tid och datum för publicering från annonskanalhanteraren
* **Annons-ID**: ID som tilldelats av den betalda kanalen och används för spårning. Klicka på knappen **[!UICONTROL Open]** bredvid det här fältet för att visa den publicerade annonsen i Meta Ads Manager
* **Upplevelseinformation**: De valda bildresurserna, texterna och metadata som tilldelats under GenStudio for Performance Marketing-aktiveringsarbetsflödet
* **Kanalinställning**: De betalda kanalkonton som används för att aktivera annonsupplevelsen

Vyn _Information_ för en misslyckad aktivering innehåller orsaken till felet.
