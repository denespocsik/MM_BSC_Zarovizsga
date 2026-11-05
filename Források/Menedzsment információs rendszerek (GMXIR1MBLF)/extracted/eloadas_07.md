# 7. előadás: 7. előadás BI a gyakorlatban II. - Kötelező tananyag

## 1. 7. előadás: BI a gyakorlatban — Kötelező Könyv

(forrás: 7.1.html)

### 1. 7. előadás: BI a gyakorlatban — Kötelező Könyv

## 2. Retrieval és a Tokola-kutatás

(forrás: 7.2.html)

### 2. Retrieval és a Tokola-kutatás

## Retrieval + Tokola et al. (2016): mit mutat egy valódi gyártási dashboard-kutatás?

### BI a gyakorlatban: valós kutatás, OLAP és adatbányászat

🔄 Gyors felidézés a 6. előadásból

Mit jelent a Goodhart-törvény egy mondatban? És mi volt az OEE három komponense?

Eddig elméleti keretekben (KPI-tervezés, Goodhart, OEE, BSC) és tervezési elvekben (Tufte, Few) gondolkodtunk. Most nézzük meg, mit mutat egy valódi, publikált tudományos kutatás arról, hogyan használnak (vagy használnak rosszul) a gyártó cégek dashboardokat.

📖 Kutatás

Tokola, H., Gröger, C., Järvenpää, E., & Niemi, E. (2016). "Designing Manufacturing Dashboards on the Basis of a Key Performance Indicator Survey" (Procedia CIRP). A szerzők gyártóüzemi dashboardokat vizsgáltak, és arra jutottak, hogy a legtöbb vállalati dashboard nem a döntéshozó tényleges kérdéseiből indul ki, hanem abból, hogy milyen adat éppen rendelkezésre áll a rendszerben. Egy strukturált tervezési módszertant javasolnak, amely a KPI-kiválasztást a felhasználói szerepkörhöz (műszakvezető, üzemvezető, felső vezetés) igazítja.

Miért fontos ez nekünk? Mert pontosan azt igazolja empirikusan, amit a 6. előadás nyitó dilemmájában (22 KPI egy képernyőn) intuitívan éreztünk: a probléma nem a mutatók száma, hanem az, hogy nem lett átgondolva, kinek, milyen döntéshez kell az adott mutató.
[kép]

Ábra: Hogyan bomlik le egy vállalati célszám (pl. OEE) a szervezeti hierarchia szintjein különböző részletezettségű dashboardokká

🤔 Reflektív kérdés

A saját céged dashboardjai a rendelkezésre álló adatból indulnak ki, vagy abból a kérdésből, amit a döntéshozónak tényleg meg kell válaszolnia?

💡 Tanulási eredmények

A fejezet elvégzése után Ön képes:

- kritikusan értékelni egy valós tudományos kutatás (Tokola et al., 2016) eredményeit és azok gyakorlati korlátait a gyártási dashboard-tervezésben

- alkalmazni az OLAP-műveleteket (szeletelés, kockázás, lefúrás, összesítés) mint gondolkodásmódot konkrét üzleti kérdések megválaszolására

- bemutatni a KDD-folyamat lépéseit, és felismerni a GIGO-probléma kockázatát az adatbányászati projektekben

- megkülönböztetni az adatbányászat fő üzleti alkalmazási területeit (társításelemzés, osztályozás, csalásdetektálás, keresletelőrejelzés, ajánlórendszer, hitelbírálat), és minden esetben azonosítani, milyen menedzseri döntést támogatnak

- kritikusan elemezni a Target-esetet a prediktív elemzés etikai határai szempontjából (hamis pozitív/negatív arányok, adatvédelem)

- szintetizálni a fejezet tanulságait saját műszaki menedzseri döntéshozatali gyakorlatára vonatkoztatva

Forrás: Tokola, H., et al. (2016). Procedia CIRP, 57, 619–624.

## 3. OLAP mint gondolkodásmód

(forrás: 7.3.html)

### 3. OLAP mint gondolkodásmód

## OLAP mint gondolkodásmód

### Nem technika, hanem nyomozás

Az OLAP (Online Analytical Processing) alapműveleteit — slice, dice, drill-down, roll-up — technikai kockaműveletként szokás tanítani. Itt egy másik nézőpontot választunk: az OLAP nem technika, hanem gondolkodásmód — az a képesség, hogy egy vezető ne csak mit lásson, hanem folyamatosan új kérdéseket tudjon feltenni az adatnak.

Nézzünk egy konkrét üzleti forgatókönyvet:

Kiinduló kérdés: "Miért nőtt a selejtarány a múlt hónapban?"

- Slice — kimetsszük az adatkockából csak a "selejt" dimenziót, adott hónapra: látjuk, hogy a selejtarány 3%-ról 5%-ra nőtt.

- Dice — több dimenziót egyszerre szűrünk: gyártósor + műszak + termékcsalád kombinációját nézzük, hogy szűkítsük a kört.

- Drill-down — lemegyünk a havi összesítésről napi, majd műszakos szintre: kiderül, hogy a növekedés túlnyomó része a hétvégi éjszakai műszakra koncentrálódik.

- Roll-up — visszalépünk magasabb szintre: megnézzük, hogy ez a hétvégi mintázat más gyártósorokon is jelentkezik-e, vagy csak egyetlen gépnél.

A gondolkodásmód lényege: minden egyes OLAP-művelet egy-egy miért-kérdésre ad választ, és minden válasz egy újabb kérdést nyit meg. Ez alapvetően különbözik attól, amikor valaki egyetlen statikus riportot néz.

Mikor elég egy OLAP-lekérdezés, és mikor kell mélyebbre menni? Az OLAP kiválóan alkalmas arra, hogy megmondja, hol van a probléma — de nem mondja meg, miért pont ott. A kiváltó ok feltárásához már mélyebb, statisztikai vagy adatbányászati elemzés kell — ez vezet át minket a következő oldalra.
[kép]

Ábra: 3D adatkocka - slice/dice/drill-down/roll-up műveletek

🤔 Menedzseri kérdés

Gondolj egy saját munkahelyi problémára — végig tudnád-e vinni ugyanezt a négylépéses "nyomozást" (slice → dice → drill-down → roll-up) a saját adataidon?

Forrás: Laudon & Laudon, Ch.6 — OLAP-alapfogalmak, kibővítve saját üzleti forgatókönyvvel.

## 4. A KDD-folyamat

(forrás: 7.4.html)

### 4. A KDD-folyamat

## A KDD-folyamat: az adatbányászat "receptje" — és ahol a legtöbb hiba történik

### GIGO: szemét be, szemét ki

Mielőtt belevágnánk a konkrét adatbányászati technikákba, tisztázzuk a folyamatot, amelybe azok illeszkednek. A KDD (Knowledge Discovery in Databases) klasszikus modelljét Fayyad, Piatetsky-Shapiro és Smyth (1996) írta le, és lényegében ma is ez az adatbányászat "receptje":

- Kiválasztás (Selection) — melyik adatforrásból, mely adatokra van szükségünk a kérdés megválaszolásához?

- Előfeldolgozás (Preprocessing) — hiányzó, hibás, duplikált adatok kezelése

- Transzformáció (Transformation) — az adat olyan formára hozása, amit az algoritmus fel tud dolgozni

- Adatbányászat (Data Mining) — maga az algoritmus futtatása (osztályozás, csoportosítás, társításelemzés stb.)

- Kiértékelés/interpretáció — az eredmény mintázatok üzleti értelmezése: valódi felismerés, vagy statisztikai véletlen?

A kulcsfontosságú tanulság: a folyamat öt lépéséből három (1–3) az adat előkészítéséről szól, és csak a negyedik lépés maga a "bányászat" — amit köznyelvben az egész folyamattal azonosítunk.
[kép]

Ábra: KDD-folyamat

Ez direkt kapcsolódik a GIGO-elvhez ("Garbage In, Garbage Out"): ha egy hibás vagy hiányos adatból indulunk ki, a legkifinomultabb algoritmus is hibás vagy félrevezető mintázatot fog "felfedezni". A Laudon-tankönyv (Ch.6) konkrét, vállalati szintű alátámasztást ad erre: a Gartner becslése szerint a nagyvállalatok adatbázisaiban a kritikus adatok több mint 25%-a pontatlan vagy hiányos. Egy széles körben idézett iparági felmérés szerint (Press, 2016, Forbes) az adatelemzők idejük kb. 80%-át töltik adat-előkészítéssel.

Hogyan segít ma az AI ebben? A Laudon 18. kiadása szerint az AI-t ma már arra is használják, hogy megkönnyítse magát az adatmenedzsmentet — osztályozásban, katalogizálásban, adatminőség-javításban, biztonságban, adatintegrációban és -elemzésben egyaránt. Ez azt jelenti, hogy a KDD-folyamat 1–3. lépése egyre inkább maga is AI-támogatottá válik — de ez nem szünteti meg a GIGO-elvet, csak áthelyezi: most már azt is meg kell kérdeznünk, hogy az adatminőséget javító AI-eszköz maga mennyire megbízható.

🤔 Reflektív kérdés

Ha egy adatbányászati projektet indítanál a saját üzemedben, becslésed szerint mennyi időt töltenél adat-előkészítéssel a tényleges "bányászathoz" képest — és ez a becslés most, hogy ismered a 80%-os arányt, változott?

Forrás: Fayyad, U., Piatetsky-Shapiro, G., & Smyth, P. (1996); Laudon & Laudon, Ch.6 (Gartner-adat, AI a data managementben); Press, G. (2016). Cleaning Big Data: Most Time-Consuming, Least Enjoyable Data Science Task, Survey Says. Forbes.

## 5. Adatbányászat I.

(forrás: 7.5.html)

### 5. Adatbányászat I.

## Adatbányászat I.: társításelemzés és osztályozás — konkrét számítással

### Mi vásárlódik együtt, és ki fog lemorzsolódni?

#### Társításelemzés (Association Rule Mining)

A társításelemzés arra a kérdésre válaszol: "mi vásárlódik/fordul elő együtt?" Nézzünk egy teljes, kiszámított példát banki ügyféladatokon:

Adatok: 10 000 ügyfélből 6000-nek van folyószámlája (C), 5000-nek megtakarítási számlája (S), ebből 5000 ügyfélnek mindkettő megvan.

- Support(S és C) = 5000/10 000 = 50%

- Confidence(C → S) = 5000/6000 = 83% — ha valakinek van folyószámlája, 83% eséllyel van megtakarítási számlája is

- Elvárt konfidencia (ha a két termék független lenne) = 85%

- Lift = Confidence / Elvárt konfidencia = 0,83/0,85 = 0,98

Az értelmezés a lényeg: mivel a Lift kisebb, mint 1, ez azt jelenti, hogy a két termék együttes birtoklása valójában nem erősebb kapcsolat, mint amit a véletlen egybeesés önmagában indokolna — annak ellenére, hogy a 83%-os konfidencia önmagában lenyűgözőnek tűnik. Egy magas konfidencia-érték félrevezető lehet, ha nem vetjük össze az elvárt (véletlenszerű) aránnyal.

#### Osztályozás (Classification) — ügyfél-lemorzsolódás (churn) előrejelzése

Az osztályozás célja, hogy egy már ismert kimenetelű adathalmazból megtanuljon egy modell, amely új, még ismeretlen ügyfeleknél előre jelzi ugyanezt a kimenetelt.

🌍 Konkrét eset

Egy maláj telekomcégen végzett kutatás (Mustafa et al., 2021) valós ügyfél-elégedettségi (NPS) adatokon egy döntési fa alapú algoritmust (CART) tanított be, amely 98%-os pontossággal jelezte előre, mely ügyfelek fognak lemorzsolódni. A modell olyan tényezőket azonosított kulcsfontosságúként, mint a panaszkezelési idő és az NPS-pontszám trendje.

Miért fontos a gyártó cégek számára is? A churn-modellezés logikája közvetlenül átültethető gépmeghibásodás-előrejelzésre: ahelyett, hogy "melyik ügyfél mondja le az előfizetést", a kérdés "melyik gép fog meghibásodni" — ugyanaz az osztályozási logika, más címke.
[kép]

Ábra: Döntési fa vázlat, amely bemutatja, hogyan vezet 2-3 kérdés egy churn/nem churn besoroláshoz]

🤔 Menedzseri kérdés

Ha a saját területeden egy magas "konfidenciájú" összefüggést találnál két esemény között, hogyan ellenőriznéd, hogy ez valódi kapcsolat, vagy csak véletlen egybeesés (azaz kiszámítanád-e a Liftet)?

Forrás: saját anyag (MIS_BIG_DATA.pdf) — bank-példa; Mustafa, N., et al. (2021), F1000Research — churn-előrejelzés.

## 6. Adatbányászat II.

(forrás: 7.6.html)

### 6. Adatbányászat II.

## Adatbányászat II.: csalásdetektálás, keresletelőrejelzés, ajánlórendszer, hitelbírálat

### Négy további üzleti alkalmazás

#### Csalásdetektálás (Fraud Detection)

A csalásdetektáló algoritmusok azon az elven működnek, hogy egy adott ügyfél/tranzakció szokásos mintázatától való eltérést keresik — nem azt tanulják meg, "milyen egy csalás", hanem azt, "milyen a normális", és onnan jelzik az anomáliát. Ez technikailag rokon a Power BI Anomaly Detection funkciójával, amit a 6. előadásban már érintettünk.

#### Keresletelőrejelzés — gyártási kontextusban

🌍 Konkrét eset

Egy kőbányavállalat esettanulmányában a szerzők CRISP-DM módszertannal — a KDD ipari szabvány-változatával — hasonlítottak össze öt különböző előrejelző algoritmust (döntési fa, neurális háló, random forest, naiv Bayes, logisztikus regresszió) a gyártási késések előrejelzésére. Nincs egyetlen "legjobb" algoritmus — a modellválasztás mindig az adott adatstruktúrától és üzleti kérdéstől függ.

Ez a keresletelőrejelzés lényege: nem egyetlen jövőbeli számot "jósolunk meg", hanem történeti mintázatok alapján valószínűségi becslést adunk — ami sosem tökéletes, de jobb, mint a puszta megérzés.

#### Ajánlórendszer (Recommendation System)

Az Amazon tételalapú kollaboratív szűrése (item-based collaborative filtering) klasszikus példa: a rendszer nem azt nézi, "kihez hasonlítasz te mint vásárló", hanem azt, "mely termékeket vásárolják gyakran együtt mások" — ez lényegében az előző oldalon tárgyalt társításelemzés kereskedelmi alkalmazása.

#### Hitelbírálat / Scoring (Credit Scoring)

A hitelbírálati modellek az ügyfél korábbi hiteltörténetét, jövedelmi és egyéb adatait dolgozzák fel, hogy megbecsüljék a jövőbeli fizetési hajlandóságot. A ZEAL Network (korábban Tipp24 AG) online lottószolgáltató esete jól mutatja, hogyan terjed ki ez a logika a hitelbírálaton túlra is: a cég prediktív modelleket épített ügyfélszegmensek viselkedésének előrejelzésére, beleértve azt is, mely inaktív ügyfelek térnek majd vissza.
[kép]

Ábra: Csalásdetektálás, keresletelőrejelzés, ajánlórendszer, hitelbírálat

🤔 Reflektív kérdés

A négy alkalmazás közül (csalásdetektálás, keresletelőrejelzés, ajánlórendszer, hitelbírálat) melyik állna a legközelebb a saját szakterületedhez — és milyen adatokra lenne szükséged hozzá?

Forrás: Laudon & Laudon, Ch.12 — ZEAL Network-eset, prediktív analitika; saját anyag (MIS_BIG_DATA.pdf) — Amazon-ajánlórendszer; friss kőbánya-esettanulmány (CRISP-DM, gyártási késés-előrejelzés).

## 7. A Target-eset

(forrás: 7.7.html)

### 7. A Target-eset

## A Target-eset: amikor az algoritmus többet tud, mint kellene

### Hamis pozitívok és a prediktív etika határai

🏭 Az eset

2012-ben egy amerikai férfi berontott egy Target áruházba, mert a lánya — még középiskolás — terhesség-témájú kuponokat kapott postán. Dühösen reklamált, majd néhány nap múlva bocsánatot kért: kiderült, lánya valóban terhes volt, csak még nem mondta el a családjának. A Target adatbányászati algoritmusa a vásárlási mintázatokból (illatmentes testápoló, bizonyos vitaminkészítmények, nagyméretű táskák) korábban jött rá erre, mint az apa.

Ez az eset túlmutat a technikai sikeren, és két kritikus kérdést vet fel:

1. Hamis pozitív/negatív arányok: egy ilyen predikciós modell sosem 100%-ban pontos. Ha a modell 100 nőt jelöl meg "valószínűleg terhesként", és ebből csak 60 valóban az, a maradék 40 esetben a cég téves, kínos, akár károkozó feltételezés alapján küld célzott reklámot valakinek, aki nem is terhes. A hamis pozitív itt nem statisztikai absztrakció — valódi emberi kellemetlenség vagy kár.

2. Az etikai határ — mit szabad megjósolni, még ha lehet is? A Target technikailag semmilyen jogszabályt nem sértett: nyilvánosan hozzáférhető vásárlási adatokból dolgozott. A kérdés mégis az, hogy egy vállalatnak van-e legitim üzleti érdeke ahhoz, hogy egy ilyen mélyen személyes információt kikövetkeztessen — és hogy ezt a tudást hogyan használja fel (a Target végül úgy változtatott a stratégiáján, hogy a terhességi kuponokat más, semleges termékek közé "keverte").
[kép]

Ábra: Confusion mátrix

Ez az eset közvetlen előremutatás a 11. fejezet (Etika, algoritmusok és felelős AI) felé — ugyanez a hamis pozitív/negatív és "mit szabad megjósolni" dilemma tér majd vissza AI-alapú felvételi vagy hitelbírálati algoritmusok kapcsán, csak nagyobb téttel.

🤔 Menedzseri kérdés

Ha a saját cégednél egy algoritmus képes lenne kikövetkeztetni egy alkalmazott vagy ügyfél olyan magánéleti körülményét, amit az nem osztott meg — hol húznád meg a határt, hogy ezt a tudást szabad-e egyáltalán felhasználni?

Forrás: nyilvánosan dokumentált, széles körben tárgyalt üzleti etikai esettanulmány (Target Corporation, 2012).

## 8. Műszaki menedzseri szintézis

(forrás: 7.8.html)

### 8. Műszaki menedzseri szintézis

## Műszaki menedzseri szintézis: hol a határ a jó KPI-rendszer és a mikromenedzsment között?

### A 6–7. előadás közös íve

Ez a két előadás (6. és 7.) egy közös ívet járt végig: a KPI-tervezéstől (Goodhart, OEE, BSC) a dashboard-etikán át az adatbányászatig és a prediktív etikáig (Target-eset). A közös szál mindvégig ugyanaz volt: minél kifinomultabb egy mérési vagy előrejelző eszköz, annál nagyobb a felelősség azt illetően, hogyan használjuk.

Gondoljunk vissza a korábbi fejezetekben tárgyalt gyártási esetekre — akár a Bosch Hatvan-i, akár a Siemens Amberg-i digitalizációs tapasztalatokra: mindkét esetben a technológia (szenzorok, valós idejű dashboardok, prediktív karbantartás) önmagában nem hozott automatikusan jobb döntéseket. A technológia sikere mindig azon múlt, hogy a szervezet emberi döntéshozói hogyan illesztették be a saját ítélőképességükbe — nem helyettesítették azzal.

🏭 Záró kritikai kérdés

Egy műszaki menedzser számára a legnagyobb kockázat ma már nem az, hogy nincs elég adata — hanem hogy túl sok, túl kifinomult, túl "objektívnek tűnő" adata van, és emiatt hajlamos lemondani a saját szakmai ítélőképességéről. A Goodhart-törvénytől a Target-esetig minden példa ugyanazt mutatta: az algoritmus vagy mutató eszköz, nem döntéshozó.

🤔 Záró reflektív kérdés

Az elmúlt két előadás alapján — mi az az egy konkrét gyakorlat, amit bevezetnél a saját munkahelyeden, hogy a KPI-k és algoritmusok eszközök maradjanak, ne váljanak döntéshozóvá?

Kitekintés: a következő fejezetekben ugyanez a kritikai szemlélet folytatódik — hogyan terjed ki mindez felhő alapú BI-rendszerekre, majd végül a mesterséges intelligencia és az etikus algoritmustervezés kérdéskörére.

## 9. Elmélyítő Kiegészítő

(forrás: 7.9.html)

### 9. Elmélyítő Kiegészítő

- Fayyad, U., Piatetsky-Shapiro, G., & Smyth, P. (1996). From data mining to knowledge discovery in databases. AI Magazine, 17(3), 37–54. DOI: https://doi.org/10.1609/aimag.v17i3.1230

- Tokola, H., Gröger, C., Järvenpää, E., & Niemi, E. (2016). Designing manufacturing dashboards on the basis of a key performance indicator survey. Procedia CIRP, 57, 619–624. DOI: https://doi.org/10.1016/j.procir.2016.11.107

- Mustafa, N., Ling, L. S., & Abdul Razak, S. F. (2021). Customer churn prediction for telecommunication industry: A Malaysian case study. F1000Research, 10, 1274. DOI: https://doi.org/10.12688/f1000research.73597.1

- Chapman, P., et al. (2000). CRISP-DM 1.0: Step-by-step data mining guide. SPSS Inc. Elérhető: http://www.crisp-dm.org/CRISPWP-0800.pdf

## 1. 7. előadás: Alapfogalmak — Opcionális Könyv

(forrás: 7.10.html)

### 1. 7. előadás: Alapfogalmak — Opcionális Könyv

## 2. BI-képességek egyszerű listája

(forrás: 7.11.html)

### 2. BI-képességek egyszerű listája

## BI-képességek egyszerű listája

### Alapfogalmak — mielőtt belevágnánk a kritikába és a technikai mélységbe

A BI-rendszerek négy alapvető képességet biztosítanak a felhasználóknak, amelyekkel a 6–7. előadásban is találkozunk:

- Dashboard — vizuális felület, amely egy pillantásra megmutatja a legfontosabb mutatókat (lásd a 6. előadás nyitó dilemmáját: mi történik, ha túl sok kerül rá egyszerre)

- Drill-down — lehetőség arra, hogy egy összesített számból lemenjünk a részletekbe (pl. éves összesítésből havi, majd napi bontásba)

- Ad hoc lekérdezés — a felhasználó saját maga állít össze egy kérdést az adatnak, nem egy előre elkészített riportot néz

- Előrejelzés/forgatókönyv-elemzés — "mi történne, ha" típusú kérdések megválaszolása, statisztikai eszközökkel

Ez a négy képesség adja a keretet ahhoz, amit a 7. előadás Kötelező Könyvének 2. oldalán (OLAP mint gondolkodásmód) részletesebben, egy konkrét forgatókönyvön keresztül bemutatunk.

Forrás: Laudon & Laudon, Ch.12

## 3. OLAP alapfogalmak egyszerűen

(forrás: 7.12.html)

### 3. OLAP alapfogalmak egyszerűen

## OLAP alapfogalmak egyszerűen

### Alapfogalmak — mielőtt belevágnánk a kritikába és a technikai mélységbe

Az OLAP (Online Analytical Processing) négy alapművelete egy többdimenziós "adatkockán" végezhető el:

Művelet | 
Mit jelent | 

Slice | Egyetlen szelet kimetszése az adatkockából (pl. csak egy adott hónap adatai) | 

Dice | Több dimenzió egyidejű szűkítése (pl. adott hónap + adott gyártósor + adott termék) | 

Drill-down | Lemenetel egy magasabb szintű összesítésről egy részletesebb szintre (pl. évesből havi bontásba) | 

Roll-up | Felmenetel egy részletes szintről egy magasabb összesítésre (pl. napi adatokból heti összesítésbe) | 

Ez a négy definíció az alapja annak, amit a Kötelező Könyv 2. oldala egy teljes, lépésről lépésre végigvitt üzleti forgatókönyvön (miért nőtt a selejtarány?) mutat be — ott már nem a definíció a lényeg, hanem az, hogyan épül egymásra a négy lépés egy valódi nyomozásban.

Forrás: Laudon & Laudon, Ch.6

## 4. A CRISP-DM módszertan

(forrás: 7.13.html)

### 4. A CRISP-DM módszertan

## A CRISP-DM módszertan

### Alapfogalmak — mielőtt belevágnánk a kritikába és a technikai mélységbe

A Kötelező Könyv 5. oldalán (keresletelőrejelzés a kőbánya-esettel) egy CRISP-DM módszertannal végzett kutatásra hivatkozunk — ez az oldal azt tisztázza, mit is jelent ez a betűszó, mielőtt a kritikai esettel találkozol.

CRISP-DM = CRoss-Industry Standard Process for Data Mining, azaz "iparágak közötti szabványos adatbányászati folyamat". Ez lényegében a KDD-folyamat (lásd Kötelező Könyv, 3. oldal) ipari, gyakorlatorientált változata — ma is ez a legelterjedtebb módszertan, amikor egy vállalat adatbányászati projektbe kezd.

A CRISP-DM hat, egymásra épülő fázisból áll:

- Üzleti megértés — mi a valódi üzleti kérdés, amit meg akarunk válaszolni?

- Adatmegértés — milyen adat áll rendelkezésre, milyen minőségben?

- Adat-előkészítés — tisztítás, transzformáció (ez jellemzően a legtöbb időt igénylő fázis)

- Modellezés — a tényleges algoritmus(ok) alkalmazása

- Kiértékelés — a modell eredménye valóban választ ad-e az 1. lépésben megfogalmazott üzleti kérdésre?

- Bevezetés (Deployment) — a modell beépítése a napi működésbe

A lényeg, amit érdemes megjegyezni: a CRISP-DM — a KDD-hez hasonlóan — nem lineáris, egyszeri folyamat, hanem ciklikus: a 6. fázis (bevezetés) tapasztalatai gyakran visszavezetnek az 1. fázishoz (üzleti megértés újragondolása).
[kép]

Ábra: CRISP-DM

🤔 Reflektív kérdés

A kőbánya-esetben (Kötelező Könyv, 5. oldal) melyik CRISP-DM fázisba sorolnád azt, hogy a kutatók öt különböző algoritmust hasonlítottak össze?

Forrás: Chapman, P., et al. (2000). CRISP-DM 1.0 — Step-by-step data mining guide.

## 5. Mi az a feltételes valószínűség?

(forrás: 7.14.html)

### 5. Mi az a feltételes valószínűség?

## Mi az a feltételes valószínűség? — hétköznapi bevezető

### Alapfogalmak — mielőtt belevágnánk a kritikába és a technikai mélységbe

A Kötelező Könyv 4. oldalán kiszámoltunk egy Lift-értéket, és megállapítottuk, hogy 0,98 — vagyis kicsit kevesebb, mint 1. De miért pont az 1 a határ, ami fölött/alatt mást jelent egy összefüggés? A válasz a feltételes valószínűség fogalmában rejlik, amit itt egy hétköznapi példán vezetünk be, számítás nélkül.

Példa: ha azt kérdezed, "mennyi az esélye, hogy ma esik az eső", az egy dolog. Ha viszont azt kérdezed, "mennyi az esélye, hogy ma esik az eső, ha már tudom, hogy mindenki esernyővel megy dolgozni", az egy feltételes valószínűség — a válasz változik attól, hogy egy plusz információt (esernyő) már ismersz.

A kulcsgondolat: ha egy plusz információ (pl. "van esernyője") semmit nem változtat az eredeti kérdés valószínűségén, akkor a két esemény független egymástól. Ha viszont az információ megváltoztatja a valószínűséget, akkor összefüggnek.

Ez pontosan az, amit a Lift mér az üzleti adatokban: ha tudjuk, hogy valakinek van folyószámlája, ez megváltoztatja-e annak esélyét, hogy megtakarítási számlája is van? Ha a Lift = 1, a válasz: nem, semennyire — a két termék pontosan úgy fordul elő együtt, mint amennyire a véletlen alapján várnánk, tehát függetlenek. Ha a Lift > 1, a folyószámla megléte növeli a megtakarítási számla esélyét — pozitív összefüggés. Ha a Lift < 1 (mint a mi 0,98-as példánkban), az összefüggés enyhén negatív.

A Haladó Könyvben ezt a gondolatot visszük tovább pontos képlettel (Bayes-tétel), és mutatjuk meg, honnan ered matematikailag a Lift = 1 mint függetlenségi határ.
[kép]

Ábra helye: Venn-diagram és elágazó fa

🤔 Reflektív kérdés

Gondolj egy saját példára a munkahelyedről, ahol két esemény függetlennek tűnik, de valójában lehet, hogy összefügg — honnan tudnád eldönteni, melyik igaz?

## 6. Miért nem elég a pontosság?

(forrás: 7.15.html)

### 6. Miért nem elég a pontosság?

## Miért nem elég az "pontosság"? — fogalmi bevezető

### Alapfogalmak — mielőtt belevágnánk a kritikába és a technikai mélységbe

A Kötelező Könyv 4. oldalán egy churn-előrejelző modellről olvastunk, amely "98%-os pontossággal" dolgozott. Ez lenyűgözően hangzik — de van egy csapda benne, amit érdemes már itt, fogalmi szinten megérteni, mielőtt a Haladó Könyv a pontos méréseket (ACC, Precision, Recall, F1) bevezeti.

Gondolatkísérlet: képzelj el egy gyártósort, ahol 1000 termékből átlagosan csak 10 hibás (1%). Ha építesz egy "modellt", amely minden egyes terméket automatikusan "jónak" minősít, anélkül hogy bármit is vizsgálna — ez a modell 99%-ban pontos lesz! Hiszen 990 terméket helyesen minősített jónak. Csakhogy ez a modell semmit nem ér, mert pontosan azt a 10 hibás terméket nem vette észre, amiért egyáltalán megépítették.

A tanulság: amikor egy esemény (churn, hibás termék, csalás) ritka a teljes adathalmazhoz képest, a puszta "pontosság" (accuracy) félrevezető lehet — egy modell úgy is "jó pontosságú" lehet, hogy közben pont a lényeges eseteket nem veszi észre. Ezért van szükség olyan finomabb mérőszámokra, amelyek külön vizsgálják: hányat talált meg a modell a valóban hibás/csaló/lemorzsolódó esetekből, és hány "hamis riasztást" adott a jó esetekre.

Ez a felismerés adja a keretet ahhoz, amit a Haladó Könyv pontos képletekkel (TP, FP, TN, FN, majd ezekből ACC, Precision, Sensitivity/Recall, F1, AUC) tárgyal.
[kép]

Ábra: A "mindenki jó" naiv modell nyilvánvaló hibája

🤔 Menedzseri kérdés

Van-e a saját területeden olyan ritka, de fontos esemény (pl. súlyos meghibásodás, csalás, lemorzsolódás), ahol a puszta "pontosság" megtévesztő lenne, ha valaki csak ezt az egy számot nézné?

Forrás: fogalmi bevezető, klasszifikációs metrikák pedagógiai előkészítése.

## 1. 6-7. előadás: Haladó Könyv — feltételes valószínűség és klasszifikáció

(forrás: 7.16.html)

### 1. 6-7. előadás: Haladó Könyv — feltételes valószínűség és klasszifikáció

## 2. Bayes-tétel és a feltételes valószínűség

(forrás: 7.17.html)

### 2. Bayes-tétel és a feltételes valószínűség

## Bayes-tétel és a feltételes valószínűség

### Haladó Könyv — amikor a KPI mögé nézünk

Az Opcionális Könyv (4. oldal) bevezette a feltételes valószínűség gondolatát az esernyő-példával: "mennyi az esélye X-nek, ha már tudjuk Y-t." Itt ezt pontos matematikai formába öntjük.

📖 Fogalmi alap — Bayes-tétel

A feltételes valószínűség definíciója: P(B|A) = P(A∩B)/P(A) — vagyis annak a valószínűsége, hogy B bekövetkezik, feltéve, hogy A már bekövetkezett, az A és B együttes valószínűségének és A valószínűségének hányadosa.

Ebből következik Bayes tétele: P(A|B) = [P(B|A) · P(A)] / P(B)

A függetlenség matematikai definíciója: A és B pontosan akkor független, ha P(B|A) = P(B) — vagyis A bekövetkezése semennyire nem változtatja meg B valószínűségét. Ez az a pont, ahol a következő oldalon tárgyalt Lift-mutató gyökerezik.

💡 Műszaki analógia

Gondolj egy érzékelőre, amely két, egymástól független paramétert mér (pl. hőmérséklet és egy másik gyártósoron mért nyomás). Ha a hőmérséklet ismerete semmit nem segít a nyomás előrejelzésében, a két mérés független — pontosan úgy, ahogy P(nyomás|hőmérséklet) = P(nyomás).

🤔 Reflektív kérdés

Ha tudod, hogy egy gépen most magas a rezgésszint, ez megváltoztatja-e annak esélyét, hogy hamarosan meghibásodik? Ha igen, a két esemény nem független — hogyan használnád ki ezt egy karbantartási stratégiában?

## 3. Asszociációs mutatók pontosan

(forrás: 7.18.html)

### 3. Asszociációs mutatók pontosan

## Asszociációs mutatók pontosan: Support, Confidence, Elvárt konfidencia, Lift

### Haladó Könyv — amikor a KPI mögé nézünk

A Kötelező Könyv 4. oldalán (7. előadás) a bank-példát számoltuk ki — itt egy másik, klasszikus kiskereskedelmi forgatókönyvön nézzük meg ugyanezt az öt mutatót, hogy lásd: az összefüggés iránya (pozitív vagy negatív) is kiolvasható belőlük.

📖 Fogalmi alap — öt mutató, egymásra épülve

Adatok: egy szupermarket 10 000 bevásárlókosarat elemez. Kávé (A) 3000 kosárban szerepel, cukor (B) 2500 kosárban, és a kettő együtt 1500 kosárban fordul elő.

Mutató | 
Képlet | 
Számpélda (Kávé→Cukor) | 

Support(A) | count(A)/N | Support(Kávé) = 3000/10 000 = 30% | 

Support(A∪B) | count(A∩B)/N | Support(Kávé∪Cukor) = 1500/10 000 = 15% | 

Confidence(A→B) | Support(A∪B)/Support(A) = P(B|A) | Confidence(Kávé→Cukor) = 1500/3000 = 50% | 

Elvárt konfidencia | Support(B) = P(B) | Support(Cukor) = 2500/10 000 = 25% | 

Lift(A→B) | Confidence/Elvárt konfidencia = P(B|A)/P(B) | 0,50/0,25 = 2,0 | 

Az értelmezés — most fordítva, mint a bank-példánál: a Lift = 2,0 azt jelenti, hogy aki kávét vesz, kétszer akkora eséllyel vesz cukrot is, mint amit a véletlen egybeesés önmagában indokolna. Ez egy erős, pozitív összefüggés — pontosan az a fajta mintázat, amit egy áruházi keresztértékesítési stratégia (pl. a kávé mellé polcra tett cukor) ki tudna használni.

A Bayes-kapcsolat explicit módon: ha a kávé- és cukorvásárlás független lenne, P(Cukor|Kávé) = P(Cukor) teljesülne, azaz Confidence = Elvárt konfidencia, és Lift = 1 lenne. Itt a Confidence (50%) duplája az Elvárt konfidenciának (25%) — ez a Lift = 2 forrása.

Összevetve a bank-példával (Kötelező Könyv, 4. oldal, Lift = 0,98): ott a két termék enyhén ritkábban fordult elő együtt, mint véletlenül várnánk (gyenge negatív összefüggés) — itt a kávé és cukor jóval gyakrabban, mint véletlenül várnánk (erős pozitív összefüggés). A Lift mindkét irányban ugyanazt méri: mennyire tér el a megfigyelt együttjárás a függetlenségtől.

🤔 Menedzseri kérdés

Ha egy webshopban két termék Confidence-e 90%, de a Lift mindössze 1,01 — mennyire lenne indokolt egy drága keresztértékesítési kampányt indítani erre az összefüggésre, a kávé/cukor-példa (Lift=2) fényében?

Forrás: illusztratív kiskereskedelmi példa, klasszikus piackosár-elemzési forgatókönyv; Agrawal-féle asszociációs szabály definíciók.

## 5. A konfúziós mátrix és az alapmutatók

(forrás: 7.19.html)

### 5. A konfúziós mátrix és az alapmutatók

## A konfúziós mátrix és az alapmutatók

### Haladó Könyv — amikor a KPI mögé nézünk

A churn-modell "98%-os pontossága" (Kötelező Könyv, 4. oldal) mögött egy konfúziós mátrix áll — négy szám, amelyekből minden további mutató levezethető.

📖 Fogalmi alap

 | 
Valóban lemorzsolódik | 
Valóban nem morzsolódik le | 

Modell: lemorzsolódik | TP (Igaz pozitív) | FP (Hamis pozitív) | 

Modell: nem morzsolódik le | FN (Hamis negatív) | TN (Igaz negatív) | 

Mutató | 
Képlet | 

Accuracy | (TP+TN)/(TP+TN+FP+FN) | 

Precision | TP/(TP+FP) | 

Recall (Sensitivity) | TP/(TP+FN) | 

Specificity | TN/(TN+FP) | 

Konkrét számpélda (visszavezetve az Opcionális Könyv 5. oldalán látott gyártósoros gondolatkísérletre, 1000 termék, 10 valóban hibás): ha egy modell mind az 1000 terméket "jónak" minősíti, akkor TP=0, FN=10, TN=990, FP=0 → Accuracy = 990/1000 = 99%, de Recall = 0/10 = 0% — a modell egyetlen hibás terméket sem talált meg, miközben "99%-ban pontos."

🤔 Menedzseri kérdés

Egy csalásdetektáló rendszernél melyik hiba drágább — a hamis pozitív (jogos tranzakciót gyanúsnak jelöl) vagy a hamis negatív (valódi csalást enged át)? Melyik mutatót (Precision vagy Recall) növelnéd ennek megfelelően?

## 6. Az F1-score

(forrás: 7.20.html)

### 6. Az F1-score

## Az F1-score: miért kell egyetlen mutató, ha van kettő?

### Haladó Könyv — amikor a KPI mögé nézünk

A Precision és a Recall gyakran ellentétes irányba mozdulnak: ha egy modellt "óvatosabbá" teszünk (csak nagyon biztos esetekben jelez pozitívot), a Precision nő, de a Recall csökken — és fordítva.

📖 Fogalmi alap

F1-score = 2 · (Precision · Recall)/(Precision + Recall) = 2TP/(2TP + FP + FN)

Ez a Precision és Recall harmonikus közepe — nem egyszerű átlaga. A harmonikus közép azért fontos, mert büntetve alacsony marad, ha az egyik komponens nagyon alacsony, még ha a másik magas is.

Például Precision=100% és Recall=1% esetén a számtani átlag 50,5% lenne (megtévesztően jónak tűnne), de az F1-score mindössze ~2% — helyesen jelezve, hogy a modell gyakorlatilag használhatatlan.

💡 Műszaki analógia

Ez olyan, mint amikor egy gép két komponensből álló hatékonysági mutatóját (pl. sebesség és pontosság) nem egyszerű átlaggal, hanem úgy kombináljuk, hogy ha bármelyik komponens nagyon rossz, az összesített szám is drasztikusan romoljon — nem lehet az egyik gyengeségét "elrejteni" a másik erősségével.

🤔 Reflektív kérdés

Számold ki fejben: ha egy modell Precision = 80% és Recall = 60%, becslésed szerint 70% fölött vagy alatt lesz az F1-score? (Válasz: a harmonikus közép mindig közelebb van a kisebb értékhez, tehát 70% alatt.)

## 7. ROC-görbe és AUC

(forrás: 7.21.html)

### 7. ROC-görbe és AUC

## ROC-görbe és AUC

### Haladó Könyv — amikor a KPI mögé nézünk

Az eddigi mutatók (Precision, Recall, F1) mind egyetlen, rögzített küszöbértékhez (threshold) tartoznak — de mi történik, ha ezt a küszöböt változtatjuk?

📖 Fogalmi alap

A ROC-görbe (Receiver Operating Characteristic) az Igaz pozitív arányt (TPR = Recall) ábrázolja a Hamis pozitív arány (FPR = 1 − Specificity) függvényében, ahogy a döntési küszöböt végigcsúsztatjuk. Az AUC (Area Under the Curve) ennek a görbének a területe:

- AUC = 0,5 → a modell nem jobb, mint a véletlen érmefeldobás

- AUC = 1,0 → tökéletes modell

- AUC interpretálható úgy is, mint annak valószínűsége, hogy egy véletlenszerűen kiválasztott pozitív eset magasabb pontszámot kap a modelltől, mint egy véletlenszerűen kiválasztott negatív eset

Miért jobb ez, mint egyetlen Accuracy-szám? Mert nem egyetlen küszöbértékhez köti magát — megmutatja a modell teljes viselkedését minden lehetséges döntési ponton, függetlenül attól, hogy a végleges alkalmazásban milyen küszöböt választanak.
[kép]

Ábra: ROC görbe

💡 Műszaki analógia

Ez olyan, mint amikor egy riasztórendszer érzékenységét állítjuk: minél érzékenyebbre állítjuk (alacsonyabb küszöb), annál több valódi riasztást fogunk el, de annál több hamis riasztást is kapunk. A ROC-görbe ezt a teljes trade-off-ot mutatja meg egyetlen képen, az AUC pedig egyetlen számban foglalja össze.

🤔 Záró menedzseri kérdés

Ha két churn-előrejelző modell közül választhatsz — az egyiknek 95%-os Accuracy-ja, de 0,60 AUC-ja van, a másiknak 85%-os Accuracy-ja, de 0,90 AUC-ja — melyiket választanád, és miért?

Forrás: Fawcett, T. (2006). An introduction to ROC analysis. Pattern Recognition Letters, 27(8), 861–874.

## 8. Források

(forrás: 7.22.html)

### 8. Források

- Molnár Bálint. Adatbányászati megoldások fejlesztési iránya — OLAP technológiájú megoldások bevezethetőségének elemzése. Kutatási tanulmány. Elérhető: https://www.researchgate.net/publication/277775747

- Abonyi János (2006). Adatbányászat: a hatékonyság eszköze. Budapest: Computer Books. ISBN 963 618 342 2. Elérhető: https://www.researchgate.net/publication/264441999

- Bodon Ferenc (2005). Adatbányászati algoritmusok. GNU licenc, szabadon letölthető egyetemi jegyzet. Elérhető: http://www.cs.bme.hu/~bodon/magyar/adatbanyaszat/tanulmany/index.html
- Fawcett, T. (2006). An introduction to ROC analysis. Pattern Recognition Letters, 27(8), 861–874. DOI: https://doi.org/10.1016/j.patrec.2005.10.010
