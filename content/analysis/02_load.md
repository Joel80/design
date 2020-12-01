---
Title: Analysrapport 2
Description: Min rapport om sidors laddningstid
Template: analysis-report
---

## Laddningstider för myndigheters webbplatser
I denna analys undersöker jag tre myndigheters webbplatser och studerar deras laddningstider.

### Urval 
Jag valde samma tre myndigheter som ingick i min förra analys: Pensionsmyndigheten, Försäkringskassan och Skatteverket. Gemensamt för de tre myndigheterna är att deras verksamhetsområden  berör de flesta medborgare under större delen av våra liv. Dessa myndigheter hanterar socialförsäkringen och skatter vilket alla medborgare förmodligen någon gång behöver få fram bra information kring. Det är därför intressant att undersöka vilken prestanda webbplatserna har, här görs detta genom att undersöka laddningstider.

### Metod 
För att granska myndigheternas webbplatser valdes tre ingående webbsidor ut. Sedan användes [Googles PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/) för att mäta sidornas prestanda. Webbsidorna utvärderades där både för mobil och desktop och betygen noterades. PageSpeedInsights ger ett betyg mellan 0 och 100 där 0-49 är ett dåligt betyg, 50-89 innebär att sidan behöver förbättras och 90-100 innebär att sidan är bra.[1] Firefox developer editions devtools användes för att mäta sidornas laddningstid, antalet resurser som laddades samt sidans totala storlek. Mätningen utfördes tre gånger för varje webbsida och sedan togs ett genomsnitt av värdena. Den data som samlades in finns i [detta kalkylark](https://docs.google.com/spreadsheets/d/1uMKB0m7V0OgIRrsCboD2ftkm0nsQL6XwbzqXR9PphPA/edit?usp=sharing). När jag valde ut vilka webbsidor som skulle vara med valde jag startsidan samt de två första "reguljära" ingångarna. Försäkringskassan hade på första plats en ingång kring corona - denna valde jag bort eftersom den (förhoppningsvis) är tillfällig och därför kanske kan sägas avvika i innehålla från de mer permanenta ingångarna. I Skatteverkets fall valde jag startsidan och de två första ingångarna i den gula "navbaren".

### Resultat
#### Pensionsmyndigheten
<img class="city-img" src= '../assets/img/pensionsmyndigheten.png' alt= "Screenshot från Pensionsmyndighetens webbplats">

Jag valde ut följande webbsidor att mäta hos Pensionsmyndigheten:

##### Startsidan
Sidan fick betyget 79 för mobil och 96 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 2,26 sekunder, hade i genomsnitt 44 resurser som efterfrågades och dess totala storlek var i genomsnitt 2 185 kB.
https://www.pensionsmyndigheten.se/ 

##### Diskussion
Sidan får ett genomsnittligt värde på PageSpeedInsights för mobiler och ett "bra" värde på desktop. Det tar i genomsnitt strax över 2 sekunder att ladda klart sidan. PageSpeedInsights ger vissa insikter kring vad som skulle kunna förbättras. Bl.a. skulle vissa resurser (i detta fall fonter) kunna laddas in i förväg, texten skulle också kunna göras synlig medan webbteckensnitten läses in. För mobil anger också PageSpeedInsights bl.a. att modernare bildformat skulle leda till en besparing i storlek på data som skickas och därmed också en tidsbesparing. För mobil verkar det också finnas en css-resurs som blockerar renderingen och skulle kunna inlinas eller skjutas upp istället.

#### Förstå din pension
Sidan fick betyget 83 för mobil och 97 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 1,84 sekunder, hade i genomsnitt 26 resurser som efterfrågades och dess totala storlek var i genomsnitt 1 941 kB. 
https://www.pensionsmyndigheten.se/forsta-din-pension  

##### Diskussion
Sidan får ett genomsnittligt värde på PageSpeedInsights för mobiler och ett "bra" värde på desktop. Det tar i genomsnitt strax under 2 sekunder att ladda klart sidan. Även här ger PageSpeedInsight tipset att förladda vissa resurser (fonter) samt att göra text synlig när webbtecknena läses in. Sidan verkar inte ha samma problem som startsidan när det gäller omoderna bildformat.

#### Gå i pension
Sidan fick betyget 80 för mobil och 94 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 1,74 sekunder, hade i genomsnitt 27 resurser som efterfrågades och dess totala storlek var i genomsnitt 1 940 kB. 
https://www.pensionsmyndigheten.se/ga-i-pension  

##### Diskussion
Sidan får ett genomsnittligt värde på PageSpeedInsights för mobiler och ett "bra" värde på desktop. Den har den kortaste genomsnittliga laddningstiden av de tre sidorna på webbplatsen även om den ligger nära de andra. Även här ger PageSpeedInsight tipset att förladda vissa resurser (fonter) samt att göra text synlig när webbtecknen läses in. Sidan verkar inte ha samma problem som startsidan när det gäller omoderna bildformat.

#### Försäkringskassan
<img class="city-img" src= '../assets/img/forsakringskassan.png' alt= "Screenshot från Försäkringskassans webbplats">
Jag valde ut följande webbsidor att mäta hos Försäkringskassan:

#### Startsidan
Sidan fick betyget 24 för mobil och 86 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 7,67 sekunder, hade i genomsnitt 44 resurser som efterfrågades och dess totala storlek var i genomsnitt 1 138 kB.
https://www.forsakringskassan.se/

##### Diskussion
Sidan får ett dåligt värde på PageSpeedInsights för mobiler och ett "genomsnittligt" värde på desktop. Laddningstiden är på nära 8 sekunder, här var det en av omladdningarna som tog lång tid (15 sekunder) som drog upp medelvärdet. Liksom för sidorna hos Pensionsmyndigheten  ger PageSpeedInsight tipset att förladda vissa resurser (fonter) samt att göra text synlig när webbtecknen läses in. Sidan har också, enligt den mobila analysen, JavaScript som inte används. Liksom hos Pensionsmyndigheten finns det vissa resurser som blockerar renderingen och som flaggas i den mobila analysen.

#### Förälder
Sidan fick betyget 28 för mobil och 89 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 2,13 sekunder, hade i genomsnitt 32 resurser som efterfrågades och dess totala storlek var i genomsnitt 1 766 kB.
https://www.forsakringskassan.se/privatpers/foralder

##### Diskussion
Sidan får ett dåligt värde på PageSpeedInsights för mobiler och ett "genomsnittligt" värde på desktop. Laddningstiden är på över 2 sekunder. Även här ger PageSpeedInsight tipset att förladda vissa resurser (fonter) samt att göra text synlig när webbtecknen läses in. Sidan har också, enligt den mobila analysen, JavaScript som inte används. Liksom på startsidan finns det vissa resurser som blockerar renderingen och som flaggas i den mobila analysen. I desktopanalysen verkar den största enskilda "boven" just vara att vissa resurser blockerar renderingen.

#### Sjuk
Sidan fick betyget 53 för mobil och 94 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 2,06 sekunder, hade i genomsnitt 32 resurser som efterfrågades och dess totala storlek var i genomsnitt 1 782 kB.
https://www.forsakringskassan.se/privatpers/sjuk

##### Diskussion
Sidan får ett dåligt värde på PageSpeedInsights för mobiler och ett bra värde på desktop. Laddningstiden är på strax över 2 sekunder. Även här ger PageSpeedInsight tipset att förladda vissa resurser (fonter) samt att göra text synlig när webbtecknen läses in. Sidan har också, enligt den mobila analysen, JavaScript som inte används. Liksom på startsidan finns det vissa resurser som blockerar renderingen och som flaggas i den mobila analysen. I desktopanalysen verkar den största enskilda "boven" just vara att vissa resurser blockerar renderingen precis som för "förälder-sidan".

#### Skatteverket
<img class="city-img" src= '../assets/img/skatteverket.png' alt= "Screenshot från Skatteverkets webbplats">

Jag valde ut följande webbsidor att mäta hos Skattteverket:

#### Startsidan
Sidan fick betyget 51 för mobil och 87 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 4,54 sekunder, hade i genomsnitt 43 resurser som efterfrågades och dess totala storlek var i genomsnitt 2 857 kB.
https://www.skatteverket.se/

##### Diskussion
Sidan får ett genomsnittligt värde på PageSpeedInsights för mobiler och ett "genomsnittligt" värde på desktop. Laddningstiden är på över 4 sekunder. I den mobila analysen verkar det främst vara olika resurser som blockerar renderingen, där listas både css-filer och js-filer bland annat. Det finns en del javascript på sidan som flaggas för att det inte används i den mobila analysen. Även för denna sida ger PageSpeedInsight också tipset att förladda vissa resurser (fonter) samt att göra text synlig när webbtecknen läses in. Sidan har också, enligt den mobila analysen, JavaScript som inte används. Liksom på startsidan finns det vissa resurser som blockerar renderingen och som flaggas i den mobila analysen. I desktopanalysen verkar den största enskilda "boven" just vara att vissa resurser blockerar renderingen men att läsa in fonter i förväg skulle också innebära en besparing.


#### Deklaration
Sidan fick betyget 25 för mobil och 81 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 3,47 sekunder, hade i genomsnitt 54 resurser som efterfrågades och dess totala storlek var i genomsnitt 3 678 kB.
https://skatteverket.se/privat/deklaration.html 

Sidan får ett dåligt värde på PageSpeedInsights för mobiler och ett "genomsnittligt" värde på desktop. Laddningstiden är på över 3 sekunder. I den mobila analysen verkar det, som för startsidan, främst vara olika resurser som blockerar renderingen. Det finns en del javascript på sidan som flaggas för att det inte används i den mobila analysen. Även för denna sida ger PageSpeedInsight också tipset att förladda vissa resurser (fonter) samt att göra text synlig när webbtecknen läses in. Sidan har också, enligt den mobila analysen, JavaScript som inte används. I desktopanalysen verkar den största enskilda "boven" vara att vissa resurser blockerar renderingen precis som för startsidan.

#### Skatter
Sidan fick betyget 30 för mobil och 88 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 4,59 sekunder, hade i genomsnitt 44 resurser som efterfrågades och dess totala storlek var i genomsnitt 2 872 kB.
https://skatteverket.se/privat/skatter.html

##### Diskussion
Sidan får ett dåligt värde på PageSpeedInsights för mobiler och ett "genomsnittligt" värde på desktop. Laddningstiden är på över 4 sekunder. I den mobila analysen verkar det, som för startsidan, främst vara olika resurser som blockerar renderingen. Det finns en del javascript på sidan som flaggas för att det inte används i den mobila analysen. Även för denna sida ger PageSpeedInsight också tipset att förladda vissa resurser (fonter) samt att göra text synlig när webbtecknen läses in. Sidan har också, enligt den mobila analysen, JavaScript som inte används. Liksom på startsidan finns det vissa resurser som blockerar renderingen och som flaggas i den mobila analysen. I desktopanalysen verkar den största enskilda "boven" just vara att vissa resurser blockerar renderingen precis som för de andra sidorna på webbplatsen men även här finns tips om att ladda in fonterna i förväg. 

### Analys
Mitt resultat visar att samtliga tre myndigheter skulle kunna förbättra framförallt sin hastigheter för mobiler. Pensionsmyndigheten får ett bra värde i desktopanalysen men Försäkringskassan och Skatteverket ligger också nära bra värden (>90) på sina sidor. Det var intressant att se att samtliga sidor fick tipset att ladda in resurser som fonter i förväg på PageSpeedInsights. Försäkringskassan och Skatteverket hade också "gemensamma" problem med att vissa resurser blockerade renderingen. 

Pensionsmyndigheten är den webbplats som kommer bäst ut i testet tycker jag. Den får både bäst betyg i PageSpeedInsights och i mina egna mätningar får den också de snabbaste laddningstiderna. Försäkringskassans startsida fick ett väldigt dåligt laddningstidsvärde på en av sina laddningar vilket drog upp snittet på den sidan markant. De andra sidorna ligger dock mellan 2-3 sekunder att jämföra med Skatteverkets vars samtliga sidor snittar på över tre sekunder, i två fall över 4. Jag placerar därför Försäkringskassan som tvåa och Skatteverket som trea. En kan ju också se i resultatet att Skatteverket i regel har större total storlek på sina sidor. 

Jag är ju själv uppväxt under telefonmodemens tid och kommer ihåg när en försökte surfa där, så personligen är jag inte så känslig för laddningstider. Den enda sida jag själv reagerade över var Skatteverkets där det vid en laddning verkligen märktes att det tog tid att rendera sidan. Så jag skulle nog säga 3 sekunder för mig innan jag reagerar (men personligen har jag större tålamod och kan vänta längre än så). För mig är alltså samtliga i testet ingående myndigheters webbplatser helt ok när det gäller hastighet. På sidor som jag bygger för andra tycker jag dock att det är bra om det går att skala av ytterligare någon sekund. Jag tycker att Pensionsmyndigheten visar att det går att komma ner runt två sekunder på myndighetssidor där det finns mycket information, det är ett mål att sträva mot tycker jag. 

### Referenser
- 1 https://web.dev/performance-scoring/ 

### Övrigt
Rapportförfattare: Joel Löfgren
