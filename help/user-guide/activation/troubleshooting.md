---
title: Optimera aktiveringen
description: Lär dig hur du optimerar aktiveringar till betalda annonskanaler från tredje part.
level: Intermediate
feature: Ad Activation
exl-id: 5bc624c2-d064-4190-8761-ed05d0629d1f
source-git-commit: 0ccdeb2b3375e9ee72bfc4458eeaff11709768cb
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# Optimera aktiveringar

Aktivering av annonsupplevelser för betalda annonskanaler omfattar två huvudfaser:

* Förbereda för aktivering

* Publicera din upplevelse till de utnämnda betalda kanalannonsansvariga

Om ni följer bästa praxis när ni skapar och aktiverar er annonsupplevelse kan ni minimera potentiella komplikationer och fel under leverans till målkanalerna.

## God praxis

Här är några vanliga metodtips och de fel som de kan förhindra.

* **Använd giltiga, fullständiga mål-URL:er**

  Ogiltiga URL-adresser kan utlösa fel. Exempelfel: _Den angivna URL:en är inte direkt till en webbplats. Ange en giltig URL och försök igen. (100)_

* **Kontrollera att programmet hanterar när token upphör att gälla korrekt**

  Program ska begära nya tokens efter behov. Autentisera igen efter behov och få en ny åtkomsttoken genom att logga in igen eller uppdatera sessionen. Exempelfel: _Det gick inte att verifiera åtkomsttoken: Sessionen har ogiltigförklarats eftersom användaren har ändrat sitt lösenord eller eftersom Facebook har ändrat sessionen av säkerhetsskäl. (190)_

* **Granska annonsuppsättningen och se till att endast en annons är aktiv åt gången**

  Om du behöver aktivera flera Meta Ads skapar du separata dynamiska Creative Ad Sets för var och en av dem. Exempelfel: _Dynamisk Creative Ad Set tillåter högst en aktiv annons i den. Användare får inte skapa mer än en annons under samma dynamiska Creative-annonsuppsättning. (100)_

* **Matcha antalet tillämpade regler med det belopp som anges av plattformen**

  Betalningskanaler förväntar sig att antalet tillämpade regler matchar det angivna formatet.  Justera vid behov antalet regler så att de matchar värdet som plattformen anger. Exempelfel: _Ad AssetFeed har X-målregler för format: formatets namn, men exakt X-målregel för det här formatet förväntas. (100)_

* **Välj en call-to-action (CTA) som är kompatibel med ditt annonsmål**

  Call-to-actions som är inkompatibla med målet i Dynamic Creative Ad Sets utlöser ett fel. Exempelfel: _call to action-typen X stöds inte för målet Y i den dynamiska Creative-annonsuppsättningen. (100)_

* **Kontrollera att målannonsmängdens tak stöder antalet annonsupplevelser**

  Bekräfta att annonsuppsättningens annonseringsgräns kan anpassa era aktiverade annonsupplevelser. Om det behövs kan du ta bort onödiga eller inaktiva annonser från annonsuppsättningen så att de ligger inom denna gräns. Du kan också skapa en ny annonsuppsättning för att aktivera fler annonser. Exempelfel: _Du har nått gränsen för kampanj, annonsuppsättning eller annonser per annonskonto. Varje annonsuppsättning kan innehålla maximalt 50 annonser. Detta inkluderar pausade/inaktiva/inaktiverade annonser. (100)_

* **Kontrollera att plattformen stöder den valda CTA-typen**

  Bekräfta att din upplevelse innehåller en CTA-typ som stöds. Exempelfel: _(#100) Ogiltig call to action-typ (100)_
