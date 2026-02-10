# POSOUZENI.CZ – Kompletní prompty pro Windsurf

## Barevná paleta a design systém

```
PRIMÁRNÍ PALETA:
- Ivory pozadí:        #FDFAF5 (hlavní background)
- Teplá bílá:          #FAF7F0 (sekce alternace)
- Zlatá/Amber akcent:  #C4943A (CTA tlačítka, akcenty)
- Tmavá zlatá hover:   #A67B2E (hover stav)
- Heading text:        #2C2416 (tmavá teplá hnědočerná)
- Body text:           #5C4F3D (teplá šedohnědá)
- Světlý text:         #8B7D6B (popisky, meta)
- Linka/border:        #E8E0D4 (jemné oddělení)
- Widget primary:      #C4943A (sladěný s celkem)

TYPOGRAFIE:
- Heading font: "Playfair Display" (serif, elegance, důvěra)
- Body font: "DM Sans" (čistý, moderní, čitelný)
- Headings: uppercase, letter-spacing: 0.05em
- Body: normal case, line-height: 1.7

WIDGET NASTAVENÍ:
primaryColor: '#C4943A'
borderRadius: '16px'
maxWidth: '520px'
shadow: 'none'
```

---

## PROMPT 1: Inicializace projektu + globální styly

```
Vytvoř nový Next.js 14 projekt (App Router) pro doménu posouzeni.cz.

Účel: Jednoduchá landing page pro sběr leadů – lidé, kteří potřebují znát tržní hodnotu své nemovitosti. Stránka obsahuje embedded widget pro odhad, který dodám já. Tvým úkolem je vytvořit okolní stránku s maximálním konverzním poměrem.

DESIGN SYSTÉM:
- Celý web má teplou, uklidňující atmosféru – ivory/cream pozadí (#FDFAF5), teplé barvy
- Hlavní akcent: zlatá/amber (#C4943A)
- Heading font: "Playfair Display" z Google Fonts – serif, elegantní, důvěryhodný
- Body font: "DM Sans" z Google Fonts – čistý, příjemný
- Všechny nadpisy: UPPERCASE, letter-spacing: 0.05em, barva #2C2416
- Body text: #5C4F3D, line-height: 1.7
- Žádné emoji, žádné ikony z balíčků – pokud ikony, tak pouze jednoduché SVG
- Border-radius na kartách a tlačítkách: 16px
- Dostatečný white-space, vzdušný layout, nic přeplácané

TECHNICKÉ:
- Tailwind CSS 3
- TypeScript
- SEO meta tagy pro češtinu, Open Graph
- Favicon placeholder
- Responsive mobile-first
- Stránka je single-page (jedna stránka, sekce pod sebou)

Vytvoř:
1. Globální layout (app/layout.tsx) s fonty a meta tagy
2. Globální CSS s custom properties pro barvy
3. Základní strukturu app/page.tsx (zatím prázdnou s komentáři kde budou sekce)
4. tailwind.config.ts s rozšířenými barvami a fonty

Meta title: "Posouzení nemovitosti online | Zjistěte tržní hodnotu zdarma"
Meta description: "Získejte nezávislé posouzení hodnoty vaší nemovitosti během 2 minut. Bezplatný odhad tržní ceny bytu, domu nebo pozemku na základě aktuálních dat z trhu."
```

---

## PROMPT 2: Hero sekce

```
Vytvoř Hero sekci pro posouzeni.cz s těmito požadavky:

LAYOUT:
- Plná šířka, min-height: 85vh na desktopu
- Dvousloupcový layout na desktopu (obsah vlevo, widget vpravo)
- Na mobilu: obsah nahoře, widget pod ním
- Pozadí: jemný gradient od #FDFAF5 do #FAF7F0

LEVÝ SLOUPEC – textový obsah:
- Malý label nahoře: "POSOUZENÍ HODNOTY NEMOVITOSTI" – uppercase, letter-spacing, barva #8B7D6B, font-size malý
- Hlavní nadpis H1 (Playfair Display, uppercase):
  "KOLIK DOOPRAVDY STOJÍ VAŠE NEMOVITOST?"
- Podnadpis (DM Sans, normální velikost, barva #5C4F3D):
  "Získejte nezávislý odhad tržní hodnoty vašeho bytu, domu nebo pozemku. Online, zdarma a během 2 minut — na základě aktuálních realizovaných prodejů ve vašem okolí."
- Pod podnadpisem 3 krátké body (NE bullet points, ale horizontální layout s jemnými SVG ikonami):
  ✓ "Odhad na základě reálných dat z katastru"
  ✓ "Výsledek ihned na obrazovce"
  ✓ "Zcela zdarma, bez závazků"
  
  Tyto body styluj jako řadu malých "badges" s teplým pozadím (#F5EDE0) a textem #5C4F3D.

- Pod tím jemný social proof text:
  "Již přes 12 000 posouzení pro majitele nemovitostí v celé ČR"

PRAVÝ SLOUPEC – widget:
- Kontejner pro widget s ID "realvisor-form"
- Widget bude mít kolem sebe jemný rámeček (#E8E0D4) a pozadí #FFFFFF s border-radius: 16px
- Nad widgetem malý text: "ZAČNĚTE ZDE" (uppercase, zlatá barva)
- Widget embed kód:
  <div id="realvisor-form"></div>
  <script src="https://realvisor-com-widget.vercel.app/widget.iife.js"></script>
  <script>
    RealvisorWidget.createValuoForm(document.getElementById('realvisor-form'), {
      apiUrl: 'https://api-production-88cf.up.railway.app/api/v1',
      formCode: 'valuo-main',
      primaryColor: '#C4943A',
      borderRadius: '16px',
      maxWidth: '520px',
      shadow: 'none'
    });
  </script>
- Widget načti přes next/script s strategy="lazyOnload"

DŮLEŽITÉ:
- Hero musí působit klidně, důvěryhodně, profesionálně
- Žádné stock-photo obrázky – čistý design
- Na pozadí může být velmi jemný geometrický pattern (SVG) nebo grain texture s nízkou opacitou
- Velké písmena v nadpisu musí být dobře čitelné, ne příliš tučné
```

---

## PROMPT 3: Sekce "Jak to funguje"

```
Vytvoř sekci "Jak to funguje" pod Hero sekcí.

NADPIS SEKCE:
- Label: "JEDNODUCHÝ PROCES" (malé, uppercase, #8B7D6B)
- H2: "TŘI KROKY K HODNOTĚ VAŠÍ NEMOVITOSTI" (Playfair Display, uppercase, #2C2416)
- Podnadpis: "Žádné složité formuláře, žádné čekání na znalce. Vše zvládnete z pohodlí domova."

TŘI KROKY – horizontální layout na desktopu, vertikální na mobilu:

Krok 1:
- Číslo: "01" (velké, zlatá barva #C4943A, Playfair Display, poloprůhledné v pozadí)
- Nadpis: "ZADEJTE ADRESU"
- Text: "Vyplňte adresu nebo katastrální údaje vaší nemovitosti. Stačí název ulice a město — systém si zbytek doplní automaticky z veřejných databází."

Krok 2:
- Číslo: "02"
- Nadpis: "UPŘESNĚTE PARAMETRY"
- Text: "Doplňte základní informace o nemovitosti — dispozici, výměru, stav a případné vybavení. Čím přesnější údaje, tím přesnější odhad."

Krok 3:
- Číslo: "03"
- Nadpis: "ZÍSKEJTE POSOUZENÍ"
- Text: "Během okamžiku obdržíte odhad tržní hodnoty vaší nemovitosti. Výsledek je založen na analýze realizovaných prodejů podobných nemovitostí ve vašem okolí."

DESIGN:
- Každý krok je na kartě s pozadím #FFFFFF, border-radius: 16px, jemný box-shadow
- Mezi kartami tenká spojovací linka (na desktopu horizontální, na mobilu vertikální) v barvě #E8E0D4
- Čísla "01", "02", "03" jsou dekorativní – velké (72px+), poloprůhledné (#C4943A s opacity 0.15) za textem
- Pod celou sekcí CTA tlačítko: "ZJISTIT HODNOTU NEMOVITOSTI" – pozadí #C4943A, text bílý, uppercase, border-radius: 16px, padding 16px 48px
- Tlačítko odscrolluje na widget v hero sekci (smooth scroll)

Pozadí sekce: #FAF7F0 (mírně odlišné od hero pro vizuální oddělení)
```

---

## PROMPT 4: Sekce důvěry a social proof

```
Vytvoř sekci budující důvěru hned pod "Jak to funguje".

NADPIS SEKCE:
- Label: "PROČ NÁM DŮVĚŘOVAT" (malé, uppercase, #8B7D6B)
- H2: "POSOUZENÍ, KTERÉMU MŮŽETE VĚŘIT" (Playfair Display, uppercase)

ČTYŘI ARGUMENTY – grid 2x2 na desktopu, 1 sloupec na mobilu:

1. "AKTUÁLNÍ DATA Z TRHU"
   "Pracujeme s daty z veřejných registrů, katastru nemovitostí a skutečně realizovaných prodejů — nikoliv s inzertními cenami, které bývají nadhodnocené."

2. "30 LET NA ČESKÉM TRHU"
   "Za službou stojí tým odborníků s více než třicetiletou praxí v oceňování a prodeji nemovitostí v České republice."

3. "NEZÁVISLÝ POHLED"
   "Nemáme důvod vaši nemovitost nadhodnocovat ani podhodnocovat. Poskytujeme objektivní posouzení bez skrytých zájmů a bez závazků."

4. "OCHRANA VAŠICH ÚDAJŮ"
   "Vaše osobní údaje zpracováváme výhradně za účelem vypracování odhadu. Nesdílíme je s třetími stranami a dodržujeme GDPR."

DESIGN KAŽDÉ KARTY:
- Pozadí: #FFFFFF
- Horní border: 3px solid #C4943A
- Border-radius: 16px
- Ikona: jednoduchý SVG symbol v barvě #C4943A (graf pro data, štít pro důvěru, lupa pro nezávislost, zámek pro GDPR)
- Jemný hover efekt – lehký posun nahoru (transform: translateY(-4px))

Pod kartami ČÍSLA V ŘADĚ (counter strip):
- "12 000+ posouzení" | "30+ let zkušeností" | "98 % spokojenost" | "Celá ČR"
- Layout: horizontální na desktopu, 2x2 grid na mobilu
- Čísla velká (Playfair Display, #C4943A), popisky malé (DM Sans, #8B7D6B)
- Oddělovač: vertikální linka #E8E0D4

Pozadí sekce: #FDFAF5
```

---

## PROMPT 5: Sekce "Pro koho je posouzení"

```
Vytvoř sekci definující cílovou skupinu.

NADPIS:
- Label: "PRO KOHO JE SLUŽBA URČENA" (malé, uppercase, #8B7D6B)
- H2: "ZNALOST HODNOTY JE PRVNÍ KROK" (Playfair Display, uppercase)
- Podnadpis: "Ať už nemovitost prodáváte, kupujete nebo jen chcete mít přehled — přesný odhad hodnoty se vždy hodí."

CÍLOVÉ SKUPINY – karty vedle sebe:

1. "PRODÁVÁTE NEMOVITOST"
   "Nastavte správnou prodejní cenu hned od začátku. Podhodnocená nemovitost znamená ztrátu peněz, nadhodnocená nemovitost znamená měsíce čekání. Správná cena přitáhne vážné zájemce."

2. "KUPUJETE NEMOVITOST"
   "Ověřte si, zda požadovaná cena odpovídá realitě. Nezávislé posouzení vám dá silnější vyjednávací pozici a ochrání vás před přeplacením."

3. "ŘEŠÍTE DĚDICTVÍ ČI ROZVOD"
   "Při vypořádání majetku potřebujete objektivní a nezpochybnitelný odhad hodnoty. Naše posouzení vám dá jasný podklad pro jednání."

4. "CHCETE MÍT PŘEHLED"
   "Sledujte, jak se mění hodnota vaší nemovitosti v čase. Ať už plánujete refinancování hypotéky nebo jen chcete znát svůj majetek."

DESIGN:
- Karty s levým borderem (4px solid #C4943A) místo horního
- Pozadí karet: #FAF7F0
- Border-radius: 16px
- Pod každou kartou malý link: "Zjistit hodnotu →" ve zlaté barvě, odkazuje smooth scroll na widget

Pozadí sekce: #FDFAF5
```

---

## PROMPT 6: FAQ sekce (accordion)

```
Vytvoř FAQ sekci s accordion komponentou.

NADPIS:
- Label: "ČASTÉ DOTAZY" (malé, uppercase, #8B7D6B)
- H2: "VŠE, CO POTŘEBUJETE VĚDĚT" (Playfair Display, uppercase)

OTÁZKY A ODPOVĚDI:

Q: "Je posouzení hodnoty nemovitosti opravdu zdarma?"
A: "Ano, základní online posouzení tržní hodnoty je zcela bezplatné a bez jakýchkoli závazků. Výsledek obdržíte ihned na obrazovce. Pokud byste v budoucnu potřebovali oficiální znalecký posudek pro banku nebo soud, rádi vás propojíme s certifikovaným odhadcem."

Q: "Jak přesný je online odhad hodnoty?"
A: "Přesnost odhadu závisí na kvalitě zadaných údajů a dostupnosti srovnatelných prodejů ve vašem okolí. U standardních bytů v městech s aktivním trhem se přesnost typicky pohybuje v rozmezí 5–10 % od skutečné tržní ceny. Odhad poskytuje spolehlivou orientaci, nikoliv závazné ocenění."

Q: "Jaké údaje o nemovitosti budu potřebovat?"
A: "Stačí základní informace: adresa nebo katastrální území, typ nemovitosti (byt, dům, pozemek), dispozice, přibližná výměra a aktuální stav. Čím přesnější údaje zadáte, tím přesnější bude výsledný odhad."

Q: "Nahradí online posouzení znalecký posudek?"
A: "Online posouzení slouží jako kvalifikovaná orientace v tržní hodnotě. Pro účely bank, soudů, dědického řízení nebo daňových přiznání je zpravidla vyžadován oficiální znalecký posudek zpracovaný soudním znalcem. Rádi vás s takovým odborníkem propojíme."

Q: "Jak nakládáte s mými osobními údaji?"
A: "Vaše údaje zpracováváme výhradně za účelem vypracování odhadu hodnoty. Nepředáváme je třetím stranám bez vašeho výslovného souhlasu a plně dodržujeme nařízení GDPR. Podrobnosti najdete v našich zásadách ochrany osobních údajů."

Q: "Mohu posouzení využít při jednání s realitní kanceláří?"
A: "Rozhodně ano. Nezávislé posouzení hodnoty vám dává silnější pozici při výběru realitního makléře i při nastavení prodejní ceny. Budete přesně vědět, co od spolupráce očekávat."

DESIGN:
- Každá otázka je řádek s tlačítkem pro rozbalení
- Aktivní otázka má zlatý levý border
- Plynulá animace rozbalení (max-height transition)
- Otázky v DM Sans semibold, odpovědi v DM Sans regular
- Pozadí: #FAF7F0
- Accordion items: #FFFFFF s jemným stínem
- Plus/minus ikona v barvě #C4943A
```

---

## PROMPT 7: Závěrečné CTA + Footer

```
Vytvoř závěrečnou CTA sekci a footer.

CTA SEKCE:
- Pozadí: jemný gradient #2C2416 (tmavá teplá) — kontrast k celé stránce
- Text bílý
- H2: "ZJISTĚTE HODNOTU SVÉ NEMOVITOSTI JEŠTĚ DNES" (Playfair Display, uppercase, bílá)
- Podnadpis: "Stačí 2 minuty. Žádné závazky, žádné poplatky." (DM Sans, #D4C8B8)
- Velké CTA tlačítko: "ZÍSKAT POSOUZENÍ ZDARMA" – pozadí #C4943A, bílý text, border-radius: 16px
- Tlačítko scrolluje na widget v hero sekci
- Pod tlačítkem malý text: "Posouzení je nezávazné a zcela bezplatné"
- Jemný dekorativní element – například tenká zlatá linka nad sekcí

FOOTER:
- Pozadí: #2C2416
- Text: #8B7D6B (tlumený)
- Obsah:
  - Logo/název: "posouzeni.cz" (Playfair Display, bílá)
  - Krátký popis: "Nezávislé posouzení hodnoty nemovitostí online. Služba provozovaná společností PTF Reality s.r.o. s více než 30 lety zkušeností na českém realitním trhu."
  - Odkazy: Ochrana osobních údajů | Obchodní podmínky | Kontakt
  - Kontakt: info@posouzeni.cz
  - Copyright: "© 2025 PTF Reality s.r.o. | Všechna práva vyhrazena"
  
- Footer je minimalistický, jednořádkový na desktopu, stackovaný na mobilu
- Žádné sociální sítě, žádné zbytečnosti
```

---

## PROMPT 8: Mobilní optimalizace a performance

```
Zkontroluj a optimalizuj celou stránku posouzeni.cz pro:

MOBILNÍ ZAŘÍZENÍ:
- Hero: widget musí být plně viditelný bez scrollování do strany, max-width: 100%
- Všechny nadpisy: na mobilu zmenšit o 25–30 %, zachovat uppercase a čitelnost
- Karty: jednosloupcový layout pod 768px
- CTA tlačítka: full-width na mobilu s dostatečným padding
- Touch targets: min 44px
- FAQ accordion: plynulý na touch zařízeních
- Žádný horizontální scroll

PERFORMANCE:
- Widget script: lazy load přes next/script strategy="lazyOnload"
- Google Fonts: preconnect + display=swap
- Obrázky: pokud nějaké jsou, next/image s lazy loading
- Celá stránka musí být renderovatelná bez JS (SSR) — widget je jediný JS-dependent prvek
- Minimální bundle size

SEO:
- Strukturovaná data (JSON-LD): LocalBusiness schema pro PTF Reality
- Canonical URL: https://posouzeni.cz
- Hreflang: cs
- Heading hierarchy: jeden H1 v hero, H2 pro sekce, H3 pro podpoložky
- Alt texty na všech obrázcích/SVG s významem
- robots.txt a sitemap.xml

ACCESSIBILITY:
- Kontrastní poměr min 4.5:1 na všech textech
- Aria labels na interaktivních prvcích
- Skip to content link
- Focus styles na tlačítkách a accordion
- Semantic HTML (main, section, nav, footer)
```

---

## PROMPT 9: Animace a micro-interactions

```
Přidej jemné animace na stránku posouzeni.cz. Styl animací: pomalé, uklidňující, elegantní – žádné rychlé bounce efekty.

SCROLL ANIMACE (Intersection Observer, žádná knihovna):
- Sekce se objevují s fade-in + translateY(20px) při scrollu do viewportu
- Delay mezi elementy v řadě (karty kroků, karty důvěry): 150ms
- Duration: 600ms, easing: cubic-bezier(0.25, 0.46, 0.45, 0.94)

HOVER EFEKTY:
- Karty: translateY(-4px) + jemné zvýraznění stínu, transition 300ms
- CTA tlačítka: pozadí ztmavne na #A67B2E, transition 200ms
- FAQ items: jemné pozadí highlight při hoveru

WIDGET KONTEJNER:
- Při načtení widgetu: jemný fade-in

COUNTER STRIP:
- Čísla: animate count-up při scrollu do viewportu (jednoduchý JS, žádná knihovna)
- "12 000+" od 0 do 12000, "30+" od 0 do 30, "98 %" od 0 do 98

SCROLL CTA TLAČÍTKA:
- Smooth scroll na widget (#realvisor-form) s offset pro header
- Behavior: smooth

OBECNĚ:
- Žádné animace na reduced-motion: @media (prefers-reduced-motion: reduce) – vypni vše
- Animace nesmí zpomalit stránku
- Vše CSS-only kromě counter animace a scroll behavior
```

---

## Souhrn struktury stránky

```
posouzeni.cz – Single page layout:

[HERO]
  ├── Label + H1 + podnadpis + badges
  ├── Social proof text
  └── Widget (RealVisor embed)

[JAK TO FUNGUJE]
  ├── 3 kroky (01, 02, 03)
  └── CTA tlačítko → scroll na widget

[DŮVĚRA]
  ├── 4 argumenty (karty)
  └── Counter strip (12 000+ | 30+ let | 98% | Celá ČR)

[PRO KOHO]
  └── 4 cílové skupiny (karty)

[FAQ]
  └── 6 otázek (accordion)

[CTA ZÁVĚR]
  └── Tmavá sekce s finálním CTA

[FOOTER]
  └── Minimalistický, právní info, kontakt
```
