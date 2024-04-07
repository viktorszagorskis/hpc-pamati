
---
title: Noderīgi izziņas materiāli
---

<!--
:include-iframe: https://hpc-testi-iframe.netlify.app/ {}

:include-iframe: http://localhost:4200/week-one {}
-->



<!--
```````columns
left:
```card diamond.svg {title: "Card Title", imageHeight: 120, imageBackground: "linear-gradient(to right, rgb(29 41 41), rgb(145, 152, 229))"}
Markdown content goes here

:include-file: snippets/file-name.js 
```

middle:
```card small-book.png {title: "Book", imageHeight: 120}
Markdown content of the card goes here
* item one
* item two
* item three
```

right:
`````card star.svg {title: "API for the Win", imageHeight: 120, imageBackground: "linear-gradient(to right, rgb(154 128 145 / 0%), rgb(255 206 206))"}
Easy to use API
```api-parameters
firstName, String, description with *markdown* support
score, Integer, another description line with *markdown* support
```
`````
````````
-->


<!--
```columns
left: 
### Pros {style: "api"}
* Item One

middle: 
### Undecided {style: "api"}
* Item Two
* Item Three

right:
### Cons {style: "api"}
* Item Four
```
--> 



#  ZINĀTNES JAUNUMI
[Symbolic Calculus for High-performance Computing From Scratch Using C++23 - Vincent Reverdy - CppCon](https://youtu.be/lPfA4SFojao)


# DATU APSTRĀDES ELEMENTI 

> Tabula ar DATU Apstrādes Elementu apzīmējumiem, kas lietoti kursā

:include-table: tables/test.csv 

# DATU KRĀTUVES 

> Tabula ar DATU Krātuvju apzīmējumiem, kas lietoti kursā

:include-table: tables/table.csv 

# DATU TĪKLI 

> Tabula ar DATU Tīklos lietotiem apzīmējumiem, kas lietoti kursā

:include-table: tables/network.csv 

# Eksperimentālā zinātne  
<!-- [Atpakaļ](studijas/ned-1#1-8-k-hpc-ietekm-pasauli) -->

Agrīnā astronomija ir eksperimentālās zinātnes piemērs. Senie astronomi vēroja debesis vispirms ar acīm un pēc tam ar teleskopiem un fiksēja Saules, Mēness, Saules sistēmas planētu un dažu zvaigžņu pozīcijas un kustības. Viņi secināja, ka novērojumi atbilst konkrētiem modeļiem. Līdzīgi mikroskopus var izmantot, lai novērotu nelielu daļiņu nejaušu kustību šķidrumā (Brauna kustība) utt.

Dažādiem eksperimentiem ir nepieciešami atšķirīgi mērīšanas aparāti, un eksperimentu veikšana var būt ļoti dārga vai pat neiespējama. Tomēr eksperimentālo zinātni var uzskatīt par fundamentālo paradigmu: teorijas un datorsimulācijas galu galā tiek apstiprinātas vai noraidītas, pamatojoties uz mērījumiem.

# Teorētiskā zinātne
<!-- [Atpakaļ](studijas/ned-1#1-8-k-hpc-ietekm-pasauli) -->

Pamatojoties uz novērojumiem, var paredzēt saulrieta laiku konkrētai dienai. Novērojumi arī parāda, ka akmens lidojuma laiks ir aptuveni vienāds 
neatkarīgi no tā svara, kad tas tiek nomests no viena augstuma. Ņūtona izstrādātie gravitācijas un dinamikas matemātiskie modeļi spēj radīt 
prognozes ķermeņu kustībai, kas ļoti labi atbilst izmērītajiem rezultātiem.

Novērojumu dati ļauj zinātniekiem tos analizēt un mēģināt tos izskaidrot, aprakstīt ar noteiktām matemātiskām formulām. Parasti vispirms ir 
novērojumi, un tad tiek izstrādāta teorija, lai tos izskaidrotu. Bet ne vienmēr. Piemēram, pirms vairāk nekā 50 gadiem teorētiķi 
Fransuā Englerts (*François Englert*) un Pīters Higss (*Peter Higgs*), lai izskaidrotu masas (matērijas, zvaigžņu, planētu) esamību, 
piedāvāja ieviest jaunu fizikālu lauku, ko tagad sauc par Higsa lauku. 
Pirmo eksperimentālo aptiprinājumu Higsa laukam ieguva tikai 2012. gadā. Savukārt 2013. gadā abi zinātnieki ieguva Nobela prēmiju par savu atklājumu.

# Skaitļošanas zinātne

<!-- [Atpakaļ](studijas/ned-1#1-8-k-hpc-ietekm-pasauli) -->

Ir ierobežojumi tam, ko var izdarīt ar pildspalvu un papīru vai kādus eksperimentus var veikt.

Piemēram, turpinot astronomisko tēmu, ir pietiekami vienkārši pierakstīt vienādojumus, kas raksturo Saules, Mēness un Zemes kustību. Šī ir tā sauktā trīs ķermeņa problēma, salīdzinoši vienkārša vienādojumu kopa, kuru tomēr nevar atrisināt analītiski, lai iegūtu iesaistīto debesu ķermeņu pozīcijas. Tomēr skaitliski var atrast aptuvenu risinājumu.

Līdzīgi var apskatīt klimatu un ledājus: ir ļoti svarīgi zināt, kas ar tiem notiks nākotnē. Bet, protams, mēs nevaram veikt eksperimentus globālā mērogā, lai to noskaidrotu. Tāpat daudzos gadījumos nepieciešamie eksperimenti būtu pārāk dārgi, pārāk bīstami, pārāk lēni, pārāk grūti vai sarežģīti, neētiski utt.

Tomēr mēs varam iegūt priekšstatu par procesiem, lietojot skaiļošanas zinātni. Skaitļošanas zinātnē parasti sarežģītus matemātiskus modeļus, kas apraksta problēmu, risina, izmantojot skaitliskus algoritmus, kurus pēc tam realizē kā datorprogrammas, ko darbina superdatoros. Skaitļošanas zinātnes uzdevuma realizēšanu var raksturot ar sekojošiem soļiem:

Vienādojumu, kas apraksta problēmu, uzrakstīšana. To sauc par matemātisko modelēšanu.
Efektīvu skaitlisko algoritmu izvēle modeļa risināšanai.
Datorprogrammu, kas efektīvi ievieš algoritmu, izveide.
Iegūtās programmas darbināšana datorā.
(2. – 4. darbību sauc par problēmas skaitlisko modelēšanu.)

Tādā veidā eksperimentus var daļēji aizstāt ar modelēšanu. Protams, tikai eksperimenti, ja tādi ir iespējami, var apstiprināt modeli un iegūtos rezultātus. Skaitļošanas zinātne parasti balstās uz teorētiskiem modeļiem. Tomēr dažos gadījumos datorus var izmantot arī, lai atklātu un pierādītu matemātikas teorijas. Piemēram, tā sauktā četru krāsu teorēma tika pierādīta 70. gados, nevis tikai ar pildspalvu un papīru, bet arī ar datora palīdzību.

# Datu zinātne

<!-- [Atpakaļ](studijas/ned-1#1-8-k-hpc-ietekm-pasauli) -->

Datu zinātni var definēt kā jomu, kas izmanto dažādas matemātiskas metodes un algoritmus, lai no datiem iegūtu zināšanas un priekšstatus. Šo informāciju atsevišķos gadījumos var izmantot jaunu matemātisko modeļu formulēšanai. Piemēram, Tiho Brahe mērījumi veidoja datus, kurus Johannes Kepler analizēja, formulējot Keplera planētu kustības likumus. Vēlāk Ņūtons parādīja, ka Keplera likumi ir viņa gravitācijas teorijas sekas.

Divas būtiskas jomas, kas ir savstarpēji saistītas datu zinātnē, un kuras pēdējos gados ir kļuvušas nozīmīgas, ir mašīnmācīšanās un mākslīgais intelekts. Mākslīgais intelekts ir datorzinātnes apakšnozare, kas nodarbojas ar intelektuālas uzvedības automatizāciju. To definē arī kā pētījumus, kā likt datoriem darīt lietas, ko pašlaik cilvēki dara labāk, vai kā skaitļošanas procesu pētījumus, kas ļauj uztvert, spriest un darboties.
