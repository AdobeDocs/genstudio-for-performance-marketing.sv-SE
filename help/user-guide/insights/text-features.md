---
title: Textfunktioner
description: Läs mer om textfunktionen i de attributkategorier som används i GenStudio for Performance Marketing.
feature: Reporting and Insights, Text Attributes, Generative AI
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
source-git-commit: 3ccc6313a7c559f1c0846c144d23b783da0aecfa
workflow-type: tm+mt
source-wordcount: '1288'
ht-degree: 1%

---

# Textfunktioner

Textfunktioner inkluderar antal för vissa textelement, t.ex. ord, meningar, känslolägesikoner och klassificeringar för semantik, känslor och ton som används för analys med [!DNL Insights]. Texten kan också få ett läsbarhetspoäng.

GenStudio for Performance Marketing använder Adobe AI och maskininlärningsfunktioner för att studera text och tillämpa [!UICONTROL Media attributes] baserat på tillhörande texttoner och berättande om marknadsföring. Processen validerar indatatexten så att den innehåller alfanumeriska tecken, tar bort extra blanksteg och tecken som inte går att skriva ut samt kortar av texten till maximalt tillåtna 1 500 ord. Innan du använder identifierade attributtaggar förutser AI den vanliga tonen.

## Ton

Ton representerar en allmän karaktär, attityd eller atmosfär som visas på ett språk. Ett enkelt val av ord och interpunktion, meningsstruktur och stil kan ändra tonen i meddelandet. Ta till exempel följande brådskande meddelanden med de tre grundläggande tonnivåerna:

| Ton | Beskrivning | Exempel |
| -------------- | ----------------------------------- | --------------------------------------------------------- |
| Formell | Snyggt och professionellt språk. | `Take advantage of this distinctive and exceptional opportunity!` |
| Konversationslayout | Vänligt och informellt språk. | `Don't miss out on this great opportunity!` |
| Direkt | Rakt fram och tillbaka. | `Don't miss the chance!` |

Andra sekundära värden för ton ger en bättre distinktion mellan meddelandets karaktär och attityd. I likhet med det tidigare exemplet på ett brådskande meddelande kan GenAI upptäcka en _poetisk_ ton i det här fantastiska exemplet: `Embrace the moment, without delay, for this occasion won't always stay.`

I följande tabell visas de tonvärden som känns igen av GenStudio for Performance Marketing AI.

| Ton | Beskrivning | Exempel |
| -------------- | ------------------------------------------------ | --------------------------------------------------------- |
| Assertiv | Konfidentiellt och kraftfullt i uttryck. | `You need to act now to secure this deal!` |
| Direkt | Rakt fram och tillbaka. | `Don't miss the chance!` |
| Empatetisk | Visar förståelse och känslighet. | `We understand your needs, and this is perfect for you.` |
| Enentusiastisk | Visar intensiv och angelägen njutning, intresse eller godkännande. | `This is an amazing opportunity you can't miss!` |
| Humoristisk/urusel | Ljushjärtad och smart. | `Why wait? Grab this deal before it's gone!` |
| Inspirerande | Uppmuntra och lyfta. | `Believe in yourself and seize this opportunity!` |
| Poetisk | Konstnärligt och uttrycksfullt. | `Embrace the dawn of a new opportunity.` |
| Kvantitativ | Baserat på numeriska data. | `99% of users loved this offer, and you will too.` |
| Sensorisk | Engagerande sinnen. | `Feel the excitement with this incredible offer!` |
| saga | Berättarröst för att förmedla ett budskap. | `Once upon a time, there was an offer you couldn't refuse.` |

## Uppmuntrade överklagande

Marknadsförarna utnyttjar de mänskliga känslor som finns för att skapa en stark koppling mellan målgruppen och varumärket. Genom att utnyttja sådana sinnen som lycka, rädsla, spänning eller nostalgi kan marknadsförarna skapa budskap som ger ett djupare intryck, driver på engagemanget och påverkar konsumenternas beteende. Uppmuntrade tilltalande hjälper till att leverera mer relaterat och minnesvärt innehåll, vilket i slutänden främjar varumärkeslojalitet och uppmuntrar till önskade åtgärder.

Övertygande taktik, marknadsföringseenden och berättande stil fungerar tillsammans för att inrikta sig på kundsegment.

- **Berättande format**, till exempel autenticitet, firande och community, hjälper till att förmedla de värden och den identitet som får genklang hos målgruppen och skapar ett mer övertygande och relaterat budskap.
- **Övertygande taktiker**, som brist på information, socialt bevis och ömsesidighet, är utformade för att påverka konsumenternas beteende genom att tilltala deras känslor och önskemål.
- **Marknadsföringskänsla** syftar till att stimulera känslor som stärker engagemanget och kopplingen till varumärket.

GenStudio for Performance Marketing AI identifierar och särskiljer dessa egenskaper genom att analysera texten med hjälp av känslomässiga tecken, färgton och berättande stil. AI använder naturliga språk- och maskininlärningsalgoritmer för att identifiera mönster och klassificera texten baserat på fördefinierade emotionella och övertygande attribut.

### Berättarstil

Attributen är berättande, eller tilltalande, och hjälper till att identifiera medier som förmedlar de värden, syften eller identiteter som får genklang till målgruppen. I följande tabell visas de berättande format som känns igen av GenStudio for Performance Marketing AI.

| Överklagandefaktor | Beskrivning | Exempel |
| ----------------- | --------------------------------------------------------------------- | ------------------------------------------ |
| Autenticitet | Äkta och äkta, ofta med fokus på öppenhet och ärlighet. | `A behind-the-scenes look at how our products are made.` |
| Firande | Markera speciella tillfällen eller prestationer med glädje och smak. | `Join us in celebrating our 10th anniversary with special offers!` |
| Community | Främja en känsla av samhörighet och samhörighet mellan en grupp. | `Our brand is built on the strength of our community.` |
| Bekvämlighet | Betonar användarvänlighet och tidsbesparande fördelar. | `Get what you need with just one click.` |
| Kraftfull | Uppmuntra och göra det möjligt för enskilda att ta kontroll och fatta beslut. | `Empower yourself with our latest tools and resources.` |
| Utforskande | Inbjudan till upptäckt och äventyr, ofta i samband med nya upplevelser. | `Discover new horizons with our travel packages.` |
| Futuristisk | Framhäv innovation och framåtblickande idéer. | `Experience the future of technology today.` |
| Hype | Generera spänning och förväntan kring en produkt eller händelse. | `Don't miss out on the most anticipated event of the year!` |
| Indulens | Fantastiska drömmar, önskningar eller tilltalande. | `Treat yourself to the finest gourmet chocolates.` |
| Sinnesro | Ger trygghet och känsla av säkerhet. | `Rest easy knowing your data is safe with us.` |
| Personalization | Anpassa upplevelser eller produkter efter individuella önskemål. | `Get a custom-fit solution just for you.` |
| Prestige | Associerar med hög status och exklusivitet. | `Join the elite with our premium membership.` |
| Tidlöshet | Betonar uthållig kvalitet och klassisk stil. | `Our designs are timeless and never go out of style.` |
| Mångsidighet | Markerar anpassningsbarhet och flera användningsområden. | `Our product fits seamlessly into any lifestyle.` |
| Välfärdssamhället | Främja hälsa, lycka och allmän välfärd. | `Enhance your well-being with our holistic approach.` |

### Övertygande taktik

Övertygningstekniker används för att påverka konsumenternas beteende och driva fram önskade åtgärder. Dessa strategier är inriktade på specifika psykologiska triggers och kundsegment för att förbättra effektiviteten i marknadsföringsbudskapen. I följande tabell visas de övertalningsmetoder som erkänns av GenStudio for Performance Marketing AI.

| Taktisk | Beskrivning | Exempel |
| --------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| Antropomorfism | Attribuera mänskliga egenskaper till produkter eller varumärken. | `Our friendly chatbot is here to help you.` |
| Jämförelse | Markera skillnader mellan alternativen för att påverka valet. | `See how we compare to the competition.` |
| Konfidentialitet | Ange specifika detaljer för att göra budskapet mer konkret. | `Save 20% on your next purchase.` |
| Bekräftelse | Godkännanden från trovärdiga källor eller påverkare. | `Recommended by top industry experts.` |
| Fot i dörren | Börja med en liten begäran om att öka sannolikheten för att en större begäran godtas. | `Try our free trial today.` |
| Överkommande reaktion | Minska motståndet genom att erkänna och ta itu med invändningar. | `We understand your concerns, and here's how we address them.` |
| Ömsesidighet | Erbjuder något av värde för att uppmuntra en återvändandetjänst. | `Get a free gift with your purchase.` |
| Scharm | Skapa en känsla av brådska genom att markera begränsad tillgänglighet. | `Only a few items left in stock!` |
| Social identitet | Utnyttja konsumenternas känsla av att tillhöra en grupp. | `Join our community of innovators.` |
| Sociala effekter | Framhäva den positiva inverkan på samhället eller miljön. | `Your purchase helps plant a tree.` |
| Socialt bevis | Använd utlåtanden eller användargenererat innehåll för att bygga upp förtroende. | `See why thousands of users love our product.` |

### Marknadsföringskänslor

Motiven fokuseras på marknadsföringsmeddelanden för att väcka specifika känslor och reaktioner hos publiken, vilket kan öka engagemanget och kopplingen till varumärket. I följande tabell visas de känslor som känns igen av GenStudio for Performance Marketing AI.

| Emotion | Beskrivning | Exempel |
| ------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| Anspiration | Inspirera till en önskan att uppnå eller uppnå något större. | `Imagine the possibilities with our premium service.` |
| Utmaning | Uppmuntra publiken att övervinna ett hinder eller ta till vara en ny uppgift. | `Are you ready to take the next step in your career?` |
| Nyhet | Satsar på intresse och en önskan att lära sig mer. | `Discover the secrets behind our success.` |
| Exklusivitet | Skapa en känsla av att vara en del av en markerad grupp. | `Join our exclusive club for members-only benefits.` |
| Fascination | Engagera publiken med spännande och spännande innehåll. | `Be amazed by our latest innovations.` |
| Gratisering | Ger nöjdhet och glädje av att använda produkten eller tjänsten. | `Enjoy the ultimate comfort with our luxury bedding.` |
| Erkännande | Att känna igen och värdera målgruppens resultat eller status. | `Get the recognition you deserve with our award-winning service.` |
| Förtroende | Skapa förtroende och tillförlitlighet för varumärket. | `Trust us to deliver quality and excellence every time.` |
| Akut | Få omedelbara åtgärder genom att betona tidskänsliga möjligheter. | `Act now before this limited-time offer expires!` |

## Läsbarhetskalförändring

Läsbarhetsbedömning avgör hur enkelt en textbit är att läsa och förstå. Det hjälper er att se till att ert innehåll passar er målgrupp. Poängen baseras på olika faktorer, bland annat meningsfull meny och ordkomplexitet. I följande tabell visas de läsbarhetsnivåer som känns igen av GenStudio for Performance Marketing AI.

| Läsbarhetsnivå | Beskrivning | Exempel |
| ------------------- | ------------------------------------------------------------------ | --------------------------------------------------------- |
| 5:e klass | Mycket enkelt språk, lämpligt för små barn. | `The cat sat on the mat.` |
| 6:e klass | Enkelt och tydligt språk, lämpligt för en bred publik. | `You can find great deals on our website.` |
| 7:e klass | Lätt att förstå, med enkel vokabulär och struktur. | `Our new product is simple to use and very effective.` |
| 8:e och 9:e klass | Klar och koncis text, lämplig för tonåringar. | `This guide will help you understand the basics of our service.` |
| 10:e till 12:e klass | Mer komplext språk, lämpligt för äldre tonåringar och vuxna. | `The comprehensive manual provides detailed instructions for setup.` |
| College | Avancerat språk som passar en välutbildad målgrupp. | `The study explores the multifaceted implications of the new policy.` |
| Studerande/högskola | Mycket avancerat språk, lämpligt för experter och specialister. | `The dissertation delves into the intricacies of quantum mechanics.` |

## Antal

Att förstå och dra nytta av räkningsattribut som hashtaggsantal, antal ord, meningar och nyckeltal kan avsevärt förbättra er innehållsstrategi. Dessa mätvärden ger värdefulla insikter om hur effektiva och relevanta era marknadsföringssatsningar är. I följande tabell visas de räkningskategorier som känns igen av GenStudio for Performance Marketing AI.

| Kategori | Beskrivning | Exempel |
| --------------------- | --------------------------------------------------------------------------- | --------------------- |
| Antal Emojis | Antalet känslolägesikoner i texten. Emojis kan förbättra engagemanget och förmedla känslor snabbt. | `😊`, `🚀`, `❤️` |
| Antal hash-taggar | Antalet hashtaggar som används i texten. Hashtags hjälper till att kategorisera innehåll och öka upptäckten i sociala medier. | `#Marketing`, `#Sale` |
| Antal ord per mening | Det genomsnittliga antalet ord per mening i texten. Kortare meningar är ofta enklare att läsa och förstå. | `10` |
| Antal ord | Det totala antalet ord i texten. Ett högre ordantal kan ge mer detaljerad information men kan också kräva mer arbete att läsa. | `1500 words` |
| Stoppordsförhållande | Förhållandet mellan stoppord och meningsfulla ord i texten. Stoppord (som &quot;a&quot; &quot;an&quot; &quot;the&quot;) ignoreras ofta i sökfrågor och sökresultat. Ett högt antal stoppord kan göra innehållet mindre engagerande och svårare att läsa. | `0.375` |
| Antal meningar | Det totala antalet meningar i texten. Fler meningar kan visa mer detaljerat innehåll, men alltför långa texter kan förlora läsarens intresse. | `75 sentences` |
