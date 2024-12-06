---
Title: Load
Description: This is our load page.
Template: analysis
---

Utvärdering av webbplatsers laddningstid.
=======================

Skriv en eller två rader om vad uppgiften handlar om.

Urval
-----------------------

Jag har valt tre olika video-streamingtjänst hemsidor med variande populäritet. <a href="twitch.tv">Twitch</a>, <a href="youtube.com">Youtube</a> och <a href="dailymotion">Dailymotion</a>.
För varje hemsida väljs 3 sidor för granskning.

Metod
-----------------------

Jag använder mig av devtools i google chrome för att mäta laddningstiden på hemsidorna. För mätning av prestandan har jag använt <a href="https://pagespeed.web.dev/">PageSpeed</a>.



<div class="embed-spreadsheet">
<iframe style="width: 100%; height: 275px; max-width: 830px;" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vT0mqIz4cqkmsve9kMhyKRPJEMfCZQcfXtYt2sgvjlyCADaAqMJ4ygF_uUx9QZQ-Ku6rbkDll1H64v5/pubhtml?widget=true&amp;headers=false"></iframe>
</div>
Resultat
-----------------------


### Youtube
![youtube](%assets_url%/img/youtube.jpg) {.bild}

Mest populära av de tre hemsidorna präglas också med sämsta laddningstiden. För sin usla laddningstid får den ett lågt prestandabetyg ~40. Enligt PSI hade en optimering av Javascript gett 3 sekunder snabbare laddningstid. Vilket hade varit väldigt stor förbättring.



### Twitch
![twitch](%assets_url%/img/twitch.jpg) {.bild}

Twitch har väldigt usla prestandabetyg trots sin märkbara snabbhet jämfört med Youtube. Javascripted väger tungt på Twitch, med enligt PSI 5,5s laddningsstid. Med ett onödigt stort DOM-träd så får får webbsidan ett väldigt lågt betyg både på mobil och desktop.

### Dailymotion
![dailymotion](%assets_url%/img/dailymotion.jpg) {.bild}

Dailymotion vinner stort i prestanda och laddningstider. Det är väldigt märkbart när man surfar på sidan att den är väldigt snabb. Som de andra sidorna klagar PSI på ett onödigt stort DOM-träd, men med detta så lyckas hemsidan ändå leverara en smidig användarupplevelse.


Analys
----------------

Gemensamt för de 3 sajterna är storleken på DOM-trädet. Ett stort DOM-träd innebär fler element för webbläsaren att rendera, vilket kan leda till längre laddningstider och sämre prestanda. 

Laddningstiderna varierar dock kraftigt mellan sajterna, där Dailymotion tydligt har optimerat sina resurser bättre än både YouTube och Twitch, trots liknande utmaningar med komplexiteten i sidstrukturen. 

JavaScript spelar en avgörande roll för prestandan på alla tre sajterna, där både YouTube och Twitch belastas av ineffektivt hanterad kod, medan Dailymotion verkar ha implementerat mer optimerade lösningar för att minimera påverkan på laddningstiderna.

________________________________________________________




Vincent Persson