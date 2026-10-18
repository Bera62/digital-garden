## Learning Log
# Model

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

Oepsie momentjes & iteraties:

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
