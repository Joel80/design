---
Title: Kmom04
Description: Min redovisning för kmom04
Template: kmom
---

## Kmom04
Dags att redovisa kmom04! Det var roligt att bygga ett nytt tema till webbplatsen - jag fick dock vända lite på uppgiften eftersom jag sedan tidigare hade utgått från och byggt ett mörkt tema. 

### Skrivuppgiften
Jag måste erkänna att jag tyckte att det var svårt att göra färganalysen. Hur jag än vände och vred på färgerna så kändes det som att det i regel var svårt att riktigt passa in dem i ett  färgschema. Jag hade hjälp av t.ex. Adbobes färghjul men det var ändå inte helt lätt att se vilken typ av schema det rörde sig om, vilken vikt som skulle läggas vid accentfärger i bedömningen och vilken vikt som bör läggas vid helhetsintrycket. Jag är inte säker på att jag fått det helt "rätt" men har försökt redovisa hur jag har tänkt i analysen.

### Mitt eget färgschema
Som jag har skrivit om i tidigare rapporter så har jag från början utgått från ett "mörkt tema". Jag blev lite fundersam först när det kom som uppgift i detta moment att bygga ett sådant men valde att vända på uppgiften och göra ett ljust tema som skulle uppfylla kraven för det "vanliga temat". Jag startade med att leta upp en ny flashbild för detta tema. Det mörka temat bygger till viss del på flashbilden  - den lila färgen i footern där är tagen från bilden. Jag valde därför en ny bild till det ljusa temat, även denna gång på en blixt och tog färgen till min "ljusa" footer därifrån. Med utgångspunkt i denna färg använde jag Adobes color wheel för att få fram ett schema. Jag valde att arbeta med ett monokromt schema eftersom jag tycker att det ger ett lugnt och behagligt intryck. Färgschemat jag fick från Adobe color wheel ser ut så här:

<table style="border-spacing: 4px; border-collapse: separate">
    <tr>
    <td style="height: 50px; width: 50px; background-color: #4A98D4">
    <td style="height: 50px; width: 50px; background-color: #65849B">
    <td style="height: 50px; width: 50px; background-color: #2F6186">
    <td style="height: 50px; width: 50px; background-color:#A5B2CF">
    <td style="height: 50px; width: 50px; background-color: #8AB4D4">
    <td style="height: 50px; width: 50px; background-color: #1D3C54">
   </tr>
    </table>

I huvudsak används basfärgen #2F6186 (tredje från vänster) som är hämtad från flash-bilden för footer och länkar, ljusare nyanser för länkarna i nav-baren och headern (#8ab4d4 för länkar i nav, den mörkare #4A98D4 för hover och aktiv ) samt ljusare nyans (#8AB4D4) i headern på analys- och rapportrutorna. Den dominerande färgen som jag använder på "störst ytor" är basfärgen #2F6186. De andra nyanserna används mer sparsamt, några som den mörkaste (#1D3C54) samt den mörkgrå (#65849B) använder jag inte i nuläget. Jag använder mig alltså i mångt och mycket av nyanser av samma färg så jag skulle inte säga att jag i detta har arbetat med någon accentfärg om en med det menar en färg som kraftigt avviker från de andra. I footern fick jag använda en färg utanför mitt färgschema för text och länkar eftersom jag fick lite problem med kontrasten i footern om jag skulle ha hållt mig enbart till färgschemat. Länkarna och texten där fick därför samma grå-vita färg som body (#ebebeb) och helt vitt (#fff) vid hover.

### Det mörka temat
Egentligen fanns ju redan mitt mörka tema som sagt. Men för att få till två teman ett ljust och ett mörkt gjorde jag så att jag skapade två nya mappar under theme -light och dark. I dessa mappar finns en base-light, en color-light samt en style.scss respektive en base-dark, en color-dark och en style-dark.scss. I color-filerna bröt jag ut de variabler som hanterade färger. Base-filerna importerar sedan colors-light eller dark beroende på tema och sedan importeras den gemensamma layouten. Därefter importeras respektive "base-fil" i style.scss respektive style-dark.scss. "Light" och "dark" "delar" alltså på samma scss-filer förutom då base- och color-filerna. Anledningen till att det i detta fall blev två base-filer är att variablerna för färg används i layout-filerna och därför måste färg laddas in innan dessa. Filerna är ganska lika varandra i övrigt så jag får fundera vidare på om det kan finnas något sätt att spara in på filer här... 

Jag tycker dock detta var ett smidigt sätt att arbeta med uppgiften - det var lätt att ändra färger mellan mina teman när de variablerna ligger i en enskild fil. De båda varianterna får också samma layout vilket jag tycker är bra.

I det mörka temat kollade jag också upp ett monokromt färgschema utifrån footer-färgen (#2e1334) och hittade där en ljusare nyans (#712f80) för mina analys- och rapportrutor. I övrigt behöll jag i stort sett samma färger men jag dämpade de vita färgerna i rubrikerna något genom att göra dem mer genomskinliga och de vanliga länkarna genom att öka på värdet i funktionen darken() som jag redan använde för dem. Jag lade också filter på mina bilder på mig själv utifrån guiden på [CSS-tricks](https://css-tricks.com/a-complete-guide-to-dark-mode-on-the-web/) däremot lade jag inga filter på bilderna eller tabellerna i analys eller rapportdelarna eftersom jag vill att färgerna där ska framstå som de verkligen är.

### Typografi
Jag valde faktiskt att behålla min typografi. Jag gillar Roboto och Open sans och tycker de passar väl med mina ganska enkla och okomplicerade teman. Jag tycker också att radhöjd, teckenavstånd och den vänsterjusterade brödtexten fungerar bra med de två teman jag utformat.

### TIL
Min TIL får bli att jag har lärt mig att använda verktyg för att hitta och analysera färgscheman (eller i alla fall börjat lära mig). Detta med färg är något jag tycker är svårt och nu känns det som att jag har verktyg som kan underlätta för mig framöver.