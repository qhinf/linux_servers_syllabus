# De module Linux en servers

Dit stukje moet nog geschreven worden.

# Eindopdracht blok 3, 2024

Je mag in tweetallen werken aan de opdrachten, geef in zo'n geval wel aan wie wat gedaan heeft voor de beoordeling.

## Doe en onderzoek iets rondom linux

Als je kiest voor deze module, dan heb je vast wat verwachtingen van linux en servers.
Dat ga je, met hulp van je docent, onderzoeken en bekijken.

## Wat lever je in

Als je iets gaat doen, dan lever je een documentje in van ongeveer 500 tot 1000 woorden (iets meer mag ook, maar het hoeft geen compleet boekwerk te zijn).

Daarin beschrijf je:

- Inleiding: Dit bevat het DOEL dat je wil bereiken en misschien een beetje waarom.
- Onderzoek: Wat had je nodig om het doel te bereiken, welke bronnen heb je gebruikt.
- Verslag: Wat heb je gedaan en wat was je ervaring. Screenshots zijn hier heel welkom!
- Samenvatting / Conclusie: Heb je bereikt wat je wilde bereiken? Wat was lastiger of makkelijker dan je dacht?

Als je iets gaat doen, dan lever je een documentje in van ongeveer 500 tot 1500 woorden (meer mag, maar het hoeft geen boek te zijn... ).

Daarin beschrijf je:
- Inleiding: Dit bevat de centrale VRAAG die je wil beantwoorden en misschien een beetje waarom dat je interesse heeft.
- Onderzoek  en resultaat
	- Hoe heb je je onderzoek aangepakt. Waar ben je begonnen met zoeken en waar kwam je uit. Bronnen zijn hier heel erg belangrijk.
	- Met wat je gevonden hebt, wat is het 'verhaal', wat is het resultaat van je onderzoek.
- Samenvatting / conclusie: Is je centrale vraag beantwoord, en wat was het antwoord. Was het eenvoudig te vinden, heeft bijvoorbeeld ChatGPT je goed op weg geholpen of juist een verkeerde kant op gewezen.


# Voorbeelden geschreven door de docent

## Command line fun

[Command_line_fun.pdf](Command_line_fun.pdf)

## Bestanden en permissies

[Voorbeelduitwerking-bestanden-en-permissies.pdf](Voorbeelduitwerking-bestanden-en-permissies.pdf)




# De Linux Kernel ('oude' info)

## Over de module

### Wat beheers je aan het eind

Na het afronden van deze module ben je een gevorderde met Linux. Je kan
met gemak je weg vinden op de command line en servers beheren. Ook kan
je een systeem helemaal inrichten zoals je voor ogen hebt.

### Hoe wordt dat bereikt

Het leren van de stof middels deze module is vooral pragmatisch gericht.
Het is de bedoeling dat je veel uitprobeert en buiten de stof om kleine
projecten opzet. Voorbeelden van deze projecten staan aan het begin van
elk hoofdstuk, met meerdere moeilijkheidsgraden.

Als je stof al kent, werk dan vooral niet nog een keer de stof door.
Zorg er wel voor dat je alle oefeningen doorkomt en terugvalt op de stof
als dat niet lukt. Deze module is om je bij te leren, niet om je te
vervelen.

Mocht je meer willen weten dan besproken wordt in deze module, blader
dan naar Appendix A voor links. In het geval van een probleem, kan je
deze bespreken in Microsoft Teams.

### Format

Elk hoofdstuk is aangeduid met een letter ervoor. Een P betekent een
praktisch hoofdstuk met 3 keuze-projecten of meerdere opgaven aan het
eind. Een T staat voor theoretisch hoofdstuk en zal alleen theorie
bevatten.

## Kennismaking

### Met elkaar

Ga in 2 rijen staan tegenover elkaar. Stel je voor en stel daarna 3
vragen. 1 persoonlijke vraag, 1 vraag over de favoriete bezigheid en 1
vraag hoeveel ze al van Linux weten.

### Met Linux en het belang ervan

Je kent Linux misschien niet, maar je bent er zeker wel in aanraking mee
gekomen. Elke website die je bezoekt draait in de achtergrond een of
meerdere Linux server om de pagina te leveren. Vrijwel elke grote game
server draait ook Linux.

Sterker nog, zelfs als je geen enkele website hebt bezocht of games
gespeeld, kan je nog in aanraking met Linux geweest zijn. Elke Android
telefoon draait namelijk ook een vorm van Linux.

Linux is overal. In de informatica wereld telt het spreekwoord
*Ignorance is bliss* niet. Informatie staat centraal, daarom is het
belangrijk om te weten wat er om je heen is en hoe het werkt. Als een
leuke bonus, hoe vet zou het zijn om het zelf te kunnen beheren en
controleren?

### Inspirerende personen en groepen rond Linux:

| Naam | Functie |
| ----- | ----- |
| Linus Torvalds | De ontwerper en hoofd codeschrijver van Linux. |
| Nederlandse Linux Gebruikers Groep (NLLGG) | Grootste vereniging voor Linux enthousiasten in Nederland. |
| TransIP | Nederlandse VPS (Virtual Private Server) provider. |

## T: Wat is Linux

### Kernel

Linux is geen besturingssysteem, zoals velen denken. Het is een kernel.
Een kernel is de basis en het centrum van een besturingssysteem. Deze
doet al het werk achter de schermen, zoals bijvoorbeeld het efficiënt
indelen van RAM (ook het toewijzen van RAM aan programma’s), het laten
werken van een muis en ervoor zorgen dat I/O werkt (Input / Output,
harde schijven en andere manieren van data-opslag en uitlezen).

Een kernel zorgt er ook voor dat een besturingssysteem op verschillende
hardware gedraaid kan worden. Zonder kernel is een besturingssysteem
alleen voor een specifieke set van hardware. Dan werkt het dus alleen op
de processor waarvoor het geschreven is en heeft het alleen drivers voor
die set hardware.

Programma’s worden ook gemaakt voor een kernel, om dezelfde reden. Een
programmeur heeft natuurlijk het liefst dat zijn programma werkt op alle
apparaten, niet alleen die van hem. Het is moeilijk genoeg om een groot
programma te schrijven, laat staan apart schrijven voor alle processors
die ooit gemaakt zijn.

Andere kernels zijn bijvoorbeeld de Windows NT kernel (voor Microsoft
Windows) en de XNU kernel (voor alle Apple besturingssystemen: iOS,
macOS, tvOS etc).

De Windows NT kernel verscheen voor het eerst met Windows NT 3.1 (het
besturingssysteem). Daarvoor gebruikte men DOS, een besturingssysteem
zonder (geavanceerde) kernel. DOS was inefficiënt en onveilig hierdoor,
maar er was destijds geen internet dus dit was nog geen groot probleem.

### Open Source

Misschien heb je al gehoord van de term Open Source. Een programma die
open source geschreven is, heeft de broncode vrij uitgegeven. Mensen
kunnen dan te allen tijde kijken wat het programma doet, en zelf
aangepaste versies maken van het programma.

Dit kan natuurlijk snel juridisch ingewikkeld worden met copyright en
dat soort zaken. Hiervoor is de GPL licentie ontwikkeld. Elk open source
project wat onder de GPL licentie gemaakt is, is vrij om aangepast te
worden zolang het nieuwe product ook open source is. De GPL licentie is
een vorm van een ‘copyleft licentie’, wat het vrij delen van kennis en
samenwerken onder ontwikkelaars stimuleert.

Linux is ook open source. Iedereen is vrij om zijn eigen versie te maken
van Linux, en daarna uit te delen of te verkopen.

### Besturingssystemen met Linux

Een besturingssysteem die Linux gebruikt als kernel, wordt een Linux
distro (korte versie van distributie) genoemd. Er zijn ontzettend veel
Linux distro’s, waarvan de meest bekende Debian, Fedora en Ubuntu zijn.
Met Ubuntu wordt kennis gemaakt iets verder in de module.

Bijna elke Linux distro is kosteloos verkrijgbaar. De meest bekende
commerciële distro’s van Linux, komen van Red Hat. Hier krijgt de klant
24/7 support en is gegarandeerd van een veilig systeem (updates worden
tegengehouden en meerdere maanden gecontroleerd voordat de gebruiker ze
krijgt).

Er is ook een veel bekendere aangepaste versie van Linux die je
misschien zelf al gebruikt: Android. De ‘aangepaste versie’ hier is om
het zo licht mogelijk te maken voor telefoons om uit te voeren. Hier
wordt de telefoon sneller van en kan ook zwaardere applicaties
uitvoeren.

## T: Geschiedenis van Linux

### Unix

In den beginne was Unix. Een van de eerste commerciële
besturingssystemen met een (geavanceerde) kernel. Unix is gemaakt door
AT&T’s Bell in 1969. Een van de fundamentele dingen van Unix is dat
alles behandeld kan worden als bestand. Een printer bijvoorbeeld, was in
Unix een bestand op een vaste plek. Als er data gekopieerd werd naar dit
bestand, werd het uitgeprint. Dit zorgde ervoor dat Unix ontzettend
makkelijk was in gebruik en om programma’s voor te schrijven.

De hoofd Unix filosofie is dat ieder programma een specifieke taak
heeft. Het Unix besturingssysteem is dan ook erg modulair en heel erg
aanpasbaar. Unix bestaat uit de centrale Unix kernel die de hoofd
programma's uitvoerde, en de hoofd programma's zelf. Een voorbeeld van
zo’n hoofd programma is de shell, waar we zelf kennis mee gaan maken
iets verder in de module.

Na een aantal lange jaren, werden er veel aangepaste versies gemaakt van
Unix. Zo ontstonden BSD en Linux. Een aangepaste versie van BSD werd
later overgenomen door Apple, waar XNU geboren werd.

Waar de grootvader van besturingssystemen rond
de 100.000 regels aan code had, hebben de modernere versies zoals Linux
rond de 13 miljoen regels. De modulariteit van Unix is nooit weggehaald
en wordt nog steeds gebruikt, het ‘alles is een bestand’ principe ook.

### Linux

Linux is geschreven door een Finse student als zijproject tijdens zijn
studie. Hij had nooit verwacht dat het zou uitgroeien naar de grootte
die het tegenwoordig heeft. Deze man, heet Linus Torvalds. In 1991,
begon Linus’ interesse in besturingssystemen en raakte gefrustreerd met
MINIX (mini-Unix), omdat het gelicenseerd was voor educatief gebruik wat
het beperkt maakte voor Linus om te kijken hoe het werkte.

Linus begon toen te werken aan zijn eigen OS, waarvoor hij de Linux
kernel schreef. Hij wou de kernel eerst Freax noemen, wat een combinatie
is van ‘free’, ‘freak’ en ‘x’ (Unix). Hij vond de naam Linux te
egoïstisch, maar dankzij Ari Lemmke (Linus’ collega-student) is het toch
Linux geworden. Ari heeft namelijk het project hernoemd zonder dat Linus
het destijds wist, Linus is uiteindelijk toch overtuigd en noemde zijn
project ‘Linux’.

### Commercieel Linux

In het midden van de jaren 90 werd Linux vooral gebruikt onder
hobbyisten. Dit veranderde toen NASA hun dure computers vervingen en
clusters van goedkopere Linux computers maakte. Hier kreeg Linux meer
bekendheid van, waardoor HP, Dell en IBM Linux commercieel begonnen aan
te bieden om de monopolie van Microsoft Windows tegen te gaan. Linux is
vooral het meest bekend geworden toen Google het verwerkte in Android.

Hier rechts is een logo van Red Hat Enterprise Linux (RHEL). Een Linux
distro met 24/7 support en extreem veilige packages.

Tegenwoordig is Linux de marktleider op het gebied van servers en
supercomputing.

## P: Testomgeving creëren

Het is nu tijd om zelf aan de slag te gaan met Linux. De mensen die al
Linux op hun computer hebben staan in plaats van Windows of macOS kunnen
dit hoofdstuk overslaan.

We gaan eerst beginnen met een Linux distro die een grafisch interface
heeft. Hiervoor is Ubuntu het makkelijkst in gebruik en om te leren.

Om te voorkomen dat je volledige Windows installatie vervangen moet
worden met Ubuntu, wordt er een virtual machine gemaakt. Een virtual
machine is een manier om een OS volledig afgesloten van je ‘host’ (de OS
op je systeem) uit te voeren.

Refereer aan de
[*Installatiehandleiding*](https://drive.google.com/open?id=1hf4DXpMUwo_HzEFQshI-zT1xZSlPW-F1PfYUU26aoWQ)
hoe je deze testomgeving creëert.

### Verschillen waar je rekening mee moet houden

Je hebt nu je eigen testomgeving gemaakt waar je vrij alles kan
proberen. Ga vooral los en ontdek Ubuntu zo veel als je kan.

Ubuntu is wel compleet anders dan Windows en macOS. Bij Ubuntu is er
bijvoorbeeld niet één systeemupdate, maar allemaal kleine
systeemprogramma’s die een update hebben.

Ook worden programma’s anders geïnstalleerd. Ubuntu werkt met een
‘package manager’: Aptitude. Een package manager installeert de
programma’s voor je zonder dat je je zorgen hoeft te maken of je wel een
juist programma binnenhaalt. Zo ben je altijd zeker dat je het juiste
programma hebt, en dat er geen virus gedownload wordt. Ook maakt dit het
installeren van het programma erg makkelijk.

Om de package manager zo gebruiksvriendelijk mogelijk te maken heeft
Ubuntu een App Store. De App Store is een grafische applicatie die dient
als versimpeling van de terminal-applicatie Aptitude.

### Opdrachten

Zorg dat je je weg een beetje rond Ubuntu weet. Probeer daarna of je dit
kan.

1)  Installeer systeemupdates.
2)  Installeer VLC uit de App Store.
3)  Voeg VLC toe aan je Dock.
4)  Maak een nieuwe gebruiker.
5)  Sluit de VM af (van binnen Ubuntu).
6)  Maak een Word document.

## P: Werken met de terminal

Mocht je de VM niet werkend hebben gekregen in de vorige paragraaf, kijk
eerst naar P: Introductie met Servers --> SSH om te kijken hoe je met
de server verbind. Zodra je verbonden bent zit je op een terminal en kan
je hier verder.

### Shell

Wanneer je een terminal opent binnen Linux, wordt er een speciaal
programma gestart zodat je kan ‘communiceren’ met het systeem. Dit
programma wordt de shell genoemd, waarvan de meest bekende de **B**ourne
**A**gain **SH**ell is (**bash**).

Er zijn ook veel andere soorten shells die verschillende functionaliteit
bieden. De oudste is simpelweg Shell (**sh**), maar deze wordt amper
gebruikt op moderne systemen. De meest moderne shell is zsh. In deze
module leer je bash, maar je kan zelf altijd een shell later kiezen.

### De Basis

#### Hoe navigeer je

De terminal kan er heel moeilijk uitzien in het begin, maar dit valt mee
zodra je er mee leert werken. Een van de eerste dingen die je wil weten,
is hoe je van map verplaatst en zien wat er in die map zit.

Het navigeren gebeurd met het commando `cd`. Dit staat voor ‘Change
directory’ en wordt gevolgd met de map die je wil bezoeken. Als je een
map ‘Downloads’ in je home folder hebt, kan je bijvoorbeeld naar die map
door `$ cd ~/Downloads` te doen. (`~` is een alias voor je home folder).

Om direct twee mappen diep te gaan, gebruik je een `/`. Een slash is een
bijzonder karakter en kan dus niet gebruikt worden in bestandsnamen. Zit
er een map ‘Drivers’ in je ‘Downloads’ map, dan doe je dus
`$ cd ~/Downloads/Drivers`.

Je shell werkt met een working directory. Dit is de map waar de shell
zich in bevindt. Je kan dat zien aan de text voor je username in de
prompt. Om het volledige pad van je working directory te printen,
gebruik je `pwd` (**p**rint **w**orking **d**irectory). Als er een map
‘Memes’ in je working directory zit, kan je daar naar toe gaan met
`$ cd Memes` (hier dus niet de `~` omdat de map ‘Memes’ niet in je home folder
zit.) Als je een map begint met `/`, dan wordt er gekeken vanaf het begin
van de schijf (ook wel de root folder genoemd).

#### Welke bestanden zitten er in een map

Om te zien wat er in een map zit, gebruik je het `ls` commando (list).
Zonder argumenten levert ls wat er in je working directory zit. Wil je
de inhoud van een andere map bekijken, dan kan je een map leveren als
argument. Zit je in de map `/boot`, dan kan je je home folder bekijken met
`$ ls ~/`.

Wanneer je alle inhoud van een map wil zien (inclusief geheime
bestanden) dan kan je de optie `-a` toevoegen aan ls. Als je de output als
lijst wil zien met een map op elke rij, dan kan je `-l` toevoegen. Dus als
je alle bestanden wil zien als lijst, doe je `$ ls -a -l`, wat je kan
verkorten naar `$ ls -al`.

Mappen maken doe je met het mkdir commando. Deze heeft alleen een
mapnaam nodig als argument. Om een map ‘test’ te maken, doe je dus
`$ mkdir test`. Ook kan je direct een submap maken samen met een
hoofdmap. Dit doe je met de `-p` optie. Dan wordt het commando dus:
`$ mkdir -p test/submap`

#### Bestanden bewerken en maken

Om een leeg bestand te maken in een map, gebruik je het `touch` commando.
Dit is een van de simpelste commando’s die er is. De syntax is hetzelfde
als het `mkdir` commando.

Om een textbestand te bewerken, moet je een editor gebruiken. Op Linux
is altijd vi standaard geïnstalleerd, maar deze is zeker niet
gebruiksvriendelijk. Daarom gebruiken we in deze module
`nano`. Om een bestand te bewerken met nano, doe je:
`$ nano <bestand>`. Vervolgens kom je in de editor terecht en kan je direct
typen. Om een zin te knippen gebruik je Control + K. Om het weer te
plakken daarna gebruik je Control + U. Je kan net zo vaak plakken als je
wil.

Om het bestand op te slaan doe je Control + O. Om nano af te sluiten,
doe je Control + X. Nano vraagt ook of je het bestand wil opslaan (als
je dat nog niet gedaan had), wanneer je nano verlaat.

Het touch commando wordt vooral gebruikt om te kijken of je genoeg
rechten hebt in een map om bestanden te kunnen maken. Als je met touch
geen bestand kan maken, kan je ook geen bestanden bewerken in die map of
mappen aanmaken.

#### Bestanden lezen

Om een bestand snel uit te lezen gebruik je cat. De syntax is als volgt:
`$ cat <bestand>`. Heb je een te groot bestand waardoor het niet
helemaal op je terminal past, gebruik je less. `$ less <bestand>`
zorgt ervoor dat je kan scrollen in het bestand met de pijlen op je
toetsenbord.

#### Informatie over een programma krijgen

Het komt vaak voor dat je wil weten hoe een programma precies werkt of
hoe je het moet gebruiken. Linux komt met een ingebouwde handleiding
waar programma’s zelf pagina’s in zetten over hoe ze gebruikt moeten
worden. Als je in C programmeert kan je in dezelfde handleiding ook
informatie opvragen over functions.

Deze handleiding is te bereiken met het `man` commando. Dit staat voor
manual. De syntax is `$ man <commando/function>`. Dus als je
informatie wil opvragen over het nano commando, doe je `$ man nano`.

#### Uitvoeren als administrator

Er zijn sommige programma’s die hogere rechten nodig hebben om te
functioneren. Om deze reden is het handig als je eigen gebruiker die
rechten kan verlenen. Hiervoor gebruiken we `sudo`. Sudo is een klein
programmaatje wat een ander programma uitvoert als administrator,
waardoor het de rechten heeft die het nodig heeft.

De syntax is simpel: `$ sudo <programma>`.

#### Output filteren

Soms wil je niet alles lezen wat een programma je geeft, maar heb je
slechts een specifiek deel nodig. Hiervoor kan je grep gebruiken. Grep
is een commando die output filtert aan de hand van een input string. De
input string wordt of gezien als letterlijke match (zonder caps) of als
een regex. Vaak heb je alleen de letterlijke match nodig.

In `/etc/passwd` staan alle gebruikers die het systeem heeft. Stel je wil
alleen je eigen gebruiker zien, dan gebruik je dus
`$ grep <gebruikersnaam> /etc/passwd`.

### Package Manager

#### Package manager?

Een package manager is een programma die andere programma’s installeert.
Deze programma’s worden gebundeld in een installatie-pakketje die een
package wordt genoemd. In het geval van Debian Linux wordt `apt` gebruikt.
Omdat Ubuntu van Debian afstamt, wordt ook in Ubuntu `apt` gebruikt.

In verschillende Linux distributies worden ook verschillende package
managers gebruikt. Zo heb je in Arch Linux `pacman` (kort voor package
manager) en in Red Hat (CentOS, Fedora, RHEL) `yum`.

#### Installeren

Het installeren van pakketten is super makkelijk. Het commando gaat als
volgt: `$ sudo apt install <pakket>`. Om te zoeken naar het pakket
wat je nodig hebt, gebruik je `$ sudo apt search <pakketnaam>`.

#### Verwijderen

In apt zijn er twee manieren van verwijderen. Een waar alle bestanden
worden verwijderd die het programma meebracht tijdens installatie (zoals
configuratie bestanden etc) en een waar alleen het programma zelf wordt
verwijderd.

De eerste wordt een ‘purge’ genoemd en doe je als volgt:
`$ sudo apt purge <pakket>`. De ander heet een ‘uninstall’ en wordt gedaan
met `$ sudo apt remove <pakket>`.

In de meeste gevallen wil je een purge doen.

#### Pipes en andere operators

In Bash en andere POSIX (centrale afspraken voor hoe een
besturingssysteem ingericht hoort te zijn) shells, kan je meer dan
alleen commando’s uitvoeren. In elk programma heb je 3 streams, de input
stream, output stream en error stream. Je kan de output van een
programma stoppen in de input stream van een volgend programma.

Dit doe je met een pipe operator: `|`. Zo kan je bijvoorbeeld een apt
search doen waar je kan scrollen door de output met less:
`$ sudo apt search vlc | less`. Dan is het net voor het tweede programma of je die
input zelf hebt getypt. In een Python script waar input() wordt
gebruikt, kan je met een pipe operator dit dus automatiseren.
`$ echo "John" | python3 -c "print(‘Hello ‘ + input())"`, zal "Hello John"
outputten.

Als je wel de output van een programma wil, maar niet door wil geven aan
een ander programma maar wil opslaan als bestand gebruik je de `>`
operator. Deze werkt exact hetzelfde als de pipe operator, alleen bij
deze geef je een bestand om de output naar te schrijven als tweede
helft. Bijvoorbeeld: `$ echo "I am a file" > file.txt`. Als je de
output wil **toevoegen** aan een bestand ipv het bestand vervangen met
de output, gebruik je twee `>`. Bijvoorbeeld:
`$ echo "I am the second line in a file" >> file.txt`

Ook kan je een commando uitvoeren als een ander commando succesvol is
uitgevoerd. Dat doe je met de `&&` operator.
`$ echo "test" && echo "worked!"`. Dit werkt omdat `echo "test"` een status code van 0
teruggeeft, wat succesvolle uitvoering betekent. Elke code anders dan 0
is een foutmelding.

Er is ook een manier om commando’s te chainen op dezelfde manier, maar
onafhankelijk van of het eerste commando goed ging of niet. Dat doe je
met een puntkomma: `;`. Bijvoorbeeld `$ cat /etc/shadow; echo "I ran!"`.
Normale gebruikers hebben geen toegang tot /etc/shadow, dus dit geeft
een access denied (andere statuscode dan 0), toch voert bash het andere
commando ook uit. Probeer dit ook met een `&&,` je zal zien dat het tweede
commando dan niet uitgevoerd wordt.

Ook is er een `||` operator. Deze wordt alleen uitgevoerd als het eerste
commando niet succesvol ging. Dit zie je echter niet vaak terug in een
commandline, maar meer in de shell scripts.

#### Command substitution

Het komt ook voor dat je de output van een programma wil gebruiken als
argument bij een ander programma. Hier komt command substitution om de
hoek kijken. Hier vervang je een deel van je originele commando met de
output van een programma. Dit doe je met `$(<command>)`

Bijvoorbeeld: `$ cat $(echo "/etc/passwd")`. Dit kan ook ingewikkelder
worden door alles aan elkaar te koppelen:
`$ cat /etc/passwd | grep $(whoami)`. Dit commando haalt alleen de informatie van jouw gebruiker
op uit het centrale gebruikersbestand. Dit kan echter als elke gebruiker
uitgevoerd worden en elke gebruiker krijgt zijn eigen informatie te
zien. Dit komt door het whoami commando, die jouw username teruggeeft.

#### Opdrachten

1)  Zorg dat je je comfortabel voelt met navigeren in de terminal.
2)  Maak een tekstbestand aan met text erin.
3)  Installeer een pakket. Bijvoorbeeld Extreme Tux Racer. Kijk daarna
    in je app launcher (het ubuntu logo linksboven) of het
    geïnstalleerd is.
4)  Lees de paragraaf hieronder en gebruik chmod om de permissies van
    een bestand aan te passen.

## T: Permissions

Net als in Windows, heeft Linux ook beveiliging op bestanden zitten. Je
kan niet een bestand bekijken als je niet bevoegd bent hiervoor. De
rechten worden verleend aan 3 gebruikers(groepen): de eigenaar, een
groep gebruikers en alle gebruikers.

Als iemand lid is van de financiën groep, maar niet de eigenaar is van
een bestand, kan deze dus wel de rechten krijgen om bijvoorbeeld een
spreadsheet te bewerken.

### Octaal

Deze rechten zijn 3 cijfers in het octale telsysteem. Dit betekent dat
het grootste getal een 7 is. Dit is in octaal gedaan omdat de rechten
uit 3 sub-rechten bestaan. Lezen, schrijven en uitvoeren. Als je iemand
de rechten wil geven om wel te schrijven en te lezen, maar niet om het
uit te voeren, krijg je in binary 110. Als je dit omzet naar octaal,
krijg je 6.

Hieronder nog wat voorbeelden voor permissions:

| Read | Write | Execute | Octaal cijfer | Betekenis
| --- | --- | --- | --- | --- |
| 1 | 0 | 0 | 4 | Gebruikers van deze permissie kunnen alleen het bestand lezen. |
| 1 | 1 | 1 | 7 | Gebruikers van deze permissie kunnen alles met het bestand. Bewerken, lezen en uitvoeren. Dit is meestal de permission die de eigenaar van een bestand heeft. |
| 0 | 1 | 0 | 2 | Gebruikers kunnen alleen schrijven naar dit bestand. Dit wordt *soms* gebruikt voor programma’s. Je moet echter wel altijd alle permissies aangeven wanneer je ze aanpast. |
| 1 | 1 | 0 | 6 | Gebruikers kunnen alleen lezen en schrijven. Elk bestand wat niet uitgevoerd hoeft te worden heeft meestal deze permission. |

Directories zijn apart. **Deze hebben het execute recht nodig** om
bekeken te kunnen worden met `ls` of `cd`, of andere programma’s.

### Users en Groups

Zoals eerder genoemd, kunnen rechten worden toegewezen aan bepaalde
gebruikers of groepen. Je kan zien wie een bestand `/` map beheerd met
`$ ls -al`. Om een bestand toe te wijzen aan meerdere gebruikers, moet
er een nieuwe groep aangemaakt worden. Het is niet mogelijk om meerdere
eigenaars van een bestand te hebben, ook niet meerdere groepen.

Om dus ervoor te zorgen dat je permissions goed staan, moet je een
aparte groep maken met alle gebruikers die het bestand mogen bewerken.

Gebruikers maak je aan met het `useradd` commando. Om een gebruiker aan te
maken met zijn thuismap, gebruik je de `-m` optie.
`$ useradd -m <username>`. Als je de gebruiker meteen lid wil maken van een
groep, gebruik je de `-G` optie. Met beide bijvoorbeeld:
`$ useradd -m -G mygroup testuser`.

Groepen maak je op eenzelfde manier aan, met het groupadd commando.
Bijvoorbeeld `$ groupadd mygroup`.

Om een bestaande user toe te voegen aan een groep doe je:
`$ usermod -aG <username> <group>`

De `-aG` staat voor '**a**dd to **G**roup'.

### SetUID en SetGID

Er is nog een andere bijzondere vorm van permissions. De SetUID (SUID)
en SetGID (SGID) bit kan ook aangezet worden op bestanden. Hierdoor
wordt een programma uitgevoerd als de gebruiker (SetUID) of de groep
(SetGID), die eigenaar is van het bestand.

Dit werkt niet op shell scripts maar alleen op gecompileerde programma’s
wegens veiligheid. Over het algemeen is het niet aan te raden om
SetUID/SetGID te gebruiken, maar soms is er geen keus. Het ping commando
op Linux bijvoorbeeld, heeft verhoogde rechten nodig om een ICMP pakket
te mogen versturen van de kernel. Deze wordt met SetUID als `root`
uitgevoerd, de centrale hoofd administrator.

### Sudo, Su en Root

Je kan ook zelf (mits je de rechten ervoor hebt) iets uitvoeren of
bewerken als root. Je hoeft je dan nooit zorgen te maken dat je de
juiste rechten hebt, maar dat kan ook verkeerd gaan. Sommige bestanden
worden met verkeerde permissions niet uitgevoerd. Ook systeembestanden.
Wees dus altijd voorzichtig waar je het root account voor gebruikt.

Omdat het zelf gebruiken van het root account geen ‘best practice’ was,
is `sudo` gemaakt. Met sudo kan je een commando uitvoeren als een andere
gebruiker. De naam is een afkorting van ‘Switch User (and) DO’. Om een
commando uit te voeren als root, doe je dus:
`$ sudo <commando> <commando argumenten>`. Om iets te bewerken als root, doe je dus
`$ sudo nano <bestand>`.

Je kan ook wisselen naar een ander account. Daar is het switch user (su)
command voor gemaakt. Net als bij sudo, als er geen user argument wordt
gegeven is de default user root. Je hebt wel het wachtwoord nodig van
het account waar je op inlogt. Dit is dus niet handig om administrator
rechten mee te krijgen. Je kan ook met het sudo commando wisselen van
gebruiker. Hiermee open je een shell als een andere user. Dat kan op
twee manieren. De eerste is de default shell van de gebruiker gebruiken:
`$ sudo -u <gebruiker> -s`. De ander is je eigen shell kiezen en
dat runnen in het command gedeelte van sudo:
`$ sudo -u <gebruiker> <shell (bijv. bash)>`.

### Permissies instellen

Je kan zelf kiezen welke permissions een bestand of map heeft. Dit doe
je met het `chmod` commando. De syntax is
`$ chmod <3 octaalnummers> <bestand/map>`.
Bijvoorbeeld `$ chmod 777 ~/test`:
Hiermee verander je de permissions op de map of het bestand test in je home folder, zodat
iedereen er naar toe kan schrijven en lezen.

De 3 octaalnummers zijn zoals hierboven beschreven op volgorde eigenaar,
groep, iedereen. `750` is dus bijvoorbeeld dat alleen de eigenaar kan
lezen en schrijven, de groep alleen kan lezen en voor de rest niemand
erbij kan.

SetUID en SetGID worden ingesteld na de normale permissions. Dat kan met
`$ chmod u+s <programma>` voor SUID en
`$ chmod g+s <programma>` voor SGID.

## P: Shell scripts

Vele systeembeheerders zitten niet te wachten om veel commando’s na
elkaar te doen, vooral niet wanneer deze vaker dan een keer uitgevoerd
moeten worden. Hier zijn shell scripts voor ontworpen. Dit zijn
tekstbestanden die uitgevoerd kunnen worden. Elke regel in een shell
script wordt uitgevoerd alsof het van de terminal zelf komt.

### De Basis

### Shebang

Om te beginnen moet er een shebang aan de bovenkant van het tekstbestand
staan op regel 1. Dit is de regel die aangeeft met welk programma het
script wordt uitgevoerd. Voor shell scripts moet de shebang een shell
bevatten, maar je kan ook aan de bovenkant van een Python script een
shebang zetten.

De shebang is het volgende format:

`#!<executable>`

Dus in ons geval:

`#!/bin/bash`

### Let the scripting begin

Na een shebang kan op elke regel een ander commando worden gezet. Ook
werken dezelfde operators zoals je gewend bent van de terminal.

Een shell script moet executable gemaakt worden met chmod voordat de
terminal hem kan uitvoeren. Daarna kan je het shell script uitvoeren
met: `$ ./script.sh` (er is dus een bestand genaamd shell.sh die de
commando’s bevat in dezelfde working directory waar de terminal zich
bevindt.)

#### Variabelen

Shell scripts kunnen meer dan alleen losse commando’s uitvoeren. Zo kan
je ook variabelen gebruiken. Wanneer `$ ./script.sh arg1 arg2` op die
manier wordt uitgevoerd, kan je de argumenten gebruiken in het script
zelf. Deze worden dan `$1` en `$2` binnen het script. Zo kan je
bijvoorbeeld een script hebben met:

```bash
#!/bin/bash

echo Hello "$1"
```

Wanneer deze wordt uitgevoerd, zal het het eerste argument teruggeven
met Hello ervoor. Zoals je ziet is `$1` met aanhalingstekens gebruikt.
Dit is zodat de variabele precies zo wordt teruggegeven als je hem
opslaat. Variabelen maak je als volgt:

```bash
#!/bin/bash

name="John"
echo Hello "$name"!
```

Er kunnen geen spaties zitten tussen je variabele naam en het = teken en
ook niet tussen het = teken en je waarde. Een variabele aanroepen doe je
met een dollarteken, gevolgd door de variabele naam. In dit geval
`$name`.

Variabelen kunnen ook de output zijn van een programma. Dat doe je als
volgt:

```bash
#!/bin/bash

username="$(whoami)" # De aanhalingstekens om het als string op te slaan
echo Hello "$username"
```

De username variabele wordt ingesteld met de output van `whoami`, wat
de gebruikersnaam van de huidige gebruiker teruggeeft. Vervolgens wordt
er hallo tegen gezegd.

#### Conditions

Het is ook mogelijk om if statements te doen binnen een shell script.
Hiermee kan je bijvoorbeeld kijken of een bestand / map bestaat of dat
de huidige gebruiker root is.

De syntax is als volgt:
```bash
if [[ "$var1" == "$var2" ]]; then
    do_stuff
fi
```

Als je wil kijken of een map bestaat gebruik je if iets anders:
```bash
if [[ -d /pad/naar/map ]]; then
```

`-d` checkt of het bestand een
map is. `-f` doet hetzelfde maar dan checkt het of het een bestand is.
Wanneer een bestand niet bestaat is de condition niet waar en wordt dus
niet uitgevoerd.

Nummers kan je ook anders laten checken:

```bash
if [[ "$var1" -eq 1 ]]; then
```
checkt of het getal gelijk is aan 1. Zo heb je ook `-gt` voor groter dan, `-lt` voor kleiner dan en `-ne` voor
niet gelijk.

Een condition kan je ook altijd met `!` beginnen zodat het tegengestelde
wordt genomen. Dan wordt gekeken of iets niet waar is. Bijvoorbeeld zien
of een map **niet** bestaat:

```bash
if [[ ! -d /pad/naar/map ]]; then
```
Vergeet niet een if altijd af te sluiten met fi op een aparte regel.

#### Loops

Met shell scripts kan je zelfs loops maken. Dit wordt niet veel gebruikt
maar kan alsnog handig zijn om over bestanden te gaan. Bijvoorbeeld om
alle bestanden te outputten in een map:

```bash
#!/bin/bash

directory="$1"
for file in ${directory}/*; do
    echo "$file"
done
```

De syntax is als volgt:
```bash
for <variabele naam> in <met spatie gescheiden objecten>; do
    do_stuff
done
```

Als je meer wil weten over loops kan je het beste deze bron gebruiken:
[*http://tldp.org/HOWTO/Bash-Prog-Intro-HOWTO-7.html*](http://tldp.org/HOWTO/Bash-Prog-Intro-HOWTO-7.html)

#### Speciale variabelen

Je kan ook zogenaamde environment variables gebruiken in shell scripts.
De meest bekende environment variable is PATH. PATH is een variabele
waar paden zijn opgeslagen waar programma’s in zitten. Zo kan je
`bash` typen in plaats van het volledige pad `/bin/bash` (/bin zit
dus in PATH).

Deze variabelen kan je gebruiken en instellen met behulp van shell
scripts **(zorg dat je alles vierdubbel hebt gecontroleerd voordat je
een environment variabele aanpast).**

Ook kan je de Internal Field Separator (IFS) gebruiken. Dit is een
bijzondere variabele in een script die aanpast hoe loops uitgevoerd
worden.

Bijvoorbeeld met:

```bash
#!/bin/bash

words="my:word is the coolest"

for word in $words; do
    echo "$word"
done
```

krijg je de output:
```
my:word
is
the
coolest
```

Maar als je IFS aanpast:
```bash
#!/bin/bash

IFS=":"
words="my:word is the coolest"

for word in $words; do
    echo "$word"
done
```

Krijg je:
```
my
word is the coolest
```

Nu wordt er dus niet meer op spaties gesplitst, maar op wat er ingesteld
is met de IFS, in dit geval een dubbele punt.

### Opdrachten

1)  Maak een shell script die naam en leeftijds argumenten neemt en ze
    terugschrijft naar de gebruiker.

2)  Maak een shell script die een entry toevoegt aan `/etc/hosts`,
    gegeven door 2 variabelen. Dat
    bestand volgt het volgende format:\
    `<ip> <hostname>`

## P: Introductie met servers

De meeste servers in de wereld draaien Linux. Er is wel een groot
verschil tussen Linux zoals Ubuntu Desktop en Ubuntu Server. Bij Ubuntu
Server heb je bijvoorbeeld helemaal geen nut aan een muis, aangezien er geen
graphical interface is. Alles gaat met de terminal.

Ook hebben de meeste servers andere versies van pakketten dan de
‘normale’ desktop distros. Dit komt omdat servers stabielere en
veiligere software draaien. De nieuwere versies worden eerst getest op
veiligheid en stabiliteit voordat ze gedownload kunnen worden met een
package manager. Bij RHEL is dit testen soms een periode van een vol
jaar.

### SSH

Omdat je als serverbeheerder vaak niet naar de serverkast wil lopen om
daar op een scherm in de terminal dingen aan te passen is er SSH. SSH
staat voor Secure SHell en is een programma waarmee je op afstand kan
verbinden met een server. Je krijgt dan een terminal waarmee je
commando’s kan uitvoeren op de server.

Verbinden met SSH gaat vaak als volgt op een Linux machine en sommige
Windows computers die SSH geinstalleerd hebben (vaak standaard).:

`$ ssh <username>@<host>`

De username is de username waar je op wil inloggen op de server. Host
geeft het ip adres of domein aan waarmee je wilt verbinden. Als je een
server hebt op het ip adres 10.20.10.1 met een gebruiker test en het
poort 52, log je als volgt in:

`ssh –p 52 test@10.20.10.1`

Jullie krijgen zelf een SSH omgeving om op te werken van de docent. Het
verbinden met SSH vanaf een Windows computer kan met het programma
PuTTY. Daar vul je de host in, username en poort. Wanneer je op
verbinden klikt verbind PuTTY met de server en vraagt om je wachtwoord.
Wachtwoorden worden hier niet getoond, maar je typt wel. Je kan ook je
VM gebruiken om met SSH te verbinden op de Linux manier zoals hierboven
beschreven.

### Web Stacks

Webservers werken vooral met Web Stacks. Een web stack is een groep
programma’s / frameworks waarop websites gebouwd en gedeployed worden.
De oudste stack is LAMP en bestaat uit:

-   Linux
-   Apache (De webserver)
-   MySQL (Database software)
-   PHP (Een programmeertaal die draait op de server zelf, maar kan
    worden bestuurd via een website)

Tegenwoordig ligt de focus meer op Javascript. Hier zijn ook veel stacks
van waarvan de meest bekende de MEAN stack is:
-   MongoDB (Database software)
-   Express.js (Framework dat ervoor zorgt dat Javascript ook als
    servertaal gebruikt kan worden)
-   AngularJS (Framework die het maken van de frontend versimpeld.)
-   Node.js (De centrale regelaar van beide frameworks)

## P: Een webserver opzetten

Als eindopdracht gaan jullie een webserver opzetten met behulp van
Nginx. Installeer dit pakket, en bewerk de configuratiebestanden in
`/etc/nginx`. Als inhoud van de website kan je je online CV gebruiken die
je bij Webdesign 1.0 hebt gemaakt.

Zorg dat alles werkt en goed ingesteld is.

Je kan de webserver starten met:
`$ /usr/sbin/nginx -g 'daemon on; master_process on;`

Als je config files hebt aangepast, reload dan Nginx:
`$ /usr/sbin/nginx -g 'daemon on; master_process on;' -s reload`

Voor bonuspunten kan je een web stack gebruiken. Maak dan ook gebruik
van alle functies van de stack.

## Appendix A

[*https://www.kernel.org/*](https://www.kernel.org/)

[*https://www.linux.org/*](https://www.linux.org/)

[*https://www.cyberciti.biz/*](https://www.cyberciti.biz/)

[*https://serverfault.com/*](https://serverfault.com/)

[*https://unix.stackexchange.com/*](https://unix.stackexchange.com/)

[*https://wiki.archlinux.org/*](https://wiki.archlinux.org/)

[*https://tutorials.ubuntu.com/*](https://tutorials.ubuntu.com/)
