---
Title: Kmom03
Description: Min redovisning för kmom03
Template: kmom
---

##Kmom03
Ok dags att redovisa kmom03! Under detta moment har jag experimenterat en hel del - framförallt med Grid. Jag tycker att jag genom läsning och övning har fått en grundläggande förståelse för Grid och Flex även om jag känner att det krävs mycket mer övning för att bemästra detta.

###CSS-grid och Flex-box
Det känns som att det har gått bra att arbeta med Grid och Flex. Flex använde jag sedan tidigare på portfolio-sidan på body-elementet (det var en del av dbwebb-temat som jag har valt att behålla) där header, main och footer staplas på varandra genom attributet flex-direction: columns. Jag fokuserade på att arbeta med Grid under detta kmom eftersom jag inte alls har arbetat med det tidigare. (Jag gjorde dock övningsuppgifterna kring Flexbox också). Det är inte helt lätt att greppa någon av teknikerna tycker jag men jag ser att de är väldigt användbara för att placera innehåll - något som jag tyckt har varit en utmaning så långt i CSS. Det fanns mycket och bra information att ta in angående ämnet och det känns som jag har bra ställen att återvända till om jag vill kolla upp något. Det var också intressant att läsa de texter som gav en historik till "rutnätets" historia inom design och hur det används på webben idag, samt texten om olika designelement. Det var tankeväckande texter och gav mig en del "aha-upplevelser". 

Jag fokuserade mest på att få till en Grid-lösning på rapportsidorna. Även om de wireframes som vi fick inte behöver efterliknas precis utan mer ska ses som en idé så ville jag ändå utmana mig själv och få min lösning så lik dessa som möjligt (fast med andra färger då). För att uppnå detta så arbetade jag med grid på "landingssidan". Här skapade jag först boxar utifrån exemplet och tisdagens föreläsning. Sen gick jag vidare och gav kmom-boxen egenskapen grid också. Där skapade jag sedan tre grid-areas för kmom-header, kmom-content och kmom-link. Dessa fick sedan varsin klass och placerades på varsin rad i boxens grid. Genom detta försökte jag efterlikna de wireframes vi fått så långt som möjligt. Jag utgick mycket från det exempel som fanns på github kring Grid för att få till detta. 

När det gäller själva informationen som visas i kmom-boxarna så använder jag en annan metod än den som presenterades i föreläsningen och inledningen på uppgiften för att visa ut den. Som jag förstod på föreläsningen så kunde man välja att antingen lägga html-koden i en markdown-fil eller i report.twig-filen. Jag valde det senare och använde mig av Picos page() funktion för att via en for-loop hämta det jag behövde från Report-mappen. Jag använde mig av metainformation kring titel för boxens header, metainformationen i description för textinnehållet i boxens content-del och sedan page.url för att få ut länken till respektive rapport. Länken visas som en pil-ikon som jag hittade på Font Awesome. På motsvarande sätt hämtar jag länkarna till rapporterna i kmom.twig från report-mappen med hjälp av pages() och page.url. Jag hade god hjälp av [Picos dokumentation](http://picocms.org/in-depth/features/pages-function) i detta arbete. 

Jag fick även anledning att tillämpa Grid på andra delar av min portfolio. Under kmom02 skapade jag en aside med resurser som låg på samtliga sidor. Nu när kmom-boxarna tar upp mycket av platsen på rapportsidan så valde jag att ta bort min aside och istället flytta resurserna till sidfoten. Även här skapade jag då en Grid där resurserna, min sidfotstext och länken till Github ligger i olika kolumner i desktop-läge och i olika rader i mobilläge. 

###SASS
Som jag skrev i förra rapporten så har jag gjort en ganska långtgående uppdelning av mina SASS-moduler där jag har försökt hitta en logisk uppdelning så att jag får relativt små och avgränsade filer som ska vara lätta att överblicka. Nu blev det ytterligare en modul för just rapport-sidorna. Det var väldigt värdefullt att hålla denna kod separat för att lättare kunna experimentera med den. 

###TIL
Jag har lärt mig mycket om Grid och Flex men min TIL för detta moment får nog ändå vara "rutnätets" betydelse för formgivning och design. Detta har jag inte tänkt på på detta sätt tidigare och nu börjar jag se detta mönster på alla möjliga ställen, i tryckta produkter såväl som på webben!
