# Proof of Concept (POC)

Hoofdvraag: 
Hoe kunnen we de app MisofoMe beter integreren in het dagelijks leven van mensen met misofonie?

Technische deelvragen:
- Is het haalbaar om de hele app binnen de daarvoor beschikbare tijd te prototypen in Framer? 
- Hoe kunnen we ons ontwerp in Sketch structureren, zodat we het overzicht bewaren en het goed overdraagbaar is en interactief gemaakt kan worden in Framer?
- Hoe kunnen we beginnende gebruikers helpen de app snel te leren begrijpen, zodat ze meteen weten wat er mogelijk is en ze direct een goede introductie krijgen?

Technische leerdoelen:
- Goed en vloeiend werkend prototype maken in Framer, voor zover dat haalbaar is binnen de beschikbare tijd.
- Basis van Framer goed begrijpen en het leerproces gestructureerd aanpakken. 
- Ontwerpen in Sketch goed leren structureren, zodat het goed te gebruiken is in Framer. 

Inleiding:
De technische deelvraag die ik in mijn Proof of Concept ga onderzoeken is:
"Hoe kunnen we ons ontwerp in Sketch structureren, zodat we het overzicht bewaren en het goed overdraagbaar is en interactief gemaakt kan worden in Framer?"

Ik denk dat deze deelvraag cruciaal is om het haalbaar te maken om onze app binnen de beschikbare tijd te prototypen in Framer, omdat het een project zal worden met veel verschillende schermen en interacties. Daarom is het erg belangrijk om het goed te structureren en het overzicht te behouden. Als we het vanaf het begin goed structureren, zal het makkelijker zijn om de code werkend te krijgen. Dit heb ik zelf regelmatig ervaren bij eerdere projecten waarbij we met code hebben gewerkt. 

Tijdens het onderzoeken van deze deelvraag wil ik meer te weten komen over hoe je je schermontwerpen en alle elementen op het scherm op een goede manier kan structureren. Ik ga onderzoeken hoe we het overzicht kunnen bewaren en hoop handige tips en adviezen te vinden over het goed en gestructureerd ontwikkelen van een Framer prototype. Hiermee wil ik de kans vergroten dat we in de beschikbare tijd ons prototype in Framer kunnen maken en daarmee de haalbaarheid (zie deelvraag 1) vergroten.

Onderzoeksplan:
Om mijn technische deelvraag te kunnen beantwoorden, ga ik desk research doen. Ik ga video's bekijken en artikelen lezen over het structureren van Sketch bestanden en de overdracht naar een interactief prototype in Framer. Daarnaast bekijk ik op de website https://framerjs.com de informatie in "Get Started" en in de gallerij kan ik voorbeelden bekijken. 

Resultaten: 

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

Conclusie:
Het is erg belangrijk om alles wat je interactief wilt maken in Sketch in een groep te plaatsen met een duidelijke naam, zonder punten en spaties erin. Door vanaf het begin al met Framer te werken, is het makkelijker om je prototype pop te bouwen en het overzicht te bewaren. Daarnaast is het erg belangrijk om comments te gebruiken in je code, zodat jij en de andere mensen die de code bekijken, begrijpen wat er staat. Er zijn veel voorbeelden te vinden over hoe je bepaalde interacties of animaties kan gebruiken in een prototype en als je deze voorbeelden en tutorial video's bekijkt, krijg je een steeds beter beeld van wat er allemaal mogelijk is in Framer en hoe je dat kan aanpakken. 

Bronnen:
- C. Deets. Framer & Sketch: An Intentional Workflow. https://medium.com/facebook-design/framer-sketch-an-intentional-workflow-f91ee2ee1cc1#.obgt1b8if
- E. Corcoran. Getting started Prototyping with Sketch & Framer Studio. https://medium.com/@MentallyFriendly/getting-started-prototyping-with-sketch-framer-studio-60636bc42690#.uykxqxtcu
- Framer. Get Started. Sketch Import. https://framerjs.com/getstarted/import/
- Framer js Tutorials - Framer Studio Basic Tutorial - Framer js - UX Hacker. https://www.youtube.com/watch?v=oM9MScfYxYw
- N. Baskanderi. Sketch tips for Framer.js. How to smoothly import Sketch files into Framer. https://medium.com/sketch-app-sources/sketch-tips-for-framer-js-73b579332993#.orgalaav3
- R. Conde. Prototyping with Framer, part 1. https://www.sketchcasts.net/episodes/prototyping-with-framer-part-1
- R. Conde. Prototyping with Framer, part 2. https://www.sketchcasts.net/episodes/prototyping-with-framer-part-2
- R. Conde. Prototyping with Framer, part 3. https://www.sketchcasts.net/episodes/prototyping-with-framer-part-3

