## Superdatora darbības ātrums

Ir vairāki izplatīti rādītāji superdatoru veiktspējas mērīšanai un to savstarpējai salīdzināšanai. Klasisks rādītājs ir peldošā komata darbību skaits, ko dators var izpildīt vienā sekundē (FLOP/s).

**Ko nozīmē FLOP/s**? 
Peldošā komata skaitlis ir reāla skaitļa attēlojums datorā. Ja mēs veicam vienu aprēķinu, kas ietver divus reālus skaitļus, piemēram, 2.1 + 4.3, vienā sekundē, tad tas ir vienāds ar vienu peldošā komata darbību sekundē (1 FLOP/s).

Lai gan datori var strādāt arī ar veseliem skaitļiem, lielāko daļu zinātnisko problēmu matemātiski var atrisināt, izmantojot tikai reālos skaitļus. Šajā rādītājā iekļautās darbības ir aritmētiskās pamatoperācijas: saskaitīšana, atņemšana, reizināšana un dalīšana. Gadu gaitā FLOP/s ir kļuvis par vispāratzītu standartu superdatoru novērtēšanā.

Piemēram, ja dators var izpildīt
+ miljards (10<sup>9</sup>) FLOP/s, tā veiktspēja ir viens *Giga* FLOP/s (**G**FLOP/s),
+ vienu triljonu (10<sup>12</sup>) FLOP/s, tad - viens *Tera* FLOP/s (**T**FLOP/s),
+ vienu kvadriljonu jeb 10<sup>15</sup> FLOP/s, tad - viens *Peta* FLOP/s (**P**FLOP/s).

**CPU kodola teorētisko skaitļošanas jaudu nosaka taktātrums un maksimālais peldošā komata darbību skaits, ko tas var veikt vienā taktī.** GPU teorētisko maksimālo veiktspēju aprēķina līdzīgi.

Piemēram, ja klēpjdatora CPU kodola takts frekvence ir 3 GHz un tas var veikt 16 peldošā komata darbības, tad kopējā kodola maksimālā veiktspēja ir 48 GFLOP/s, jo

3 × 10<sup>9</sup> 1/s × 16 FLOP = 48 GFLOP/s

Visa superdatora teorētisko maksimālo veiktspēju iegūst, reizinot tā CPU un GPU teorētisko maksimālo veiktspēju ar sistēmā izmantoto komponentu (CPU un GPU) skaitu.

Termins *teorētiskais* norāda uz to, ka šo skaitļošanas jaudu parasti nevar sasniegt reālos aprēķinos. Lai centrālais procesors varētu aprēķināt 2.1 + 4.3, tam no atmiņas ir jāiegūst divi skaitļi, un pēc tam rezultāts jāsaglabā atpakaļ atmiņā. Tas nenotiek uzreiz, tāpēc praksē skaitļošanas ātrumu nosaka ne tikai CPU tīrā skaitļošanas jauda, bet arī tas, cik ātri CPU var piekļūt atmiņai.

Superdatoros viena mezgla centrālajam procesoram var būt nepieciešams piekļūt datiem arī citā mezglā. Tādējādi datu pārraides ātrums starp mezgliem arī var ierobežot praktisko veiktspēju. Turklāt reālajām lietojumprogrammām arī ir jālasa un jāieraksta dati diskā, kas nozīmē, ka ievades/izvades ātrums vai datu pārsūtīšana starp procesoriem un datu krātuvi var vēl vairāk ierobežot veiktspēju.

| Darbības sekundē | Zinātniskais apzīmējums | Metriskais prefikss | Mērvienība |
|--------------|:-----:|:-----:|-----------:|
| 1 000 |  10<sup>3</sup> |        kilo | KFLOP/s |
| 1 000 000  |  10<sup>6</sup> |          mega | MFLOP/s |
| 1 000 000 000  |  10<sup>9</sup> |          giga | GFLOP/s |
| 1 000 000 000 000  |  10<sup>12</sup> |          tera | TFLOP/s |
| 1 000 000 000 000 000  |  10<sup>15</sup> |          peta | PFLOP/s |
| 1 000 000 000 000 000 000  |  10<sup>18</sup> |          eksa | EFLOP/s |
