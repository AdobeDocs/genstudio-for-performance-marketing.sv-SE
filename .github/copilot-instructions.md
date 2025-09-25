---
source-git-commit: 8ed1e6853c9f844c72431dc692b556ece9c215a8
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---
## Syfte

Hjälp AI-kodassistenter att göra små, säkra redigeringar i GenStudio for Performance Marketing dokumentationsrapport.

## Arkitektur på hög nivå (kort)- Den här rapporten är en dokumentationswebbplats som består av Markdown under `help/` med delade inkluderingar i `help/_includes/` och strukturerade bilder under `help/_includes/assets/`.- Versionsinformation, användarhandbok och utökningsbart innehåll finns under `help/`. Stora innehållsändringar bör bevara den befintliga rubrikstrukturen.- Webbplatsen byggs med Jekyll och finns på GitHub-sidor. Byggprocessen använder Jekyll-standardkonventioner med vissa anpassade plugin-program.

## Projektspecifika konventioner- Markörregler: Anpassad automatisering och vägledning finns i `.cursor/rules/*.mdc`. Exempel: `.cursor/rules/docs-lint.mdc` (lint-process), `.cursor/rules/generate-release-notes.mdc` (versionskommentarsformat). Följ dessa för automatiska uppgifter.- Filnamn och filnamn:   - Versionsinformation kräver en specifik förhandsgranskning (se `.cursor/rules/generate-release-notes.mdc`).   - Använd&quot;kebabcase&quot; för regelfiler och tillägget `.mdc`.- Formateringskonventioner: Dokumenten använder GitHub-smaksatt Markdown. Rubriker följer vanligen inledande och korta stycken. Föredra `*` punkter för listor i versionsinformation och `###` för funktionsavsnitt.

## Riktlinjer för dokumentationsformat- Följ [Microsoft Writing Style Guide](https://learn.microsoft.com/en-us/style-guide/) för bästa praxis inom teknisk dokumentation:   - Skriv tydliga, kortfattade meningar med fokus på användaråtgärder   - Använd aktiv röst och visa spänning   - Dela upp text i korta, skannade segment   - Håll en varm, direkt ton samtidigt som du bibehåller den tekniska precisionen- Redigering:   - Använd inledande versal för rubriker (endast första ordet)   - Håll styckena korta (2-3 meningar) för läsbarhet   - Lägg till tomma rader före och efter rubriker och listor   - Använda bakgrunder för UI-element, filsökvägar och kod   - Inkludera alternativ text för alla bilder   - Länka till specifika avsnitt med beskrivande text

## Säkerhetsregler för redigering (vad AI bör göra)- Lägg aldrig till Jira-ID:n, interna länkar eller företagshänvisningar till offentliga dokument. Se avsnittet `generate-release-notes.mdc`&quot;Ärendeuppföljning&quot;.- Bevara förhandsgranskningen av YAML exakt när du redigerar filer som innehåller den. Många mallar och versionsinformation använder fasta nycklar (titel, beskrivning, roll, exl-id).- För kodkorrigeringar bör du föredra automatiserade, depotenta redigeringar från `.cursor/rules/docs-lint.mdc` (ta bort efterföljande blanksteg, se till att den sista raden används). Exempelkommandon som används av människor:

```sh
sed -i '' 's/ $//' <file>
sed -i '' '$ { /^$/d; }' <file> && echo "" >> <file>
```

## Exempel (vad som ska ändras och hur)- Korrigeringar för små kopior: uppdatera text i `help/` Markeringsfiler, behåll rubriker och ankarpunkter intakta.- Bilduppdateringar: referensbilder under `help/_includes/assets/`. Flytta inte eller byt namn på bilder utan att uppdatera alla referenser.

## Var ska du titta först?- `help/_includes/` - delade fragment och bilder.- `.cursor/rules/` - riktlinjer för automatisering och linting. Använd dessa som auktoritativa regler för formatering och processer.- `markdownlint_custom.json` - lokal marknedladdning åsidosätter.- `.github/pull_request_template.md` - PR-förväntningar.

## När ska man fråga- Om en ändring kräver att Docker-baserade verktyg körs eller ändras (Lint-regeln talar om Docker) eller påverkar rörledningar för bygge av webbplatser.- Om en fil refererar till en okänd extern konfiguration (t.ex. `markdownlint.json` saknas) frågar du om den ska skapas eller ignoreras.

## Minimala kommandon för människor

```sh
# Install linter (if not present)
npm install -g markdownlint-cli

# Run lint locally using project config
markdownlint --config markdownlint_custom.json "help/**/*.md"

# Project lint via yarn (preferred if available in environment)
yarn lint
```

&#x200B;---
Om du vill kan jag sammanfoga detta i `.github/copilot-instructions.md` i svaret (eller justera formuleringen/längden). Vad ska jag ändra eller lägga till?
