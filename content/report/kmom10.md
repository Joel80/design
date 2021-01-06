---
Title: Kmom10
Description: Min redovisning för kmom10
Template: kmom
---

## Kmom10
Ok dags att redovisa kmom10 och projektet! Det har varit intressanta att arbeta med detta projekt. Det har också stundtals varit ganska utmanande. Under förra kursen (htmlphp) kände jag att CSS var en av de mer utmanade bitarna. Nu känner jag att jag har fått mycket övning och säkert höjt mig några snäpp. Åtminstone tillräckligt mycket för att inse att det finns väldigt mycket mer att lära sig!

### Kunden
Jag valde att göra en personsida åt webbutvecklaren Bew Gorp. Detta eftersom jag tyckte att det skulle vara intressant att prova på att göra en sida för en sådan kund eftersom det är något jag kanske kan ha nytta av om jag i framtiden vill göra en liknande sida för mig själv. I en av mina tidigare analyser hade jag också tittat på webbutvecklare/designers webbplatser och jag kände att det vore roligt att prova på att bygga en egen sådan sida.

### Uppdrag 1: Webbplats
Jag valde att börja om arbetet från grunden i detta projekt istället för att använda mig av min tidigare portfolio som grund. Detta gjorde jag främst eftersom jag ville repetera stegen vi gått igenom under kursen. Det gav mig anledning att gå igenom kursmomenten igen och sätta upp ett nytt (privat) GitHub repo, fixa med package.json, konfigurera cimage, sätta upp sessionen m.m. Jag vill tro att denna upprepning gav en hel del nu andra varvet och ledde till en drös med polletter trillade ner.

Precis som för min egen portfoliosida så utgick jag från dbwebb-temat och lånade över de delar som jag tyckte var relevanta från dess twig och CSS-filer. Till skillnad från i arbetet med min egen portfolio-sida valde jag att göra uppdelningar av twig-koden på så sätt att jag en gemensam header.twig och footer.twig som inkluderas i alla sidor. 

Jag valde att använda mig av en hero-bild som laddas som en bakgrundsbild via CSS. Herobilden finns på alla sidor eftersom jag tycker att det är bra sätt att skapa igenkänning och enhet på en webbplats. Om sidhuvudet ser likadant ut på alla sidor är det lätt för användaren att veta att denne inte har lämnat sidan.

Jag skapade en egen logga för Bew Gorp i GIMP. Det blev en enkel textlogga med utvecklarens initialer "BG". Jag tänkte att eftersom det är en portfolio-sida så blir det bra med initialerna i för- och efternamn som logga. Som favicon tog jag en bild på en datormus från [Open Clipart](https://openclipart.org/) - jag tyckte att denna anspelade på ämnet webbutveckling på ett bra sätt. 

När det gäller navigeringen använde jag mig av den navigering som följde med dbwebb-temat. Som jag förstår det är det en del javascript inblandat i att få denna att fungera och javascript är något som jag inte är särskilt insatt i ännu så den fick vara som den är. Navigeringen som denna meny ger fungerar bra både på desktop och mobil tycker jag.

Själva innehållet har jag till stora delar hittat på själv (förutom bilderna som jag har hämtat från Unsplash). Här har jag försökt tänka igenom vad som kan vara relevant att lyfta. På startsidan valde jag därför att först lyfta Bew Gorps långa erfarenhet av webbutveckling och därefter ge en ingång till de projekt som han har arbetat med. Projektsidan valde jag utforma som det galleri som vi arbetade med under kursens gång - genom att klicka på en av bilderna i galleriet kommer en till en sida där det finns en kort text om projektet ifråga. Längre ned placerade jag text om och "ingångar" till informationen om sidan och kontaktuppgifterna. Kontaktuppgifterna i sig valde jag att lägga som ikoner i webbplatsens footer. Min tanke här är att användare förmodligen letar efter kontaktuppgifter här - de är också tillgängliga på alla sidor på webbplatsen så när användaren känner för kontakt är det bara att skrolla ner.

De flesta bilderna laddas in via twig och här har jag arbetat med picture och source/srcset samt cimage för att göra bilderna responsiva. Vid olika skärmstorlekar använder jag olika queries som skickas till cimage för att minska bredden på bilden och i vissa fall också kvaliten. På hero-bilden som laddas via CSS används också cimage för att begränsa bredden och på så sätt få ned storleken.

Om-sidan var ganska rolig att skriva eftersom jag här själv ju fick sätta ihop en bakgrund åt Bew och försöka sätta mig in i vad han borde önska för slags webbplats. Här landade jag ganska snabbt i att det viktiga var att få fram huvudbudskapet kring Bew Gorps erfarenhet på central plats - även att peka på projekten och att ge enkel tillgång till kontaktuppgifter såg jag som viktigt efter att ha tänkt igenom hur en utvecklare borde vilja ha sin portfolio-sida.

### Uppdrag 2: Tema
I Om-sidan fick jag också möjlighet att fundera lite över vilket slags tema som skulle passa Bew. Jag kom fram till att Bew ville att sidan skulle ge ett stilrent, harmoniskt och enkelt intryck och vara lätt att navigera på. Besökaren skulle få en känsla av av stilrenhet, lugn, harmoni och kompetens. Jag valde därför att utgå från den blå färg som jag hade i ett av mina teman på min egen portfolio sida. Blått tolkas ibland som en "fredens" färg och jag tänkte att det kunde hjälpa att ge en lugn och harmonisk känsla. Samtidigt tänkte jag att en utvecklare säkert också vill ge ett "tekniskt" intryck för att visa på teknisk kompetens. Jag letade därför efter ett typsnitt som kunde upplevas som tekniskt och fastnade för Orbito. För att skapa harmoni och balans arbetade jag med Grid för att få till lika stora delar med innehåll på sidan som skapade ett mönster och upprepning som i sin tur ger harmoni. Detta gjorde jag både på Hem-sidan och Projekt-sidan Jag beskriver detta mer utförligt på den dolda sida om temat som nås via webbplatsens Om/about-sida.

### Uppdrag 3: Responsivitet och tillgänglighet
#### Responsivitet
Förutom att ge mig möjlighet att arbeta med upprepning har jag också använt Grid och Flexbox tillsammans med media queries för att skapa en responsiv webbplats. Sidorna ligger i grunden i en Flexbox som ordnar header, main och footer i en kolumn. Flexbox används också i headern för att placera ut logga, huvudrubrik och navbar på lagom avstånd från varandra. Loggan tyckte jag tog för mycket plats på de minsta skärmarna så jag valde att dölja den för skärmar som är mindre än 600px breda.

Main-delen på index-sidan ("Hem") är indelad i ett grid. Här använder jag sedan konstruktionen grid-template-areas för att skapa områden för olika typer av innehåll på desktop. I mobilt läge ställs main om till en flexbox som lägger innehållet i en kolumn. Detta för att varje del ska vara lika stor på fullskärm men inte ta upp mer vertikalt utrymme än nödvändigt på mindre skärmar. 

Footern använder sig av Grid för att placera ut innehållet. Det ligger i två kolumner på fullskärm men på mindre skärmar ställs detta om till en kolumn.

Som jag skrev ovan har jag också använt cimage, picture och source för att göra mina bilder responsiva och anpassade till olika skärmstorlekar.

Detta är exempel på hur jag har arbetat med webbplatsens responsivitet och såvitt jag kan se undviks horisontella scrollbars även på mindre skärmar.

#### Tillgänglighet
Mitt huvudsakliga verktyg för att arbeta med webbplatsens tillgänglighet var Lighthouse. När jag testkörde där så fick jag följande anmärkningar och vidtog de listade åtgärderna:

##### Hem
###### Desktop:
"Focusable descendents within an `[aria-hidden="true"]` element prevent those interactive elements from being available to users of assistive technologies like screen readers"
element: div.logo

Åtgärd: tog bort länken vid loggan eftersom jag inte tyckte att även loggan behöver vara länkad när huvudrubriken är det. 

###### Mobilt: 
Some elements have a [tabindex] value greater than 0
Failing Elements: a#nav-toggle.nav-toggle

Åtgärd: Tog bort tab-index för nav eftersom det ändå är första elementet på sidan så bör det fungera bra ändå.

Detta var de problem som hittades på Hem-sidan när de hade åtgärdats fick jag 100% i tillgänglighet på samtliga sidor i Lighthouse.

Vidare har jag laddat in de publicerade sidorna på [Toptotal Colorblind Web Page Filter](https://www.toptal.com/designers/colorfilter/) för att kolla om de ser ok ut med hänsyn till olika typer av färgblindhet - min bedömning är att de gör det.

### Uppdrag 4: Alternativt tema
Jag valde att göra det optionella uppdrag 4 och skapa ett alternativt tema. Här fick jag återigen försöka sätta mig in i vilket slags alternativt tema Bew skulle vilja ha och fundera kring hur jag skulle ändra på designelement och designprinciper. Jag kom fram till att Bew ville ha ett mer "färggrannt" och utmanande tema, som gav en känsla av futurism men som också skulle kännas mer organiskt. Känslan av stilrenhet och kompetens skulle behållas. Jag letade därför upp en ny hero-bild med neonfärger i sig och utgick från en av dessa färger. För att få mer variation i färgerna utgick jag från ett analogt istället för ett monokromt schema. Bakgrunden fick bli mörk för att bryta av mot det ljusa i det grundläggande temat. Jag ändrade typsnittet till ett mjukare och bestämde mig också för att använda mycket rundade former för att ge en mer organisk känsla. Bilderna i det grundläggande temat är skuggade för att ge en känsla av djup - i det alternativa temat valde jag att ta bort alla skuggor för att ge ett plattare intryck. Denna något mer minimalistiska stil kopplar jag själv samman med futurism - kanske för att minimalism verkar vara en trend på uppåtgående inom webbdesign. På Hem-sidan bytte jag också ut den vertikala balansen från den grundläggande sidan till en radiell balans för att på så sätt ge detta tema ett helt annat första intryck.

### Uppdrag 5: Analys aktuell webbplatsdesign
Jag valde att göra det optionella uppdrag 5 och göra en analys av aktuell webbplatsdesign. Jag valde att titta på försäkringsbolag och för att få till ett urval att titta på valde jag ut de fyra bolag som har störst marknadsandelar inom skadeförsäkring. För att kunna uttala mig om vilken webbplatsdesign som dessa företag använder sig av bröt jag sedan ned deras startsidor utifrån olika designelement och designprinciper för att se vilka gemensamma nämnare de hade och vad som skilde dem åt. Jag kom fram till att den moderna försäkringswebbplatsen är luftig, har en dragning mot det platta och minimalistiska. Formmässigt föredras en organisk känsla genom rundade former. Enhet skapas genom användande av ett fåtal typsnitt (ett eller två) och harmoni skapas genom att använda sig av rutnätslayout som upprepas över sidan. 

Det var intressant att arbeta med analysen eftersom det gav mig tillfälle att upprepa en hel del av det som vi tidigare har gått igenom kring designelement och designprinciper och repetera och befästa kunskaperna inom området.


### Uppdrag 6: Analys valfri
Jag valde att göra det optionella uppdrag 6. Jag valde här att göra en analys av laddningstiderna, delvis eftersom jag redan hade skrivit en del om färg och design på min Om-sida men kanske mest för att jag var lite nyfiken på att se vilken prestanda webbplatsen hade. Jag funderade också på om jag skulle analysera båda mina teman eller bara det grundläggande. Efter en fråga chatten och ett snabbt svar fick jag veta att båda sätten var ok. Jag valde att analysera båda mina teman eftersom de på vissa ställen använder olika bilder och jag ville se om det skulle påverka resultatet. Det visade sig att det till viss del gjorde det eftersom jag fick en "anmärkning" på min hero-bild i det alternativa temat men inte i det grundläggande. De flesta av mina bilder verkade dock passera analysen utan anmärkning - något jag blev glad över eftersom jag arbetat med cimage, picture och srcset för att se till att de anpassar sig efter användarens enhet. Jag lärde mig en hel del annat av resultatet också bl.a. vikten av att försöka undvika att CSS:en blockerar renderingen och att inte ha för mycket onödig CSS. Tyvärr landade jag väl också i slutsatsen att jag med mina nuvarande kunskaper inte kan åtgärda allt detta - men det har också gjort mig taggad att lära mig mer. 


## Om projektet
Projektet har varit roligt och intressant. Det har krävt en hel del arbete från min sida tycker jag men inte mer än förväntat. En hel del tid har faktiskt gått åt till att pröva sig fram med utformningen av teman. Under arbetets gång kastade jag faktiskt ett alternativt tema som jag hade arbetat med och började om. Det kanske låter som ett tidsslöseri men jag kunde återanvända mycket av den grundläggande CSS:en från detta tema ändå. Det var också en nyttig erfarenhet att ta det steget och kasta något som jag arbetat mycket med eftersom jag (och som jag tänkte mig kunden) inte var nöjd. Annars är det väl just CSS-koden som jag har kämpat mest med och också lärt mig mycket om. Otaliga små problem har hopat sig  och jag har slitit med att förstå mig på padding och marginaler och varför saker hamnar där de hamnar. Jag har fått en djupare förståelse både för Grid och Flexbox som jag tycker är väldigt bra konstruktioner för att placera innehåll, de ger kontroll. 

Jag tycker att projektet var ett rimligt projekt att avsluta kursen med. Jag tycker att det är bra att det finns optionella uppdrag så att en själv kan anpassa sin insats efter den tid en har. 

## Om kursen
Som jag skrev inledningsvis så tycker jag att det har varit en intressant och rolig kurs. Jämfört med mina kunskaper i början av kursen börjar jag nu se mönster i och förstå CSS - jag tycker nu att jag har en del grundläggande kunskaper även om det finns mycket kvar att lära sig också. Det har varit väldigt roligt och nyttigt att arbeta med verktyg som NPM, GitHub, Pico och SASS.

Att arbeta utifrån designprinciper har också varit nyttigt - jag ser verkligen nyttan nu med att kunna något om området för att arbeta som utvecklare. Jag blir nog aldrig designexpert men att nu åtminstone ha en aning om hur det "fungerar" och att det finns principer som styr detta är en rolig och intressant lärdom.

Kursen har också gett många värdefulla källor att hämta kunskap ifrån både när det gäller CSS och designelement och principer. Guiderna har varit bra och känts uppdaterade. Har något saknats (vilket ju nästan är ofrånkomligt då det är en ny version av kursen) så har det kommit snabbt på plats. Föreläsninganrna har också varit jättebra. Det har varit en bra kombo med en praktisk föreläsning på tisdagen med tips på hur en kan ta sig an veckans moment och en mer teoretisk föreläsning på onsdagen som fördjupar förståelsen för momentet. Det är ett upplägg som jag tycker att ni ska fortsätta med. 

Även på denna kurs (liksom förut htmlphp) har supporten från er i lärarteamet varit helt fantastiskt med extremt snabba och kunniga svar i chatten. 

Jag är väldigt nöjd med kursen och skulle rekommendera den till intresserade vänner, den får en 10:a av mig.
