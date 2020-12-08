Laddningstid och användbarhet
=======================

Under denna undersökning ska tre olika webbplatser testas för hur snabbt dem laddas och om dem innehåller några saker som kan förbättras med tanke på användbarhet och laddningstid.

Urval
-----------------------

[Zalando](https://www.zalando.se/), [Asos](https://www.asos.com/se/kvinna/) och [Sportamore](https://www.sportamore.com/se)

Jag har valt att undersöka tre olika webbplatser som säljer kläder då jag själv varit inne på dessa sidor på sistone.

Metod
-----------------------

Pagespeed Insights används för att analysera data som sidans hastighet och tips om vad man kan förbättra med hemsidan för att få den att bli snabbare. Jag använder mig även av devtools där data kan hittas på diverse webbplatser.

Resultat
-----------------------

<h3>Asos</h3>

<div class="report-img">
<img src="../assets/img/asos.png">
</div>

[Asos Pagespeed Insights](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fwww.asos.com%2Fse%2F&tab=desktop)

När Asos hemsida körs i Pagespeed insights får hemsidan 60 av 100 i resultat och mobilversionen får 21 av 100. Detta betyder att hemsidan och mobilsidan inte klarar testet. För att de ska få bättre resultat så behöver dem radera oanvänd javascript. Pagespeed Insights[[1]](https://developers.google.com/speed/docs/insights/BlockingJS) menar att när en hemsida körs igenom så behöver den "stanna" upp för javascript och om koden inte är nödvändig då tar det mer tid för sidan att laddas. De anser att ungefär 0.59 sekunder i laddningstid skulle sparas på hemsidan och 2.76 sekunder på mobilsidan.

När man kollar i devtools är antalet resurser som laddas ner 4,4MB, laddningstiden på sidan är 1,06s och 109 requests.




<h3>Zalando</h3>

<div class="report-img">
<img src="../assets/img/zalando.png">
</div>

[Zalando Pagespeed Insights](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fwww.zalando.se%2F&tab=desktop)

Zalando fick 80 av 100 i resultat och 22 av 100 på mobilversionen. Detta betyder att Zalando inte klarade testet enligt Pagespeed Insights. För att klara testet skulle de behöva bland annat skala ner bilderna på sidan. Det skulle spara dem ungefär 0.91 sekunder och då skulle man även spara data.

När devtools kollas så är antalet resurser som laddas ner 5,2MB, 261 requests och sidan laddas in på 651ms. 

Enligt Pagespeed insights[[2]](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fwww.zalando.se%2F&tab=desktop) skulle hemsidan laddas in snabbare om Zalando skala ner bilderna på hemsidan. Det skulle spara ungefär 0.91 sekunder. Man skulle kunna försöka göra bilderna mer responsiva och komprimera bilderna. Zalando skulle även spara tid och data på att radera oanvänt javascript.



<h3>Sportamore</h3>

<div class="report-img">
<img src="../assets/img/sportamore.png">
</div>

[Sportamore Pagespeed Insights](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fwww.sportamore.com%2Fse&tab=desktop)

Sportamore fick 46 av 100 och mobilversionen 21 av 100 poäng. Även Sportamore klarar då alltså inte testet enligt Pagespeed Insights. För att de ska förbättra deras hemsida så skulle de behöva bland annat komprimera deras bilder. De skulle ungefär spara 0.9 sekunder i laddningstid. Web.dev[[3]](https://web.dev/uses-webp-images/?utm_source=lighthouse&utm_medium=unknown) anser att använda sig av JPEG 2000, JPEG XR eller Webp som bildformat.  Sportamore skulle även också behöva radera oanvänt javascript.
Resurerna som laddas ner är 31MB, 178 requests och sidan laddar in på 1,86s. 




Analys
-----------------------

Zalando, Asos, och Sportamore är hemsidor som säljer kläder vilket betyder att det är mer vanligt att man har många bilder för att visualisera det man säljer därav storleken på hemsidorna. Sportamore har mest bilder på deras startsida och det visar sig i resultatet då hemsidan är 31MB stor. De har även en video på startsidan som också tar upp mycket data.


Zalando och Sportamore skulle behöva komprimera deras bilder och skala ner dem för att spara data och laddningstid. Det kan dem göra genom att formatera om deras bilder genom att använda sig av JPEG 2000, JPEG XR eller Webp enligt Web.dev[[4]](https://web.dev/uses-webp-images/?utm_source=lighthouse&utm_medium=unknown).


Hemsidorna presterar inte bra på mobilversionen men det är inte så konstigt då Zalando och Asos har egna appar som är först och främst till för de kunder som handlar ofta hos dem men också för att apparna oftast är snabbare. Mobilversionen av sidan kommer alltid att finnas där och vara utvecklad, men fokuset är nog mer riktat mot deras appar. 

<!-- Om en hemsida har stor data som användaren måste ladda in betyder att man kommer använda sig av mer internet och om personen sitter på en mobil tex kommer det kosta mer för användaren att vara inne på hemsidan.
Desto större storlek på hemsidan desto mer "pengar" kostar sidan för användaren. -->

<h3> Mitt test </h3>
<div class="report-img">
<img src="../assets/img/table.png">
</div>

När jag utsåg en vinnare för detta test så kollade jag på Pagespeed Insights totala resultat, devtool requests, speed result, och resources. Den hemsidan som fick bäst resultat vann. Det blev en delad 1: a plats. Det var lite svårt att utse en vinnare då ingen hemsida klarade Page speed insights testet, varken på mobilversionen eller på dator. Asos kunde ha haft bättre laddningstid eller bättre poäng i det totala resultatet som Page speed Insights gav och då hade de vunnit mitt test!

<h3> Vinnare i testet:</h3> 

1: a plats Zalando & Asos

2: a plats: Sportamore.com/se

<h3> Min gräns för absolut laddningstid: </h3>

Jag testade mig runt på olika hemsidor för att se om det var en sida jag kände laddade långsamt och den tiden jag märkte av mest var över 2.5 sekunder. Om en sida laddas in på över 2.5 sekunder skulle jag uppfatta som en långsam webbplats. Det betyder då att de webbplatser jag valt ut har klarat mitt gränsvärde. Rent generellt skulle jag säga att man känner av att Sportamore är långsammare än dem andra två men det är nog för att dem använder sig av en video på startsidan och den tar längre tid att ladda in. Annars klarar dem sig bra!

Referenser
-----------------------
[1 Blocking Js](https://developers.google.com/speed/docs/insights/BlockingJS)

[2 Zalando Desktop](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fwww.zalando.se%2F&tab=desktop)

[3 Web.dev](https://web.dev/uses-webp-images/?utm_source=lighthouse&utm_medium=unknown)

[4 Web.dev](https://web.dev/uses-webp-images/?utm_source=lighthouse&utm_medium=unknown)

Övrigt
-----------------------

Rapporten är skriven av Josefine Niirola.
