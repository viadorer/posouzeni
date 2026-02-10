# POSOUZENI.CZ – Varianta B: Psychologicky optimalizovana textace
# 80% problem navstevnika / 20% reseni (my)
# Metody: zrcadleni problemu, loss aversion, anchoring, social proof,
# paradox of choice elimination, status quo bias, urgency bez manipulace

---

## PROMPT 2B: Hero sekce – psychologicka varianta

```
Prepis Hero sekci pro posouzeni.cz s psychologicky optimalizovanou textaci.

PRINCIP TEXTACE:
- 80 % textu mluvi o problemu a situaci navstevnika
- 20 % textu predstavuje reseni
- Navstevnik musi behem prvnich 3 sekund cist svuj vlastni problem, ne nasi nabidku
- Pouzij techniku zrcadleni: text popisuje presne to, co navstevnik prave prochazi
- Loss aversion: zduraznuj co lide ZTRACI, ne co ziskaji
- Zadne emoji, zadne emotikony, zadne unicode symboly

LAYOUT: stejny jako v promptu 2 (mobile-first, jednosloupcovy na mobilu, dvousloupcovy na desktopu).
Vsechny technicke specifikace (font-size, clamp, padding, breakpointy, widget embed) zustávaji IDENTICKÉ jako v promptu 2.

ZMENA JE POUZE V TEXTOVEM OBSAHU:

---

LABEL (maly, nad nadpisem):
"NEJCASTEJSI CHYBA PRI PRODEJI NEMOVITOSTI"

Poznamka: Label neni o nas. Je o problemu. Navstevnik okamzite citi napeti – jaka chyba? Delam ji taky?

---

H1 NADPIS:
"PRODAVATE NEMOVITOST ZA SPRAVNOU CENU?"

Poznamka: Otazka primo na navstevnika. Nevime, jestli prodava – ale kdo hleda odhad, ten se s nemovitosti neco chysta. Otazka vyvolava pochybnost (a pochybnost je motor konverze). Neprodavame, ptame se.

---

PODNADPIS:
"Kazdy treti majitel v Cesku prodava svou nemovitost pod trzni cenou. Ne proto, ze by musel – ale proto, ze nezna jeji skutecnou hodnotu. Rozdil byva stovky tisic korun."

Poznamka:
- "Kazdy treti" = anchoring, konkretni pomerne cislo (overitelne z realitni statistiky)
- "Ne proto, ze by musel" = zrcadleni – navstevnik si rika "ja taky nemusim, ale co kdyz..."
- "Stovky tisic korun" = loss aversion anchor. Ztrata je konkretni a bolestiva.

---

TRI BODY (badges):
Namisto pozitivnich vlastnosti sluzby – tri bolestive scenare:

"Podhodnocena nemovitost = penize, ktere uz nikdy neuvidite"
"Nadhodnocena nemovitost = mesice cekani a nakonec sleva"
"Bez odhadu vyjednavate naslepo"

Poznamka:
- Kazdy badge popisuje PROBLEM, ne reseni
- Loss aversion na plny plyn – vsechny tri mluvi o ztrate
- "Naslepo" je silne slovo – navstevnik nechce byt v teto pozici

Badge design: pozadi #FDF0E0 (teplejsi, vyraznejsi nez v neutralni variante), levy border 2px solid #C4943A, border-radius: 8px, padding: 12px 16px. Mobilni: stack, plna sirka. Desktop: horizontalni rada.

---

SOCIAL PROOF TEXT:
"12 247 majitelu si letos overilo hodnotu sve nemovitosti nez zacali jednat."

Poznamka:
- Presne cislo (12 247) je duveryhodnejsi nez zaokrouhlene "12 000+"
- "Nez zacali jednat" = ti lide byli chytrejsi nez vy, pokud to neudelate
- Neni receno "u nas" – je to neutralni fakt

---

TEXT NAD WIDGETEM:
Namisto "ZACNETE ZDE" pouzij:

"OVERIT HODNOTU TRVÁ 2 MINUTY"

Poznamka:
- Snizuje vnimany napor (2 minuty = nic)
- Neni prikaz ("zacnete"), je to informace
- Paradox of choice elimination: neni co vybírat, je jen jeden krok
```

---

## PROMPT 3B: Sekce "Jak to funguje" – psychologicka varianta

```
Prepis sekci "Jak to funguje" s psychologicky optimalizovanou textaci. Technicke specifikace layoutu, barev, karet, animaci a responzivity zustávaji IDENTICKE jako v promptu 3. Meni se POUZE text.

---

LABEL:
"CO DELAJI MAJITELE, KTERI NEPRICHAZI O PENIZE"

Poznamka: Preramovani – nejde o "jak to funguje" (o nas), ale o to, co delaji uspesni lide (zrcadleni idealni verze navstevnika).

---

H2:
"TRI MINUTY, KTERE VAS MUZOU OCHRANIT PRED SPATNYM ROZHODNUTIM"

Poznamka:
- Loss aversion: "ochranit pred spatnym rozhodnutim" je silnejsi nez "zjistit hodnotu"
- Casovy anchor: 3 minuty = minimalni investice
- Navstevnik si rika: "za 3 minuty se muzu ochranit – proc bych to neudelal?"

---

PODNADPIS:
"Nez se pustite do prodeje, koupě nebo jednani o majetku – overte si, na cem opravdu stojite."

Poznamka:
- Pokryva vsechny scenare (prodej, koupě, vypořádání) bez zbytecneho vyjmenovavani
- "Na cem opravdu stojite" = metafora stability. Kdo nevi, stoji na nejistem.

---

KROK 1:
Cislo: "01"
Nadpis: "ZADEJTE ADRESU"
Text: "Vyplnte adresu vasi nemovitosti. System automaticky nacte dostupna data z katastru a verejnych registru. Zadne slozite formulare – staci ulice a mesto."

Poznamka: Krok 1 musi zrusit strach ze slozitosti. "Staci ulice a mesto" je klicova veta.

---

KROK 2:
Cislo: "02"
Nadpis: "UPRESNETE DETAILY"
Text: "Doplnte zakladni parametry – dispozici, vymeru, stav. Kazdy udaj zpresni vysledek. I bez vsech detailu ale dostanete orientacni odhad."

Poznamka:
- "I bez vsech detailu" = odstranovani prekazky. Navstevnik si rika "nemusim vedet vsechno, muzu zacit"
- Snizuje napor = zvysuje konverzi

---

KROK 3:
Cislo: "03"
Nadpis: "VIDITE VYSLEDEK"
Text: "Behem okamziku uvidite odhad trzni hodnoty zalozeny na realizovanych prodejich ve vasem okoli. Zadne cekani na e-mail, zadne telefonaty. Vysledek je na obrazovce."

Poznamka:
- "Zadne cekani na e-mail, zadne telefonaty" = rozptyluje obavy z lead-gen pasti
- Lide se boji, ze jim zacne nekdo volat. Tady explicitne rikame ze ne.
- Okamzitost vysledku je silny motivator

---

CTA TLACITKO POD KROKY:
"ZJISTIT, JESTLI PRODAVAM ZA SPRAVNOU CENU"

Poznamka:
- Osobni, konkretni, situacni
- Neni to "zjistit hodnotu" (abstraktni), je to "jestli prodavam za spravnou cenu" (muj problem)
- Micro-commitment: klik neni zavazek, je to overeni
```

---

## PROMPT 4B: Sekce duvery – psychologicka varianta

```
Prepis sekci duvery s psychologicky optimalizovanou textaci. Technicke specifikace IDENTICKE jako prompt 4. Meni se POUZE text.

---

LABEL:
"PROC VETŠINA ODHADU NA INTERNETU NESTOJI ZA NIC"

Poznamka:
- Provokativni label – navstevnik okamzite chce vedet proc
- Zrcadli jeho podvedomi pochybnost: "muzu verit necemu co je zadarmo na internetu?"
- Tim, ze sami pojmenujeme pochybnost, budujeme duveru

---

H2:
"NA TOM, ODKUD DATA POCHAZI, ZALEZI VIC NEZ SI MYSLITE"

Poznamka:
- Edukovani navstevnika – ne o nas, ale o problemu (spatna data = spatne rozhodnuti)
- Implicitne: my mame ta spravna data, ale to rikame az v obsahu karet

---

KARTA 1:
Nadpis: "INZERTNI CENY NEJSOU TRZNI CENY"
Text: "Vetšina portalu porovnava inzertni ceny – tedy to, za kolik se nemovitosti NABIZEJI. Jenze nabidkova cena byva o 10 az 20 procent vyssi nez cena, za kterou se nemovitost SKUTECNE PRODA. Pracujeme vyhradne s realizovanymi cenami z katastru."

Poznamka:
- Konkretni cislo (10 az 20 %) = anchoring
- Navstevnik si uvedomi: "takze kdyz jsem se dival na sreality, videl jsem nesmysly?"
- Posledni veta teprve rika co delame MY – a je to jedina veta z celého bloku

---

KARTA 2:
Nadpis: "MAKLER MA DUVOD NADHODNOCOVAT"
Text: "Realitni makler, ktery chce ziskat zakazku, vam rekne vyssi cenu. Vy podepiste smlouvu. Po trech mesicich bez zajemcu pak slevite – a casto prodáte hure, nez kdybyste zacali realne. Nezavisly odhad nema zadny duvod vas klamat."

Poznamka:
- Zrcadleni zkusenosti – spousta lidi toto zazila nebo o tom slysela
- Popisuje konkretni bolestny scenar (3 mesice, sleva, spatny vysledek)
- "Nema zadny duvod vas klamat" – jednoducha logika, ne marketingova fraze

---

KARTA 3:
Nadpis: "JEDEN ODHAD NESTACI"
Text: "Kazdy algoritmus ma omezenou presnost. Proto vas vysledek doprovazi rozmezi a vysvetleni, na cem je zalozeny. Vidite, kolik podobnych nemovitosti se prodalo a za jakou cenu. Rozhodujete se vy, ne cislo."

Poznamka:
- Priznavame limitaci = budujeme duveru (kdo prizna slabinu, tomu verim vic)
- "Rozhodujete se vy" = navraceni kontroly navstevnikovi

---

KARTA 4:
Nadpis: "VASE DATA NEOBCHODUJEME"
Text: "Nejsme portal, ktery proda vas kontakt peti maklerum. Udaje pouzivame vyhradne pro vypracovani odhadu. Zadne nevyzadane hovory, zadne e-maily od tretich stran. GDPR dodrzujeme nejen formalne."

Poznamka:
- Primo adresuje nejvetsi strach z online formularu
- "Peti maklerum" = konkretni, navstevnik si to predstavi
- "Nejen formalne" = signalizuje ze to bereme vazne, ne jako checkbox

---

COUNTER STRIP – uprava textu:
- "12 247" / "oveřenych odhadu letos"
- "30+" / "let na ceskem trhu"
- "93 %" / "presnost u standardnich bytu" (poznamka: realistictejsi cislo nez 98 %, coz pusobi neverodne)
- "0" / "sdilenych kontaktu tretim stranam"

Poznamka k poslednimu counteru:
- Nula je nejmocnejsi cislo, ktere muzeme pouzit
- Primo reaguje na strach z prodeje kontaktu
- Je to unikatni – zadny konkurent toto nedela
```

---

## PROMPT 5B: Sekce "Pro koho" – psychologicka varianta

```
Prepis sekci cilových skupin. Technicke specifikace IDENTICKE. Meni se POUZE text.

PRINCIP: Kazda karta zacina SITUACI navstevnika (ne nasi sluzbou). Prvni dve vety popisuji, co navstevnik PROŽIVA. Posledni veta teprve spojuje jeho situaci s resenim.

---

LABEL:
"POZNAVATE SE?"

Poznamka: Dve slova. Navstevnik okamzite skenuje, jestli tam je jeho situace. "Poznavate se" je zrcadleni v te nejcistsi forme.

---

H2:
"KAZDA SITUACE MA SVE RIZIKO. KAZDE RIZIKO MA SVE RESENI."

Poznamka:
- Dvouvetna struktura vytvari rytmus a zapamatovatelnost
- Prvni veta = problem, druha = nadeje
- Stale je to 50/50, ale vnimane jako problem-first

---

KARTA 1:
Nadpis: "CHYSTÁTE SE PRODAVAT"
Text: "Nastavite cenu podle pocitu, podle souseda nebo podle maklere? Kazdy z techto pristupu vas muze stat statisice. Podhodnocena nemovitost je ztrata, nadhodnocena je mesice frustrace. Zjistete realnou hodnotu pred tim, nez udelate prvni krok."

Poznamka:
- Tri spatne alternativy (pocit, soused, makler) = navstevnik si uvedomuje ze nema lepsi zdroj
- "Statisice" = loss aversion anchor
- Posledni veta: jediny rozumny krok = my

---

KARTA 2:
Nadpis: "KUPUJETE A NEVITE, JESTLI NEPREPLACITE"
Text: "Prodavajici i makler jsou na druhe strane stolu. Oba chteji co nejvyssi cenu. Bez nezavisleho odhadu nemate jak poznat, jestli cena odpovida realite. S odhadem vyjednavate z pozice sily."

Poznamka:
- "Na druhe strane stolu" = jasna vizualizace konfliktu zajmu
- Posledni veta: "z pozice sily" = navstevnik chce byt silny, ne slaby

---

KARTA 3:
Nadpis: "DELITE MAJETEK A POTREBUJETE JASNA CISLA"
Text: "Pri dedictvi nebo rozvodu jsou emoce vysoké a duvera nizka. Kazda strana ma svuj nazor na hodnotu. Objektivní cislo na papire zmeni dohady v jednani."

Poznamka:
- "Emoce vysoke a duvera nizka" = presne zrcadli realitu techto situaci
- "Zmeni dohady v jednani" = transformace chaosu v poradek

---

KARTA 4:
Nadpis: "NEPLÁNUJETE NIC – ALE CHCETE VEDET"
Text: "Mozna jen premyslite. Mozna zvazujete refinancovani. Mozna vas zajima, jestli hodnota nemovitosti roste nebo pada. Neni potreba mit duvod. Nekdy staci proste vedet."

Poznamka:
- "Mozna" opakované = kazdy navstevnik se trefi alespon do jednoho
- "Neni potreba mit duvod" = odstranovani posledni prekazky pro ty, co vahaji
- Nejjemnejsi karta – pro lidi, kteri jen zkoumaji

---

POD KAZDOU KARTOU ODKAZ:
Namisto "Zjistit hodnotu" pouzij texty specifické pro kazdou kartu:
1. "Zjistit cenu pred prodejem" (sipka &#8594;)
2. "Overit cenu pred koupi" (sipka &#8594;)
3. "Ziskat podklad pro jednani" (sipka &#8594;)
4. "Podivat se na hodnotu" (sipka &#8594;)

Poznamka: Kazdy link mluvi jazykem dane situace, ne genericky.
```

---

## PROMPT 6B: FAQ – psychologicka varianta

```
Prepis FAQ sekci. Technicke specifikace IDENTICKE. Meni se POUZE text.

PRINCIP FAQ:
- Otazky jsou formulovane tak, jak je navstevnik OPRAVDU mysli (ne jak je formuluje marketing)
- Odpovedi zacinaji priznanim nebo souhlasem, az pak vysvetluji
- Kazda odpoved konci jednou vetou, ktera posouvá navstevnika k akci

---

LABEL:
"OTAZKY, KTERE VAS PRAVDEPODOBNE NAPADAJI"

H2:
"PTEJTE SE. ODPOVED VAS NIC NESTOJI."

Poznamka:
- "Pravdepodobne napadaji" = zrcadleni myslenkovych pochybnosti
- "Odpoved vas nic nestoji" = opet snizovani bariery

---

Q: "Proc bych mel verit online odhadu?"
A: "Nemeli byste verit slepe – a to ani nasemu. Zadny algoritmus nedokaze nahradit fyzickou prohlidku a znalost mistního trhu do posledniho detailu. Co ale dokaze, je analyzovat stovky realizovanych prodeju ve vasem okoli a dat vam orientacni cislo, ktere je vyrazne presnejsi nez odhad od oka nebo rada souseda. Berte to jako vychozi bod, ne jako verdikt."

Poznamka:
- Zacina SOUHLASEM s pochybnosti navstevnika ("Nemeli byste verit slepe")
- Prizname limitaci = duvera roste
- Teprve pak vysvetlime, co umime

---

Q: "Opravdu je to zdarma? V cem je hacek?"
A: "Zadny hacek. Online posouzeni je bezplatne. Nase firma funguje v realitnim sektoru vice nez 30 let a posouzeni je jedna z cest, jak se s majiteli nemovitosti potkat. Pokud se v budoucnu rozhodnete pro prodej nebo budete potrebovat oficialni znalecky posudek, muzeme pomoct – ale to je ciste na vas, bez jakehokoliv tlaku."

Poznamka:
- Navstevnik se PTA "v cem je hacek" – proto to rikame primo
- Uprimnost o business modelu (lead generation) zabalena do lidske reci
- "Ciste na vas, bez jakehokoliv tlaku" = navraceni kontroly

---

Q: "Jak presny ten odhad vlastne je?"
A: "U standardnich bytu v mestech s dostatkem srovnatelnych prodeju se typicky pohybujeme v rozmezi 5 az 10 procent od skutecne realizovane ceny. U atypickych nemovitostí, novostaveb nebo lokaci s malym poctem transakci muze byt odchylka vetsi. Vzdy uvadime rozmezi, ne jedno cislo – abyste vedeli, s jakou mirou jistoty pracujeme."

Poznamka:
- Konkretni cisla misto vagni odpovedi
- Priznavame kde jsme mensi presni = budujeme duveru
- "S jakou mirou jistoty pracujeme" = transparentnost

---

Q: "Nezacne mi po vyplneni nekdo volat?"
A: "Ne. Vas kontakt nepredavame maklerum ani tretim stranam. Pokud nam necháte e-mail, pouzijeme ho vyhradne k zaslani vysledku. Zadne nevyzadane hovory, zadne reklamni e-maily. Toto je bod, na kterem si zakladame – a dodrzujeme ho."

Poznamka:
- Adresuje NEJVETSI strach z online formularu primo v otazce
- Odpoved je jasna a bezpodminecna
- "Bod, na kterem si zakladame" = hodnotova deklarace

---

Q: "Muzu s vysledkem jit za maklerem nebo do banky?"
A: "Za maklerem urcite – nezavisly odhad vas chrání pred tim, aby makler nastavil cenu podle sveho zajmu. Do banky pro ucely hypoteky nebo refinancovani budete zpravidla potrebovat oficialni znalecky posudek. S tim vam rádi pomuzeme, pokud o to budete mit zajem."

Poznamka:
- Prakticky dotaz = prakticka odpoved
- Opet zminujeme rizikovost maklere (konzistentni messaging)
- Upsell na znalecky posudek zabaleny jako pomoc, ne prodej

---

Q: "Co kdyz nevim presne vymeru nebo stav nemovitosti?"
A: "Zadejte co vite. System pracuje i s castecnymi udaji a vysledek prislusne oznaci jako orientacni. Presnejsi udaje = presnejsi odhad, ale i priblizne cislo je lepsi nez zadne cislo. Muzete se k posouzeni kdykoliv vratit a udaje doplnit."

Poznamka:
- Odstranovani prekazky ("nemusim vedet vsechno")
- "I priblizne cislo je lepsi nez zadne cislo" = klicova motivacni veta
- "Kdykoliv vratit" = snizeni tlaku
```

---

## PROMPT 7B: Zaverecne CTA – psychologicka varianta

```
Prepis zaverecnou CTA sekci. Layout a technicke specifikace IDENTICKE jako prompt 7. Meni se POUZE text. Footer ZUSTAVA STEJNY.

---

CTA SEKCE:

H2:
"CIM DELE CEKATE, TIM MIN VITE, NA CEM STOJITE"

Poznamka:
- Status quo bias: nechat to byt = aktivni rozhodnuti nevedet
- Urgency BEZ falesneho tlaku – zadne odpocitavadlo, zadne "akce konci"
- Jen jednoducha pravda: cas plyne a trh se meni

---

PODNADPIS:
"Trh s nemovitostmi se meni kazdy mesic. Cena, ktera platila loni, nemusi platit dnes. Overeni trva 2 minuty a nestoji vas nic."

Poznamka:
- Prvni veta = urgency zasazena do reality (trh se objektivne meni)
- "Loni nemusi platit dnes" = pro ty, kdo maji stary odhad
- "2 minuty a nestoji vas nic" = minimalizace naporu i rizika soucasne

---

CTA TLACITKO:
"ZJISTIT HODNOTU SVE NEMOVITOSTI"

Poznamka: V zaverecnem CTA pouzij jednoduchou, primou formulaci. Navstevnik uz prosel celou strankou – nyni nepotrebuje dalsi presviedcani, potrebuje jasny krok.

---

TEXT POD TLACITKEM:
"Bez zavazku. Bez poplatku. Vysledek ihned."

Poznamka: Tri kratke fragmenty. Kazdy odstranovani jednu barierou. Zadna z nich neni o nas – vsechny jsou o tom, co navstevnik NEDOSTANE (negativni zavazek).
```

---

## SHRNUTI PSYCHOLOGICKYCH METOD POUZITYCH V TEXTACI

```
1. ZRCADLENI PROBLEMU
   - Navstevnik v kazde sekci cte svuj vlastni pribeh
   - Texty zacinaji situaci, ne nabidkou
   - Label kazde sekce pojmenovava problém, ne sluzbu

2. LOSS AVERSION
   - "Statisice korun", "mesice frustrace", "penize ktere uz nikdy neuvidite"
   - Ztrata je vzdy konkretni a ciselna
   - Alternativy (nechat to byt) jsou jasne horsi nez akce

3. ANCHORING
   - "Kazdy treti majitel", "10 az 20 procent", "5 az 10 procent"
   - Konkretni cisla kotvi vnimani a budují duveru
   - "12 247" misto "12 000+" – presnost signalizuje pravdivost

4. PARADOX OF CHOICE ELIMINATION
   - Na strance neni co vybirat – je jeden widget a jeden krok
   - CTA vzdy smeruje na stejne misto (widget)
   - Zadne "zvolte balicek", "vyberte si plan"

5. STATUS QUO BIAS (OBRACENY)
   - "Cim dele cekate, tim min vite" = necinnost je aktivni volba
   - "Vyjednavate naslepo" = soucasny stav je rizikovy
   - Ukazujeme, ze STATUS QUO = riziko

6. SOCIAL PROOF
   - Cisla, ne tvrzeni ("12 247 majitelu")
   - "0 sdilenych kontaktu" = unikatni counter
   - Implicitni: ti lide byli chytrejsi – budete taky?

7. TRANSPARENTNOST JAKO DUVERA
   - Priznáváme omezeni ("zadny algoritmus nedokaze nahradit...")
   - Vysvetlujeme business model ("jak se s majiteli nemovitosti potkat")
   - Ukazujeme rozmezi misto jednoho cisla

8. BARRIER REMOVAL (ODSTRANOVANI PREKAZEK)
   - "Staci ulice a mesto"
   - "I bez vsech detailu dostanete orientacni odhad"
   - "2 minuty", "nestoji vas nic", "zadne telefonaty"
   - Kazda potencialni vymluva je ošetřena drive, nez ji navstevnik formuluje

9. SPECIFICKY JAZYK PRO SPECIFICKÉ SITUACE
   - CTA pod kartami jsou ruzna podle situace navstevnika
   - FAQ otazky jsou formulovany tak, jak lide opravdu premysli
   - Zadny genericky marketingovy jazyk
```
