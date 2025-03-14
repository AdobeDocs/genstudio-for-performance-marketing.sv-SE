---
title: Textfunktioner
description: Läs mer om textfunktionen i de attributkategorier som används i GenStudio for Performance Marketing.
feature: Insights, Attributes, Generative AI
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
source-git-commit: 808ffdb7f55f7ff938e9346b8513fab46f86df7c
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Textfunktioner

Textfunktioner inkluderar antal för vissa textelement, t.ex. ord, meningar, känslolägesikoner och klassificeringar för semantik, känslor och ton som används för analys med [!DNL Insights]. Texten kan också få ett läsbarhetspoäng.

GenStudio for Performance Marketing använder Adobe AI och maskininlärningsfunktioner för att studera text och tillämpa [!UICONTROL Media attributes] baserat på tillhörande texttoner och berättande om marknadsföring. Processen validerar indatatexten så att den innehåller alfanumeriska tecken, tar bort extra blanksteg och tecken som inte går att skriva ut samt kortar av texten till maximalt tillåtna 1 500 ord. Innan du använder identifierade attributtaggar förutser AI den vanliga tonen.

## Ton

Ton representerar en allmän karaktär, attityd eller atmosfär som visas på ett språk. Ett enkelt val av ord och interpunktion, meningsstruktur och stil kan ändra tonen i meddelandet. Ta till exempel följande brådskande meddelanden med de tre grundläggande tonnivåerna:

- `Formal`

  ```
  Take advantage of this distinctive and exceptional opportunity!
  ```

- `Conversational`

  ```
  Don't miss out on this great opportunity!
  ```

- `Direct`

  ```
  Don't miss the chance!
  ```

AI identifierar ytterligare en nyansfull ton. Om du använder samma brådskande sats från det tidigare exemplet används en vit `poetic`-ton i följande version:

- `Poetic`

  ```
  Embrace the moment, without delay, for this occasion won't always stay.
  ```

Andra sekundära värden för ton är: `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal`

## Berättande

Med de berättande attributen kan du identifiera medier som förmedlar de värden, syften och identiteter som ligger till grund för målgruppen.

| Berättande | Beskrivning | Exempel |
| ----------------- | ----------- | ------- |
| `Authenticity` |             |         |
| `Celebration` |             |         |
| `Community` |             |         |
| `Convenience` |             |         |
| `Empowerment` |             |         |
| `Exploration` |             |         |
| `Futuristic` |             |         |
| `Hype` |             |         |
| `Indulgence` |             |         |
| `Peace of mind` |             |         |
| `Personalization` |             |         |
| `Prestige` |             |         |
| `Timelessness` |             |         |
| `Versatility` |             |         |
| `Well-being` |             |         |

## Läsbarhetskalförändring

Läsbarhetsbedömning avgör hur enkelt en textbit är att läsa och förstå. Det hjälper er att se till att ert innehåll passar er målgrupp. Poängen baseras på olika faktorer, bland annat meningsfull meny och ordkomplexitet.

| Poäng | Skolnivå | Anteckningar |
| ----------- | ------------------ | ------------------------------------------------------------------------- |
| 100.00-90.00 | 5:e klass | Mycket lätt att läsa. Enkelt att förstå för en 11-årig elev. |
| 90.0-80.0 | 6:e klass | Lätt att läsa. Engelska konversationer för konsumenter. |
| 80.0-70.0 | 7:e klass | Lättläst. |
| 70.0-60.0 | 8:e och 9:e klass | Vanligt engelskt. Enkelt att förstå för 13- till 15-åriga elever. |
| 60.0-50.0 | 10:e till 12:e klass | Mycket svårt att läsa. |
| 50.0-30.0 | College | Svårt att läsa. |
| 30.0-0.0 | Studerande/högskola | Mycket svårt att läsa. Förstå bäst för universitetsstuderande. |

## Räkna ord

TBD

I följande tabell visas de bildfunktionskategorier som känns igen av GenStudio for Performance Marketing AI.

| Kategori | Beskrivning | Exempel |
| -------------------- | ------------- | --------------------- |
| Antal Emojis |             |        |
| Antal hash-taggar |             |        |
| Nyckelord |             |        |
| Marknadsföringsevenemang | Motiven fokuseras på marknadsföringsmeddelanden för att väcka specifika känslor och reaktioner hos publiken, vilket kan öka engagemanget och kopplingen till varumärket. | `Aspiration`, `Challenge`, `Curiosity`, `Exclusivity`, `Fascination`, `Gratification`, `Recognition`, `Trust`, `Urgency` |
| Övertygande strategier | Tekniker som används för att påverka konsumenternas beteende och driva önskat agerande. Dessa strategier är inriktade på specifika psykologiska triggers och kundsegment för att förbättra effektiviteten i marknadsföringsbudskapen. | `Social identity`, `Social proof`, `Endorsement`, `Concreteness`, `Foot in the door`, `Overcoming reactance`, `Reciprocity`, `Comparison`, `Social impact`, `Scarcity`, `Anthropomorphism` |
| Ton | Den allmänna karaktär, attityd eller atmosfär som förmedlas i ett marknadsföringsmeddelande genom ordval, interpunktion, meningsstruktur och stil. | `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal` |
