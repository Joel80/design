---
Title: Analysrapport 4
Description: Analys av projektwebbplatsens laddningstid
Template: analysis-report
---
## Analys av laddningstider för Bew Gorps portfolio-sida
I denna analys undersöker jag laddningstider för tre av de sidor som ingår på den portfolio-webbplats som jag har skapat åt Bew Gorp.

### Metod och verktyg
För att granska webbplatsen valdes tre, på webbplatsen ingående, webbsidor ut. När jag valde ut vilka webbsidor som skulle vara med valde jag de tre "huvudsidorna" - startsidan (Hem), sidan om webbplatsen (Om) samt sidan där projekten presenteras (Projekt). Jag valde också att analysera både det grundläggande temat och det alternativa temat som jag skapade enligt uppdrag 4 i projektet. Eftersom dessa olika teman laddar lite olika bilder så vore det intressant att se om detta får någon påverkan. 

Sedan användes [Googles PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/) för att mäta sidornas prestanda. Webbsidorna utvärderades där både för mobil och desktop och betygen noterades. PageSpeedInsights ger ett betyg mellan 0 och 100 där 0-49 är ett "dåligt" betyg, 50-89 är ett "genomsnittligt" betyg som innebär att sidan behöver förbättras och 90-100 innebär att sidan är "bra".[1] PageSpeedInsights gav flera tips på hur sidorna kunde förbättras. I diskussionen kring varje sida har jag inte lyft alla förslag utan lyft några exempel. 

Firefox developer editions devtools prestandaanalys användes sedan för att mäta sidornas laddningstid, antalet resurser som laddades samt sidans totala storlek. Mätningen utfördes tre gånger för varje webbsida och sedan togs ett genomsnitt av värdena. De värden som registrerades var de som uppmättes med cache inaktiverat. 

De data som samlades in i analysen finns i [detta kalkylark](https://docs.google.com/spreadsheets/d/1cZsULlnXN8thB2Y4hTcDDGbG2Y_UucfvLIVZEDroUFs/edit?usp=sharing). 

### Resultat

#### Det grundläggande temat
<picture>
<source media="(min-width: 668px)" srcset="../image/bew_gorp_portfolio.png?w=600" alt="Screenshot från Bew Gorps portfolio">
<source media="(min-width: 376px)" srcset="../image/bew_gorp_portfolio.png?w=325" alt="Screenshot från Bew Gorps Portfolio">
<img class= "report-image" src="../image/bew_gorp_portfolio.png?w=270" alt="Screenshot från Bew Gorps portfolio">
</picture>

#### Det alternativa temat

<picture>
<source media="(min-width: 668px)" srcset="../image/bew_gorp_dark.png?w=600" alt="Screenshot från Bew Gorps portfolio">
<source media="(min-width: 376px)" srcset="../image/bew_gorp_dark.png?w=325" alt="Screenshot från Bew Gorps Portfolio">
<img class= "report-image" src="../image/bew_gorp_dark.png?w=270" alt="Screenshot från Bew Gorps portfolio">
</picture>

#### Hem
Sidan fick, för det grundläggande temat betyget 87 för mobil och 98 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 1,3 sekunder, hade i genomsnitt 19 resurser som efterfrågades och dess totala storlek var i genomsnitt 493,83kB.

För det alternativa temat var betyget 84 för mobil och 98 för desktop på PageSpeedInsights. Sidan med alternativt tema laddade i genomsnitt på 0.88 sekunder, hade i genomsnitt 14 resurser som efterfrågades och dess totala storlek var i genomsnitt 423,3kB.

##### Diskussion -grundläggande tema
Sidan får ett "genomsnittligt" värde på PageSpeedInsights för mobiler och ett "bra" värde på desktop. Det tar i genomsnitt strax över 1 sekund att ladda klart sidan. PageSpeedInsights ger vissa insikter kring vad som skulle kunna förbättras. Vissa resurser blockerar renderingen och skulle kunna ge en tidsbesparing. Här tycks det som att jag skulle kunna arbeta mer med sidans css (det är den filen som listas för både mobil och desktop). För att arbeta vidare med detta skulle en kunna se över CSS-filen. Några förslag som PageSpeedInsights ger är t.ex. att dela upp CSS-filen i olika delar och sedan med hjälp av media quieries bara skicka den fil som är anpassad till användarens enhet. 

En annan möjlighet för mobil enligt PageSpeedInsight skulle vara att ladda in vissa resurser (i detta fall fonter från FontAwesome) i förväg. 

Slutligen finns det en del oanvänd CSS som flaggas i mobilanalysen. Här är det återigen CSS-filen som flaggas av PageSpeedInsights. En tänkbar anledning till detta är ju t.ex. att FontAwesomes filer läses in i CSS:en och jag använder bara några få av de ikonerna. 

##### Diskussion - alternativt tema
Det alternativa temat får snarlika betyg på PageSpeedInsights. Möjligheterna till förbättring som PageSpeedInsights visar är lika förutom på en punkt: i den mobila analysen flaggas min Hero-bild (som är en annan än i det grundläggande temat). Här menar PageSpeedInsights att ett modernare bildformat skulle kunna snabba upp sidan. Jag har bilder i .jpg format både i det grundläggande och i det alternativa temat men bilden i det alternativa temat är dubbelt så stor i grunden. Det skulle jag gissa är anledningen till att denna bild flaggas här.

Länk till sidan:  
[Hem|Bew Gorp](http://www.student.bth.se/~jolf20/dbwebb-kurser/design/me/kmom10/)


#### Om

Sidan fick betyget 87 för mobil och 98 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 0,89 sekunder, hade i genomsnitt 17 resurser som efterfrågades och dess totala storlek var i genomsnitt 499,98kB.

För det alternativa temat var betyget 85 för mobil och 98 för desktop på PageSpeedInsights. Sidan med alternativt tema laddade i genomsnitt på 0.89 sekunder, hade i genomsnitt 13 resurser som efterfrågades och dess totala storlek var i genomsnitt 354,87kB.

##### Diskussion -grundläggande tema
Sidan får ett "genomsnittligt" värde på PageSpeedInsights för mobiler och ett "bra" värde på desktop. Det tar i genomsnitt strax under 1 sekund att ladda klart sidan. Här ger PageSpeedInsights exempel på precis samma möjligheter som för sidan Hem. Det handlar alltså om resurser (css-filen) som skulle kunna förbättras kanske genom en uppdelning, samt om fonter från FontAwesome. Liksom för Hem-sidan flaggas blockerande resurser för både desktop och mobil. 

##### Diskussion - alternativt tema
Det alternativa temat får även här snarlika poäng i PageSpeedInsights analyser. Samma saker som flaggas för Hem-sidan flaggas även i analyserna av denna sida.

  
Länk till sidan:  
[Om|Bew Gorp](http://www.student.bth.se/~jolf20/dbwebb-kurser/design/me/kmom10/about)

#### Projekt
Sidan fick betyget 81 för mobil och 95 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 2,69 sekunder, hade i genomsnitt 26 resurser som efterfrågades och dess totala storlek var i genomsnitt 919,87kB.

För det alternativa temat var betyget 86 för mobil och 97 för desktop på PageSpeedInsights. Sidan med alternativt tema laddade i genomsnitt på 2,20 sekunder, hade i genomsnitt 22 resurser som efterfrågades och dess totala storlek var i genomsnitt 788,79kB.

##### Diskussion
Sidan får ett "genomsnittligt" värde på PageSpeedInsights för mobiler och ett "bra" värde på desktop. Den har den längsta genomsnittliga laddningstiden av de tre sidorna som testades. Detta ligger i linje med att det är den tyngsta av sidorna där flest tunga resurser laddas.

PageSpeedInsights ger liknande förslag på möjligheter även för denna sida. Här flaggas resurser som blockerar renderingen  både på desktop och mobil. För deskop flaggas också möjligheten att läsa in resurser från FontAwesome i förväg och för mobil flaggas oanvänd CSS som för de andra sidorna.

##### Diskussion - alternativt tema
Det alternativa temat får även här snarlika poäng i PageSpeedInsights analyser. PageSpeedInsight ger samma möjligheter för förbättringar som för de båda andra sidorna för denna sida.

Länk till sidan:  
[Projekt|Bew Gorp](http://www.student.bth.se/~jolf20/dbwebb-kurser/design/me/kmom10/gallery)

### Analys
Resultatet visar att det finns vissa saker att förbättra på webbplatsen. Framförallt tycks det handla om att se till att CSS-filen inte blockerar renderingen mer än nödvändigt. Här tyckte jag att det var ett intressant förslag som PageSpeedInsights gav med möjligheten att dela upp sin css-fil i flera mindre och sedan bara skicka den fil som är anpassad till användarens enhet. Det är inget jag kommer att titta på i detta projekt eftersom jag har satt upp SASS-kompileringen till enbart en CSS-fil enligt anvisningarna på tidigare moment, jag har för närvarande också lite för lite kunskap, som jag ser det, för att genomföra detta nu. Men jag tar definitivt med mig det framöver som ett möjligt sätt att arbeta. Jag tar också med mig tipset att inte ladda in för mycket onödig CSS. Jag tror ju här som jag skrev ovan att CSS:en från FontAwesome kan vara en del av problemet här. Jag väljer att inte göra något åt det nu, återigen eftersom jag inte är helt säker på hur jag ska göra för att bara ladda in det jag behöver, men det är definitivt något som jag tänker att det är bra att hålla ögonen på framöver. Slutligen fick jag enbart nedslag på en av mina bilder - hero-bilden i det alternativa temat. Det visar att det var viss skillnad mellan mina teman och att det kan vara värdefullt att analysera även alternativa teman - särskilt om de innehåller olika bilder. Jag har använt cimage för att minska bredden på den bilden - men den flaggas ändå i analysen. Det problem jag ställs inför här är att det är en bakgrundsbild som läses in via CSS och återigen ställer sig min bristande kunskap i vägen. Det problem jag skulle få om jag konverterade den till en webp-bild är att alla webbläsare inte kan läsa sådana bilder. Jag skulle då behöva ha en alternativ bild för dessa läsare. Om bilden låg inbäddad i HTML så tror jag att jag skulle kunna klura ut hur jag skulle göra detta med hjälp av picture och source men jag vet tyvärr inte hur jag åstadkommer detta i CSS. I övrigt är jag nöjd med att mitt arbete med bilderna och cimage verkar ha gett resultat - bilderna flaggas inte som förbättringsmöjligheter i analyserna vilket jag tar som tecken på att de är anpassade i lagom grad.

### Rangordning av sidorna
Hem och Om-sidorna får snarlika betyg av PageSpeedInsights. Om-sidan laddar dock något snabbare i båda mina teman så därför får det bli den vinnande sidan, med Hem-sidan som tvåa och projektsidan som trea. Det är ju egentligen inget märkligt resultat i "tävlingen" eftersom Om-sidan är den sida som laddar minst antal resurser och i stort bara består av text. Att det tar längtst tid att ladda den bildrikaste sidan är också naturligt.

### Gräns för absolut laddningstid
Vad är en rimlig laddningstid för en sida? Som jag skrev i min analys av laddningstider på myndigheters webbplatser så är jag själv relativt tålmodig när det gäller laddningstider. Det måste nog gå en tre sekunder innan jag reagerar. Som jag lyfte i den analysen så verkar det ju dock som att människor i allmänhet bara tar ett par sekunder på sig att bestämma sig för om en sida är intressant eller inte - det vore därför bra om sidan är färdigladdad innan dessa sekunder har gått. Här är min projektsida med galleriet över olika projekt mest i farozonen. Den tar visserligen under 3 sekunder att ladda så jag kanske inte skulle reagera men den tar samtidigt över 2 sekunder att ladda så andra kanske gör det. Med mer kunskap kring att dela upp CSS-filerna och bara skicka den fil som motsvarar användarens enhet hade jag nog försökt mig på detta för att förbättra laddningstiden för denna och de andra sidorna och försökt komma under 2 sekunder på samtliga sidor.

### Övrigt
Rapportförfattare: Joel Löfgren

### Referenser
- 1 [Lighthouse performance scoring](https://web.dev/performance-scoring/)