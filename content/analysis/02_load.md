---
Title: Rapport KMOM05
Description: Rapport om bilder och laddningstid

---

Rapport om bilder och laddningstid
=======================

Syftet med denna rapport är att undersöka bilder och laddningstider på olika webbplatser och utforska vad som påverkar laddningstiden.

Urval
-----------------------

Jag genomförde en sökning på snabba respektive långsamma webbplatser för att identifiera intressanta webbsidor för analys. Urvalet baserades på sökresultaten, där jag valde tre webbplatser som jag redan hade viss kännedom om och som representerar olika typer av prestanda – både snabba och långsamma sidor.

Metod
-----------------------

För att mäta och analysera prestandan använde jag Google PageSpeed Insights och webbläsarens DevTools Network-flik. PageSpeed Insights användes för att få en analys av webbplatsernas prestanda och DevTools Network användes för att mäta laddningstid, antal resurser och webbsidans totala storlek. Varje sida mättes tre gånger för att få ett mer tillförlitligt genomsnittsvärde. Laddningen utfördes genom att använda CTRL + R för att rensa cache och simulera en första hämtning av webbsidan. Samtliga värden dokumenterades i ett Google Kalkylark. Kalkylarket är strukturerat för att visa både enskilda mätningar och beräknade snittvärden för varje sida, vilket ger en överblick av webbplatsernas prestanda.


Resultat
-----------------------

### Resultat

![Wikipedia](../image/kmom05/wikipedia.png)

Webbplatsen **Wikipedia** har den bästa prestandan med ett lågt antal förfrågningar (22), liten mängd överförd data (208 kB) och snabb laddningstid (0,448 sekunder). Dessutom har Wikipedia de högsta PageSpeed-betygen för mobil (91) och näst högsta för desktop (99). Den enkla och avskalade designen, som till största delen består av text och enstaka bilder, bidrar till den höga prestandan och snabba laddningstider. Ett förbättringsområde för att minska filstorlek på bilder skulle vara att konvertera bilder till mer moderna format, såsom WebP samt att anpassa så att bilder inte laddas in i en onödigt stor upplösning. En annan insikt från PageSpeed är att Wikipedia har ett relativt stort DOM-träd med 1 106 element och att HTML-strukturen kan behöva ses över.

![Smashing Magazine](../image/kmom05/smashinmagazine.png)

**Smashing Magazine** hamnar i mitten med fler förfrågningar (117), något mer överförd data (602 kB) och en något längre laddningstid (3,12 sekunder). PageSpeed-betygen blir bäst för desktop (100) och något lägre för mobil (89), vilket ändå visar att webbsidan har god optimering trots mer visuellt innehåll. Det blir kanske också tydligt att webbsidan främst är optimerad för desktop. Förbättringsområden vad gäller webbsidan i mobil kan vara att reducera JavaScript och CSS som inte används samt att förbättra Largest Contentful Paint (LCP), vilket representerar tiden från att sidan laddas till det största synliga innehållselement visas för användaren.

![Reddit](../image/kmom05/reddit.png)

Webbplatsen **Reddit** presterar sämst med högst antal förfrågningar (287), betydligt mer överförd data (2890 kB) och en mycket längre laddningstid (31,13 sekunder). PageSpeed-betyg är låga både för mobil (51) och desktop (62), vilket tyder på bristande optimering och behov av förbättringar för en snabbare användarupplevelse. Insikter från PageSpeed visar att DOM-trädet är komplext med 5 059 element vilket kan påverka prestandan. Andra förbättringsområden kan vara att reducera och optimera JavaScript, bilder och CSS. Överlag innehåller Reddit många bilder och mycket innehåll vilket påverkar prestandan.

---

<iframe width="100%" height="300" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSuRz0cDHQSbCpKy7TqEHd1IWHyKMzSK2T0loQ07__v7sMLelU-b3G6FOBPCmDhZQVunmkbQ-Js61kg/pubhtml?gid=1398884053&amp;single=true&amp;widget=true&amp;headers=false"></iframe>

Sammanfattningsvis är **Wikipedia** klart överlägsen i prestanda, men webbsidans avskalade design är kanske mindre intressant jämfört med **Smashing Magazine**, som balanserar innehåll och optimering väl och skapar en mer visuellt intressant webbsida. **Reddit** å andra sidan hamnar lågt i betyg och har stora behov av förbättring.

Återkommande förbättringsområden för de analyserade webbplatserna inkluderar bilder, där optimering kan ske genom att använda moderna format som WebP och anpassa bildstorlekar för att undvika onödigt stora filer. Även JavaScript och CSS behöver ofta reduceras och komprimeras för att förbättra webbsidans laddningstid. Ett annat återkommande område är DOM-trädet, där förenkling av HTML-strukturen kan minska antalet element och förbättra webbsidans prestanda.

En snabb laddningstid är självklart något att sträva efter, och **Wikipedia** visar verkligen hur det kan göras med sin avskalade design och laddningstid på under en sekund. Sidan innehåller massor av information och är effektiv för sitt syfte, men ärligt talat är den inte särskilt rolig. Om poängen med en webbsida är att vara mer tilltalande och engagerande, behövs visuellt innehåll som gör sidan intressant att besöka. Visst kan det innebära en något längre laddningstid, men det handlar om att hitta rätt balans mellan snabbhet och en engagerande användarupplevelse.

Utifrån de webbsidor jag har analyserat kan jag uppleva att **Reddit** är långsamt, segt och påverkar användarupplevelsen medan jag inte upplever riktigt detsamma med **Smashing Magazine** och absolut inte med Wikipedia. Samtidigt kanske det är rimligt att en webbsida med mer innehåll tar lite längre tid, men utifrån de webbsidor jag studerat skulle jag säga att en absolut gräns för en långsam webbsida går när laddningstiden överstiger omkring 3 sekunder. Jag kan se att **Smashing Magazine** skulle kunna vara något snabbare för en bättre användarupplevelse.

Övrigt
-----------------------

Författare till denna rapport är Jessica Ragnar.
2024-11-26
