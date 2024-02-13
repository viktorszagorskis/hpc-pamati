---
title:  Vecais variants - Sho nenjemt par pilnu

---



#  3.4 PARALĒLO ALGORITMU VEIDI

> Domājiet par to - kā cep picu.

Reālajos uzdevumos izmantojamie paralēlie algoritmi ietver gan ar mijiedarbību, gan atkarību. Kā divi pretpoli uzskatāmi:

vienkārši paralēlie (trivially parallel) un
savstarpēji cieši saistītie (tightly coupled) algoritmi.
iepriekšējā piemērā, mijiedarbība starp diviem apakš-uzdevumiem Annas un Jāņa piemērā par 20 skaitļu saskaitīšanu ir tikai par darba uzdevumu sadalīšanu un beigu rezultātu saskaitīšanu. Katram veicot savu skaitļu saskaitīšanu nekāda mijiedarbība nav vajadzīga, tāpēc šo algoritmu var uzskatīt par vienkārši paralēlo. Ja Annai aprēķinu veikšanas laikā būtu regulāri jāsadarbojas ar Jāni, tad tas jau būtu cieši saistītais algoritms. Kā šādu piemēru varētu pieminēt Sudoku spēles uzdevuma risināšanu tandēmā.

No programmēšanas viedokļa vienkārši paralēlie algoritmi ir vieglāk realizējami un tiem nevajag nodrošināt savienojumu starp procesoriem, kuri veic šo paralēlos uzdevumus.  
- Viens no tādiem piemēriem varētu būt folding@home projekts, kurā caur internetu apvienoti daudzu brīvprātīgo lietotāju personālie datori veic paralēlos skaitļošanas uzdevumus.

Savstarpēji cieši saistītu algoritmu gadījumā programmēšana ir sarežģītāka un ātrdarbīgs savienojums ar mazu aizturi (mazu latentumu) starp centrālajiem procesoriem ir ļoti svarīgs augstas veiktspējas nodrošināšanai. Laika apstākļu prognozēšanas uzdevums ir viens no šādiem piemēriem. Daudzi citi reālie skaitļošanas uzdevumi ir kaut kur pa vidu starp šīm divām galējībām.

#  3.5 Tests
Kādi ir PARALĒLās skaitļošanas VEIDI?



# 3.6 Kā organizēt paralēlos aprēķinus? Veids Nr1 

Viens no veidiem kā realizē paralēlo skaitļošanu ir, piemēram, skaitļu masīva sadalīšanu starp skaitļošanas mezgliem. Šeit katrs skaitļošanas elements (piemēram, CPU kodols) zina savu atbildības zonu, darbu apjomu un algoritmu - ko ar datiem darīt.

![](https://hpc-ievads.netlify.app/_astro/distribution.f7d79adf_ZxvPHX.avif)

Katrā skaitļošanas elementā ir daļa no kopējā datu apjoma un katrs no šiem elementiem veic ar tiem identiskas vai ļoti līdzīgas darbības. Līdzīgi kā piemērā ar Annu un Jāni, katrs no viņiem paņem no kopējā masīva sev paredzēto datu daļu,
saskaita/reizina/dala/vai kā citādi apstrādā viņu rīcībā esošos skaitļus/datus.

# 3.7 Tests 
Vai Tu spēj uzrakstīt formulu?

# 3.8 Kā organizēt paralēlos aprēķinus? Veids Nr2

- 2. daļa – piemērs par to kā summēt praktiski

...

# 3.9 Tests
Ko Tu spēj summēt praktiski?

Jautājumi...

# 3.10 Nedēļas Tests 
Nedēļas beigu tests no somu kursa (8 jautājumi, pareizi jāatbild 6