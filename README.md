## Learning Log
# Model

￼
<details>
  <summary>Sprint 3</summary>

<img width="3619" height="2696" alt="IMG_0580" src="https://github.com/user-attachments/assets/852a0269-f193-46e0-a039-8dc425680646" />
<img width="3492" height="2526" alt="IMG_0578" src="https://github.com/user-attachments/assets/32ae22d0-2b8e-4bf4-a5b5-bd62eac3ccab" />
<img width="3303" height="2482" alt="IMG_0577" src="https://github.com/user-attachments/assets/cec34736-3ac7-4c60-b4b5-5fbba53bfda6" />

Opdracht 1:
Ik heb met mijn schetsen vooral gekeken naar grootte en plaatsing. Bij sommige schetsen wilde ik YMCA meer laten opvallen en bij andere juist het woord fun. Zo probeerde ik meer afwisseling in de tekst te krijgen

Opdracht 2:
Wat wil je bij de kijker bereiken met je vormgeving?:

Dat de tekst interessant en speels overkomt.

Hoe voegt jouw opzet iets toe aan de tekst?:

Door te spelen met grootte, plaatsing en ruimte komt er meer speling in de tekst en valt YMCA meer op.

Welke schets wil je digitaal uitwerken?
De schets waarbij YMCA in het midden staat en de rest van de tekst verdeeld staat in de hoeken. Die vind ik het meest interessant omdat YMCA goed opvalt.

Hoe zou je dit kunnen aanpakken in code?
Door de tekst in HTML op te delen en in CSS te spelen met grootte,regelafstand, letterafstand en de plaatsing van de tekst.

Stap 1:
<img width="2288" height="1156" alt="image" src="https://github.com/user-attachments/assets/e3026c12-fe48-410c-bdf1-b91b37c4a366" />
HTML opzet: Bewust géén klasses en géén divs gebruikt. Elk stukje tekst heeft een semantische betekenis gekregen die past bij de song: `<h1>` voor het refrein, `<em>` voor klemtoon op 'fun', `<strong>` voor 'to stay', en `<p>` voor de verbindende tekstfragmenten. Hierdoor is de HTML zuiver en betekenisvol.

Stap 2:
<img width="2290" height="1606" alt="image" src="https://github.com/user-attachments/assets/b622c847-90b2-4efd-b2af-9a05ac99dcb3" />
<img width="2296" height="1682" alt="image" src="https://github.com/user-attachments/assets/638db9d9-4da2-4e6a-97dd-365f701a5708" />
<img width="2302" height="710" alt="image" src="https://github.com/user-attachments/assets/46d2dc09-ef87-4869-8df9-4f86c2066fb6" />
CSS styling zonder klasses: Elementen direct aangesproken via hun tag (em, strong, h1). Voor de twee paragrafen zijn de logische pseudo-classes :first-of-type en :last-of-type gebruikt. Het 3x3 grid plaatst alles op de posities van de schets: hoeken aan de randen en 'YMCA' gigantisch in het midden. Geen kleur toegepast, uitsluitend macro-typografische contrasten (groot vs. klein, italic vs. rechtop, tracking).

Extra uitleg: Omdat classes geen semantische betekenis hebben, wilde ik ze niet gebruiken. Ik heb de songtekst verdeeld over logische tags: em voor de nadruk op fun, strong voor to stay, en h1 voor het refrein. In CSS hoefde ik daardoor alleen die elementen aan te roepen, plus :first-of-type en :last-of-type voor de eerste en laatste paragraaf. Dat houdt de HTML 100% semantisch en schoon.

Checkout maandag wg 1 sprint 3:  
Vraag 1: Begrippen uit de artikelen

* Kerning: De ruimte tussen twee specifieke letters netjes maken. Soms staan letters als 'T' en 'y' standaard te ver uit elkaar of botsen ze bijna, en met kerning schuif je dat een stukje bij. 
* Tracking: De tussenruimte over een heel woord of een hele regel tegelijk aanpassen. Dit gebruik je vooral bij hoofdletters (kapitalen) om ze wat meer ademruimte te geven zodat het makkelijker leest. 
* Leading: Gewoon de regelafstand, oftewel de ruimte van de ene regel tekst naar de volgende regel eronder. 
* Flush-left: Tekst die strak links begint en aan de rechterkant rafelt (links uitgelijnd). Dit leest het fijnst omdat je ogen links steeds op dezelfde plek beginnen. 
* Flush-right: Tekst die juist strak rechts staat en links rafelt. Leuk voor een klein stukje tekst of een quote, maar voor hele verhalen leest het irritant. 
* Centered: Tekst netjes in het midden uitgelijnd. Staat chic en netjes voor een titelpagina of uitnodiging, maar is drama voor lange lappen tekst. 
* Justified: Uitgevulde tekst die links én rechts kaarsrecht langs de kantlijn loopt, net zoals in een krant. Nadeel is dat er soms gekke witte gaten tussen woorden ontstaan. 
* Indent: Dat het eerste regeltje van een alinea een stukje naar binnen springt om te laten zien dat er een nieuw stukje begint. 
* Outdent: Precies andersom: de eerste regel steekt juist naar links uit buiten de rest van de alinea. 
* Modular scale: Een soort vaste trap van lettergroottes met een vaste rekenformule. Daardoor gok je niet zomaar wat pixels bij elkaar, maar passen alle koppen en teksten logisch bij elkaar. 
* Movable type: De oude manier van drukken met losse loden of houten blokjes letters die je met de hand in een bak zette. Hier komen bijna al onze huidige typografieregels vandaan. 
* Focus punt (Focal point): Het allereerste ding op je scherm waar je oog meteen naartoe getrokken wordt omdat het eruit springt. 
* Vijf soorten contrast: De manieren om zo'n focuspunt te maken: 
    1. Grootte (size): Iets heel groot of juist piepklein maken. 
    2. Kleur (color): Iets feller, lichter of donkerder maken. 
    3. Ruimte (space): Iets helemaal apart zetten met een bak witruimte eromheen. 
    4. Gewicht (weight): Een tekst extra dik (bold) of juist superdun maken. 
    5. Vorm (shape): Een opvallende vorm kiezen, zoals schuin/cursief tegenover strakke rechte letters. 
* Spatial tension: De visuele spanning op je scherm door hoe dingen staan. Als je iets expres niet saai in het midden zet maar juist strak tegen de rand plakt, voelt je ontwerp meteen levendiger. 

Vraag 2: Jouw ideale regellengte (measure) en waarom
Voor gewone tekst vind ik 45 tot 75 tekens per regel (inclusief spaties) het fijnst.
Waarom:
Als regels te lang zijn (meer dan 75 tekens), raken je ogen snel vermoeid en moet je steeds zoeken waar de volgende regel links nou begint. Maar als regels te kort zijn (minder dan 45), vliegen je ogen telkens heen en weer en krijg je superveel afgebroken woorden. Daartussenin leest het gewoon lekker vlot weg.

Vraag 3: Eén variabele voor hiërarchie (en waarom)
Als ik er echt maar één mocht kiezen, ga ik voor Grootte (Size).
Waarom:
Grootte snapt iedereen meteen. Je kijkt altijd instinctief eerst naar het grootste ding op een pagina. Zelfs als je geen kleuren gebruikt en maar één lettertype hebt, kun je puur door het formaat direct laten zien: "dit is de titel en dit zijn de details". Dat zag je ook bij mijn YMCA-schets: doordat YMCA mega groot in beeld staat, weet je meteen waar het over gaat.

Huiswerk voor woensdag (sprint 3, werkgroep 2)
<img width="3024" height="1722" alt="image" src="https://github.com/user-attachments/assets/fd40796d-520a-4661-a5bb-7c42202152a1" />

Ik heb mijn schets als eerste omgezet naar gewone HTML en een beetje basis-CSS. De hele zin heb ik opgeknipt in losse stukjes: p, em, strong en een h1 voor het midden. In de CSS heb ik die woorden naar de vier hoeken geduwd en 'YMCA' flink groot in het midden gezet. Dit is nu de eerste ruwe versie in zwart-wit met het Seraphs lettertype.

Dingen die ik nog niet naar CSS kon vertalen (Huiswerkvraag 2)
- Het schalen van 'YMCA': In mijn schets vult 'YMCA' echt lekker het midden. Maar in de browser met vaste pixels of rems werd het op mobiel meteen veel te groot waardoor de tekst afbrak, en op een groot scherm juist weer te klein. Ik wist nog niet goed hoe ik dit soepel mee kon laten schalen met het scherm.  
- De witruimte en afstanden: De woorden staan nu wel ongeveer in de hoeken, maar de marges heb ik gewoon een beetje op het oog gedaan. Ik weet nog niet hoe je die afstanden echt netjes koppelt aan een vast typografisch ritme of grid.  
- De variabele assen van Seraphs: Op papier hebben woorden als 'fun' en 'to stay' net even een andere vibe. Nu heb ik gewoon standaard em en strong gepakt, maar ik moet nog uitzoeken hoe je die specifieke assen van het Seraphs font aanpast met font-variation-settings.  
- (De spanning uit de schets: Op papier voelt de witruimte tussen het midden en de hoeken een stuk beter. In de browser oogt het nu nog wat stijfjes, vooral omdat het nog niet strak in een goed grid vastzit.)
—————————————————————————————————————————

Opdracht:

1.Bepaal de line-height bij je gekozen font-size
2.Baseer je column-width op een veelvoud van je line-height
3.Kun je daarmee een grid maken dat past bij je  pagina ontwerp, rekening houdend met je measure?
4.Ja? Ga dan verder met bouwen aan je page Nee? Pas line-height en/of font-size aan en ga terug naar 1.

Antwoorden:  
1. Voor de normale tekst heb ik een font-size van 1.25rem (20px) gekozen. Daar heb ik een line-height van 1.5 bij gepakt, wat uit de artikelen ook naar voren kwam als fijne verhouding. Dat betekent dat één regelhoogte bij mij 20px × 1.5 = 30px is. Die 30px is meteen mijn vaste bouwsteen voor de rest van de pagina.
2. Mijn basiseenheid is 30px. Voor de twee buitenste kolommen (waar de woorden in de hoeken in staan) heb ik dat vermenigvuldigd met 5: 5 × 30px = 150px. De middelste kolom heeft gewoon 1fr gekregen, zodat 'YMCA' alle overgebleven ruimte in het midden opeist.
3. Ja, dit werkt heel relaxed. Omdat er in die hoeken maar korte stukjes tekst staan zoals it’s en to stay, passen die letters makkelijk binnen die 150px breedte zonder dat ze raar worden afgebroken.
4. Ik heb die 30px ook direct doorgevoerd in de rest van de pagina: de padding rondom het hele scherm is precies 2 × 30px = 60px. Zo klopt de witruimte overal wiskundig met de regelafstand van de tekst.
<img width="1282" height="260" alt="image" src="https://github.com/user-attachments/assets/3bb3f35c-22c9-49ad-8d28-86c99ed2f2eb" />
<img width="850" height="326" alt="image" src="https://github.com/user-attachments/assets/62210482-6560-4b0b-a2a2-1051b27388d7" />
Hier heb ik het grid gekoppeld aan de typografie. Mijn normale tekst is 20px met een regelafstand van 1.5, wat neerkomt op 30px per regel. In plaats van willekeurige getallen te kiezen, heb ik de zij-kolommen 150px breed gemaakt (5 × die 30px) en de padding rond het scherm 60px (2 × die 30px). De middelste kolom pakt 1fr voor 'YMCA'. Zo klopt de verhouding overal met één vaste ritme-eenheid.

<img width="3024" height="1722" alt="image" src="https://github.com/user-attachments/assets/9cd3f433-e056-4417-87f7-c587abd61e5f" />

Het resultaat in de browser met de grid-overlay aan. Je ziet dat de woorden in de hoeken netjes binnen de berekende kolommen van 150px blijven en 'YMCA' precies in het midden staat. Door clamp() schaalt de grote titel vanzelf mee met het scherm, zonder dat hij uit zijn gridvak breekt.

Checkout woensdag sprint 3 werkgroep 2:  
1. Waarom een grid gebruiken?
Voor mij als ontwerper: Het geeft een soort houvast en structuur. Ik hoef niet steeds te gokken waar iets moet staan. Mijn CSS blijft hierdoor overzichtelijk.
Voor de bezoeker: Het zorgt voor rust. Doordat elementen op vaste lijnen staan, begrijpt je sneller hoe de pagina in elkaar zit en leest het veel fijner.

3. Drie manieren om chaos in je ontwerp te voorkomen
1. Een vaste schaal of modulair grid gebruiken: Geen random groottes of marges kiezen, maar vaste stappen (zoals een modular scale). 
2. Niet alle contrasten tegelijk aanzetten: Als alles groot, dik, scheef en gekleurd is, valt niks meer op. Zorg voor een of twee opvallende dingen en houd de rest rustig. 
3. Elementen strak uitlijnen: Zorgen dat teksten en blokken duidelijke horizontale en verticale lijnen volgen in plaats van overal los.

3. Hoeveel gekkigheid moet er in je werk zitten?
Net genoeg om het anders te maken, maar niet zoveel dat het afleidt van de inhoud.


———————————————————————————————————————

HUISWERK VRIJDAG (VOOR MAANDAG) SPRINT 3
<img width="3211" height="2363" alt="IMG_0584" src="https://github.com/user-attachments/assets/df0712cd-c489-40c3-921f-b788df295c5c" />
<img width="3275" height="2283" alt="IMG_0585" src="https://github.com/user-attachments/assets/984665e7-d05a-4268-bf11-1491999c3639" />
<img width="3303" height="2417" alt="IMG_0586" src="https://github.com/user-attachments/assets/12d23486-d085-45a5-9850-a23e9b17f81b" />

Ik kies voor schets 3 (YMCA groter en kleiner). 'YMCA' is al het focuspunt in mijn ontwerp, maar ook in het liedje. Door dit woord te laten pulseren/groter en kleiner te maken, versterk ik het refrein van het lied. In plaats van alleen in te zoomen, combineer ik dit met het variabele font: het lettertype wordt tijdens het groter worden ook zwaarder in gewicht en schreef. Zo blijft de compositie in balans en gebruik ik de eigenschappen van het variabele fontbestand.

<img width="1142" height="366" alt="image" src="https://github.com/user-attachments/assets/09cef47d-adf3-4d4c-b254-45ab87c473b3" />

Voor deze stap heb ik mijn gekozen schets ('YMCA wordt groter en kleiner') uitgewerkt door de twee deep dives van Sanne te combineren:
1. Deep dive: Variabele fonts In plaats van alleen een standaard scale() te gebruiken, pas ik direct de variabele assen van het Seraphs lettertype aan via font-variation-settings. Bij 0% staat het gewicht (wght) op 200 en zijn de schreven minimaal (SERF op 0). Richting 100% vloeit dit door naar een dik gewicht van 900 en een volle schreef van 100. Omdat het een variabel font is, berekent de browser automatisch alle tussenstappen (tweening).
2. Deep dive: CSS animaties Ik heb een @keyframes aangemaakt met de naam --pulse-ymca. Door animation-direction: alternate te gebruiken, speelt de animatie vanzelf soepel heen en weer tussen 0% en 100% met een rustige ease-in-out timing. Om rekening te houden met de toegankelijkheid heb ik de animatie binnen een @media (prefers-reduced-motion: no-preference) media query gezet. Hierdoor beweegt het woord alleen als de bezoeker via zijn instellingen geen bezwaar heeft tegen beweging op het scherm.
Zo ondersteunt de typografische beweging het ritme van het lied, zonder dat de layout in het grid kapot gaat."

<img width="3024" height="1964" alt="image" src="https://github.com/user-attachments/assets/780291b5-cebd-4f24-8583-5032dd7ae523" />
Op zn kleinst (tijdens het pulseren)

<img width="3024" height="1964" alt="image" src="https://github.com/user-attachments/assets/74e7070c-3f21-4906-94b2-6571b0eb266a" />
Op zijn grootst (tijdens het pulseren)

Iteratie van hierboven:
<img width="1135" height="405" alt="image" src="https://github.com/user-attachments/assets/72bf70e7-cf02-4b59-adf8-64a4552aa33e" />
Wat er gebeurde bij de eerste versie:
In mijn eerste versie probeerde ik het gewicht en de schreven tegelijkertijd te animeren via font-variation-settings: "wght" 200, "SERF" 0. Maar toen ik dit in de browser testte, zag ik dat het woord eigenlijk alleen groter en kleiner werd door de scale(). De letters zelf veranderden niet soepel van dikte.
Het probleem onderzocht:
Ik ontdekte twee dingen:
1. Browsers hebben moeite om de losse tekst-strings van font-variation-settings vloeiend tussen stappen te berekenen (tweenen) binnen @keyframes.
2. In mijn CSS stond op main h1 nog een vaste font-weight: 900;, waardoor de browser die dikte vasthield in plaats van vanaf een lichte dikte te starten.
De iteratie (de oplossing):
Ik heb mijn code aangepast. In plaats van de "wght"-as in font-variation-settings te forceren, gebruik ik nu direct de standaard CSS-property font-weight in de keyframes (van 100 naar 900). De browser kan deze eigenschap wél perfect vloeiend interpoleren. Ook heb ik de vaste font-weight: 900 van de h1 afgehaald. Nu zie je de letters tijdens het ademen daadwerkelijk van heel dun naar moddervet vloeien, precies zoals bedoeld in de deep dive.

<img width="3024" height="1964" alt="image" src="https://github.com/user-attachments/assets/90a35a72-9d0c-4c4b-952c-8d8ce776ba24" />
Op zijn kleinst (tijdens het pulseren)

<img width="3024" height="1964" alt="image" src="https://github.com/user-attachments/assets/68583a72-e39e-4c9b-b83b-887e841c4237" />
Op zijn grootst (tijdens het pulseren)

Feedback klasgenoot: “misschien is het leuker om de letters “Y.M.C.A.” Los van elkaar te laten pulseren.


Koppelen aan mijn digital garden:       
<a href="./oefeningen/ymca-digitalgarden/ymca.html" class="nav-btn-ymca">YMCA EXPERIMENT →</a>
-> ik heb deze code geplakt in mijn header.  

<img width="2994" height="1714" alt="image" src="https://github.com/user-attachments/assets/94ab6033-7a9c-463f-a822-6df4f9444b49" />


Ik heb mijn typografie nu gekoppeld aan mijn Digital Garden. In de header van mijn homepage heb ik een hele simpele link toegevoegd die navigeert naar ./oefeningen/ymca-digitalgarden/ymca.html.
Voor nu heb ik dit heel simpel gehouden in HTML, zodat het experiment te vinden is en getest kan worden vanaf mijn site. Later ga ik deze link met CSS stylen en bepalen waar hij binnen de en layout van mijn Digital Garden het beste past.

WO 21 OKT BI-WEEKLY GEEK 3: 
<img width="3266" height="2329" alt="image" src="https://github.com/user-attachments/assets/c00e7be4-4e5a-4636-a808-6a95c04500db" />

Naast de bi-weekly geek gingen we aan de slag met peerfeedback geven met 3 verschillende klasgenoten en bij ons zat er een studentassisten bij om extra goed het formulier in te vullen.
<img width="2577" height="3487" alt="IMG_0601" src="https://github.com/user-attachments/assets/41e0e2d0-959b-46d6-8940-aadb91aab600" />
<img width="2678" height="3721" alt="IMG_0603" src="https://github.com/user-attachments/assets/a5e2cb54-bbbe-4c9d-8c2b-feb9c65f204d" />
Ik heb op de meeste dingen een goede score gekregen op een paar punten na. 

Mijn top 3 belangrijkste verbeterpunten heb ik op het formulier opgeschreven en hier ga ik de komende tijd aan werken om dit in orde te maken. 
Top 3:
1. Learning log compleet maken
2. Focus state vormgeven in thema van mijn site
3. Css verminderen en de html verbeteren.

De studentenassistent heeft mijn code bekeken en heeft mij vervolgens feedback en verbeterpunten gegeven. Hiernaast heeft hij mij handige tips gegeven die ik ook zou kunnen toepassen/mee kan nemen voor in de toekomst. 

Een paar punten wat hij heeft benoemd:
- In een article moet altijd een h2,3,4 etc staan.
- minder classes: nth of type mag, input is makkelijker dan button, maar er moet een formulier omheen
- teksten achter de card moeten h2 zijn
- nesting gebruiken ipv classes

#Focus state vormgeving in thema van mijn site:
<img width="1166" height="348" alt="image" src="https://github.com/user-attachments/assets/c85ded92-db91-45a9-b181-0fbe6c1e1419" />
Before
<img width="1044" height="342" alt="image" src="https://github.com/user-attachments/assets/7227d5c0-8b8a-43cf-9d7e-393556e6355a" />
After

Toelichting:
Tijdens de peerfeedback sessie kreeg ik de tip dat de standaard blauwe focusring (als je tabt met je toetsenbord) niet paste bij de donkere stijl van mijn site.

Ik wilde het randje niet uitzetten voor de toegankelijkheid, dus heb ik in mijn CSS bij de * reset 1 regel toegevoegd: outline-color: var(--color-accent);. Hierdoor blijft toetsenbordnavigatie gewoon goed werken, maar is de kleur veranderd naar rood en past dit bij de thema van mijn site.




</details>


### Fotografie toevoegen: De Shutter & Viewfinder Reel (CSS)
Na twee filmrollen met videobreakdowns wilde ik onderaan de pagina iets anders doen. Naast videografie doe ik ook aan fotografie, dus het leek me tof om een speciale sectie voor stills toe te voegen. Ik wilde niet zomaar een standaard fotogalerij neerzetten, maar bezoekers echt het gevoel geven dat ze door een camera kijken en zelf een foto "schieten".

Hoe ben ik erop gekomen:

Het idee was een continu bewegende filmstrook van beelden (alsof de wereld aan je zoeker voorbijtrekt) met rechtsboven een fysieke ontspanknop (shutter button).

Zodra je op de sluiter drukt, bevriest de strip direct op het huidige beeld, switcht de knop naar een groen focus-lampje en verschijnt eronder een tekstblok met cameradetails over het bevroren frame.

Omdat we voor school zo min mogelijk of geen JavaScript mogen gebruiken voor dit soort interacties, wilde ik kijken of ik dit 100% werkend kon krijgen met pure HTML en CSS.

Wat heb ik gedaan & keuzes die ik heb gemaakt:

Checkbox-hack voor de interactie: In plaats van een JS-click event heb ik een verborgen checkbox (#shutterToggle) gebruikt met een gestylede <label> als camera-sluiterknop. Met CSS selectors zoals #shutterToggle:checked ~ .viewfinder-frame .reel-track pauzeer ik de animatie (animation-play-state: paused;) en wissel ik direct tussen de lopende en gepauzeerde tekstblokken.

Viewfinder styling: Het kader heb ik voorzien van subtiele witte vizierhoeken op de vier hoeken en een crosshair in het exacte midden. Hierdoor voelt het kader meteen als een professionele zoeker (viewfinder/cameramonitor) in plaats van een simpel plaatjesvak.

Uitbreiden van de fotoreeks: Met een korte set beelden viel de sluiter te vaak op dezelfde foto's. Ik heb de reeks uitgebreid naar 11 unieke foto's (en die 1x gedupliceerd voor een naadloze CSS translate loop). Hierdoor voelt elke klik onvoorspelbaar en als een echte momentopname.

iteraties:

Afgekapte portretfoto's: Veel van mijn foto's zijn staande portretten. Omdat het kader maar 260px hoog was met object-fit: cover, werden alle hoofden onthoofd. Opgelost door de viewfinder te verhogen naar 380px en object-position: top center mee te geven. Hierdoor vullen de beelden nog steeds het hele vlak, maar blijven gezichten en ogen altijd scherp en netjes in beeld.

Verdwenen detailtekst door een div-fout: Na het toevoegen van de 22 foto-items was ineens het hele tekstblok onder de zoeker verdwenen. Na inspectie bleek dat er per ongeluk een extra afsluitende </div> was blijven hangen tussen de foto's. Hierdoor werd de container te vroeg afgesloten en kon de CSS-combinator (~) het tekstblok niet meer bereiken. Na het verwijderen van de extra div werkte alles direct weer zoals verwacht.

HTML compact houden: Om het overzicht in mijn code niet te verliezen tussen 22 foto-items, heb ik alle afzonderlijke <div class="reel-item"><img ...></div> elementen netjes strak op één regel gezet in plaats van uitgesmeerd over meerdere regels.

Resultaat:
Een interactieve, analoge zoeker-ervaring die perfect past binnen het cinematische concept van mijn digitale tuin, compleet functioneel in pure CSS zonder ook maar één regel script.

<img width="1920" height="1080" alt="Scherm­afbeelding 2026-10-18 om 21 37 05 (2)" src="https://github.com/user-attachments/assets/dbbb304e-30eb-419c-ab5f-59e5a1e95006" />
<img width="368" height="211" alt="Scherm­afbeelding 2026-10-18 om 22 39 28" src="https://github.com/user-attachments/assets/a9b569ae-f655-4e55-96c4-c8712fb54f99" />
<img width="360" height="240" alt="Scherm­afbeelding 2026-10-18 om 22 39 18" src="https://github.com/user-attachments/assets/fe3a93b8-fd89-4c85-98a8-ff15d95a350a" />
<img width="718" height="649" alt="Scherm­afbeelding 2026-10-18 om 22 39 00" src="https://github.com/user-attachments/assets/ca52d1d6-0a7f-4d71-8de2-5ad4e121d427" />
<img width="1395" height="803" alt="image" src="https://github.com/user-attachments/assets/ac821e4e-2c1e-4571-957d-ce5ae73ae8ea" />


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


### Concept, structuur en Light/Dark zonder JS
Vandaag de basis gelegd voor mijn digital garden. Ik wil er een minimalistisch en cinematisch videodossier van maken onder de naam BERA74K, gefocust op video-edits en storytelling (begonnen met shots van Kreta).

Wat heb ik gedaan:

De opzet verdeeld over 3 logische schermen: index.html (de zoeker/viewfinder knop), home.html (de privacy consent card) en log.html (het daadwerkelijke videodossier).

In eerste instantie stonden de links en paginavolgorde andersom, maar na testen toch besloten om eerst de strakke 'Enter Garden' viewfinder te tonen en daarna pas door te verwijzen naar de privacyverklaring.

Gewerkt aan een light/dark mode toggle. Schoolregel was om dit zo modern mogelijk te doen: dus geen JavaScript, maar 100% native CSS met color-scheme: light dark, de light-dark() functie en :has() gekoppeld aan radio buttons (licht en donker).

Wat viel op:

Dat je met :has([value="light-theme"]:checked) een hele pagina van thema kan laten switchen zonder JS aan te raken.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Semantiek opschonen & rare bugs fixen
Vandaag feedback verwerkt over semantische HTML. Mijn code zat nog vol met divs en spans en dat mocht eigenlijk niet meer van school tenzij het echt niet anders kon.

Wat heb ik veranderd:

Alle losse blokken omgezet naar echte semantische tags: de kaartenrij in een <ul> met <li>, artikelen in <article>, knoppengroepen in <nav>, en de beelden in geneste <figure> tags met <figcaption>.

Spans rond radioknoppen en knopteksten weggehaald of vervangen door <small> en <strong>.

Oepsie momentjes & bugs gefixt:

Tekst horizontaal gepropt: Ik had de teksten in de kaarten eerst in een <header> gezet. Maar omdat mijn hoofdnavigatie bovenaan ook als header in de CSS stond met display: flex; justify-content: space-between;, werd ineens alle tekst in de kaarten horizontaal op één gekke rij geperst. Opgelost door de hoofdnavigatie specifiek .main-header te noemen en de kaartinhoud netjes in een <section class="card-content"> te zetten.

Doorstreep-bug in de privacy-card: Op home.html liep er opeens een streep dwars door de titel 'DATA & PRIVACY'. Bleek dat de algemene h1 een negatieve marge had (margin-bottom: -1.5rem) voor het overlap-effect op de log-pagina. De border van de container werd daardoor dwars door de tekst omhoog getrokken. Gefixt door de h1 binnen de consent-box te resetten naar margin: 0.

Hoogteverschil: De tekst van kaart 3 (colorgrading) begon veel hoger dan de rest. De 3 fotootjes stonden per ongeluk op 160px terwijl de rest van de foto's 200px was. Gelijkgetrokken en nu lijnen alle tekstvakken perfect uit.

Typfout: Zag ineens dat mijn box-sizing reset kapot was door een typefout (- { in plaats van * {). Gelijk hersteld.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Filmrol esthetiek & iteratie
Feedback gekregen dat de site nog meer het cinematische / film thema mag uitstralen. Het idee kwam op om iets met een filmrol te doen.

Eerste poging (verworpen):

Ik begon met het idee om alleen van het 3e vakje (de colorgrading-shots) een 35mm filmstrip te maken met tandwielgaatjes (sprocket holes) via repeating-linear-gradient.

Conclusie: Het zag er leuk uit, maar het voelde gek dat maar één los vakje een filmrol was terwijl de rest gewone webkaartjes bleven.

Tweede keuze (definitief):

Roer omgegooid: de complete rij (.cards-grid) omgebouwd tot één grote, doorlopende 35mm filmrol!

De tandwielperforaties lopen nu boven en onder over de hele breedte door en elk project/shot fungeert als een echt filmnegatief. Op mobiel scrolt het nu ook horizontaal alsof een filmspoel afrolt.

Thema-contrast verbeterd:

Toen ik switchte naar light mode zag het er niet uit: de filmrol bleef keihard zwart (#0b0b0d), wat veel te zwaar contrasteerde tegen de lichte achtergrond.

Opgelost door CSS-variabelen toe te voegen (--film-bg en --film-hole) met light-dark(). In dark mode is het analoog donker, en in light mode switcht de filmrol mee naar een zachte, vintage grijstint.

<img width="1920" height="1038" alt="Scherm­afbeelding 2026-10-18 om 18 32 03" src="https://github.com/user-attachments/assets/1634c175-f3d4-4dcd-ad23-ac2459a0cbdb" />
-> 
<img width="1512" height="982" alt="Scherm­afbeelding 2026-10-18 om 21 37 03" src="https://github.com/user-attachments/assets/18f96d54-01e2-4144-ac1d-9899c8dc0d12" />



------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Video 02 toevoegen & responsive titels
Vandaag de placeholder van Video 02 aangepakt en inhoud gegeven.

Wat heb ik gedaan:

Video 02 wordt een motivatievideo, dus als grote achtergrondtitel gekozen voor MOTIVATIONAL (als tegenhanger van CINEMATIC).

Omdat MOTIVATIONAL 12 letters telt en veel langer is dan CINEMATIC, liep de tekst op kleinere schermen buiten beeld. In de CSS heb ik font-size: clamp(2.4rem, 8.5vw, 4rem) toegepast zodat lange titels automatisch soepel meeschalen met het scherm.

Net zoals bij Video 01 een strakke 4-koloms layout gemaakt:

Kolom 1: De uiteindelijke edit (video02.graded.jpeg).

Kolom 2: Tijdlijn / Sound design (voorlopig een leeg filmkader gehouden met behoud van de 200px verhouding).

Kolom 3: Colorgrading drieluik met video02.log.jpeg, video02.709.jpeg en video02.graded.jpeg.

Kolom 4: Typografie / Boodschap (ook voorlopig leeg gehouden).

Resultaat:
Alles staat nu semantisch goed in elkaar, valideert netjes, de styling is responsive en de filmrol sluit perfect aan bij mijn thema en schoolopdracht.

<img width="1512" height="982" alt="Scherm­afbeelding 2026-10-18 om 21 37 05" src="https://github.com/user-attachments/assets/3c22873f-5149-494d-a867-781ca0659838" />
<img width="415" height="428" alt="timeline02" src="https://github.com/user-attachments/assets/2b1db65c-da07-4cc0-8722-1c2b52b89c4e" />



------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Sprint 2 (21 sept - 02 okt)

## 30 sept checkout: 
1. Waar staat WCAG en A11y voor?
- WCAG: Web Content Accesibillity Guidelines
- A11y: A11y staat voor teogankelijkheid: ervoor zorgen dat iedereen een website of app kan gebruiken, ook mensen met een beperking.

2. Wat vind je lastiger, je laptop/websites alleen met een toetsenbord bedienen of met een screenreader? Waarom? Waar moet je nog mee oefenen?
- Ik vind het moeilijker om een laptop/website te bedienen met een screenreader. Omdat ik eigenlijk altijd gewend ben om een muis te gebruiken en merk ineens een erg grote verschil omdat dit nieuw voor me is. Zodra ik de shortcuts ken en onder de knie heb zal het wat makkelijker zijn, dus ik moet hiermee oefenen.

3. Met welke beperking rekening houden vind je het meest lastig?
Vind je dat je beperkt wordt in wat je kunt ontwerpen?
Of heb je al manieren gevonden om vanuit een solide basis  - die voor iedereen toegankelijk is - allemaal leuke en mooie extra's toe te voegen als je bezoekers dat goed vinden?
- Ik vind het vooral lastig om rekening te houden met mensen met een visuele beperking, omdat je bij het ontwerpen vaak gebruikmaakt van kleuren, afbeeldingen en visuele elementen. Ik vind niet dat je daardoor beperkt wordt in wat je kunt ontwerpen. Je moet alleen zorgen dat de basis voor iedereen toegankelijk is. Daarna kun je extra’s toevoegen die het ontwerp leuker en mooier maken, zolang ze de toegankelijkheid niet in de weg zitten.

## 28 sept checkout:
1. Wat bedoelt Vasilis met de uitspraak: Semantiek doet mij niet zo veel, ik ben liever bezig met de UX van HTML?
- dat het niet uitmaakt of je code theoretisch volgens alle regeltjes klopt, maar hoe de HTML voor de bezoeker werkt.
2. Wat voor type beperkingen hebben invloed op het gebruiken van websites?
- Visueel, Auditief, Motorisch, Cognitief
3. Noem drie manieren om door een website te navigeren met jouw screenreader.
- Tab 
- Shortcuts 
- Luisteren

Het staat model voor digitale tuintjes welke bij 'Het web is voor iedereen' door studenten worden gemaakt.

1. Wat is HTML validatie, waarom is het belangrijk en hoe heb je dat vandaag uitgevoerd?
- een manier om te checken of je code netjes is en welke foutmeldingen er zijn. Ook kan je zien of er betere alternatieven zijn voor bepaalde code.
2.  Welke dingen vielen je op?
- Dat er ook alternatieven worden gegeven en niet alleen errors

3. Welke feedback heb je ontvangen tijdens het gesprek met je docenten?
- Alle schetsen en logboek goed bijhouden. En meer doen met het thema "cinema". Bijvoorbeeld verwerken in de cookies pop-up en achtergrond van de stappenplan in vorm van een filmstrip etc etc.

### Sprint 1 (7 sept - 18 sept)

### 16 sept checkout
1. Noem 3 Gestaltprincipes op en laat de ander uitleggen wat ze betekenen en doen.
- Symmetrie: Elementen die aan weerszijden in balans en evenwichtig zijn opgebouwd
- Nabijheid: Elementen die dicht bij elkaar staan
- Gelijkheid: Elementen die dezelfde vorm, kleur of stijl delen

2. Een grid biedt ruimte om te spelen (vrijheid), maar tegelijkertijd ook eenheid en structuur (vastigheid). 
Wat wordt hiermee bedoeld? 
- Vastigheid: De lijnen en kolommen zorgen voor strakke uitlijning, gelijke witruimte en rust over de hele pagina
- Vrijheid: Binnen die lijnen bepaal je hoe je elementen combineert. je kiest zelf hoeveel kolommen een afbeelding of tekst pakt om een layout te maken.

3. Welk principe neem je mee in een laatste iteratie van je ontwerp? 
- Consistentie

### 8/9 sept -



### 7 sept - checkout
1. Een digital garden is een website die nooit compleet is en altijd aangevuld kan worden.

2. Een website dat echt webby is moet een aantal punten bevatten. Fluide/adaptief, interactief en een duidelijke hierarchy hebben, waardoor alles goed te vinden is. Het moet ook toegankelijk zijn voor iedereen. (oud, jong, blind etc.)

3. Ik wil een digital garden maken over mijn videografie/fotografie. Mijn werk/verhalen laten zien en de keuzes hierachter duidelijker uitleggen. Ook wil ik vertellen over andere filmmakers, regisseurs en cinematographers waar ik mijn inspiratie vandaan haal.

<img width="3773" height="2705" alt="7septss" src="https://github.com/user-attachments/assets/4d9de59b-b64b-431f-97d3-0672d8688b5e" />



### Sprint 0 (31 aug - 4 sept)

### [...]
test test
[...]

### 3 sept - [Workshop]

[...]

### 31 aug - Kickoff

Een fork van de model repository gemaakt en gepubliceerd via mijn eigen Github omgeving.
