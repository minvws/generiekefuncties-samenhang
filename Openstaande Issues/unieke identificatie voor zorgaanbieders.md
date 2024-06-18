# Inleiding
Een zorgvuldige organisatie van databeschikbaarheid in de zorg, vraagt om afspraken op alle niveau’s. Op het organisatie niveau gaat het daarbij ondermeer om de vraag: hoe kunnen zorgaanbieders uniek geïdentificeerd worden? Dat is een van de centrale vragen van de norm I&A. Het URA (uzi register abonneenummer) geeft een unieke identificatie van zorgaanbieders die elektronisch gegevens uitwisselen. Omdat VWS in de uitvoering verantwoordelijk is voor Uzi-register, is afstemming over de (on)mogelijkheden en (on)wenselijkheden van belang van een landelijke keuze voor het URA. Daartoe kan deze notitie dienen: als afstemming en opmaat voor beleid, zodat in het normtraject een goede en realistische en toekomstvaste keuze gemaakt kan worden.

# Waarom URA nodig is voor elektronische uitwisseling
Zorgaanbieders zijn gedefinieerd in de WKKGZ en hebben een toelatingsprocedure onder de WTZi. Zorgaanbieders zijn zorginstellingen en solo-werkende zorgverleners. Die laatsten worden als zorgaanbieder aangesproken op wat ze voor de organisatie van zorg moeten doen, niet op wat ze als individuele behandelaar moeten doen. Het gaat dus om het organisatorische aspect bij de term zorgaanbieder. 
In de wetten over de (elektronische) uitwisseling van medische gegevens, zoals Wabvpz en Wegiz, wordt ook de term zorgaanbieder gebruikt in de zin van WKKGZ. Voor de generieke functies die deze uitwisseling verder gaan standaardiseren, is een unieke identificatie van ‘zorgaanbieder’ nodig.
Het UZI-register is destijds opgericht, o.a. omdat KvK niet specifiek genoeg is voor zorgaanbieders (organisaties buiten de zorg hebben ook een KvK nummer) en omdat AGB te ‘vervuild’ bleek als basis voor zorgvuldige onderlinge uitwisseling.
Met de ontvlechting van het UZI-register, wordt het wellicht eenvoudiger om een URA aan te vragen, omdat het niet meer gekoppeld is aan een middel (servercertificaat of smartcard).

# URA in relatie tot generieke functies

## Identificatie en authenticatie
In de zorginformatiebouwsteen wordt nog open gelaten welk van de drie codestelsel wordt gebruikt voor zorgaanbiederID: AGB, KvK, of URA. Wenselijk is dat de norm I&A zich uitspreekt dat URA altijd verplicht is en dat KvK en AGB optioneel als extra ID meekunnen.

## Adressering
Het adresseren van zorgaanbieders start met een uniek zorgaanbiederID, bv URA. In een adresfunctie (bv digitaal zorgadresboek) kan op basis van een URA het benodigde (technisch) adres opgevraagd worden. Dat kunnen adressen zijn van afdelingen, maar ook van beschikbare gegevensdiensten.

## Lokalisatie
Voor het lokaliseren van dossierhouders (‘waar’) is een uniek ID van een zorgaanbieder nodig. Een van de gestandaardiseerde attributen van zorgaanbieders is het zorgaanbiedertype. Dat is handig bij de lokalisatie, omdat een opvrager gericht kan zoeken naar bv de apotheken van een patiënt, en dan niet alle ziekenhuizen en paramedici erbij krijgt.

## Toestemming
Voor het vastleggen van toestemmingen is een uniek zorgaanbiederID nodig, om de eenduidigheid van een toestemming te borgen. Het gaat hierbij enerzijds om een zorgaanbieder die herkenbaar moet zijn voor de burger die een toestemming registreert en anderzijds om een ID van diezelfde zorgaanbieder die gebruikt wordt in de uitwisseling op basis van die toestemming. Naast het vastleggen van een toestemming voor één dossierhouder, kan een burger ook voor een categorie (bv alle apotheken) een toestemming vastleggen. Daarmee blijft het aantal specifieke toestemming voor de hele zorg beperkt tot zo’n 35 keuzes (minder is niet specifiek genoeg en meer is niet overzichtelijk/begrijpelijk/eenduidig). Iedere URA moet dus een herkenbaar eenduidig zorgaanbiedertype hebben.

## Autorisatie
Autorisatie van toegang tot bepaalde gegevens kan op zorgaanbieder en op zorgverlener niveau. Voor het zorgaanbiederniveau is een uniek zorgaanbiederID nodig, inclusief het zorgaanbiedertype, omdat op het zorgaanbiederniveau de autorisatieregels (bv in de informatiestandaard) doorgaans gebaseerd zijn op zorgaanbiedertype. Bijvoorbeeld: PS van huisartsenpraktijken naar huisartsenposten, BGZ voor medische specialistische zorg onderling, etc.

# Vraagstuk bij zorgbrede keuze voor URA
Bij veel zorgaanbieders is er geen twijfel bij het toekennen van een URA. Zo heeft een openbare apotheek in een dorp met één locatie gewoon één uniek URA. In de praktijk blijkt echter dat er in andere situaties discussie kan ontstaan of een organisatie die voldoet aan de criteria van het UZI register en dus een URA kan krijgen, eigenlijk beschouwd moet worden als 2 zorgaanbieders, en dus 2 URA’s toegekend zou moeten krijgen.
Op basis van de Wabvpz en WKKGZ wordt door het Uzi-register het begrip ‘zorgaanbieder’ gehanteerd. Vanwege de compliance met Etsi worden er een koppeling met de KvK gelegd. Uitgangspunt is dat een abonnee in het Uzi-register uniek herleidbaar moet zijn naar rechtspersoon in de KvK. Dat gebeurt nu op basis van de KvK nummer en bijbehorende KvK-naam. De KvK naam wordt letterlijk overgenomen als URA-naam.

Bij het Uzi-register zijn er diverse ‘known-issues': 
De eerste betreft een apotheek die onder dezelfde KvK nummer valt als het ziekenhuis. Indien de apotheek een eigen status heeft, en een eigen herkenbaarheid en ook bij de inspectie apart geregistreerd is, maakt het CIBG hier een uitzondering: de apotheek kan in die uitzonderlingssituatie een aparte URA krijgen. Vanwege de herleidbaarheid naar de KvK kan voor de apotheek desgewenst nog een aparte handelsnaam in het KvK geregistreerd worden.
De tweede situatie betreft een zorgaanbieder met diverse vestigingen, waarbij de vestigingen zich als aparte zorgaanbieders presenteren. Er is dan één rechtspersoon met één of meer KvK nummers en per vestiging een andere (handels)naam. Dat is weliswaar niet conform het uitgangspunt één URA per rechtspersoon, maar komt in de praktijk wel tegemoet aan de herkenbaarheid en herleidbaarheid van verschillende zorginstellingen (ook al zijn ze dezelfde BV, of GMBH, en hebben ze één RvB).

# URA issues in het kader van generiek functies
Voor de generieke functies die VZVZ gerealiseerd heeft en waar VWS in het kader van IZA concreet beleid over opstelt en waar de Nen met normering bezig is, is het zeer wenselijk dat er landelijk beleid komt dat zorgbreed en generiek toegepast kan worden.
Voor een zorgbrede analyse van deze problematiek, zijn op hoofdlijnen 3 perspectieven te onderscheiden:

1.	Huisvesting: als één juridische organisatie in 5 steden een gebouw heeft, zijn dat voor patiënten 5 verschillende organisaties. Vanuit de generieke functie ‘toestemming’ zou je deze afzonderlijke organisaties apart toestemming willen kunnen geven, bijvoorbeeld omdat je alleen naar de organisatie gaat in je eigen woonplek. Het gezondheidscentrum in Almere is daarom enkele jaren geleden van 1 naar 30 URA’s gegaan.
2.	Juridisch: als een huisartsenpraktijk en een fysiotherapiepraktijk in één gebouw zitten, en het zijn in de KvK 2 organisaties dan kunnen ze 2 URA’s krijgen. Is het echter één organisatie met één vestiging in de KvK, dan kunnen ze maar 1 URA krijgen. Voor de generieke functies is het wenselijk dat ook in die situatie (1 juridische entiteit in 1 gebouw, maar voor patiënt herkenbaar verschillende instellingen, met aparte balies en eigen systemen) de gegevensstroom onderscheiden kan worden, dat ze dus 2 URA’s zouden moeten hebben. Immers als je niet bij die huisarts zit, maar wel bij de fysio in dat gebouw, dan heeft de huisartsenpraktijk niets met jouw fysio gegevens te maken, en andersom. Ook mag deze zorginstelling niet te boek staan als “de huisartspraktijk van deze patiënt”. Het onderscheid tussen twee typeringen maakt dat het voor de patiënt twee verschillend identificeerbare praktijken zijn. Dan moet de URA als identificerend nummer ook beide kunnen onderscheiden. Alle generieke functies kunnen daarvan profiteren. De uitzondering met ‘handelsnamen’ zou dan misschien een regulier proces moeten worden, om beide een URA te kunnen geven. 
3.	Technisch: als een ziekenhuis en een thuiszorgorganisatie ieder een eigen vestiging heeft, maar wel dezelfde RvB (juridisch dus één), dan zouden er 2 URA’s uitgegeven moeten kunnen worden om de gegevensstroom te kunnen onderscheiden. Bijvoorbeeld voor het lokaliseren van medische beelden: dan is de thuiszorg niet relevant om te bevragen. Als er echter sprake is van één systeem waar het ziekenhuis en de thuiszorgorganisatie in werken, zodat een inschrijving in het ziekenhuis, betekent dat je ook in de thuiszorgorganisatie bekend bent, dan is het onderscheid met 2 URA’s niet technisch tot en met de dossiergegevens door te voeren. Vanuit het oogpunt van de generieke functies zou dan met 1 URA kunnen volstaan.  

Het is wenselijk om voor de generieke functies een eensluidend beleid te formuleren voor deze situaties. Dan kan op basis van dat beleid zowel het Uzi-register als de generieke functies uitgewerkt worden. 
Vanuit de generieke functies zouden de wensen/eisen t.a.v. bovenstaande problematiek beschreven kunnen worden. Wellicht komt daar een eisenpakket uit naar voren waarmee alle generieke functies gebaat zijn. De nu bekende ‘bespreekgevallen’ / ‘uitzonderingen’ / usecases van zorgaanbieder-organisaties zouden dan in een procesflow opgenomen kunnen worden, zodat een zorgaanbieder hoeveel URA’s handig zijn en zodat het UZI-register weet onder welke voorwaarden er ‘extra’ URA’s aangevraagd kunnen worden.

# Voorbeelden van 'exoten'

1.	Ziekenhuizen kunnen een eigen apotheek in een apart gebouw hebben. Eén KvK, twee vestigingen, ieder eigen handelsnaam en eigen adres. Er kan met één URA volstaan worden, maar twee is ook mogelijk als dat voor een of meer generieke functies nodig of wenselijk is.
2.	Ziekenhuizen kunnen een inpandige apotheek hebben. Eén KvK, één vestiging. In principe één URA, maar als de apotheek in de nacht een dienstapotheek wordt (dus als zorgaanbieder onder openbare apotheken valt) en als zodanig ook geregistreerd is, bv bij IGJ, zijn twee URA’s wenselijk. Dat is de enige ‘uitzondering’ die het Uzi-register ondersteunt.
3.	Ziekenhuizen kunnen een inpandige apotheek hebben die in alles onder het ziekenhuis valt. Dan kan voor alle generieke functies volstaan worden met één URA. NB ook als er aparte systemen gebruikt worden door de apotheek en door de rest van het ziekenhuis, kan dat op basis van één URA.
4.	Ziekenhuizen met een inpandige huisartsenpraktijk met één KvK nummer en één vestiging. Deze kunnen volstaan met één URA. Zeker als de ‘huisartsenpraktijk’ fungeert als een ‘polikliniek generalistische zorg’. Indien de huisartsenpraktijk echter als een zelfstandige zorgaanbieder fungeert, met een eigen patiënt administratie, alleen juridisch onder dezelfde RvB valt, wil je voor de functie toestemming, lokalisatie en wellicht ook adressering toch onderscheid kunnen maken. Dan zijn twee URA’s wenselijk, en moet afgesproken worden welke voorwaarden in KvK van toepassing zijn (bv aparte registratie als nevenvestiging met een eigen handlesnaam t.b.v. tweede URA). 
5.	Ziekenhuizen met andersoortige zorgaanbieders in aparte gebouwen, bijvoorbeeld een fysiopraktijk of een thuiszorgorganisatie die juridisch onder dezelfde rechtspersoon vallen, zouden vanuit de generieke functies toestemming en lokalisatie en adressering als aparte zorgaanbieders, dus met aparte URA’s geïdentificeerd moeten worden. Het UZI-register kan wellicht op basis van de nevenvestiging met een andere handelsnaam en een ander adres, hiervoor 1 of meer URA’s toekennen.  
6.	Gezondheidscentrum dat in één gebouw 3 zorgaanbieders huisvest, waarbij de zorgaanbieders allemaal een eigen WTZI/A registratie hebben, moeten 3 URA’s kunnen krijgen ook al zijn hun verschillende KvK nummer gehuisvest op hetzelfde adres. Eis vanuit Uzi-register: alle drie een andere handelsnaam, of is ander KvK nummer voldoende?
7.	Gezondheidscentrum dat als één rechtspersoon met één KvK nummer 3 zorgaanbieders huisvest, met een eigen balie en ieder een eigen systeem (dus ook eigen patiëntregistraties) moeten ook 3 URA’s kunnen krijgen. Immers voor de generieke functies is er (vanuit patiëntperspectief) geen verschil met vorige situatie. IGJ hanteert de norm: de grootste / overkoepelende rechtspersoon is aanspreekpunt, dus één URA is juridisch voldoende, maar voor de herkenbaarheid voor de patiënt (waar de generieke functies betrekking op hebben) is er wel degelijk onderscheid, en zo ook op systeemniveau en dus in de gegevensuitwisseling. Vermeden moet worden dat gegevens die op alle lagen gescheiden zijn, alleen vanwege één URA opeens benaderbaar / beschikbaar komen.

| Item| Juridisch #RvB| Huisvesting #adressen|Technisch #epd/ecd|Voorbeelden & Opmerkingen|Advies #URA's|
| :---| :------: | :----------:|:-------:|:---------:|:------:|
| 1   | 1 | 1 | 1 |huisartspraktijken, openbare apotheken   |1|
| 2   | 1 | 1 | >1|GGZ met ECD en EVS <br>opm: >1 technisch endpoint per URA |1|
| 3   | 1 | >1| 1 |Apotheek met nevenvestiging <br>opm: >1 URA is mogelijk maar onwenselijk want data in 1 systeem|1|
| 4   | 1 | >1| >1|Ziekenhuis met apart apotheekgebouw <br>opm: iedere vestiging eigen systeem|1|
| 5   | >1 | 1| 1|mag niet voorkomen, gescheiden data! |nvt|
| 6   | >1 | 1| >1|Huisarts en fysio onder één dak|>1|
| 7   | >1 | >1| 1|mag niet voorkomen, gescheiden data!|nvt|
| 8   | >1 | >1| >1|Zorgcentrum met nevenvestigingen|>1|



# Plaatje om gesprek binnen werkgroep adressering te voeren
![eerste uitwerking identifier-vraagstuk irt adressering](https://github.com/minvws/generiekefuncties-samenhang/assets/123090714/69a9d55f-2804-4637-9b09-d8ab79786076)
