# Proof of Concept (POC)

Hoofdvraag: 

Hoe kunnen we de app MisofoMe beter integreren in het dagelijks leven van mensen met misofonie?

# Technische deelvragen:
- Is het haalbaar om de hele app binnen de daarvoor beschikbare tijd te prototypen in Framer? 
- Hoe kunnen we ons ontwerp in Sketch structureren, zodat we het overzicht bewaren en het goed overdraagbaar is en interactief gemaakt kan worden in Framer?
- Hoe kunnen we beginnende gebruikers helpen de app snel te leren begrijpen, zodat ze meteen weten wat er mogelijk is en ze direct een goede introductie krijgen?

# Technische leerdoelen:
- Goed en vloeiend werkend prototype maken in Framer, voor zover dat haalbaar is binnen de beschikbare tijd.
- Basis van Framer goed begrijpen en het leerproces gestructureerd aanpakken. 
- Ontwerpen in Sketch goed leren structureren, zodat het goed te gebruiken is in Framer. 

# Inleiding:

De technische deelvraag die ik in mijn Proof of Concept ga onderzoeken is:
"Hoe kunnen we ons ontwerp in Sketch structureren, zodat we het overzicht bewaren en het goed overdraagbaar is en interactief gemaakt kan worden in Framer?"

Ik denk dat deze deelvraag cruciaal is om het haalbaar te maken om onze app binnen de beschikbare tijd te prototypen in Framer, omdat het een project zal worden met veel verschillende schermen en interacties. Daarom is het erg belangrijk om het goed te structureren en het overzicht te behouden. Als we het vanaf het begin goed structureren, zal het makkelijker zijn om de code werkend te krijgen. Dit heb ik zelf regelmatig ervaren bij eerdere projecten waarbij we met code hebben gewerkt. 

Tijdens het onderzoeken van deze deelvraag wil ik meer te weten komen over hoe je je schermontwerpen en alle elementen op het scherm op een goede manier kan structureren. Ik ga onderzoeken hoe we het overzicht kunnen bewaren en hoop handige tips en adviezen te vinden over het goed en gestructureerd ontwikkelen van een Framer prototype. Hiermee wil ik de kans vergroten dat we in de beschikbare tijd ons prototype in Framer kunnen maken en daarmee de haalbaarheid (zie deelvraag 1) vergroten.

# Onderzoeksplan:

Om mijn technische deelvraag te kunnen beantwoorden, ga ik desk research doen. Ik ga video's bekijken en artikelen lezen over het structureren van Sketch bestanden en de overdracht naar een interactief prototype in Framer. Daarnaast bekijk ik op de website https://framerjs.com de informatie in "Get Started" en in de gallerij kan ik voorbeelden bekijken. 

# Resultaten: 

Tips voor structureren in Sketch:
- Gebruik geen spaties en punten in de namen van je artboards en lagen, want dat kan problemen opleveren met de syntax van de Framer Coffeescript. Gebruik daarom camelCase of names_with_underscores.
- Gebruik specifieke namen om verwarring te voorkomen. 
- Als je een Sketch bestand in Framer importeert, is het alleen mogelijk om groepen aan te spreken. Alle lagen die je wilt animeren of interactief wilt maken, moet je daarom in een aparte groep in Sketch plaatsen.
- In Framer kan je geen tekst van kleur veranderen of lagen vervormen, dus dat moet je in gedachte houden bij het maken van je schermen in Sketch.

Tips voor overzicht in Framer:
- Gebruik variabelen als je de waarde meerdere keren in de code gebruikt, zodat je een aanpassing maar 1 keer hoeft in te typen.
- Gebruik comments in je code om het voor jezelf en voor anderen die de code willen lezen of aanpassen begrijpelijk is.
- Ga op en neer van je Sketch file naar je Framer prototype en bouw zo stap voor stap verder aan je prototype. Zo zie je meteen resultaat en is het nog wat overzichtelijker in Framer, omdat er nog minder Sketch groepen zijn.
- Sketch group = Framer layer & Sketch subgroups = Framer subLayer
- Schrijf eerst alles wat het prototype moet doen in normale tekst uit en geef hierbij aan of je te maken hebt met een user interactie of met een interface actie of animatie. Voorbeeld: Tap icon (user action) to open app to main view (zoom animation), vards load in (loading animation) enz. De user actions worden de action events en de interface acties worden de animaties. 

Framer tips:
- Children groepen in een groep kan je direct aanspreken door de sketchnaam.groep aan te spreken.
- Alle lagen selecteren door: for name, layer of sketchnaam
- Let op: Lagen moeten in Sketch gepositioneerd zijn op 0,0, zodat ze in Framer in het canvas verschijnen. Daarna 425,0 en 850,0 of 400,0 en 800,0 Relatief aan de eerste.
- De app Frames of Frameless kun je gebruiken om je prototype op een device te gebruiken, ook zonder internet connectie. 
- deviceWidth = Framer.Device.screen.width en dit kan ook voor height.
- Gebruik print "..." om te testen of een event werkt.

# Conclusie:

Het is erg belangrijk om alles wat je interactief wilt maken in Sketch in een groep te plaatsen met een duidelijke naam, zonder punten en spaties erin. Door vanaf het begin al met Framer te werken, is het makkelijker om je prototype op te bouwen en het overzicht te bewaren. Daarnaast is het erg belangrijk om comments te gebruiken in je code, zodat jij en de andere mensen die de code bekijken, begrijpen wat er staat. Er zijn veel voorbeelden te vinden over hoe je bepaalde interacties of animaties kan gebruiken in een prototype en als je deze voorbeelden en tutorial video's bekijkt, krijg je een steeds beter beeld van wat er allemaal mogelijk is in Framer en hoe je dat kan aanpakken. 

# Bronnen:
- C. Deets. Framer & Sketch: An Intentional Workflow. https://medium.com/facebook-design/framer-sketch-an-intentional-workflow-f91ee2ee1cc1#.obgt1b8if
- E. Corcoran. Getting started Prototyping with Sketch & Framer Studio. https://medium.com/@MentallyFriendly/getting-started-prototyping-with-sketch-framer-studio-60636bc42690#.uykxqxtcu
- Framer. Get Started. Sketch Import. https://framerjs.com/getstarted/import/
- Framer js Tutorials - Framer Studio Basic Tutorial - Framer js - UX Hacker. https://www.youtube.com/watch?v=oM9MScfYxYw
- N. Baskanderi. Sketch tips for Framer.js. How to smoothly import Sketch files into Framer. https://medium.com/sketch-app-sources/sketch-tips-for-framer-js-73b579332993#.orgalaav3
- R. Conde. Prototyping with Framer, part 1. https://www.sketchcasts.net/episodes/prototyping-with-framer-part-1
- R. Conde. Prototyping with Framer, part 2. https://www.sketchcasts.net/episodes/prototyping-with-framer-part-2
- R. Conde. Prototyping with Framer, part 3. https://www.sketchcasts.net/episodes/prototyping-with-framer-part-3

# Tentamenvragen:
- Waarom is het belangrijk om comments in je code te gebruiken? Geef twee redenen.
Antwoord: 1. Door comments toe te voegen, behoud je zelf het overzicht in de code en kan je snel dingen terugvinden. Als je op een later moment verder gaat met je code begrijp je al snel hoe het ook al weer is opgebouwd. 2. Door comments toe te voegen, kun je je werk beter overdragen aan iemand anders en kun je beter samenwerken. Door comments begrijpen anderen je code eerder.
Bron: Framer Workshop
- Waarom kun je beter geen punt (.) gebruiken in een naam voor een map in Sketch als je deze later in Framer wilt gebruiken?  Noem twee geschikte manieren van naamgeving.
Antwoord: Als je een . gebruikt, kan dat problemen opleveren met de syntax in Framer. Wat wel goede manieren zijn om je mappen een naam te geven: camelCase en names_with_underscores. Bron: https://medium.com/@MentallyFriendly/getting-started-prototyping-with-sketch-framer-studio-60636bc42690#.besuqeu5p https://framerjs.com/getstarted/import/

# Reflectie 

Wat heb ik geleerd?
- Ik heb geleerd om Sketch in combinatie met Framer te gebruiken.
- Het is het makkelijkst om zelf je ontwerp in Framer te maken en dit vervolgens om te zetten naar een Framer prototype, omdat je goed moet weten hoe de verschillende lagen heten. Als iemand anders het Sketch bestand maakt, is het veel moeilijker interactief te maken, omdat je eerst voor alle lagen die je interactief wilt maken, moet kijken hoe deze lagen genoemd zijn. Ook al probeer je het nog zo goed te structureren in groepen in Framer, het wordt al snel erg complex. Ik ontdekte dat je met de stateSwitch en events allerlei verschillende interacties kunt maken.
- Ik heb geleerd hoe je kan states aanmaakt en hoe je kan switchen tussen verschillende states om elementen in of uit beeld te zetten, bijvoorbeeld bij een onClick of onSwipe.
- Ik heb geleerd hoe je onderdelen van een pagina scrollbaar kan maken.
- Ook heb ik geleerd hoe je animaties aan kan passen, waardoor er bij het wisselen tussen states een animatie (animate in plaats van stateSwitch) plaatsvindt.

Leerdoelen behaald?
- Goed en vloeiend werkend prototype maken in Framer, voor zover dat haalbaar is binnen de beschikbare tijd.
Ik ben blij met het resultaat van het Framer prototype. Het is nog geen volledig werkend prototype met een vloeiende flow door de bugs hier en daar, maar we hebben wel goed de beoogde werking kunnen tonen aan de klant door de schermvideo's met interacties die ik heb gemaakt. Het was voor mij niet haalbaar om alle bugs eruit te halen en om alle minder relevante interacties werkend te maken, maar in het maken van het prototype is veel tijd gaan zitten. Ik merkte wel dat hert gedurende het project vorderde en het prototoype steeds meer ging werken, het steeds makkelijker werd om te bedenken hoe ik een interactie werkend zou kunnen maken. Echter blijft het best tijdrovend, omdat je voor veel states een nieuw scherm of element moet maken in Sketch. 
- Basis van Framer goed begrijpen en het leerproces gestructureerd aanpakken. 
In het begin heb ik wel wat video tutorials en voorbeelden bekeken. Ik merkte daarbij dat het vaak makkelijk lijkt, maar dat je het dan toch nog helemaal moet vertalen naar je eigen prototype en dat is ingewikkelder dan het lijkt. Daarom ben ik vooral veel zelf gaan proberen en ik merkte dat je er dan toch vaak wel uitkomt, al heeft het vaak wel even tijd nodig. 
- Ontwerpen in Sketch goed leren structureren, zodat het goed te gebruiken is in Framer. 
Ik heb de tips gebruikt die in mijn Proof of Concept onderzoek naar voren kwamen. Zo heb ik steeds goed nagedacht over hoe ik de verschillende groepen zou noemen en heb ik de namen zo veel mogelijk in camelCase geschreven. Ik merkte dat Framer automatisch groepen met dezelfde naam, bijvoorbeeld op verschillende schermen, een nummer geeft. Dit maakte het soms wat ingewikkelder, omdat je daardoor eerst in Framer moest uitzoeken welk nummer het element had gekregen wat je interactief wil maken. Als je een scherm verwijdert in Sketch, verandert de nummering en doen sommige interacties in Framer het opeens niet meer, terwijl het scherm wat je verwijderde een scherm was wat ik niet gebruikte in Framer. Dit kwam door de automatische nummering. Eigenlijk zou je dus alle groepen een eigen naam moeten geven. 

Issues op Github

Ik heb de dingen die nog niet gelukt zijn, aangegeven in de vorm van issues in Github. Zo zien de volgende teams die met het project aan de slag gaan precies waar de bugs en verbeterpunten liggen: 

https://github.com/MerelBakker/Share-Care-Misofonie/issues

Link naar eindrapport en Framer Prototype

https://drive.google.com/drive/folders/0B8dhNqa8u-pMS1YzTTBCZkoyNjA?usp=sharing
https://framer.cloud/pjrVq/


