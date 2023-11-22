# Matlab_Project_Rahaf

Perspektivkurs Matlab Project 2048
Cristofer Englund, Pablo del Moral, Eric J¨arpe, Awais Ashfaq Augusti 2021

1	Introduction
V¨alkommen till slutdelen i projektet i Perspectives-kursen d¨ar du kommer att forts¨atta utveckla heuristik f¨or att l¨osa 2048-spelet.
Projektet ¨ar uppdelat i tv˚a delar, d¨ar del 2 ¨ar valfri och riktar sig till de som vill ha en st¨orre utmaning.
Spelet 2048 ¨ar ett spel som spelas p˚a en spelplan som ¨ar 4 g˚anger 4 rutor. Styrsignalerna till spelet ¨ar ∈ (↑, ↓, →, ←), dvs pilarna p˚a tangentbordet. Ett f¨orsta exempel visas i figuren 1a och figuren 1b, mellan den f¨orsta och den andra figuren har spelaren tryckt p˚a h¨ogerpilen. De tv˚a tv˚aorna har kombinerats till en fyra och en ny tv˚a kommer fram p˚a spelplanen. Det nya talet som dyker upp vid varje f¨orflyttning ¨ar antigen en tv˚aa (90%) eller en fyra(10%) (ur orginalkoden f¨or 2048: var value = Math.random() < 0.9 ? 2 : 4;). M˚alet med spelet ¨ar att kombinera talen och bilda 2048. F¨or att prova 2048 kan man kan spela i en browser p˚a. git1
Att spela 2048 ¨ar p˚a ett s¨att en enkel uppgift, vi har bara fyra m¨ojliga styrsignaler (pilarna) och en begr¨ansad spelplan och tydliga regler. Samtidigt kr¨aver det en strategi och en f¨orm˚aga att organisera talen spatialt (i rummet). Fel drag vid fel tillf¨alle eller de nya talet (tv˚aan eller fyran) dyker upp p˚a fel st¨alle leder till problem som ¨ar sv˚ara att fixa. Som ett exempel se:  https:
//sztupy.github.io/2048-Hard/. Tidigare har datorer framg˚angsrikt anv¨ants f¨or komplicerade spel som schack2 eller med mer information p˚a engelska3). Andra spel som haft stor p˚averkan ¨ar backgammon4 F¨or att ˚aterg˚a till 2048. Det ¨ar relativt l¨att att skriva ett program som spelar 2048.

2	Varianter av 2048
Naturligtvis kan man ¨andra grundversionen p˚a innovativa s¨att.

1http://git.io/2048 2http://sv.wikipedia.org/wiki/Deep Blue
3http://en.wikipedia.org/wiki/Deep Blue %28chess computer%29
4http://www.bkgm.com/ articles/tesauro/tdl.html
 


2.1	L¨angre ¨an 2048 - max po¨ang
Genom att inte stanna p˚a n¨ar den h¨osta brickan ¨ar 2048 kan man unders¨oka hur h¨og po¨ang man kan f˚a.

2.2	2048 med minst antal drag
Genom att framf¨orallt optimera slutspelet kan man f¨ors¨oka hitta s¨att att n˚a 2048 genom s˚a f˚a drag som m¨ojligt.

2.3	Flest po¨ang under en viss tid
Genom att s¨atta en begr¨ansning i tid kan man se vem som har f˚att flest po¨ang under en viss tid. Strategien h¨ar kan vara annan ¨an f¨or varianter som s¨oker max po¨ang.

2.4	2048 p˚a minst klocktid
Genom att m¨ata tiden fr˚an spelstart till 2048 kan man m¨ata effektiviteten hos en l¨osning.

3	Slumpen
Det ¨ar slumpmomentet som g¨or spelet utmanade, om det ¨ar en tv˚aa eller en fyra samt placeringen av dem. Slumpen g¨or att resultatet kommer att bli olika i tv˚a olika k¨orningar. D¨arf¨or ¨ar det viktigt att n¨ar man j¨amf¨or:
1.	anv¨ander samma slumptal (seed)
2.	att utv¨ardera ¨over flera utfall, det vill s¨aga kanske 100 k¨orningar.

4	Del 1
Del 1 riktar sig till de studenter som tycker programmeringen ¨ar sv˚ar och som k¨anner att utmaningen blir f¨or stor. Till er blir uppgiften att anv¨anda de agenter (AI) som du utvecklade i Lab 3. Du ska i detalj beskriva samtliga rader som din AI exekverar (i t.ex. myAIx). Du ska simulera igen och visa med statistiska metoder att det finns en skillnad i prestanda mellan de olika AIna, den som du f˚att (t.ex. myAI4) och j¨amf¨or med den du utvecklade, eller om du vill vidareutveckla h¨ar i projektet. I rapporten skriver du tydligt vad som g¨or att din AI ¨ar b¨attre ¨an tidigare versioner, eller vad som skiljer de olika AIna som du j¨amf¨or.
 


Inl¨amning av projektrapport
En rapport som tydligt beskriver
1.	Namn,
2.	Vilket program och kurs du ¨ar registrerad p˚a,
3.	Koden som du anv¨ant f¨or att skapa resultaten,
4.	Tydliga f¨orklaringnar i koden som beskriver vad som h¨ander i koden p˚a varje rad.
5.	Histogram ¨over po¨angen f¨or simuleringarna,
6.	Resultat fr˚an ttest2 som visar om din ”nya” heuristik ¨ar b¨attre ¨an den du j¨amf¨or med.

5	Del 2
F¨or dig som vill ha en st¨orre utmaning, l¨agg till i rapporten
1.	Ny kod som du anv¨ant f¨or att skapa en ny AI/heuristik.
2.	Tydliga f¨orklaringnar i koden som beskriver vad som h¨ander i den nya koden p˚a varje rad.
3.	Histogram ¨over po¨angen f¨or simuleringarna,
4.	Resultat fr˚an ttest2 som visar om din nya heuristik ¨ar b¨attre ¨an den du j¨amf¨or med.

Checklist
1.	Jag har l¨ast hela instruktionen f¨or projektet
2.	Jag har gjort minst uppgiften i Del 1.
3.	Jag har tydligt f¨orklarat med statistika metoder fr˚an kursen att min ”nya” AI ¨ar b¨attre ¨an den jag j¨amf¨or med.
4.	Jag har s¨akerst¨allt att alla filer som beh¨ovs f¨or att skapa en pdf finns med bland de filer jag laddat upp
5.	Jag har s¨akerst¨allt att de .m filer jag skapat finns med bland de filer jag laddat upp
6.	Jag har s¨akerst¨allt att jag laddat upp en pdf med slutrapporten.
 

6	Sammanfattning
Labbarna tidigare i kursen och de labbbar som ing˚ar i projektet ska ha gett en god bas f¨or att kunna utf¨ora projektet. I projektet ska du f¨ordjupat dina kunskaper i hur man g¨or funktioner i Matlab samt hur man bygger effektiva funktioner som genererar h¨oga po¨ang i spelet 2048.
Du ska kunna anv¨anda statistiska metoder f¨or att argumentera att din metod
¨ar b¨attre ¨an en befintlig. Du ska kunna presentera dina resultat b˚ade skriftligt i en projektrapport samt muntligt inf¨or era klasskamrater.

