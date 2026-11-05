# 11. előadás: 11. előadás Etika, algoritmusok és felelős AI - Kötelező tananyag

## 1. MIR — 11. Fejezet: Etika, algoritmusok és felelős AI (Kötelező Könyv)

(forrás: 11.1.html)

### 1. MIR — 11. Fejezet: Etika, algoritmusok és felelős AI (Kötelező Könyv)

## 2. Amikor a gép megtanulja a múlt hibáit

(forrás: 11.2.html)

### 2. Amikor a gép megtanulja a múlt hibáit

## Amikor a gép megtanulja a múlt hibáit

### Etika, algoritmusok és felelős AI

💬 Nyitó dilemma

Egy nagy technológiai vállalat 2014-ben belefogott egy ambiciózus projektbe: automatizálni akarta a toborzási folyamatot. A cél egyszerű volt — egy AI-rendszer, amely száz beérkező önéletrajzból kiválasztja az öt legjobbat, és a HR-csapatnak már csak a döntést kell meghoznia. A rendszert az elmúlt tíz év jelentkezési anyagain tanították be, hiszen ki tudná jobban megmondani, milyen egy "jó jelölt", mint a vállalat saját, bevált felvételi gyakorlata?

2015-re kiderült a probléma: a rendszer szisztematikusan hátrébb sorolta azokat az önéletrajzokat, amelyek a "women's" szót tartalmazták (pl. "women's chess club captain"), és előnyben részesítette a hagyományosan férfias kódolású igéket, mint az "executed" vagy "captured". A vállalat megpróbálta kijavítani ezeket a konkrét torzításokat, de végül nem tudta garantálni, hogy a rendszer más, rejtettebb módokon nem részesít-e továbbra is előnyben férfi jelölteket. A projektet leállították.

🤔 Mit gondolsz: hibázott-e valaki ebben a történetben — és ha igen, ki? A fejlesztő, aki megírta a kódot? A HR-vezető, aki jóváhagyta a projektet? Vagy senki, mert a rendszer "csak" a valóságot tükrözte?

💡 Tanulási eredmények

A fejezet elvégzése után Ön képes:

- megkülönböztetni a szabályalapú és a gépi tanulásos rendszerek torzítás-mechanizmusát

- elhatárolni egymástól a felelősség, elszámoltathatóság és jogi felelősség fogalmait

- klasszikus etikai elvek mentén értékelni egy AI-alapú üzleti döntést

- alkalmazni az EU AI Act kockázatalapú besorolási logikáját egy konkrét vállalati helyzetre

- kritikusan mérlegelni, mit garantálhat, és mit nem garantálhat egyetlen etikai, jogi vagy technikai védvonal sem

Ábra helye: két önéletrajz-köteg — az egyik papír, a másik adatfolyamként (bináris kód) áramlik egy fekete doboz-ikonba, amiből csak bizonyos önéletrajzok jönnek ki a másik oldalon

De hogyan is "tanul" egy ilyen rendszer — és miért másképp torzít, mint amit a 9. fejezetben megismert szabályalapú szakértői rendszerek? Erről szól a következő oldal.

Forrás: Dastin, J. (2018). Amazon Scraps Secret AI Recruiting Tool That Showed Bias Against Women. Reuters.

## 3. Emlékszel még a szakértői rendszerre?

(forrás: 11.3.html)

### 3. Emlékszel még a szakértői rendszerre?

## Emlékszel még a szakértői rendszerre?

### Retrieval — vissza a 9. fejezethez

A 9. fejezetben megismerted a szabályalapú szakértői rendszert (rule-based expert system): egy szakértő tudását explicit „HA... AKKOR...” szabályokba foglalják, és a rendszer ezek alapján hoz döntést — például eldönti, adjunk-e hitelt egy ügyfélnek, vagy diagnosztizáljunk egy gépi hibát.

💡 Műszaki analógia

Egy szabályalapú rendszer olyan, mint egy nagyon részletes, előre megírt folyamatábra — minden elágazás valakinek a tudatos döntése. Ha torzítás kerül bele, az azért van, mert valaki, valahol, egy konkrét szabályba beleírta (tudatosan vagy figyelmetlenségből).

🤔 Reflektív kérdés

Ha egy banki hitelbírálati szakértői rendszer szabályai közé valaki beírná, hogy „a 25 év alatti jelentkezők kockázati pontszámát emeljük meg 10 ponttal” — ki lenne felelős ezért? Hogyan deríthetnéd ki, hogy ez a szabály egyáltalán létezik?

Ez a kérdés a szabályalapú rendszereknél viszonylag könnyen megválaszolható: a szabálybázis átlátható és visszakereshető — pontosan meg lehet mutatni, melyik sor okozza a problémát. Ez az elszámoltathatóság egyik alapfeltétele, amivel az 5. oldalon részletesebben foglalkozunk.

De mi történik akkor, ha a rendszer nem kész szabályokat kap, hanem maga alakítja ki a döntési logikáját — ahogyan az Amazon-féle toborzási AI is tette? Erről szól a következő oldal.

Forrás: MIS_KMS.pdf, 3. modul — Tudásmenedzsment. Óbudai Egyetem, ÜTDI, Prof. Dr. Tick Andrea.

## 4. Amikor a rendszer nem szabályt kap, hanem mintázatot tanul

(forrás: 11.4.html)

### 4. Amikor a rendszer nem szabályt kap, hanem mintázatot tanul

## Amikor a rendszer nem szabályt kap, hanem mintázatot tanul

### A gépi tanulásos torzítás mechanizmusa

A gépi tanulásos rendszer alapvetően másképp működik, mint a szabályalapú elődje. Nem kap kész szabályokat — helyette egy nagy mennyiségű történeti adatból statisztikai mintázatokat von ki. Az Amazon-esetben a rendszer tíz év önéletrajzán tanult; mivel a technológiai szektor hagyományosan férfi-dominanciájú volt, ezek az önéletrajzok túlnyomórészt férfiaktól származtak. A rendszer ebből nem azt „tanulta meg”, hogy nőket kell hátrányosan kezelni — hanem azt, hogy bizonyos szavak és mintázatok (amelyek véletlenül gyakrabban fordultak elő a „sikeresnek” minősített, jellemzően férfi jelentkezők anyagaiban) magasabb pontszámmal járnak.

A lényegi különbség a szabályalapú torzításhoz képest:

Szempont | Szabályalapú rendszer | Gépi tanulásos rendszer | 

A torzítás forrása | Egy konkrét, valaki által megírt szabály | Az adathalmaz statisztikai eloszlása | 

Visszakereshetőség | Könnyű — megmutatható a hibás szabály | Nehéz — a döntés több ezer súly együttes hatása | 

Szándékosság | Általában tudatos (vagy hanyagságból eredő) | Jellemzően nem szándékos, hanem „örökölt” | 

Miért nevezik „fekete doboznak”? | Nem releváns — a logika olvasható | Mert a belső működés nem emberi léptékben értelmezhető | 

A modern, különösen a mély tanulási (deep learning) rendszerek emiatt számítanak „fekete doboznak” (black box) — nehéz betekinteni a belsejükbe, ami komoly problémát jelent az átláthatóság és elszámoltathatóság szempontjából.

💡 Műszaki analógia

Képzeld el, hogy nem egy folyamatábrát kapsz, hanem több ezer, egymással összefonódó mérleget, amelyek együttesen billennek egyik vagy másik irányba — nincs egyetlen mérleg, amit „kicserélve” megoldanád a problémát.

⚠️ Kritikai figyelmeztetés

Fontos tudatosítani: a torzítás nem azért keletkezik, mert az algoritmus „rosszindulatú” volna. Az adattorzítás akkor jelenik meg, amikor a tanító adathalmazban bizonyos csoportok alul- vagy túlreprezentáltak; ettől függetlenül létezik algoritmikus torzítás is, amikor maga a modell felépítése vagy súlyozási módja okoz torzítást. A felelősség emberi marad — csak a hiba mechanizmusa más.

Forrás: Dastin, J. (2018). Reuters.

## 5. Hat elv, egy valós gyártási döntés

(forrás: 11.5.html)

### 5. Hat elv, egy valós gyártási döntés

## Hat elv, egy valós gyártási döntés

### Klasszikus etikai elvek egy műszaki döntési helyzetre alkalmazva

📖 Fogalom

Laudon hat klasszikus etikai elvet azonosít, amelyek segítenek eligazodni morális dilemmákban.

A helyzet: egy gyártó vállalat mérlegeli, hogy bevezet-e egy gépi tanulásos, gépi látáson alapuló minőségellenőrző rendszert, amely 97%-os pontossággal szűri ki a hibás termékeket — de a fennmaradó 3%-ot senki nem ellenőrzi emberi szemmel, mert ez lenne a teljes költségmegtakarítás lényege.

Etikai elv | Rövid meghatározás | Alkalmazás erre a helyzetre | 

Aranyszabály | Tedd másokkal azt, amit szeretnél, hogy veled tegyenek | Elfogadnád-e, hogy a te biztonságodat érintő terméket egy 3%-os hibaarányú, felügyelet nélküli rendszer engedje át? | 

Kant kategorikus imperatívusza | Csak úgy cselekedj, hogy a cselekvésed elve egyetemes törvénnyé válhasson | Ha minden gyártó feladná az emberi ellenőrzést a költségmegtakarítás kedvéért, elfogadható lenne-e ez társadalmi szinten? | 

Lejtő-elv (slippery slope) | Egy látszólag ártalmatlan lépés visszafordíthatatlan folyamatot indíthat el | Ha ma elfogadjuk a 3%-os felügyelet nélküli hibaarányt, holnap elfogadjuk-e az 5%-ot is, ha az még olcsóbb? | 

Utilitarista elv | Azt a cselekvést válaszd, amely a legtöbb embernek a legtöbb hasznot hozza | A megtakarított költség hány munkahelyet menthet meg — szemben a hibás termékek okozta esetleges károkkal? | 

Kockázatkerülési elv | A legnagyobb kárt okozó lehetőséget kerüld, még alacsony bekövetkezési valószínűség esetén is | Mi történik, ha éppen a 3%-ba egy biztonságkritikus alkatrész-hiba esik? | 

„Nincs ingyen ebéd” elv | Minden érték valakinek a tulajdona vagy munkája — ha felhasználod, kompenzációt kell adnod | Ha a rendszer az eddigi minőségellenőrök tapasztalatán (történeti hibaadatokon) tanult, jár-e nekik valamilyen elismerés vagy átképzési lehetőség? | 

🤔 Reflektív kérdés

Melyik elv alapján hoznál te döntést ebben a helyzetben — és mit tennél, ha kettő közülük ellentétes következtetésre vezetne?

Forrás: Laudon, K. C., & Laudon, J. P. Management Information Systems. 15. kiadás, 4. fejezet.

## 6. Három fogalom, amit gyakran összekevernek

(forrás: 11.6.html)

### 6. Három fogalom, amit gyakran összekevernek

## Három fogalom, amit gyakran összekevernek

### Felelősség, elszámoltathatóság, jogi felelősség

Felelősség (responsibility)

Annak elfogadása, hogy valaki viseli döntéseinek költségeit, kötelezettségeit és következményeit.

 | 

Elszámoltathatóság (accountability)

Rendszerek és intézmények jellemzője — olyan mechanizmusok megléte, amelyek lehetővé teszik annak megállapítását, ki tett valamit, és ki felelős érte.

 | 

Jogi felelősség (liability)

A felelősség fogalmának kiterjesztése a jog területére — olyan jogi keret, amely lehetővé teszi, hogy az egyének kártérítést követeljenek másoktól elszenvedett károkért.

 | 

💡 Műszaki analógia

Gondolj egy repülőgép-balesetre. A felelősség azé, aki hibázott. Az elszámoltathatóság az a rendszer (a fekete doboz, a karbantartási napló), ami lehetővé teszi, hogy egyáltalán kiderítsük, ki hibázott. A jogi felelősség az, ami alapján az áldozatok családja kártérítést kaphat.

#### Hazai eset — amikor a „van emberi döntés a végén” sem elég

2022-ben a Nemzeti Adatvédelmi és Információszabadság Hatóság (NAIH) megállapította, hogy egy hazai bank közel négy éven keresztül olyan mesterséges intelligencia alapú hangelemző rendszert alkalmazott, amely automatikusan elemezte az ügyfélszolgálatra telefonáló ügyfelek hanghordozását és érzelmi állapotát. Bár a folyamat végén formálisan emberi döntés született, a NAIH megállapította, hogy az adatkezelés az érintettekre nézve joghatással bírhatott, és a bank nem tájékoztatta megfelelően az érintetteket az alkalmazott logikáról és annak következményeiről.

⚠️

Ez a hazai eset pontosan azt mutatja, amiről ez az oldal szól: az, hogy „végül egy ember dönt”, önmagában nem old meg minden elszámoltathatósági problémát — ha az ember nem érti, vagy nem tudja megmagyarázni, milyen logika alapján kapta a rendszer javaslatát, az elszámoltathatóság akkor is sérülhet.

🤔 Reflektív kérdés

Ha egy vállalati AI-rendszer hibás döntést hoz, és a fejlesztő azt mondja „a rendszer magától tanulta ezt, nem én programoztam bele” — elfogadható-e ez válasznak?

A magyarázhatóság technikai eszközeiről — pl. Explainable AI (XAI) — bővebben az ÜIA Adat és MI-etika leckéjéből és az Opcionális Könyvből tudhatsz meg többet.

Forrás: Laudon, K. C., & Laudon, J. P. Management Information Systems. 15. kiadás, 4. fejezet. — NAIH-85-3/2022 határozat, Nemzeti Adatvédelmi és Információszabadság Hatóság.

## 7. A matematikai méltányossági paradoxon

(forrás: 11.7.html)

### 7. A matematikai méltányossági paradoxon

## Amikor a méltányosság nem technikai, hanem matematikai kérdés

### A matematikai méltányossági paradoxon

⚠️ Kritikai figyelmeztetés

Ez a fejezet legmélyebb, legfontosabb belátása: a méltányosság nem „megoldható” probléma — hanem tudatos kompromisszum.

2016-ban Jon Kleinberg, Sendhil Mullainathan és Manish Raghavan matematikailag bebizonyították, hogy — ha a csoportok között eltérő az alap-előfordulási gyakoriság (base rate) — nem létezik olyan algoritmus, amely egyszerre tudná teljesíteni a következő két, önmagában ésszerűnek tűnő méltányossági kritériumot: hogy a kockázati pontszám ugyanazt jelentse minden csoportra nézve (kalibráció), és hogy a pozitív, illetve negatív besorolású egyének átlagos pontszáma megegyezzen csoportonként (osztályozási egyensúly) — kivéve, ha az algoritmus tökéletes előrejelzést érne el.

💡 Műszaki analógia

Ez olyan, mint amikor egy híd tervezésénél egyszerre szeretnéd maximalizálni a teherbírást, minimalizálni a költséget, és minimalizálni az építési időt — bizonyos kombinációk egyszerűen matematikailag kizárják egymást, nem azért, mert rosszul terveztél, hanem mert a matematika ezt diktálja.

🤔 Reflektív kérdés

Ha egyszerre nem lehet minden méltányossági kritériumnak megfelelni, ki dönti el, melyik számít fontosabbnak — a fejlesztő, a vállalat vezetése, a jogalkotó, vagy a bíróság?

Ez nem csak elméleti tétel — egy valós, nagy port kavaró kutatás pontosan ezt igazolta gyakorlatban is. Erről szól a következő oldal.

Forrás: Kleinberg, J., Mullainathan, S., & Raghavan, M. (2016). Inherent Trade-Offs in the Fair Determination of Risk Scores.

## 8. A ProPublica COMPAS-kutatás

(forrás: 11.8.html)

### 8. A ProPublica COMPAS-kutatás

## Amikor két fél közül mindkettő igazat mond — és mégis vitáznak

### A ProPublica COMPAS-kutatás

A ProPublica (amerikai oknyomozó újságírói szervezet) 2016-ban megvizsgálta a COMPAS nevű szoftvert, amelyet amerikai bíróságokon használnak a vádlottak visszaesési kockázatának becslésére. A ProPublica azt találta, hogy azok közül, akik a következő két évben nem estek vissza bűnözésbe, az afroamerikai vádlottak 45%-át tévesen sorolta magas kockázatúnak a rendszer, míg a fehér vádlottaknál ez az arány csak 24% volt.

A rendszer fejlesztője azzal válaszolt, hogy az eltérés a két csoport eltérő alap-visszaesési arányából adódik — és technikailag igaza volt: a rendszer kalibrált volt, csak nem volt egyben osztályozásilag kiegyensúlyozott is. Ez pontosan a Kleinberg–Mullainathan–Raghavan-tétel gyakorlati megnyilvánulása (6. oldal) — mindkét fél technikai szempontból igazat állított, mégis homlokegyenest ellenkező következtetésre jutottak.

🤔 Reflektív kérdés

Ha te lennél a bíróság döntéshozója, és tudnád, hogy egy ilyen rendszer matematikailag nem lehet egyszerre mindenre nézve méltányos — használnád-e egyáltalán a döntésed támogatására?

Az Amazon-eset és a COMPAS-eset ugyanazt üzeni: a méltányosság technikai garantálása korlátozott — az emberi felügyelet és a tudatos értékválasztás nem kiváltható.

Forrás: Angwin, J., Larson, J., Mattu, S., & Kirchner, L. (2016). Machine Bias. ProPublica.

## 9. Nem minden AI egyforma kockázatú

(forrás: 11.9.html)

### 9. Nem minden AI egyforma kockázatú

## Nem minden AI egyforma kockázatú

### Az EU AI Act kockázatalapú szabályozása egy gyártó cég szemszögéből

⚠️ Fontos: ez a szabályozási táj folyamatosan mozog

E tananyag elkészültekor (2026 nyara) az EU AI Act magas kockázatú kötelezettségei éppen módosuláson mennek át: az eredetileg 2026. augusztus 2-i határidőt egy 2026 májusában elért politikai megállapodás 2027. december 2-ra halasztja a toborzási/teljesítményértékelő rendszerek esetében. Ez jól mutatja: a szabályozás maga is élő, változó folyamat — mire ezt olvasod, érdemes ellenőrizned az aktuális állást.

Az EU AI Act (2024-ben elfogadott rendelet) a világ első átfogó, jogilag kötelező erejű AI-szabályozása, amely kockázatalapú megközelítést alkalmaz: minél nagyobb a kockázat, annál szigorúbb a szabályozás.

#### Gyakorlati példa — egy közepes méretű magyar gyártó cég AI-alkalmazásai

Kockázati kategória | Példa a gyártó cégnél | Következmény | 

Minimális kockázat | Gépi látáson alapuló hibafelismerő rendszer a gyártósoron | Nincs különös szabályozás | 

Korlátozott kockázat | Ügyfélszolgálati chatbot | Átláthatósági kötelezettség: jelezni kell, hogy AI-val kommunikál a felhasználó | 

Magas kockázat | Automatizált toborzási/előszűrő rendszer (mint az Amazon-eset), vagy munkavállalói teljesítményértékelő AI | Kockázatértékelés, dokumentáció, emberi felügyelet, átláthatóság kötelező | 

Elfogadhatatlan kockázat | Munkavállalók valós idejű biometrikus viselkedés-megfigyelése a gyártócsarnokban | Tilos | 

#### Fontos megkülönböztetés — ki a „te” ebben a táblázatban?

A fenti táblázat a te vállalatod által használt AI-rendszerek kockázati besorolásáról szól. Magukat az AI-modelleket (pl. amit egy chatbot mögött használsz) fejlesztő cégekre (OpenAI, Anthropic, Google) külön, párhuzamos szabályozási réteg vonatkozik: az AI Act V. fejezete (51–56. cikk) már 2025 augusztusa óta kötelezi az általános célú AI-modellek (GPAI) fejlesztőit technikai dokumentáció, szerzői jogi megfelelési politika és nyilvános tanítóadat-összefoglaló közzétételére. Ezt a kötelezettséget nem érinti a fenti halasztás.

🤔 Reflektív kérdés

Te, mint leendő műszaki menedzser: melyik kategóriába sorolnál egy olyan rendszert, amely a munkavállalók billentyűzet-aktivitását figyeli „termelékenységi” célból?

Forrás: EU AI Act Omnibus Agreement — Postponed High-Risk Deadlines and Other Key Changes, Gibson Dunn (2026). — Article 53: Obligations for Providers of General-Purpose AI Models, EU Artificial Intelligence Act.

## 10. Mennyibe kerül energetikailag egy AI-válasz?

(forrás: 11.10.html)

### 10. Mennyibe kerül energetikailag egy AI-válasz?

## Mennyibe kerül energetikailag egy AI-válasz?

### Rövid technikai kitekintés: az AI energiaköltsége

Ahogy az ÜIA Fenntartható IT leckéjéből már tudod, az adatközpontok energiafogyasztása jelentős. Amit érdemes hozzátenni: maga a mesterséges intelligencia feladattípusa is drámaian eltérő energiaköltséggel jár. Egy 2025-ös kutatás szerint egy rövid AI-lekérdezés megválaszolása kb. 0,4 Wh energiát igényelhet, míg egy hosszú, összetett következtetést igénylő feladat akár 33 Wh-t is elérhet — vagyis közel 80-szoros a különbség.

🤔 Reflektív kérdés

Ha te vezetnél egy céget, amely AI-alapú döntéstámogató rendszert vezet be, figyelembe vennéd-e, hogy egy „egyszerű igen/nem döntés” vagy egy „részletes elemzés” kérése a rendszertől mekkora energiaköltséggel jár?

Ez ugyanaz a stratégiai szemlélet, amit a 10. fejezetben a felhő-döntéseknél is megtanultál: a technológiai döntés soha nem csak informatikai kérdés, hanem üzleti és fenntarthatósági döntés is.

Forrás: Jegham, N. et al. (2025). Benchmark study of 30 large language models.

## 11. Vissza a kiindulóponthoz

(forrás: 11.11.html)

### 11. Vissza a kiindulóponthoz

## Vissza a kiindulóponthoz

### Szintézis, pozitív ellenpélda és kritikai záróértékelés

✅ Pozitív ellenpélda, kontrasztként

Nem minden hasonló helyzet végződik kudarccal. Amikor a LinkedIn 2018 körül hasonló problémát észlelt saját Talent Search algoritmusában — a keresési találatok nem tükrözték arányosan a releváns, képzett jelöltek nemek szerinti eloszlását —, nem eltitkolta vagy csendben leállította a rendszert. Mérnökei egy méltányosság-tudatos újrarangsorolási algoritmust fejlesztettek, amely a végső találati listát úgy állítja össze, hogy arányosan tükrözze a releváns jelölti kör összetételét, és ezt szakmai, lektorált tudományos konferencián publikálták. Ugyanaz a probléma-típus, mint az Amazon-esetnél — csak átlátható, dokumentált, technikailag ellenőrizhető megoldással.

🔁 Záró visszatérés a nyitó dilemmához

Emlékezz az 1. oldal Amazon-esetére. Most már tudod: miért torzult a rendszer (3. oldal), milyen elvek mentén értékelhetted volna (4. oldal), ki lett volna felelős (5. oldal), miért nem lehetett volna egyszerűen „kijavítani” a méltányosságot (6–7. oldal), milyen jogi kategóriába esne ma (8. oldal) — és hogy létezik jobb út is (LinkedIn-eset, fent).

#### Kritikai záróértékelés: elég-e mindez együtt?

A fejezet három védvonalat mutatott be: etikai elvek, elszámoltathatósági mechanizmusok, szabályozás. Érdemes együtt is megnézni: elégséges-e ez a három védvonal?

✅ Pro

- Az etikai elvek döntési keretet adnak, amikor a jog még nem szabályoz
- Az elszámoltathatóság legalább visszakövethetővé teszi a hibát
- A szabályozás jogilag kikényszeríthető keretet ad
- Együttesen jelentősen csökkentik a kockázatot

 | 

⚠️ Kontra

- Az elvek gyakran ellentmondanak egymásnak — nem adnak egyértelmű választ
- A méltányossági paradoxon miatt az audit is csak azt mutatja meg, melyik kritérium sérül
- A jogalkotás mindig lassabb, mint a technológia
- Együttesen sem garantálják egy új, ismeretlen torzítási mintázat időbeni felismerését

 | 

Műszaki-menedzseri szemszög: a te felelősséged nem az, hogy magad írj AI-algoritmust — hanem hogy fel tudd tenni a helyes kérdéseket: milyen adaton tanult a rendszer? Ki tudja megmagyarázni a döntéseit? Milyen kockázati kategóriába esik? Milyen emberi felügyeletet igényel?

🤔 Záró reflektív kérdés

Ha holnap a te vállalatod vezetése elé kerülne egy hasonló AI-projekt-javaslat, milyen három kérdést tennél fel először?

A következő fejezetben azt vizsgáljuk meg, hogyan segíthet egy jól megválasztott AI- és digitalizációs stratégia — beruházás-gazdaságossági szempontból is — abban, hogy egy vállalat valóban felkészült legyen a digitális jövőre.

Forrás: Geyik, S. C., Ambler, S., & Kenthapadi, K. (2019). Fairness-Aware Ranking in Search & Recommendation Systems with Application to LinkedIn Talent Search. KDD '19.

## 12. Elmélyítő kiegésztő

(forrás: 11.12.html)

### 12. Elmélyítő kiegésztő

- Fabris, A., Baranowska, N., Dennis, M. J., Graus, D., Hacker, P., Saldivar, J., Zuiderveen Borgesius, F., & Biega, A. J. (2024). Fairness and Bias in Algorithmic Hiring: A Multidisciplinary Survey. ACM Transactions on Intelligent Systems and Technology. https://doi.org/10.1145/3696457
- Kleinberg, Mullainathan & Raghavan (2016/2017) — Inherent Trade-Offs in the Fair Determination of Risk Scores (arXiv:1609.05807) https://doi.org/10.4230/LIPIcs.ITCS.2017.43
- NAIH-85-3/2022 határozat + a WP251 (29. cikk szerinti Adatvédelmi Munkacsoport) iránymutatása az automatizált döntéshozatalról 
- https://www.naih.hu/hatarozatok-vegzesek?download=517%3Amesterseges-intelligencia-alkalmazasanak-adatvedelmi-kerdesei; kiegészítő iránymutatás: 29. cikk szerinti Adatvédelmi Munkacsoport, WP251 https://www.naih.hu/files/wp251rev01_hu.pdf
- Csatlós Erzsébet: Az ügyfél és a hatósági döntéshozatal a digitalizáció korában (Pro Futuro, 2023/1.) DOI: https://doi.org/10.26521/profuturo/2023/1/13356

## 1. MIR — 11. Fejezet: Etika, algoritmusok és felelős AI (Opcionális Könyv)

(forrás: 11.13.html)

### 1. MIR — 11. Fejezet: Etika, algoritmusok és felelős AI (Opcionális Könyv)

## 2. Fogalmak, amikre a fejezet épül

(forrás: 11.14.html)

### 2. Fogalmak, amikre a fejezet épül

## Fogalmak, amikre a fejezet épít

### AI-etika alapfogalom-tár

Ez az oldal összegyűjti azokat az alapfogalmakat, amelyeket a Kötelező Könyv több helyen is használ — érdemes ide visszalapozni, ha egy kifejezés nem egyértelmű.

Fogalom | Rövid meghatározás | 

Fairness (méltányosság) | Annak elve, hogy egy algoritmus döntései ne részesítsenek indokolatlanul előnyben vagy hátrányba egyes csoportokat védett tulajdonságaik (pl. nem, életkor, etnikai hovatartozás) alapján. | 

Bias (torzítás) | Egy rendszeres, nem véletlenszerű eltérés, amely miatt egy AI-rendszer kimenete következetesen kedvezőbb vagy kedvezőtlenebb egy adott csoport számára. | 

Explainability (magyarázhatóság) | Annak képessége, hogy egy AI-rendszer döntését emberi nyelven, érthetően meg lehessen indokolni. | 

AI-governance (AI-kormányzás) | Azon szabályok, folyamatok és felelősségi körök összessége, amelyek egy szervezeten belül biztosítják az AI-rendszerek felelős fejlesztését és üzemeltetését. | 

Responsibility (felelősség) | Annak elfogadása, hogy valaki viseli döntéseinek költségeit és következményeit. | 

Accountability (elszámoltathatóság) | Olyan mechanizmusok megléte, amelyek lehetővé teszik annak megállapítását, ki tett valamit, és ki felelős érte. | 

Liability (jogi felelősség) | A felelősség jogi kiterjesztése — olyan keret, amely alapján kártérítés követelhető. | 

Forrás: Laudon, K. C., & Laudon, J. P. Management Information Systems. 15. kiadás, 4. fejezet. — ÜIA Adat és MI-etika lecke.

## 3. Torzítás-csökkentési technikák alapszinten

(forrás: 11.15.html)

### 3. Torzítás-csökkentési technikák alapszinten

## Mit jelent a gyakorlatban az "adatok kiegyensúlyozása"?

### Torzítás-csökkentési technikák alapszinten

A Kötelező Könyv 3. oldala bemutatta, hogy a gépi tanulásos torzítás forrása gyakran maga a tanító adathalmaz. Ezen az oldalon néhány alapszintű technikát mutatunk be, amivel ez a probléma csökkenthető.

Technika | Mit jelent egyszerűen | 

Adat-újrasúlyozás (reweighting) | A tanítás során az alulreprezentált csoportokhoz tartozó adatpontok nagyobb súlyt kapnak, hogy a rendszer ne „tanulja meg alábecsülni” őket. | 

Adat-kiegyensúlyozás (rebalancing) | Ha egy adathalmazban egy csoport aránytalanul kevés, mesterségesen több példát vonnak be belőle (vagy csökkentik a túlreprezentált csoport arányát), hogy a végeredmény kiegyensúlyozottabb legyen. | 

Utólagos küszöbérték-korrekció | A rendszer már meghozta a döntést, de csoportonként eltérő elfogadási küszöböt alkalmaznak, hogy a végeredmény arányai kiegyenlítettebbek legyenek. | 

Fontos tudni: ezek a technikák csökkentik, de nem szüntetik meg teljesen a torzítás kockázatát — ahogy a Kötelező Könyv 6. oldala bemutatja, bizonyos méltányossági kritériumok matematikailag nem teljesíthetők egyszerre.

Forrás: ÜIA Adat és MI-etika lecke.

## 4. XAI alapfogalmak

(forrás: 11.16.html)

### 4. XAI alapfogalmak

## Mi az a "magyarázható AI"?

### XAI alapfogalmak

A Kötelező Könyv 5. oldala említi, hogy léteznek technikai eszközök egy AI-rendszer döntésének megmagyarázására. Ez az oldal két elterjedt módszert mutat be, nagyon egyszerű szinten.

Módszer | Mit csinál egyszerűen | Fő korlátja | 

LIME (Local Interpretable Model-agnostic Explanations) | Egy adott egyedi döntés körül egy egyszerűbb, érthető modellt épít, hogy megmutassa, mely tényezők befolyásolták leginkább az eredményt. | Csak az adott egyedi esetre ad magyarázatot, nem az egész rendszer működésére. | 

SHAP (SHapley Additive exPlanations) | Minden egyes bemeneti tényezőhöz (pl. életkor, végzettség) egy „hozzájárulási pontszámot” rendel, megmutatva, mennyit nyomott a latba a végső döntésben. | Számításigényes, és a pontszámok értelmezése technikai háttértudást igényelhet. | 

Ezek az eszközök nem oldják meg a „fekete doboz” problémát teljesen, de segítenek abban, hogy legalább utólag, esetenként belátható legyen, mi vezetett egy adott döntéshez.

Forrás: ÜIA Adat és MI-etika lecke.
