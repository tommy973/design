---
Title: Design principles
Description: Analysis of design principles.
Template: analysis
---

Designanalys
=======================


Uppgiften hör till Kmom06 i kurser *Design* och handlar om att analysera andra personers webbsidor (personsidor) och försöka identifiera olika designprinciper.


###Urval

Jag har valt tre webbsidor för personer inom olika områden. Det handlar om komikern Jesper Rönndahl, artisten Alanis Morisette samt datorpionjären och filantropen Bill Gates.

###Metod

För att analysera webbsidorna använder jag material från kursen för att se om det finns några tydliga delar som lutar mot någon designprincip. Som jämförelse använder jag till stor del webbsidan *Design elements and priciples*. För att plocka fram vilket eller vilka typsnitt som används och även titta närmare på koden bakom sidan så använder jag Firefox inbyggda **Inspect**-funktion.

###Resultat och analys

#####jesperronndahl.se
<div class="embed-document">
    <a href="http://jesperronndahl.se/index.html"><img src="%base_url%?/image/jr_small.png" class="color-analysis-image" alt="jesperronndahl.se"></a>
</div>
jesperronndahl.se är en webbsida om komikern Jesper Rönndahl.

Syftet med webbplatsen är att visa upp en portfolio med delar av vad Jesper Rönndahl har gjort själv och medverkat i. Det finns också kontaktinformation för vart man ska vända sig för att anlita Rönndahl för föreställning.

Webbsidan har i grunden en design som är väldigt avskalad. Det är en vit bakgrund med svart text. All brödtext använder typsnittet *Courier New* och menyn samt rubrikerna består av bilder där texten ger känslan av att vara handskriven.

Jag upplever att sidan är designad för att likna ett dokument, exempelvis ett brev eller CV, som är skapat med hjälp av en skrivmaskin och som någon sedan har gjort anteckningar på med en tuschpenna. Tuschpennan gör att det blir en lite mer personlig känsla. 

Jag tycker att sidans **komposition** till stor del är bra då den visar tydligt upp budskapet, vilket är att ge en introduktion till vem Rönndahl är och vad han gjort samt olika kontaktvägar. I och med att sidan inte innehåller speciellt mycket överflödiga detaljer så **riktas** användarens öga till det som finns, vilket på startsidan är en bild på Rönndahl, en meny och en kort introduktionstext. Webbsidan är också tydlig med vart användaren är då både menyn och rubriker skiljer sig från mycket från själva brödtexten och därigenom skapar en tydlig **kontrast**. Här skulle jag påstå att det också finns en viss **hierarki** från rubriken, som har en färgglad ton, till brödtexten via menyn som visserligen har samma färg som brödtexten men vars typsnitt liknar rubrikerna. Texten har en bra bredd på runt 90 tecken per rad i desktopläge och ett bra radavstånd. Sidan är uppdelad så att main-elementet täcker 60% av skärmen och är indelad med hjälp av **flex** för att skapa strukturen mellan menyn och sidans innehåll. Dock har det blivit, vad jag tror är ett misstag, på vissa undersidor där rubriken hamnar i ett eget header-element som ligger utanför main-content. Flex gör då att main-content blir smalt och innehållet förflyttar sig till höger på skärmen.

I och med att innehållet tar upp 60% av skärmen så anpassas innehållet till mindre skärmar. Även menyn anpassar sig och blir en ”*hamburger-meny*”.

#####alanis.com
<div class="embed-document">
    <a href="https://alanis.com/"><img src="%base_url%?/image/am_small.png" class="color-analysis-image" alt="alanis.com"></a>
</div>

alanis.com är en webbsida för den Kanadensisk-amerikanska sångerskan och skådespelerskan Alanis Morissette.

Sidan fokuserar på musiken och syftet är att visa upp vad artisten gjort tidigare, i form av exempelvis diskografi, och vad artisten gör just nu. Här finns information om kommande spelningar och turnéer och även möjlighet att köpa biljetter och merchendise.

Webbsidan är uppbyggd av fyra stora block-sektioner som skapar en tydlig struktur på sidan. De fyra delarna har ingen linje mellan varandra utan använder olika färger till bakgrund och innehåll vilket delar upp och visar att det är olika information. Då sidan använder en ljusare grå nyans som bakgrundsbild och en ljusare färg på navigationsmenyn så hamnar användarens fokus **riktas** mot en banner högst upp som har en mörkare grå bakgrund där information om biljetter finns.

**Typsnittet** som används genomgående på sidan är samma typsnitt som används på några av Morissettes skivomslag, vilket kan ses på diskografisidan. På startsidan uppmärksammas ett 25-års jubileum av skivan *Jagged Little Pill* vilken använder samma typsnitt vilket kan vara anledningen till valet av typsnitt. Typsnittet i sig liknar en skrift från en skrivmaskin vilket är lätt att läsa och det är lätt att koppla till sidans innehåll.

Flera av element **repeteras** då tre av de fyra boxarna på förstasidan till stor del innehåller en bakgrundsbild, ett h1-element och ett div-element som fungerar som en knapp. Dessa knappar, tillsammans med flertalet andra element, återkommer på flera av undersidorna. Även typsnittet används genomgående på alla undersidor vilket skapar en enhetlig sida.

Även denna sida är responsiv vad gäller både bilder, text och menyer.

#####gatesnotes.com
<div class="embed-document">
    <a href="https://www.gatesnotes.com/"><img src="%base_url%?/image/bg_small.png" class="color-analysis-image" alt="gatesnotes.com"></a>
</div>

Webbplatsens syfte är dels att fungera som Bill Gates blogg men det finns också historik om Gates både före, under och efter tiden på Microsoft. Sidan innehåller också information om olika organisationer, podcasts med mera som Gates är delaktig i eller intresserad av.

Designen påminner om en nyhetstidning med rubrik och ingress med tillhörande bild vilket är lite olikt en klassisk blogg där varje nytt inlägg hamnar överst i en lodrät riktning.

Webbsidan använder en tydlig struktur och lägger upp allt innehåll enligt lodräta och vågräta rutnät med hjälp av **flex** som gör att allt känns väldigt ordnat och genomtänkt. Webbsidan använder sig av färgkombinationen svart och vit som den alternerar genom att varva svart textfärg mot vit bakgrund och vit bakgrund mot svart textfärg. Detta skapar en tydlig **kontrast** och gör det även väldigt lättläst. Detta i kombination med bilder i lugna färger skapar en behaglig miljö för ögat. Det finns en **balans** i den här sidan både på bredden och på höjden där ytan för artiklarna på höger och vänster sida är jämnt fördelat. Designen ser i stort sett likadan ut på alla undersidor. Typsnitten, färgvalen och fördelningen av yta följer med och skapar en enhetlig webbplats. 

Den undersidan som sticker ut från mängden är *About Bill*, vilket är en sida som handlar just om Bill Gates. Här återges de största milstolparna med hjälp av en lodrät tidslinje. Designen här frångår det svartvita färgvalet och blandar in vad som liknar penseldrag med varma färger mot en vit bakgrund. Här får också tidslinjen fungera som en mittlinje där information om varje viktigt årtal fördelas på både vänster och höger halva. Den bidrar så att det blir en asymetrisk balans mellan elementen här. En annan detalj som återfinns här är vissa textstycken som använder sig av CSS-funktionen translate för att skapa en **rörelse** på sidan och som fångar användarens intresse.

#####Sammanfattning
Samtidigt som alla tre sidorna vill berätta om personen bakom så både skiljer de sig från varandra men har även vissa likheter. De har allihop en genomtänkt och enhetlig typografi där samma val av typsnitt återkommer genom hela webbplatsen. Oftast följer också färgvalen med längs hela webbplatsen. De tre sidorna har också en tydlig uppdelning av ytan fast de har valt tre olika sätt. Rönndahls sida är väldigt sparsam med innehåll vilket gör att det blir väldigt tydligt vad som är menyn och vad som är innehållet. Morissette´s webbplats använder olika färger på bakgrunderna för att dela upp ytan medan Gates använder den vita eller svarta bakgrunden för att skapa en *gutter* mellan artiklarna.

Även om den estetiska delen skiljer sig väldigt mycket mellan de tre sidorna så tycker jag att designen lämpar sig för webbplatsens syfte och kanske på något sätt också återspeglar en del av den roll som man vill förmedla. Alla tre är innehållsmässigt genomtänkta och det är lätt att navigera sig mellan sidorna och till det användaren söker.

#####Analys av egen sida
<div class="embed-document">
    <img src="%base_url%?/image/tj_small.png" class="color-analysis-image" alt="Tommys portfolio">
</div>
Webbplatsen använder genomgående en dämpad ljusgrön bakgrundsfärg med en svart färg på all text och ikoner. Det finns två stycken bilder på förstasidan som består av en glad smiley som är handritad på rutat papper. Det finns också en titelbild som visar upp några rader av handskriven HTML-kod. Då detta är en sida som hör till en kurs i Webdesign så är titelbilden mer lämpad till området än den ritade presentationsbilden.

Sidans innehåll är indelat med hjälp av raka linjer som avgränsar menyn i headern från innehållet. Längre ner så är även footern avgränsad med linjer och i sin tur indelad i två delar. De fyra typsnitten som är valda skapar en bra läsbarhet men det är aningen för breda textstycken, runt 120 istället för runt 80-90. Största delarna på sidan är uppbyggda med flex för att fördela webbsidans yta för de olika elementen. All design återkommer på de flesta undersidorna. Sidan innehåller en ganska enkel design och har en grön lugnande bakgrundsfärg.

Efter att ha gjort undersökningen så ser jag några olika tips på design som jag skulle kunna använda på min portfoliosida. Jag har testat att bygga upp sidan utan linjer och istället dela upp sidan i block med hjälp av färger. Här utgick jag från min gröna färg som jag hade från början och behöll den på header och footer medans jag bytte på main-content. Jag använde mig av Adobe Colorwheel för att få en färg som matchade den gröna. Det skulle gå att få en tydligare gränsdragning med andra färgkombinationer men jag tyckte båda färgerna var trevliga för ögat att läsa från så det får vara dessa.
Med tanke på att läsa så valde jag också att minska antalet tecken på varje rad där det finns mycket text. 

###Referenser

* Design elements and priciples: https://www.canva.com/learn/design-elements-principles/ (2024-01-31)

* Beaird, J., Walker, A., & George, J. (2020). The Principles of Beautiful Web Design.

* Föreläsningar i kursen *"Teknisk webbdesign och användbarhet"*

###Övrigt

Tommy Johannesson


