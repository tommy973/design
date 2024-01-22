---
Title: Loadingtime
Description: Analysis of loadingtime.
Template: analysis
---

Laddningstid
=======================

Uppgiften hör till Kmom05 i kurser *Design* och handlar om att mäta laddningstider för tre utvalda webbsidor med efterföljande analys utifrån eventuella förbättringsområden.

###Urval

Mitt urval består av de tre största tillverkarna av spelkonsoller och deras hemsidor. Urvalet hamnade på följande sidor:
* https://www.nintendo.se/
* https://www.xbox.com/sv-SE
* https://www.playstation.com/sv-se/

Utifrån dessa tre domäner valde jag att undersöka deras startsida, supportsida och spelsida.


###Metod

Jag använder webbtjänsten **Pagespeed Insights** för att mäta laddningstiden för de olika webbsidorna. Har även använt Google och Firefox inbyggda **Devtools** Sedan sammanställs dessa i ett **Google Kalkylark** för att göra resultatet överskådligt.

###Resultat

#####Nintendo
<div class="embed-document">
    <img src="%base_url%?/image/nintendo_start_small.png" class="color-analysis-image" alt="Nintendo">
</div>

* Startsida: https://www.nintendo.se/
* Spelsida: https://www.nintendo.se/spel
* Supportsida: https://www.nintendo.se/support

#####Xbox
<div class="embed-document">
    <img src="%base_url%?/image/xbox_start_small.png" class="color-analysis-image" alt="Xbox">
</div>

* Startsida: https://www.xbox.com/sv-SE
* Spelsida: https://www.xbox.com/sv-se/games?xr=shellnav
* Supportsida: https://support.xbox.com/sv-SE/

#####Playstation
<div class="embed-document">
    <img src="%base_url%?/image/playstation_start_small.png" class="color-analysis-image" alt="Playstation">
</div>

* Startsida: https://www.playstation.com/sv-se/
* Spelsida: https://www.playstation.com/sv-se/ps5/games/
* Supportsida: https://www.playstation.com/sv-se/support/

#####Laddningstider

<div class="embed-document">
    <iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSqWTRfBvNALsmmNaxTZ4GpRNc1PG7fgRNnmVtmn9IJ2y7HSr7Mptyomc5m5apjNGZUPWotViql-iNF/pubhtml?gid=477722291&amp;single=true&amp;widget=true&amp;headers=false"></iframe>
</div>

###Analys

De tre startsidorna är uppbyggda på liknande sätt. Det är genomgående en fin design där användarens fokus fångas upp med hjälp av bilder på produkter som exempelvis byts ut efter ett visst intervall. De har en spelsida som är till stor del fylld med bilder på olika spel till olika konsoler. Till sist har de en supportsida som oftast är relativt ren från bilder utan använder sig mest av text.

#####Nintendo:
Nintendos startsida använder främst bilder med filändelsen .webp och som har en filstorlek som är relativt blygsam då den största bilden är 257 kB stor. Sidan har dock den längsta laddningstiden på närmare 77 sekunder. Egentligen har sidan en snabbare laddningstid på runt 3-4 sekunder men det enligt Nätverksverktyget så laddas en JavaScript-fil vid några tillfällen och det är därför som laddningstiden drar iväg.
Spelsidan är uppbyggd av flertalet thumbnails för alla spelen som hör till deras senaste konsol. Sidan är designad så att det finns två kolumner med thumbnails som laddas allt eftersom användaren scrollar ner på sidan. Så bilderna laddas inte in direkt i början.
Supportsidan är mer eller mindre enbart text och information. Inga tunga bilder eller filer.

#####Xbox:
Likt Nintendos startsida så har Xbox också ett antal bilder som visar deras produkter på startsidan. Här laddas alla bilder, där de flesta är i jpeg-format och har liknande storlek som Nintendos. Den största är 281 kB och alla bilderna har en tillhörande text som ger lite information. Dock får sidan lägst poäng av de tre på Pagespeed Insights. Exempelvis 4 poäng (mobil) och 43 poäng (desktop) av 100 på prestanda, vad jag kan se på resultatsidan så beror detta till stor del på sidans JavaScript.
Även spelsidan får dåligt betyg på prestanda och vad jag kan se så är det också här JavaScript som belastar. Det finns också några bilder som är aningen större (runt 500 kB) men inga onödigt stora.
På supportsidan finns det ett antal bilder men mestadels information i form av text.

#####Playstation:
Även Playstations startsida har ett antal bilder som visar deras produkter, både spel och merchendise. Sidan har, i sammanhanget, ganska stora filstorlekar dels på bildfilerna, dels på JavaScript och CSS och just bilderna är något som Pagespeed anmärker på. Största bilderna ligger på runt 880 kB, vilket i sig inte är enormt men det skulle nog gå att skala ner lite.
Spelsidan är ganska effektfull med mycket bilder och blandar thumbnails för spel med större bilder och detta gör att filstorleken skjuter iväg. Några bilder ligger över 1 MB. Det är också enda sidan som får ett ! som betyg, och detta kommer från att Pagespeed Insights anser att kontrasten gör att texten kan vara svårläslig.
Supportsidan är ganska avskalad även här och innehåller mestadels information och hänvisningar till olika kategorier av support.

#####Sammanfattning:
Jag tycker att alla tre sidorna har en bra struktur av innehållet. De har alla tre använt väldigt mycket bilder på sina startsidor. Bilder är ju givetvis effektfulla och kan skapa ett intresse på ett annan sätt än text. Till stor del har alla tre även försökt att hålla nere filstorleken genom att välja olika filtyper som ämnar sig bättre för exempelvis bilder som inte är fotografier. Jag tycker att de alla har valt en design och färgval som knyter an till företagets logotyp och som är genomgående på alla startsidor och dess undersidor.

Genomgående i testerna så fick ju ingen av sidorna speciellt bra betyg från tjänsten Pagespeed Insights gällande prestanda. Det var mycket kommentarer om att DOM-trädet var onödigt stort, att det var tunga JavaScript och på några sidor fanns en del JavaScript-kod som inte användes. Angående filstorleken på bilderna så stack Playstations sida ut jämte de andra två med att ha vissa filer på 4 gånger så stor storlek. Här borde det gå att skala ner en del utan att sänka kvalitén på bilden eller ta bort intrycket som bilden ska ge användaren.

Att använda mycket bilder på ”spelsidan” är inget konstigt utan mer en självklarhet för att kunna visa upp speltillverkarens produkter. Xbox laddar hela sidans innehåll från början medan Playstation och Nintendos sidor laddar in materialet allt eftersom användaren scrollar neråt på sidan. Detta borde ju vara mest effektivt och kräva minst datorkraft i och med att om användaren vill titta på en titel som ligger långt upp i listan så behöver inte alla bilder laddas. Även här använder Playstation bilder med mycket större storlek än de andra två. Största filen på Playstations sida ligger på 1 MB som kan jämföras med Xbox 490 kB och Nintendos 75kB. En anledning kan vara att Nintendo Switch inte har möjlighet för lika skarp grafik som Playstation och Xbox, som då behöver använda mer högupplösta bilder för att visa upp sitt material. Men när många filer ska läsas in så är det ju bra att hålla nere filstorleken.

På företagens supportsidor finns inte mycket bilder alls, vilket är logiskt då just den avdelningen på sidan strävar mot att vara tydlig och lättanvänd då användaren oftast är där för att söka information till någon form av problem som uppstått. Här finns mestadels text och det är också de tre sidorna som utan tvekan laddas snabbast.


Utifrån testerna så skulle jag nog säga att Nintendos webbsida är vinnaren bland dessa tre. Den har visserligen en väldigt lång laddningstid på startsidan men den har också de två snabbaste laddningstiderna i fältet. De har även effektiviserat laddningen genom att använda bilder med liten filstorlek men som ändå gör att webbsidan är tilltalande.

Andra- och tredjeplatsen är svårare att bestämma då Xbox har ett fruktansvärt betyg på ”Prestanda” men väldigt bra på ”Tillgänglighet”. Detta medan Playstation har fördelningen tvärtom. På själva laddningstiderna så segrar nog Playstation över Xbox.

Angående laddningstider så skulle jag väl säga att runt 4 sekunder upplevs väl ganska ok. Utifrån mina mätningar är det inte många sidor som klarar den spärren men ändå upplevs sidorna flyta och ladda helt ok.

###Referenser

Beaird, J., Walker, A., & George, J. (2020). The Principles of Beautiful Web Design. 

###Övrigt

Tommy Johannesson
