---
Title: Kmom01
Description: Min redovisning för kmom01
Template: kmom
---
##Kmom01

Ok - dags för första rapporten på design-kursen! Det har varit utmanande men också roligt att arbeta med detta kursmoment. Jag har lärt mig en del - inte minst om Git vilket jag trodde var det jag åtminstone skulle ha lite koll på redan från början.

Ramverk och CMS:er
------------------
Jag har inte jobbat så mycket med ramverk eller CMS:er tidigare. Det enda jag har någon liten erfarenhet av är Episerver men det är flera år sedan jag använde det och det skiljer sig ju en hel del från Pico. Så i stort är detta en helt ny erfarenhet för mig att arbeta med ramverk och CMS:er.

Verktyg och tekniker
--------------------
Det var en hel del som var nytt för mig här. Jag har arbetat lite på hobbynivå med Git och Github tidigare men jag stötte trots det på en del problem just med Git och Github. För det första råkade jag initiera repot med en readme-fil när jag skapade det. (Skulle ha väntat in tisdagens föreläsning där det framgick klart och tydligt att repot inte skulle initieras!) Det ledde till att jag hade svårt att pusha och pulla från det repo jag hade skapat lokalt eftersom Git menade att de hade helt olika historik. Jag lyckades komma runt det genom att tvinga Git att igonerera den skilda historiken. Dock kändes det som att detta ledde till en lite "tråkig" start på historiken så jag tog bort alla repon och startade om. Jag hade också problem med att Git inte kunde skriva till config-filen. Det skapades hela tiden en config.lock och ömsom menade Git att den inte hade tillstånd att skriva till filen ömsom att det inte gick att låsa filen. Efter mycket sökning så tror jag att jag lyckats spåra problemet till att jag hade filerna inklusive repot på Dropbox. Misstänker att Git och Dropbox hamnade i konflikt med varandra och att Git då (i regel) inte kunde skriva till config/låsa config eftersom Dropbox samtidigt "höll" filen för synkning. Lösningen blev att flytta ut kursmaterial och repo från Dropbox och köra lokalt (jag kan ju använda Git nu för att arbeta med portfolion på flera datorer om jag vill - det var huvudanledningen till att jag hade filerna på Dropbox). 

Markdown är ett annat nytt verktyg som jag inte alls har använt tidigare. Dock har jag inte stött på några större problem ännu och det cheat-sheet som visades i en av videorna samt John Grubers introduktion fungerar bra som guider så långt. Make och composer har fungerat felfritt för mig i den utsträckning jag har använt dem. 

När det gäller Pico i sig så har jag nu under första momentet försökt hitta bland mappar och filer och provat att ändra en del för att se vad som händer och var olika saker kan ställas in. Det känns som att det är mycket nytt här, videos och annat material har varit till stor hjälp för mig att komma igång.

Design, användbarhet och layout
-------------------------------
Jag kan väl sägas ha en "fördom" om design och användbarhet: att det är svårt. Det är svårt att få till en design som lyfter innehållet utan att störa och det är svårt att göra gränssnitt som fungerar bra för alla användare. Samtdigt tycker jag att användarvänlighet och tillgänglighet är viktiga värden som en bör sträva efter att nå. Och även om det kanske då handlar om UX mer än "ren" design så kan en design som inte är bra sänka användarupplevelsen och tillgängligheten. En fördom jag har om mig själv är väl att jag inte på något sätt har en naturlig talang för design. Det är med viss bävan jag går in i denna kurs men samtidigt känner jag att jag vill lära mig så mycket jag kan om detta och framförallt tekniker som kan få mig att bli bättre.

När det gäller arbetet med mitt eget tema - så ville jag försöka få till ett "dark -theme". Min första tanke var att utgå från en bild på en blixt som jag hittat på Unsplash och låna färger från bilden till sidan. Dock blev det lite för mycket lila och för stark vit färg på texten. Jag backade lite och googlade efter tips för "dark-themes" och insåg då att det kunde vara bra att tona ned texten lite vilket jag gjorde med opacity. Jag bytte också från helt svart till mer av en gråton efter tips jag hittade under mina sökningar. Under arbetet med stylen så utgick jag från den befintliga css:en och "twigen" från dbwebb-temat samt det jag hade från kursmomentets övning. Sen tog jag bort en del saker som jag inte tyckte jag behövde just nu (men lät en del bra-att-ha-saker ligga kvar även om de inte används nu) och ändrade annat så att det skulle passa temat - mest rörde det sig då om att ändra färger. Jag har låtit det nya temat vara aktivt vid uppladdning till studentservern.

TIL
---
Min TIL för detta moment får bli Git och Github. Jag fick kämpa en del för att få det att funka men det gjorde också att jag nu kan mer om detta än tidigare - slitsamt men det känns bra.
