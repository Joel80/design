---
Title: Kmom01
Description: Part 1
---

Kmom01
======
Ok -dags för första rapporten på design-kursen! Det har varit utmanande men också roligt att arbeta med detta kursmoment - jag har lärt mig en del - inte minst om git vilket jag trodde var det jag åtminstone skulle ha lite koll på.

Ramverk och CMS:er
------------------
Jag har inte jobbat så mycket med ramverk eller CMS:er tidigare. Det enda jag har någon liten erfarenhet är Episerver men det är flera år sedan jag såg det och det skiljer sig ju en hel del från Pico. Så i stort är detta en helt ny erfarenhet för mig att arbeta med ramverk och CMS:er

Verktyg och tekniker
--------------------
Det var en hel del som var nytt för mig här. Jag har arbetat lite på hobbynivå med Git och Github tidigare men jag stötte trots det på en del problem just med Git och Github. För det första råkade jag initiera repot med en readme-fil när jag skapade det. Det ledde till att jag hade svårt att pusha och pulla från det repo jag hade skapat lokalt eftersom git menade att de hade helt olika historik. Jag lyckades komma runt det genom att tvinga git att igonerera den skilda historiken. Dock kändes det som att detta ledde till en lite "tråkig" start på historiken så jag tog bort alla repon och startade om. Jag hade också problem med att git inte kunde skriva till config-filen. Det skapades hela tiden en config.lock och ömsom menade git att den inte hade tillstånd att skriva till filen ömsom att det inte gick att låsa filen. Efter mycket sökning på tror jag att jag lyckats spåra problemet till att jag hade filerna inklusive repot på Dropbox. Misstänker att git och Dropbox hamnade i konflikt med varandra och att git då (i regel) inte kunde skriva till config/låsa config eftersom Dropbox samtidigt "höll" filen för synkning. (Nåt sånt). Lösningen blev att flytta ut kursmaterial och repo från Dropbox och köra lokalt (jag kan ju använda git nu för att arbeta med portfolion på flera datorer om jag vill - det var huvudanledningen till att jag hade filerna på Dropbox). 

Markdown är ett annat nytt verktyg är ett annat nytt verktyg som jag inte alls har använt tidigare. Dock har jag inte stött på några större problem ännu och det cheat-sheet som visades i en av videorna samt John Grubers introduktion fungerar bra som guider så långt. Make och composer har fungerat felfritt för mig i den utsträckning jag har använt dem. 

När det gäller Pico i sig så har jag nu under första momentet försökt hitta bland mappar och filer och provat att ändra en del för att se vad som händer och var grejer sätts. Det känns som att det är mycket nytt här, videos och annat material har varit till stor hjälp för mig att komma igång.

Design. användbarhet och layout
-------------------------------
Jag kan väl sägas ha en "fördom" om design och användbarhet: att det är svårt. Det är svårt att få till en design som lyfter innehållet utan att störa och det är svårt att göra gränssnitt som fungerar bra för alla användare. Samtdigt tycker jag att användarvänlighet och tillgänglighet är viktiga värden som man bör sträva efter att nå. En fördom jag har om mig själv är väl att jag inte på något sätt har en naturlig talang för design. Det är med viss bävan jag går in i denna kurs men samtidigt känner jag att jag vill lära mig så mycket jag kan om detta och framförallt tekniker som kan få mig att bli bättre. 

När det gäller arbetet med mitt eget tema - så stack jag väl iväg lite när det gäller färg osv. Är inte helt säker på att det är så användarvänligt och förmodligen något som jag vill ändra framöver. Jag utgick ändå ganska mycket i de tekniska bitarna från övningen samt den index.twig och css som finns för dbwebb-temat. En del värden skruvade jag dock på för att få sidan att bli lite annorlunda och för att försöka förstå vad som händer om man skruvar lite här och där. Men som sagt temat, färgkomposition och läsbarhet är väl något som jag tänker mig att jag borde se över lite mer framöver. Det gick väl helt ok men jag ser det som ett experiment än så länge. 

TIL
---
Min TIL för detta moment får bli Git och Github. Jag fick kämpa en del för att få det att funka men det gjorde också att jag nu kan mer om detta än tidigare - slitsamt men det känns bra.