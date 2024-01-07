
<!-- # Sākam kursu ... -->
:include-image: pix/kurss-hpc-pamati-logo.png { scale: 0.7, align: "center"}

> Septiņi jautājumi atbildēti septiņās minūtēs.

<!-- [Ievada video](https://vimeo.com/893412677) -->

:include-iframe: https://player.vimeo.com/video/893412677?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479

<!-- :include-iframe: iframe/custom.html {
  fit: true
} -->

<!-- :include-iframe: iframe/uzdevums.html {
    title: "Uzdev.",
  fit: false, 
  aspectRatio: "7:6",
  border: null,
} -->


<!-- :include-iframe: https://player.vimeo.com/video/893412677?h=bf6da07fd5 {aspectRatio: "1:1" } -->

# Kas ir HPC?

- **Augstas veiktspējas skaitļošana** jeb **HPC** (no angļu valodas *High Performance Computing*) ir iespēja apstrādāt datus un veikt sarežģītus aprēķinus lielā ātrumā.
- HPC ļauj izmantot skaitļošanas jaudu, kas ir ievērojami lielāka nekā pieejama tipiskā klēpjdatorā vai galddatorā.
- Lai izmantotu augstas veiktspējas skaitļošanu, ir nepieciešamas divas lietas:
- gan **aparatūra**, t.i., specifisks jaudīgs dators, ko sauc arī par superdators,
- gan **programmatūra**, t.i., rīki HPC lietojumprogrammu programmēšanai un superdatora lietošanai.

# Eksperimentālā zinātne

**Agrīnā astronomija** ir eksperimentālās zinātnes piemērs. Senie astronomi vēroja debesis vispirms ar acīm un pēc tam ar teleskopiem un fiksēja Saules, Mēness, Saules sistēmas planētu un dažu zvaigžņu pozīcijas un kustības. Viņi secināja, ka novērojumi atbilst konkrētiem modeļiem. 

Līdzīgi mikroskopus var izmantot, lai novērotu nelielu daļiņu nejaušu kustību šķidrumā (Brauna kustība) utt.

Dažādiem eksperimentiem ir nepieciešami atšķirīgi mērīšanas aparāti, un eksperimentu veikšana var būt ļoti dārga vai pat neiespējama.

Tomēr eksperimentālo zinātni var uzskatīt par fundamentālo paradigmu: teorijas un datorsimulācijas galu galā tiek apstiprinātas vai noraidītas, pamatojoties uz mērījumiem.

![Teleskops un mikroskops](https://raw.githubusercontent.com/viktorszagorskis/hpc-pamati/main/pix/TeleskopsMikroskops.png)

# Teorētiskā zinātne

Pamatojoties uz novērojumiem, var paredzēt saulrieta laiku konkrētai dienai. Novērojumi arī parāda, ka akmens lidojuma laiks ir aptuveni vienāds 
neatkarīgi no tā svara, kad tas tiek nomests no viena augstuma. Ņūtona izstrādātie gravitācijas un dinamikas matemātiskie modeļi spēj radīt 
prognozes ķermeņu kustībai, kas ļoti labi atbilst izmērītajiem rezultātiem.

Novērojumu dati ļauj zinātniekiem tos analizēt un mēģināt tos izskaidrot, aprakstīt ar noteiktām matemātiskām formulām. 
Parasti, vispirms ir novērojumi, un tad tiek izstrādāta teorija, lai tos izskaidrotu. Bet ne vienmēr. Piemēram, pirms vairāk nekā 50 gadiem teorētiķi 
Fransuā Englerts (*François Englert*) un Pīters Higss (*Peter Higgs*), lai izskaidrotu masas (matērijas, zvaigžņu, planētu) esamību, 
piedāvāja ieviest jaunu fizikālu lauku, ko tagad sauc par Higsa lauku. 
Pirmo eksperimentālo aptiprinājumu Higsa laukam ieguva tikai 2012. gadā. Savukārt 2013. gadā abi zinātnieki ieguva Nobela prēmiju par savu atklājumu.

# Skaitļošanas zinātne

Ir ierobežojumi tam, ko var izdarīt ar pildspalvu un papīru vai kādus eksperimentus var veikt. 

Piemēram, turpinot astronomisko tēmu, ir pietiekami vienkārši pierakstīt vienādojumus, kas raksturo Saules, Mēness un Zemes kustību. 
Šī ir tā sauktā trīs ķermeņa problēma, salīdzinoši vienkārša vienādojumu kopa, kuru tomēr nevar atrisināt analītiski, 
lai iegūtu iesaistīto debesu ķermeņu pozīcijas. Tomēr skaitliski var atrast aptuvenu risinājumu.

Līdzīgi var apskatīt klimatu un ledājus: ir ļoti svarīgi zināt, kas ar tiem notiks nākotnē. 
Bet, protams, mēs nevaram veikt eksperimentus globālā mērogā, lai to noskaidrotu. 
Tāpat, daudzos gadījumos nepieciešamie eksperimenti būtu pārāk dārgi, pārāk bīstami, pārāk lēni, pārāk grūti vai sarežģīti, neētiski utt. 

Tomēr mēs varam iegūt priekšstatu par procesiem, lietojot skaiļošanas zinātni.
Skaitļošanas zinātnē parasti sarežģītus matemātiskus modeļus, 
kas apraksta problēmu, risina, izmantojot skaitliskus algoritmus, kurus pēc tam realizē kā datorprogrammas, ko darbina superdatoros. 

Skaitļošanas zinātnes uzdevuma realizēšanu var raksturot ar sekojošiem soļiem:
  1.	Vienādojumu, kas apraksta problēmu, uzrakstīšana. To sauc par matemātisko modelēšanu.
  2.	Efektīvu skaitlisko algoritmu izvēle modeļa risināšanai.
  3.	Datorprogrammu, kas efektīvi ievieš algoritmu, izveide.
  4.	Iegūtās programmas darbināšana datorā.
  (2. – 4. darbību sauc par problēmas skaitlisko modelēšanu.)

Tādā veidā eksperimentus var daļēji aizstāt ar modelēšanu. Protams, tikai eksperimenti, ja tādi ir iespējami, var apstiprināt modeli un iegūtos rezultātus.
Skaitļošanas zinātne parasti balstās uz teorētiskiem modeļiem. Tomēr dažos gadījumos datorus var izmantot arī, lai atklātu un pierādītu matemātikas teorijas. 
Piemēram, tā sauktā [četru krāsu teorēma](https://lv.wikipedia.org/wiki/%C4%8Cetru_kr%C4%81su_teor%C4%93ma) tika pierādīta 70. gados, nevis tikai ar pildspalvu un papīru, bet arī ar datora palīdzību.

# Datu zinātne

Datu zinātni var definēt kā jomu, kas izmanto dažādas matemātiskas metodes un algoritmus, 
lai no datiem iegūtu zināšanas un priekšstatus. Šo informāciju atsevišķos gadījumos var 
izmantot jaunu matemātisko modeļu formulēšanai. Piemēram, _Tiho Brahe_ mērījumi veidoja datus, 
kurus _Johannes Kepler_ analizēja, formulējot Keplera planētu kustības likumus. 
Vēlāk Ņūtons  (_Isaac Newton_) parādīja, ka Keplera likumi ir viņa gravitācijas teorijas sekas.

Divas būtiskas jomas, kas ir savstarpēji saistītas datu zinātnē, un kuras pēdējos gados ir kļuvušas nozīmīgas, 
ir **mašīnmācīšanās** un **mākslīgais intelekts**. Mākslīgais intelekts ir datorzinātnes apakšnozare, kas 
nodarbojas ar intelektuālas uzvedības automatizāciju. To definē arī kā pētījumus, kā likt datoriem darīt lietas, 
ko pašlaik cilvēki dara labāk, vai kā skaitļošanas procesu pētījumus, kas ļauj uztvert, spriest un darboties. 
