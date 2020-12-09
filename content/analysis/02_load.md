---
Title: Analysrapport 2
Description: Min rapport om sidors laddningstid
Template: analysis-report
---

## Laddningstider för myndigheters webbplatser
I denna analys undersöker jag tre myndigheters webbplatser och studerar deras laddningstider.

### Urval 
Jag valde att analysera samma tre webbplatser som under förra kmomet. Alltså Pensionsmyndighetens, Försäkringskassans och Skatteverkets webbplatser. Gemensamt för de tre myndigheterna är att deras verksamhetsområden  berör de flesta medborgare under större delen av våra liv. Dessa myndigheter hanterar socialförsäkringen och skatter vilket alla medborgare förmodligen någon gång behöver få fram bra information kring. Som jag skrev i förra analysen så arbetar myndigheterna efter den statliga värdegrunden där effektivitet och service är en ingående del.[1] Det är därför intressant att undersöka vilken prestanda webbplatserna har, här görs detta genom att undersöka laddningstider.

### Metod 
För att granska myndigheternas webbplatser valdes tre, på webbplatsen ingående, webbsidor ut. När jag valde ut vilka webbsidor som skulle vara med valde jag startsidan samt det jag uppfattade som de två första "reguljära" ingångarna. Försäkringskassan hade på första plats en ingång kring corona - denna valde jag bort eftersom den (förhoppningsvis) är tillfällig och därför kanske kan sägas avvika i innehåll från de mer permanenta ingångarna. I Skatteverkets fall valde jag startsidan och de två första ingångarna i den gula "navbaren".

Sedan användes [Googles PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/) för att mäta sidornas prestanda. Webbsidorna utvärderades där både för mobil och desktop och betygen noterades. PageSpeedInsights ger ett betyg mellan 0 och 100 där 0-49 är ett "dåligt" betyg, 50-89 är ett "genomsnittligt" betyg som innebär att sidan behöver förbättras och 90-100 innebär att sidan är "bra".[2] PageSpeedInsights gav flera tips på hur sidorna kunde förbättras. I diskussionen kring varje sida har jag inte lyft alla förslag utan lyft några exempel. 

Firefox developer editions devtools prestandaanalys användes sedan för att mäta sidornas laddningstid, antalet resurser som laddades samt sidans totala storlek. Mätningen utfördes tre gånger för varje webbsida och sedan togs ett genomsnitt av värdena. De värden som registrerades var de som uppmättes med cache inaktiverat. 

De data som samlades in i analysen finns i [detta kalkylark](https://docs.google.com/spreadsheets/d/1uMKB0m7V0OgIRrsCboD2ftkm0nsQL6XwbzqXR9PphPA/edit?usp=sharing). 

### Resultat
#### Pensionsmyndigheten
<img class="report-image" src= '../assets/img/pensionsmyndigheten.png' alt= "Screenshot från Pensionsmyndighetens webbplats">

Jag valde ut följande webbsidor att mäta hos Pensionsmyndigheten:

##### Startsidan
Sidan fick betyget 79 för mobil och 96 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 2,26 sekunder, hade i genomsnitt 40 resurser som efterfrågades och dess totala storlek var i genomsnitt 2 186kB.


###### Diskussion
Sidan får ett "genomsnittligt" värde på PageSpeedInsights för mobiler och ett "bra" värde på desktop. Det tar i genomsnitt strax över 2 sekunder att ladda klart sidan. PageSpeedInsights ger vissa insikter kring vad som skulle kunna förbättras. Bl.a. skulle vissa resurser (i detta fall fonter) kunna laddas in i förväg, texten skulle också kunna göras synlig medan webbteckensnitten läses in. För mobil anger också PageSpeedInsights bl.a. att modernare bildformat skulle leda till en besparing i storlek på data som skickas och därmed också en 
tidsbesparing. Det verkar också finnas resurser som blockerar renderingen och som skulle kunna inlinas eller där inladdningen skulle kunna vänta till senare.  
  
Länk till sidan:  
[Pensionsmyndighetens startsida](https://www.pensionsmyndigheten.se/)


###### Förstå din pension

Sidan fick betyget 83 för mobil och 97 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 1,84 sekunder, hade i genomsnitt 26 resurser som efterfrågades och dess totala storlek var i genomsnitt 1 942kB. 

###### Diskussion
Sidan får ett "genomsnittligt" värde på PageSpeedInsights för mobiler och ett "bra" värde på desktop. Det tar i genomsnitt strax under 2 sekunder att ladda klart sidan. Även här ger PageSpeedInsight tipset att förladda vissa resurser (fonter) samt att göra text synlig när webbtecknena läses in.
  
Länk till sidan:  
[Pensionsmyndigheten - Förstå din pension](https://www.pensionsmyndigheten.se/forsta-din-pension)

##### Gå i pension
Sidan fick betyget 80 för mobil och 94 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 1,74 sekunder, hade i genomsnitt 27 resurser som efterfrågades och dess totala storlek var i genomsnitt 1 940kB. 

###### Diskussion
Sidan får ett "genomsnittligt" värde på PageSpeedInsights för mobiler och ett "bra" värde på desktop. Den har den kortaste genomsnittliga laddningstiden av de tre sidorna på webbplatsen även om den ligger nära de andra. Även här ger PageSpeedInsight tipset att förladda vissa resurser (fonter) samt att göra text synlig när webbtecknen läses in.
  
Länk till sidan:  
[Pensionsmyndigheten - Gå i pension](https://www.pensionsmyndigheten.se/ga-i-pension)

#### Försäkringskassan
<img class="report-image" src= '../assets/img/forsakringskassan.png' alt= "Screenshot från Försäkringskassans webbplats">
Jag valde ut följande webbsidor att mäta hos Försäkringskassan:

##### Startsidan
Sidan fick betyget 24 för mobil och 86 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 7,67 sekunder, hade i genomsnitt 44 resurser som efterfrågades och dess totala storlek var i genomsnitt 1 138kB.

###### Diskussion
Sidan får ett "dåligt" värde på PageSpeedInsights för mobiler och ett "genomsnittligt" värde på desktop. Den genomsnittliga laddningstiden är på nära 8 sekunder, här var det en av omladdningarna som tog lång tid (15 sekunder) som drog upp medelvärdet rejält. Liksom för sidorna hos Pensionsmyndigheten  ger PageSpeedInsight tipset att förladda vissa resurser (fonter) samt att göra text synlig när webbtecknen läses in. Sidan har också, enligt den mobila analysen, JavaScript som inte används. Liksom på Pensionsmyndighetens startsida finns det vissa resurser som blockerar renderingen och som flaggas i den mobila analysen.
  
Länk till sidan:  
[Försäkringskassans startsida](https://www.forsakringskassan.se/)

##### Förälder
Sidan fick betyget 28 för mobil och 89 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 2,13 sekunder, hade i genomsnitt 32 resurser som efterfrågades och dess totala storlek var i genomsnitt 1 766 kB.

###### Diskussion
Sidan får ett "dåligt" värde på PageSpeedInsights för mobiler och ett "genomsnittligt" värde på desktop. Laddningstiden är på över 2 sekunder. Även här ger PageSpeedInsight tipset att förladda vissa resurser (fonter) samt att göra text synlig när webbtecknen läses in. Sidan har också, enligt den mobila analysen, JavaScript som inte används. Liksom på startsidan finns det vissa resurser som blockerar renderingen och som flaggas i den mobila analysen. I desktopanalysen verkar den största enskilda "boven" just vara att vissa resurser blockerar renderingen.
  
Länk till sidan:  
[Försäkringskassan - Förälder](https://www.forsakringskassan.se/privatpers/foralder)

##### Sjuk
Sidan fick betyget 53 för mobil och 94 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 2,06 sekunder, hade i genomsnitt 32 resurser som efterfrågades och dess totala storlek var i genomsnitt 1 782 kB.

###### Diskussion
Sidan får ett "dåligt" värde på PageSpeedInsights för mobiler och ett "bra" värde på desktop. Laddningstiden är på strax över 2 sekunder. Även här ger PageSpeedInsight tipset att förladda vissa resurser (fonter) samt att göra text synlig när webbtecknen läses in. Sidan har också, enligt den mobila analysen, JavaScript som inte används. Liksom på startsidan finns det vissa resurser som blockerar renderingen och som flaggas i den mobila analysen. I desktopanalysen verkar det som har störst enskild påverkan just vara att vissa resurser blockerar renderingen precis som för "förälder-sidan".
  
Länk till sidan:  
[Försäkringskassan - Sjuk](https://www.forsakringskassan.se/privatpers/sjuk)

#### Skatteverket
<img class="report-image" src= '../assets/img/skatteverket.png' alt= "Screenshot från Skatteverkets webbplats">

Jag valde ut följande webbsidor att mäta hos Skattteverket:

##### Startsidan
Sidan fick betyget 51 för mobil och 87 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 4,54 sekunder, hade i genomsnitt 43 resurser som efterfrågades och dess totala storlek var i genomsnitt 2 857 kB.

###### Diskussion
Sidan får ett "genomsnittligt" värde på PageSpeedInsights för mobiler och ett "genomsnittligt" värde på desktop. Laddningstiden är på över 4 sekunder. I den mobila analysen verkar det främst vara olika resurser som blockerar renderingen, där listas både css-filer och js-filer bland annat. Det finns en del javascript på sidan som flaggas för att det inte används i den mobila analysen. Även för denna sida ger PageSpeedInsight tipset att förladda vissa resurser (fonter) samt att göra text synlig när webbtecknen läses in. I desktopanalysen flaggas för att vissa resurser blockerar renderingen, att läsa in fonter i förväg är också här ett exempel på vad som skulle kunna åtgärdas för att sidan ska ladda snabbare.
  
Länk till sidan:  
[Skatteverkets startsida](https://www.skatteverket.se/)

##### Deklaration
Sidan fick betyget 25 för mobil och 81 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 3,47 sekunder, hade i genomsnitt 54 resurser som efterfrågades och dess totala storlek var i genomsnitt 3 678 kB.

###### Diskussion
Sidan får ett "dåligt" värde på PageSpeedInsights för mobiler och ett "genomsnittligt" värde på desktop. Laddningstiden är på över 3 sekunder. I den mobila analysen verkar det, som för startsidan, främst vara olika resurser som blockerar renderingen. Det finns även här en del javascript på sidan som flaggas för att det inte används i den mobila analysen. Även för denna sida ger PageSpeedInsight också tipset att förladda vissa resurser (fonter) samt att göra text synlig när webbtecknen läses in. Sidan har också, enligt den mobila analysen, JavaScript som inte används. I desktopanalysen verkar den största enskilda faktorn vara att vissa resurser blockerar renderingen.
  
Länk till sidan:  
[Skatteverket - Deklaration](https://skatteverket.se/privat/deklaration.html)

##### Skatter
Sidan fick betyget 30 för mobil och 88 för desktop på PageSpeedInsights. Den laddade i genomsnitt på 4,59 sekunder, hade i genomsnitt 44 resurser som efterfrågades och dess totala storlek var i genomsnitt 2 872 kB.


###### Diskussion
Sidan får ett "dåligt" värde på PageSpeedInsights för mobiler och ett "genomsnittligt" värde på desktop. Laddningstiden är på över 4 sekunder. I den mobila analysen verkar det, som för startsidan, främst vara olika resurser som blockerar renderingen som är problemet. Det finns en del javascript på sidan som flaggas för att det inte används i den mobila analysen. Även för denna sida ger PageSpeedInsight tipset att förladda vissa resurser (fonter) samt att göra text synlig när webbtecknen läses in. I desktopanalysen flaggas, liksom i flera av fallen ovan, att vissa resurser blockerar renderingen av sidan samt att vissa resurser (även här fonter) skulle kunna laddas i förväg.
  
Länk till sidan:  
[Skatteverket - Skatter](https://skatteverket.se/privat/skatter.html)

### Analys
Mitt resultat visar att samtliga tre myndigheter skulle kunna förbättra webbplatserna framförallt när det gäller laddningshastighet för mobiler. Pensionsmyndigheten får ett "bra" värde i desktopanalysen men Försäkringskassan och Skatteverket ligger också nära "bra" värden  på sina sidor. Det var intressant att se att samtliga sidor fick tipset att ladda in resurser som fonter i förväg på PageSpeedInsights. Ett annat "gemensamt" problem var att vissa resurser blockerade renderingen. Vanligt förekommande var också att det på sidorna fanns javascript som inte användes. Jag funderar på om resultatet kan bero på att myndigheterna har designat för desktopanvändare i första hand. Kanske tänker de att det i första hand är via dator webbplatserna används. Här tror jag dock att det i så fall kan finnas anledning att tänka om eftersom jag tror att många användare även använder denna typ av sidor mobilt (jag är själv ett exempel på detta) och att denna form av användning troligen kommer öka ännu mer i framtiden även för denna typ av webbplatser.

Pensionsmyndigheten är den webbplats som kommer bäst ut i testet tycker jag. Den får både bäst betyg i PageSpeedInsights och i mina egna mätningar får den också de snabbaste laddningstiderna. Försäkringskassans startsida fick ett väldigt dåligt laddningstidsvärde på en av sina laddningar vilket drog upp snittet på den sidan markant. De andra sidorna ligger dock mellan 2-3 sekunder att jämföra med Skatteverkets vars samtliga sidor snittar på över tre sekunder, i två fall över 4. En kan ju också se i resultatet att Skatteverket i regel har större total storlek på sina sidor vilket ju också bör ha påverkan på laddningstiden. Jag placerar därför Försäkringskassan som tvåa och Skatteverket som trea. 

Vad är då en rimlig laddningstid för en sida? Jag är ju själv uppväxt under telefonmodemens tid och kommer ihåg när en försökte surfa där, så personligen är jag inte så känslig för laddningstider. Den enda sida jag själv reagerade över var Skatteverkets där det vid en laddning (utanför mätning) verkligen märktes att det tog tid att rendera sidan. Så jag skulle nog säga 3 sekunder för mig innan jag reagerar men betydligt längre tid innan jag ger upp. För mig är alltså samtliga i testet ingående myndigheters webbplatser helt ok när det gäller laddningshastighet. Men det är min egen uppfattning. Under onsdagens föreläsning framkom ju att mätningar visar att en användare kanske bara stannar på en webbplats i ett par sekunder innan hen tappar intresset. Därför tänker jag att jag själv vill ha som mål för de sidor som jag skapar att ha en kortare laddningstid än vad jag själv tolererar.

### Referenser
- 1 [Förvaltningskultur](https://www.forvaltningskultur.se/statliga-vardegrunden/)
- 2 [Lighthouse performance scoring](https://web.dev/performance-scoring/)

### Övrigt
Rapportförfattare: Joel Löfgren
