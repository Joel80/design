---
Title: Kmom02
Description: Part 2
---

##Kmom02
Ok - dags att redovisa kmom02! Det har varit intressant att arbeta med SASS, jag gillar möjligheterna att dela upp css-koden och att kunna arbeta med variabler och "nästning". Det har också varit intressant att se hur man kan arbeta med olika fonter och ikoner. Det känns dock som att det kommer behövas mer övning innan jag har greppat allt.

###SASS
Jag gillar SASS och möjligheterna det ger att styla en webplats på ett lite mer strukturerat sätt. Jag har testat att lägga in variabler för färger på text och bakgrund, för att sätta storlek på min main och aside samt för att sätta font-storlekar och radavstånd (på det sätt som visades i onsdagens föreläsning). Jag tycker att detta ger mycket bättre kontroll över CSS:en - nu känns det som att jag bara börjat och att detta säkert kan utvecklas mer. Jag har också provat att "nästa" lite främst i listor (t.ex. den med resurser i min aside). Jag tycker att "nästandet" är ett intuitivt och bra sätt att strukturera kod - lätt att se att t.ex. "detta ska gälla för länkarna i just denna klass". 

Att kompilera SASS var också intressant - jag har inte satt upp någon watch utan kört kommandot varje gång. Några felmeddelanden har jag fått ibland och jag tycker att de har varit lättlästa och bra. Jag sätter förmodligen upp en watch senare men just nu har det kännts bra att "nöta in stegen" - ändra i scss-filen, kompilera och kolla resultatet. Det ger mig en bild över flödet

###Node och npm
Jag har inte arbetat med node, npm eller npm-scripts tidigare så det har varit helt nytt för mig. För min del klarnade en del under onsdagens föreläsning. Jag hade kört med npm lite innan då, installerat, hämtat alla paket och satt upp scriptet för att kompilera enligt guiderna. Men det var nog först under föreläsningen som polletten trillade ner på riktigt och jag förstod hur det hängde ihop och nyttan med detta. Jag gillade särskilt biten om att detta är ett bra sätt att bygga en gemensam utvecklingsmiljö för en grupp eller team - det gjorde att jag fick en djupare förståelse för nyttan med npm och npm scripts.

###Mitt tema
Som jag skrev i min förra rapport så är grundtanken med mitt tema att det ska vara en slags "dark-style". Målsättningen är väl ett relativt enkelt tema med ett fåtal färger som inte ska störa för mycket. Det är ju lite en utmaning att få till det när det ska vara ett mörkt tema tycker jag (så vi får se hur länge det hänger kvar...) som jag skrev i förra rapporten har jag fått leta lite information kring hur man kan tänka kring bakgrund och text-färg. Denna gång utvecklades temat mest genom nya fonter och ikoner. Där följde jag guiderna rätt nära för att få till det. 

###Uppdelning av koden
Inledningsvis under detta kmom så hade jag bara en "liten" uppdelning av kod - ungefär den uppdelning som följde på övningarna. D.v.s. en base.scss som laddar normalize, variables och layout. Min layout-fil var sedan en ganska stor fil som i princip såg ut och var uppdelad som min gamla style.css. En bit in i veckan valde jag dock att dela upp denna fil i flera mindre och i det sammanhanget också gå vidare i att rensa ut saker som jag inte behöver. Så nu har jag 9 .scss-filer som jag importerar in i layout.scss som sedan importeras i base.scss. Jag gillar möjligheten att dela upp koden på detta sätt, det ger bättre överblick i regel tycker jag. Sedan är det också, enligt min mening, en balansgång mellan små och lättlästa filer och att kunna få en snabb överblick eller hitta saker vilket kan bli svårare med många filer. Det kan också vara en utmaning att hitta en bra fil att lägga visa saker generella saker eller "fixar" i.



