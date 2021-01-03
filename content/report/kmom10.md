---
Title: Kmom10
Description: Min redovisning för kmom10
Template: kmom
---

## Kmom10
Här kommer snart min rapport för kmom10 och projektet

Skapa en ny webbplats till din kund i katalogen me/kmom10 i kursrepot.

Du kan välja mellan att använda din me/portfolio som grund eller börja ifrån grunden med en helt ny installation från example/portfolio. Välj väg och glöm inte redigera filen .htaccess.

Beskriv i redovisningstexten hur du gör och varför du valde det sättet.

Kunden vill givetvis att sidan skall fungera bra för alla grupper av intressenter och betonar därför att sidan skall se bra ut på en mobil och att sidan ska ha bra tillgänglighet (accessibility).

Berätta i din redovisningstext hur du har åstadkommit två nedanstående krav och vilka delar du har valt att fokusera på inom responsivitet och tillgänglighet.
Responsivitet

Sidan skall använda CSS-grid och/eller flexbox för att presentera innehållet på ett främjande sätt.

Sidan skall fungera väl på mobila enheter, dvs inga horisontella scrollbars.

Bilder ska anpassas efter enhet med hjälp utav cimage och <picture>/srcset.
Tillgänglighet

Samtliga sidor på sidan skall ha 100 i “accessibility” enligt Lighthouse (via devtools).
Vid genomgång hittades följande problem för tillgängligheten i Lighthouse:

Hem: 
Desktop:
"Focusable descendents within an `[aria-hidden="true"]` element prevent those interactive elements from being available to users of assistive technologies like screen readers"
element: div.logo
Åtgärd: tog bort länken vid loggan. 

Mobilt: 
Some elements have a [tabindex] value greater than 0
Failing Elements
a#nav-toggle.nav-toggle

Åtgärd: Tog bort tab-index för nav (ändå första elementet)

Inga andra fel har hittats - kolla också sidan i verktyg för color-blind och för kontrast. 


Färgvalet på sidan ska ta färgblindhet i åtanke, ni kan använda Toptal - Colorblind Web Page Filter för att testa er publicerade sida.

På din redovisningssida, skriv följande:

1.1 För varje krav du implementerat, dvs 1-6, skriver du ett textstycke om ca 5-10 meningar där du beskriver vad du gjort och hur du tänkt. Poängsättningen tar sin start i din text så se till att skriva väl för att undvika poängavdrag. Missar du att skriva/dokumentera din lösning så blir det 0 poäng. Du kan inte komplettera en inlämning för att få högre betyg.

1.2 Skriv ett allmänt stycke om hur projektet gick att genomföra. Problem/lösningar/strul/enkelt/svårt/snabbt/lång tid, etc. Var projektet lätt eller svårt? Tog det lång tid? Vad var svårt och vad gick lätt? Var det ett bra och rimligt projekt för denna kursen?

1.3 Avsluta med ett sista stycke med dina tankar om kursen och vad du anser om materialet och handledningen (ca 5-10 meningar). Ge feedback till lärarna och förslå eventuella förbättringsförslag till kommande kurstillfällen. Är du nöjd/missnöjd? Kommer du att rekommendera kursen till dina vänner/kollegor? På en skala 1-10, vilket betyg ger du kursen?