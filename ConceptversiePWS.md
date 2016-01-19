#Hacking: The art of exploitation
Matej Curcic
Mike Wong
Mohamed Ettejani
Begeleider: Eduard van Dam


Netwerk scan. Dit krijgen hackers te zien als ze een netwerk uitpluizen op beveiligings gaten.








Inhoudsopgave

Hacking: The art of exploitation
Plan van aanpak
Inleiding
Theoretisch kader
Wat is hacken nou eigenlijk en wat is de definitie van een hacker?
De moraliteit van hackers:
Vóór de les
Wat gaat er gebeuren?
Doelen
Planning
Ná de les
Wat is er gebeurd?
(On)Bereikte doelen
Logboek
Bronnen:
Internet:
Boeken:
Digitaal materiaal:
Nawoord
Conclusie




Plan van aanpak
Ons profielwerkstuk gaat over ‘The art of exploitation’, de kunst van het blootleggen. We willen weten wat de reactie is van mensen als ze een cursus hacken krijgen. De verkregen informatie zullen wij met elkaar vergelijken en uiteindelijk goede conclusies trekken.

Onderzoeksvraag:
Wat is de reactie van mensen wanneer zij uitgenodigd worden voor een cursus hacken en wat zijn hun reacties tíjdens de cursus hacken als ze besloten hebben mee te doen? 

Deelvragen:
Zullen er enthousiaste reacties komen van degenen die uitgenodigd zijn, of zullen wij met negatieve gevoelens bekeken worden?
Wordt het onderwerp hacken door de maatschappij in een negatief daglicht gezien?
Heeft de gemiddelde leerling enige ervaring met hacken?
Hoe lang zal, als het er is, het enthousiasme en de interesse van de leerlingen aanhouden tijdens de les?

Hypotheses:
Wij denken dat de meeste mensen wel willen leren te hacken, voornamelijk omdat het interessant klínkt. Als wij ze echter zouden vragen wat zij denken dat hacken inhoudt, zullen zij waarschijnlijk meestal een verkeerd antwoord geven. Het standaard idee van een hacker is:
“In het bijzonder wordt het woord hacker gebruikt in volgende betekenissen:
Iemand die een programmeertaal of -omgeving zo goed kent dat hij/zij zonder zichtbare moeite een programma kan schrijven.
Iemand die onconventionele maar adequate oplossingen bedenkt tegen lekken, fouten en problemen van andere aard met behulp van beschikbare middelen.
Iemand die tracht om via illegale wegen een computersysteem binnen te dringen teneinde een beveiligingsprobleem te kunnen aantonen en indien mogelijk te verhelpen.
In deze laatste betekenis hebben hackers vaak een negatieve bijklank. Sommige hackers houden zich niet aan de hackersethiek, hebben geen respect voor andere mensen en hacken met de intentie informatie bloot te leggen. Daarmee beïnvloeden ze de publieke opinie om aanhangers te winnen voor bepaalde opvattingen of standpunten.”

Waarschijnlijk vinden veel mensen hacken als onderwerp wel interessant, maar zien mensen over het algemeen hacken als een negatief iets. Iets dat illegaal en gevaarlijk is of kan zijn.
De meeste leerlingen zullen waarschijnlijk geen of zeer weinig ervaring met hacken hebben. Het is niet iets wat je in korte tijd en op jonge leeftijd zomaar ergens kunt leren en begrijpen. Het vergt namelijk veel ervaring en kennis die je over de jaren opdoet.
Het enthousiasme en de interesse van de leerlingen zal waarschijnlijk afnemen tijdens de les, wanneer ze merken dat het erg lastig is om de trucs van en kennis over het hacken onder de knie te krijgen.

















Inleiding
Later wil je een leuk beroep uitoefenen, en je weet in ieder geval dat je computer security wilt gaan studeren en dat je de uitdaging aan wil gaan in de wereld van hackers. Na je opleiding wil je je verder gaan specialiseren. Het hacken zegt je wel wat, maar wat is het nou precies? Welke wegen moet je afleggen om een hacker te worden? Allerlei vragen die opkomen, waarop je graag duidelijke antwoorden wilt krijgen.

Hacker worden is wel leuk, maar niet iedereen is er voor geschikt. Als je dit wilt doen, moet je bepaalde dingen goed kunnen. Hacker zijn vereist veel geduld en motivatie, maar vooral veel interesse. Door ons profielwerkstuk krijg je een beeld over wat ‘cybersecurity’ inhoudt.







Theoretisch kader:
De ms08-067_netapi exploit maakt gebruik van een gat in de beveiliging van Window versies 2000 tot en met de Windows versie 2003 SP2. Het gaat hierbij om een programmeerfout in de “NetAPI32.dll” en “WNetAPI32.dll” bestanden die deze systemen gebruiken. Je krijgt, na het uitvoeren van de exploit, op afstand, systeem rechten op de machine waarop je de exploit hebt uitgevoerd.

Dit gat is te beveiligen door alle nieuwste updates van windows te installeren en door een anti-virus programma te installeren.

SQL-injection is het uitbuiten van onverantwoordde syntaxen in sql query’s. Een voorbeeld hiervan zou een query zijn die niet op validiteit wordt gecontroleerd. In zo een query kan een gebruiker invoeren wat hij wil. Je krijgt dan de mogelijkheid om het volgende met een database te doen:
Gegevens uit een database opvragen
Gegevens wissen
Gegevens aanpassen
Gebruikers toevoegen
Tabellen toevoegen en verwijderen

SQL-injection is meestal tegen te gaan door middel van “prepared statements” en “input validation”. Prepared statements zijn voorgemaakte sjablonen, waarin variabelen worden gebruikt om veranderende elementen aan te geven. Een prepared statement kan efficient uitgevoerd worden, omdat de invoer dan aan bepaalde eisen moet voldoen, kan het programma zich daar dan al op ‘voorbereiden’. Bovendien erg veilig is omdat de programmeur aangeeft welke variabele welke soort is: integer(heel nummer), double(kommagetal), string(text) of BLOB (Binary Large Object). Een BLOB is overigens het gevaarlijkste om te gebruiken in het geval van SQL-injection. Dit omdat je alle mogelijke tekens en zelfs bestanden in deze ‘data type’ kunt opslaan. Op deze manier kan een hacker bijvoorbeeld code toevoegen aan het einde van een plaatje en deze uploaden naar de database op een pagina waar de web developer hier niet op is voorbereid. Dit terwijl de andere ‘data types’ specifieke doelen hebben en daardoor ook op hun functie gefilterd kunnen worden. Input validation is het process van nagaan of de tekst, die de gebruiker heeft ingevoerd, voldoet aan de ‘regels’ en eisen die de programmeur van tevoren opstelt.

Command injection is het toevoegen van een eigen commando aan een functie, die via de webapplicatie direct op de server wordt uitgevoerd. Een voorbeeld hiervan is de ping applicatie op de “Damn Vulnerable Web Application” (dvwa). Hierbij wordt een ping commando uitgevoerd op de server en het resultaat weergegeven op de website. Door een puntkomma in de invoer te zetten, kun je ook je eigen commando op de server uitvoeren. Dit gebeurt dan met de rechten die de gebruiker, onder wie de website gehost wordt, uitgevoerd. Als het dus een administrator gebruiker is, dan heb jij, als hacker, ook administrator rechten op de server: je kunt dus alles doen wat je wil.

XSS, ook wel bekend als “Cross Side Scripting”, wordt gebruikt om je eigen scripts, lokaal bij andere bezoekers van de webapplicatie, uit te voeren. Deze scripts kunnen van alles zijn (denk maar aan keyloggers of cookie stealers). Deze methode wordt vooral uitgevoerd door middel van commentaar. Als je als commentaar “<script>alert(‘Hacked’);</script>” invoert op een onbeveiligde webapplicatie, dan komt bij iedere bezoeker die de pagina bezoekt het berichtje “Hacked” naar voren.


Wat is hacken nou eigenlijk en wat is de definitie van een hacker?
In het algemeen is hacken het vinden van een toepassing van bijvoorbeeld een object, voor iets waar het eerst niet voor bedoeld was. Bijvoorbeeld een paperclip gebruiken als boekenlegger, of het plaatsen van een veertje in een deuropening om later te kunnen zien of iemand je kamer binnengekomen is, zijn technisch gezien hacks.
Door de meeste mensen wordt de term “Hacken” ten onrechte aangezien voor bijvoorbeeld het illegaal binnendringen van een computersysteem, daaruit informatie te halen of codes in te voeren, en allerlei andere illegale activiteiten uit te voeren.

Een hacker, als in bij het onderwerp “Computers”, is iemand die op een obscure manier een computer, applicatie, computernetwerk en dergelijke binnendringt, al dan niet door de beveiliging te omzeilen. Dit gebeurt niet altijd om daden te plegen zoals het verzamelen van gevoelige informatie, maar ook om aan te tonen dat een netwerk onvoldoende beveiligd is of als “sport”. Hierbij gaat een groepje hackers met elkaar wedijveren wie het snelste een bepaald systeem binnen kan komen.
Een hacker kan op verschillende manieren omschreven worden. Bijvoorbeeld:
Iemand die m.b.v. eventuele programma’s, apps en tools een systeem binnen kan komen en die dan de behendigheid heeft om allerlei informatie te lezen en te veranderen.
Iemand die 
Het eerste voorbeeld heeft verschillende groepen met verschillende hoeveelheden ervaring, die we voor nu even klasses gaan noemen. Hieronder een tabel met de namen en een omschrijving:

Beginnende hackers
(Script kiddies)
“Script kiddies” worden door de meeste mensen gezien als amateurs of zelfs nephackers. Zij halen al hun codes van het internet af, en kopiëren en plakken ze regelrecht in de kladblokken en andere tekstverwerkers die ze gebruiken om hun codes in te voeren, waarna ze op het beste hopen en de code uitvoeren.
Gemiddelde hackers
Dit zijn de hackers die wel degelijk iets kunnen. Zij gebruiken meestal voorgeschreven tools, die ze dan zodanig aanpassen dat ze er merendeels hun doel mee kunnen bereiken. Zij kunnen meestal programmeren en weten hoe netwerken, besturingssystemen, radiogolven etc. werken en in elkaar zitten. Ze kennen hun theorie die ze dan toepassen.
Geavanceerde hackers
(Code monkey’s)
Dit zijn de meest geavanceerde hackers. Deze klasse weet hoe computers, netwerken, programmeertalen etc. in elkaar zitten en hoe deze uit te buiten zijn. Zij schrijven meestal hun eigen tools, meestal voor prive gebruik.

De moraliteit van hackers:
De moraliteit van hackers is te verdelen in drie groepen (of hats):

“White hat”
Dit zijn de ethische, professionele hackers die je wel eens in bedrijven ziet werken. Zij worden meestal door bedrijven aangenomen om diens beveiliging te beoordelen. Na afloop van de “Hack sessie” dienen deze hackers een verslag in met alle informatie erin, die ze hebben kunnen vinden. Deze informatie houdt meestal o.a. in: 
wat ze hebben gedaan
welke gebieden van het systeem ze getest hebben
welke fouten en gaten ze hebben gevonden
hoe het bedrijf de gevonden problemen op kan lossen

“Grey/Gray hat”
Dit zijn hackers die niet altijd even ethisch zijn. Zij voeren meestal hacks uit om de juiste redenen, maar op de illegale en onjuiste manier. Een voorbeeld van Grey/Gray hats zijn hackers die hacken voor de burgers van de middenklasse of hackers die informatie vrijgeven op sites zoals wikileaks. Hun methodes zijn illegaal en ‘slecht’, maar hun bedoeling is meestal grotendeels goed.
“Black hat”
Dit zijn de hackers die iedereen voor zich ziet als ze aan hackers denken. De Black hats hacken om slechte redenen, op een illegale manier. Dit zijn de hackers die van banken stelen of de infrastructuur van een bedrijf digitaal slopen, omdat ze het kunnen.





Vóór de les
Planning en ideeën voor de cursus

We moesten een planning maken waarbij we regelmatig bij elkaar konden komen om allerlei dingen voor de cursus te bespreken, en waarin Matej ook de kans kreeg om Mike en Mohamed informatie over hacken te geven. We zagen al snel dat we alle drie de meeste dinsdagen konden, dus werd dat onze vaste dag. Ook werd er afgesproken om af en toe een zaterdag wat meer uurtjes bij elkaar te komen waarbij Mike en Mohamed weer wat meer over hacken leerden van Matej. We moesten ook een aantal keren met meneer Van Dam af zien te spreken, en een mailtje naar de leerlingen van het Cartesius Lyceum sturen waarin we ze uitnodigden voor onze cursus. De les was gepland op dinsdag 1 december. Er zou die dag een verkort rooster waar we rekening mee moesten houden. Het lesuur werd gepland op het zevende en “achtste” lesuur.
Tijdens de keren dat we samen kwamen, bedachten we eerst dat we meerdere ideeën nodig zouden hebben voor de cursus. Uiteindelijk werden dat de onderwerpen “Het binnendringen en beveiligen van een Windows XP systeem” en “Het binnendringen en beveiligen van een webapplicatie”. We wilden twee uren achter elkaar les geven, om zo genoeg tijd te hebben om beide onderwerpen uitvoerig te kunnen behandelen.
Verder wilden we de leerlingen nog aan het begin van de les, in het midden van de les en aan het einde van de les, een enquête laten invullen, om te zien wat hun mening over hacken in eerste instantie was en of deze zou veranderen tijdens onze les.
Wat moesten wij zélf weten en kunnen:

In ieder geval moest ieder van ons voor het begin van de les zélf weten wat we de leerlingen wilden leren. Hiervoor zou Matej Mike en Mohamed veel leren, en moesten de laatste twee ook zelf op zoek gaan naar informatie. De les zou volgens de planning gaan over het binnendringen van een webapplicatie en een Windows XP systeem. Hiervoor kende Matej verschillende manieren, die hij Mike en Mohamed dus zou leren.
Doelen:
Wat wilden wij de leerlingen leren: De basis van hacken. Dit houdt het uitbuiten van een webapplicatie en een Windows XP machine in. Hieruit volgt direct het leren beschermen tegen hackers.
Wat wilden wij zelf leren: Weten wat de gemiddelde leerling van het Cartesius vindt van hacken, en wat zij denken dat hacken is. Verder is het ook goed voor Mike en Mohamed om van alles te leren over hacken. Matej heeft er baat bij Mike en Mohamed te leren over hacken, doordat hij er extra ervaring als leraar van krijgt.
Ná de les
Wat is er gebeurd?
We hebben in de afgelopen weken een aantal keren met elkaar afgesproken. Een aantal keren konden we met zijn drieën bijeenkomen, maar helaas was Mohamed een aantal keren ziek. Verder waren Matej en Mike er een enkele keer niet. Met meneer Van Dam zijn wij helaas maar één keer met zijn allen samengekomen..
Bij de keren dat Matej en Mike met meneer Van Dam waren samengekomen hebben ze wel een aantal dingen af kunnen spreken. Onder andere over het eerder genoemde onderwerp over de benaming van de cursus, maar ook over wat slim zou zijn en wat niet. Meneer Van Dam vulde ook nog de ideeën aan die wij zelf hadden bedacht. Eerst wilden wij bijvoorbeeld alleen mensen aannemen die zelf computers hadden, maar meneer Van Dam bracht ook op dat we de schoolleiding konden vragen of we de schoolcomputers mochten gebruiken voor de les. Hij heeft ook geholpen met het bedenken van hoe we de mail zouden moeten opstellen aan de leerlingen van het Cartesius Lyceum.

(On)Bereikte doelen
We hebben uiteindelijk de les gegeven, en het meeste van wat we de leerlingen wilden leren hebben we met ze kunnen behandelen. We begonnen met het uitleggen over hoe ze een webapplicatie konden binnendringen. De uitleg en de voorbereidingen van de les liepen helaas uit, waardoor we niet meer toe kwamen aan het uitleggen over het binnendringen van een Windows XP systeem.
De enquêtes waren grotendeels ingevuld. Alleen de laatste enquêtes niet, want doordat de les uitliep konden we niet alles bespreken. Sommige leerlingen moesten weg, maar er bleven een paar die de enquêtes wel invulden. Na de les heeft Matej nog een mail gestuurd naar de leerlingen, waarin de overige informatie stond in de vorm van een korte uitleg en links naar websites die er informatie over verstrekken.









Logboek
Datum
Activiteit
Mike W (54,5)
Matej (67.5)
Mohamed E (37,5)
22-09-2015
Met elkaar in de kantine gezeten, besproken wat er gaat gebeuren en veel geleerd over commando’s in linux.
4
4
4
23-09-2015
Matej zoekt in de tussentijd naar websites, digitale stof/media en andere bronnen die hij Mohamed en Mike kan sturen om over hacken te lezen en te leren.


3


07-10-2015
Met elkaar gezeten waarbij Matej Mike wat leerde over hacken. Mohamed moest nog wat voor informatica doen.
2,5
2,5


27-10-2015
Met elkaar gezeten achter de computer waarbij Matej Mike weer wat meer leerde over hacken. Mohamed was ziek.
1,5
1,5


03-11-2015
Deze keer waren we er alle drie, en Matej leerde Mike en Mohamed weer wat over hacken.
3
3
3
04-11-2015
In de tussentijd zoeken Mohamed en Mike op het internet naar informatie over hacken, bijvoorbeeld over het onderwerp “SQL-injection”.
3


3
07-11-2015
Met z’n drieën de halve dag bij elkaar gezeten in de bieb, waarbij er nagadacht werd over de PWS.
6
6
6
17-11-2015
Gesprek met begeleider, Matej was ziek en Mohamed werd door de docent geroepen om iets voor Engels te doen.
1






Ondertussen hebben Mohamed en Mike thuis wat gedaan. Mohamed deed wat met CMD toen hij ziek was, en Mike zocht allerlei informatie op over hacken.
1.5


3
24-11-2015
Even met meneer Van Dam gesproken, maar helaas was Mohamed ziek, dus afspraak is verplaatst naar 25-11. Daarna praatten Matej en Mike verder over de komende cursus. Mike heeft later nog wat thuis gedaan en opgezocht over kali linux en SQL injection en Matej heeft de hele avond aan de PWS gewerkt en gezocht naar websites die hij Mike en Mohamed op kon sturen.
3.5
5




In de tussentijd is Mike bezig om van alles te proberen met kali linux, die hij op een CD te leen heeft gekregen van Matej.
2.5




25-11-2015
Matej begon om half 11 te werken aan de PWS. Ondertussen hadden Mike en Mohamed nog les. Om kwart voor twaalf begon ook Mike te werken aan de PWS, Mohamed kwam later pas. Deze dag hebben we ook meneer Van Dam gesproken, en een mail ter uitnodiging geschreven aan leerlingen uit de vijfde en zesde leerjaren.
4
6
3,5
28-11-2015
Na even op zoek te zijn gegaan naar USB’s en DVD’s, waren we in de oba samengekomen om de webapp exploitation en beveiliging nog een keer door te nemen. Ook hebben we het binnendringen en beveiligen van Windows XP nog eens behandeld.
4
4
3,5
29-11-2015
Matej begon om half 9 met het opzetten van de webapplicatie die gebruikt gaat worden tijdens de cursus. Daarna werkte Matej verder aan de aangepaste linux systemen die tijdens de cursus gebruikt gaan worden.


14


30-11-2015
Matej heeft de linux iso’s op de usb flash drives en dvd’s gebrand, na de linux distributie nog verder te hebben aangepast.


7


1-12-2015
Na het lokaal met zijn allen te hebben voorbereid, gaven wij de cursus aan de leerlingen.
3
3
3
8-12-2015
Mike werkt aan het verslag van de PWS, of de conceptversie er van. 
6




30-11-2015
Mohamed heeft de enquete gemaakt en werd verbeterd en geholpen door Mike. Mike en Matej hebben vervolgens de ppt gemaakt voor de cursus.
3
3
2


10-12-2015
Mike, Matej en Mohamed zitten aan  het verslag te werken.
3.5
3,5
3,5
11-12-2015
Mike, Matej en Mohamed zitten aan  het verslag te werken.
3
2
2
19-01-2015
Mike, Matej en Mohamed zitten aan het verslag te werken.


?
?
?










Bronnen:
Internet:
Guldberg, K. (2014). So you want to be a Hacker. Retrieved October 1, 2015, from 
https://www.linkedin.com/pulse/20140914093124-8752964-so-you-want-to-be-a-hacker?trk=prof-post&trk=prof-post

Guldberg, K. (2014).So you want to be an Offensive security Guy or a Defensive security Guy? Retrieved October 11, 2015, from  https://www.linkedin.com/pulse/20141113184204-8752964-so-you-want-to-be-an-offensive-security-guy

Guldberg, K. (2014). Hacking myth dispelled - Hacking secrets revealed. Retrieved October 11, 2015, from  
https://www.linkedin.com/pulse/hacking-myth-dispelled-secrets-revealed-kim-guldberg

Wikipedia: https://nl.wikipedia.org/wiki/Hacker

Sql-injection
http://www.dvwa.co.uk/
http://www.w3schools.com/sql/sql_injection.asp
http://null-byte.wonderhowto.com/

Boeken:
Ebbens, S. & Ettekoven, S. (2013). Effectief leren: basisboek. Groningen: Noordhoff Uitgevers.
Baloch, R. (2015). Ethical Hacking and Penetration Testing Guide. London: CRC Press.
''Computernetwerken - James Kurose''
Kurose, J. F. & Ross, K. W. (2002). Computernetwerken: een ‘top-down’-benadering. Boston: Addison-Wesley.

Digitaal materiaal:
Basis Kali Linux: http://kali.org/
Damn Vulnerable Web Application: http://www.dvwa.co.uk/
Apache: https://www.apache.org/
VirtualBox: https://www.virtualbox.org/
Metasploit: https://www.metasploit.com/











Nawoord
Een profielwerkstuk maken is redelijk lastig. Om de onderzoeksvraag goed te beantwoorden moesten we een aantal aspecten onderzoeken en informatie verzamelen van de enquêtes. Eerst wisten we niet zo goed aan welke eisen een profielwerkstuk moest voldoen, dus we begonnen meer aan de theoretische kant. Een deel van de profielwerkstuk moest wel praktisch zijn. Dat werd  helder gemaakt door de meneer Van Dam, onze begeleider. Een onderzoek uitvoeren en informatie verzamelen zijn eigenlijk twee dingen die samen veel tijd in beslag nemen. Mohamed en Matej willen allebei Computer Science studeren en deze profielwerkstuk helpt ze een eindje ver weg.

Conclusie


