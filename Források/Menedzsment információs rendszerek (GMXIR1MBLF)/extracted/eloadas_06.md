# 6. előadás: 6. előadás BI a gyakorlatban I. - Kötelező tananyag

## 1. 6. előadás: KPI-tervezés kritikusan — Kötelező Könyv

(forrás: 6.1.html)

### 1. 6. előadás: KPI-tervezés kritikusan — Kötelező Könyv

## 2. Amikor 22 KPI kevesebbet mond, mint 3

(forrás: 6.2.html)

### 2. Amikor 22 KPI kevesebbet mond, mint 3

## Amikor 22 KPI kevesebbet mond, mint 3

### KPI-tervezés kritikusan: a Goodhart-csapdától az OEE-gamingig

🏭 Nyitó dilemma

Egy közepes méretű gyártóüzem vezetése úgy dönt: mostantól minden fontos szempontot lát akar a napi dashboardon. A rendszer 22 KPI-t jelenít meg egyetlen felületen — selejtarány, OEE, energiafogyasztás, túlóra-arány, beszállítói pontosság, vevői reklamáció, karbantartási költség és így tovább, mind egy képernyőn, mind zölden vagy pirosan villogva.

Három hónap múlva a műszakvezetők egyre kevesebbet néznek rá a dashboardra. Nem azért, mert nem érdekli őket az adat, hanem mert nem tudják eldönteni, melyik szám számít most igazán. Amikor minden piros, semmi sem sürgős; amikor minden zöld, semmi sem árulkodik a valódi kockázatról.

A jelenséget a szakirodalom "elemzési bénultságnak" (analysis paralysis) nevezi. Ez a fejezet erről szól: nem arról, hogyan mérjünk többet, hanem arról, hogyan mérjünk jól — és mi történik, ha egy mérőszám átveszi a döntéshozó helyét.

[kép]

Ábra: dashboard-képernyő illusztráció 

🤔 Reflektív kérdés

Gondolj egy olyan rendszerre a saját munkahelyeden, ahol túl sok mutatót követnek egyszerre. Emlékszel-e olyan helyzetre, amikor pont a legfontosabb probléma veszett el a sok szám között?

💡 Tanulási eredmények

A fejezet elvégzése után Ön képes:

- felismerni a Goodhart-törvény csapdáját, és megtervezni egy KPI-rendszert úgy, hogy az ne torzítsa el a mögötte lévő valós teljesítményt

- kiszámítani az OEE (rendelkezésre állás × teljesítmény × minőség) mutatót, és kritikusan értékelni annak korlátait ("OEE gaming", helyi vs. rendszerszintű optimalizálás)

- értékelni a Balanced Scorecard erősségeit és korlátait egy adott vállalati helyzetben, kritikai szemszögből

- alkalmazni a dashboard-tervezés tudományos alapelveit (data-ink ratio, Lie Factor), és megítélni, hol húzódik a határ a hangsúlyozás és a manipuláció között

- összekapcsolni a KPI-tervezési elveket egy konkrét Power BI-alapú gyakorlati alkalmazással

- reflektálni arra, hol húzódik a határ egy jó KPI-alapú vezetői gyakorlat és a mikromenedzsment között

Forrás: vezetői döntéshozatali szakirodalom (elemzési bénultság jelensége).

## 3. A Goodhart-csapda

(forrás: 6.3.html)

### 3. A Goodhart-csapda

## A Goodhart-csapda: amikor a mutató lesz a cél

### Mi történik, ha egy jó KPI-t célként kezdenek kezelni?

A KPI-tervezés alapszabályai (SMART-kritériumok, lag- és lead-mutatók megkülönböztetése) már ismertek — ezekre most nem térünk vissza részletesen, hanem egy sokkal kényesebb kérdést teszünk fel: mi történik, amikor egy jól megtervezett KPI-t elkezdenek célként kezelni, nem mérőeszközként?

📖 Fogalmi alap

Goodhart törvénye (Charles Goodhart, 1975, eredetileg monetáris politikai kontextusban): "amikor egy mutató célponttá válik, megszűnik jó mutatónak lenni."

Konkrét példa: egy ügyfélszolgálati call centerben az átlagos hívásidőt (Average Handling Time, AHT) vezetik be egyetlen teljesítménymutatóként. Rövid távon az AHT javul — az ügyintézők gyorsabban zárják le a hívásokat. De ha megnézzük az ismételt hívások arányát, az drasztikusan nő: az ügyfelek problémája valójában nincs megoldva, csak a hívás rövidebb lett. A mutató javult, a valódi cél romlott.

Ugyanez történik gyakran gyártási környezetben: ha az egyetlen KPI a "gyártott darabszám/műszak", a dolgozók megtalálják a módját, hogyan lehet ezt a számot úgy növelni, hogy közben a minőség vagy a gépkarbantartás rovására megy.

💡 Műszaki analógia

Ez ugyanaz a logika, mint amikor egy szenzort kalibrálnak úgy, hogy mindig a kívánt tartományban mérjen — a szenzor "jó" adatot ad, de a mért folyamat valósága nem változott. A mutató és a valóság elszakad egymástól.

A Goodhart-csapda az AI korában sem tűnt el — sőt. Thomas és Uminsky (2022) Patterns (Cell Press) folyóiratban megjelent tanulmánya szerint a mai mesterséges intelligencia rendszerek — különösen a mélytanulási modellek — lényegében "fegyverként használják" a Goodhart-törvényt: sikerük abból fakad, hogy könyörtelenül optimalizálnak egyetlen metrikára. Ez pontosan ugyanahhoz a torzuláshoz vezet, mint a call center-példa: a gép "megjátssza" a mérőszámot, miközben az eredeti cél sérül.

🤔 Menedzseri kérdés

Ha egyetlen KPI-t kellene kiválasztanod a saját területeden, amelyet mindenki hajszolna — milyen "kiskaput" találnának meg rá a beosztottjaid három hónapon belül?

Forrás: Goodhart, C. (1975); Thomas, R. L., & Uminsky, D. (2022). Reliance on metrics is a fundamental challenge for AI. Patterns, 3(5).

## 4. Az OEE technikai mélységben

(forrás: 6.4.html)

### 4. Az OEE technikai mélységben

## Az OEE technikai mélységben: pontos képlet és a "gaming"-kritika

### Amikor egy technikailag pontos mutató mégis megjátszható

Az OEE (Overall Equipment Effectiveness / Teljes Eszközhatékonyság) a gyáripar egyik legelterjedtebb összetett mutatója.

📖 Fogalmi alap — pontos képlet

OEE = Rendelkezésre állás × Teljesítmény × Minőség

- Rendelkezésre állás = tényleges üzemidő ÷ tervezett üzemidő

- Teljesítmény = (ciklusidő × legyártott darabszám) ÷ tényleges üzemidő

- Minőség = jó darabszám ÷ összes legyártott darabszám

Számpélda: ha egy gép a tervezett 480 perces műszakból 432 percet üzemel (Rendelkezésre állás = 90%), a tényleges üzemidő alatt a névleges kapacitás 85%-át hozza (Teljesítmény = 85%), és a legyártott darabok 98%-a megfelelő minőségű (Minőség = 98%):

OEE = 0,90 × 0,85 × 0,98 = 0,75, azaz 75%

Ez világszínvonalúnak számít a gyáriparban (a "world class" OEE ~85% körül van, a legtöbb üzem valós OEE-je 40–60% között mozog).
[kép]

Ábra: OEE-vízesés-diagram

A kritikai réteg — "OEE gaming": mivel az OEE három komponens szorzata, egy műszakvezető megtalálhatja a módját, hogy az egyik komponenst a másik rovására javítsa:

- A Teljesítmény-komponens javítható úgy, hogy a gépet a hivatalos névleges sebességnél alacsonyabb "ideális ciklusidővel" veszik nyilvántartásba.

- A minőségi hibákat a műszak végén rögzítik, nem valós időben.

- A helyi optimalizálás rendszerszintű kárt okozhat: ha egy gépcsoport OEE-jét egyedileg hajtják fel, miközben a sor egésze (bottleneck-gép) nem gyorsul, a rendszer átfutási ideje nem javul.

💡 Műszaki analógia

Ez olyan, mintha egy autó fogyasztását úgy "javítanád", hogy csak lejtőn méred — a szám jobb lesz, az autó valós teljesítménye nem változott.

🤔 Reflektív kérdés

Ha a saját üzemedben/csapatodban egy komponens mesterségesen javítható lenne a másik kettő rovására, felismernéd-e időben — és milyen ellenőrzés szűrné ki?

Forrás: OEE gyáripari szakirodalom, "gaming"-kritika.

## 5. A Balanced Scorecard kritikai nézőpontból

(forrás: 6.5.html)

### 5. A Balanced Scorecard kritikai nézőpontból

## A Balanced Scorecard kritikai nézőpontból

### Stratégiai eszköz vagy bürokratikus rituálé?

A Balanced Scorecard (BSC) négy perspektívája — pénzügyi, vevői, belső folyamat, tanulás-fejlődés — jól ismert alapfogalom. Kaplan és Norton eredeti szándéka szerint a BSC nem egyszerű mutatólista volt, hanem egy oksági lánc: a tanulás-fejlődési beruházások javítják a belső folyamatokat, azok javítják a vevői elégedettséget, ami végül pénzügyi eredményben csapódik le.

A gyakorlatban azonban a legtöbb BSC-bevezetés nem így működik. A kritikai szakirodalom rendszeresen rámutat, hogy a szervezetek gyakran:

- utólag illesztik a mutatókat a már meglévő jelentési struktúrához, ahelyett hogy valódi oksági stratégiai térképet (strategy map) építenének,

- a négy perspektívát négy külön silóként kezelik, nem egymásra épülő láncként,

- a rendszer idővel bürokratikus rituálévá válik: negyedévente kitöltött táblázat, amit senki nem használ tényleges döntéshozatalra.

Ez a jelenség rokon a Goodhart-csapdával: a BSC eredetileg stratégiai gondolkodási eszköznek készült, de ha a mutatók kitöltése önmagáért való céllá válik, elveszti stratégiai funkcióját.

💡 Műszaki analógia

Ez olyan, mint amikor egy karbantartási checklistát rutinból pipálnak ki anélkül, hogy ténylegesen elvégeznék a mögötte lévő ellenőrzést — a dokumentum megvan, a valós biztonság nem feltétlenül.

🤔 Menedzseri kérdés

Van-e a saját szervezetedben olyan "stratégiai" jelentés, amit rendszeresen kitöltenek, de valójában senki nem használ döntéshozatalra? Mi jelezné, hogy ez történt?

[kép]

Forrás: Kaplan, R. S., & Norton, D. P. (1996) eredeti koncepciója, kritikai kontraszttal a gyakorlati implementációs szakirodalomból.

## 6. A dashboard-tervezés tudománya

(forrás: 6.6.html)

### 6. A dashboard-tervezés tudománya

## A dashboard-tervezés tudománya: kiemelés vagy manipuláció?

### Tufte, Few és a Lie Factor — most AI-kontextusban is

A dashboard-tervezés két klasszikus forrása: Edward Tufte data-ink ratio elve (minden vizuális elemnek információt kell hordoznia) és Stephen Few 13 gyakori dashboard-hibája (túlzsúfoltság, félrevezető skálázás, felesleges 3D-effektek stb.).

📖 Fogalmi alap — Lie Factor

A grafikonon látható vizuális változás mértékének aránya a mögötte lévő valós adatváltozáshoz képest. Ha egy oszlopdiagram y-tengelyét nem nulláról indítják, egy 2%-os valós növekedés vizuálisan akár 200%-osnak is tűnhet.

[kép]

Ábra: Lie Factor
Ez nem csak esztétikai, hanem etikai kérdés. Egy vezető, aki tudatosan csonkolt y-tengelyt használ egy negyedéves eredményjelentésben, nem hazudik technikai értelemben — de manipulál. A dashboard-tervező itt olyan hatalommal bír, mint egy szerkesztő: eldönti, mit látunk meg először.

Ez a kérdés az AI-korban élesebbé válik. Az AI-alapú döntéstámogatás kockázatait külön is ki kell emelni: beépült torzítás (bias), az átláthatóság hiánya, és etikai kérdések. Amíg egy emberi dashboard-tervező tudatosan dönt a csonkított tengelyről, egy AI-alapú "automatikus kiemelés" funkció (pl. Power BI Key Influencers) öntudatlanul is torzíthat — a torzítás forrása ilyenkor a tanítóadat vagy az algoritmus jellemzője, ami nehezebben azonosítható.

🤔 Reflektív kérdés

Láttál-e már olyan vállalati riportot, ahol a vizuális megjelenítés — talán szándék nélkül is — jobb színben tüntetett fel egy eredményt, mint amilyen a valóságban volt?

Forrás: Tufte, E. R.; Few, S.; Laudon & Laudon (18. kiad.), Ch.12 — "Risks Introduced by Using AI in Decision Making".

## 7. Power BI-specifikus gyakorlati kapocs

(forrás: 6.7.html)

### 7. Power BI-specifikus gyakorlati kapocs

## Power BI-specifikus gyakorlati kapocs: az OEE-től az AI-alapú anomáliadetektálásig

### A GE Predix-esettől a saját laboredig

Amit eddig elméletben tárgyaltunk, a gyakorlatban is megjelenik — mégpedig pontosan abban a szoftverben, amit a laborotokon használtok.

🌍 Nemzetközi eset — GE Predix

A General Electric Predix platformja jól illusztrálja, hogyan válik a hagyományos, emberi felügyeletű KPI-monitorozás AI-alapú anomáliadetektálássá: a GE repülőgép-hajtómű flottájának adatait elemezve a rendszer felismerte, hogy bizonyos üzemeltetési környezetek (pl. Közel-Kelet, Kína hőmérsékleti és porviszonyai) szisztematikusan gyorsabb kopáshoz vezettek — ez a felismerés nem egyetlen gép adatából, hanem a teljes flotta összevetéséből derült ki.

A Power BI-ban ehhez hasonló, kisebb léptékű funkciók már elérhetők: a Key Influencers vizuál automatikusan azonosítja, mely tényezők befolyásolják leginkább egy kiválasztott mutatót (pl. mi korrelál leginkább az OEE ingadozásával), az Anomaly Detection funkció pedig önműködően jelzi, ha egy idősor szokatlanul viselkedik.

💡 Műszaki analógia

A Power BI Key Influencers funkciója olyan, mint egy tapasztalt karbantartó, aki évek alatt "beleérzi" magát a gép hangjába — csak itt az algoritmus szerzi meg ezt a tapasztalatot adatokból, emberi intuíció helyett.

A kritikai kérdés, amit a labor-gyakorlat során is érdemes szem előtt tartani: ezek a funkciók megkönnyítik a mintázatfelismerést, de nem mentesítenek a Goodhart- és OEE-gaming kritikák alól — sőt, egy automatikusan generált "kiemelés" még nehezebben megkérdőjelezhető, mert "objektívnek" tűnik.

🤔 Menedzseri kérdés

Ha a Power BI automatikusan kiemel egy "kulcsbefolyásoló tényezőt" a te KPI-adataidban, mennyire bíznál meg benne kritika nélkül — és mi alapján ellenőriznéd?

Forrás: Laudon & Laudon (15. kiad.), Ch.12 — GE Predix-eset.

## 8. Szintézis — jó KPI-rendszer vagy mikromenedzsment?

(forrás: 6.8.html)

### 8. Szintézis — jó KPI-rendszer vagy mikromenedzsment?

## Szintézis: hol a határ a jó KPI-rendszer és a mikromenedzsment között?

### Eszköz marad-e a mutató, vagy döntéshozóvá válik?

Térjünk vissza a nyitó dilemmához: a 22 KPI-t egyszerre megjelenítő dashboard nem azért volt rossz megoldás, mert a mutatók hibásak lettek volna egyenként — hanem mert a rendszer egésze nem tett különbséget a fontos és a kevésbé fontos között.

Amit ez a lecke végigvitt:

- A Goodhart-törvény megmutatja, hogy bármelyik jól megtervezett KPI elromolhat, ha céllá válik — és ez a jelenség az AI-rendszerekben is megjelenik.

- Az OEE technikai pontossága nem garancia a manipuláció ellen — a "gaming" mindig a helyi optimalizálás és a rendszerszintű cél közötti feszültségből fakad.

- A Balanced Scorecard csak akkor marad stratégiai eszköz, ha nem engedik bürokratikus rituálévá silányulni.

- A dashboard-tervezés sosem "semleges" — akár ember, akár AI választja ki, mit emeljen ki, ez mindig tartalmaz értékítéletet.

🏭 Záró tanulság

Egy jó KPI-rendszer arra való, hogy támogassa a döntéshozó ítélőképességét — nem arra, hogy helyettesítse azt. Amikor egy vezető minden döntését kizárólag a dashboardra hivatkozva hozza meg, és nem meri megkérdőjelezni a mutatót, az már nem adatvezérelt vezetés, hanem mikromenedzsment automatizált álruhában.

🤔 Záró reflektív kérdés

Hol húznád meg a határt a saját munkahelyeden — mettől kezdve válik egy KPI-alapú vezetési stílus mikromenedzsmenté?

Kitekintés a következő előadásra: a 7. előadásban azt vizsgáljuk, mi történik, amikor a mutatók mögötti mintázatokat nem az ember, hanem a gép fedezi fel — az OLAP-tól a valódi adatbányászatig, egészen a Target-cég híres, etikailag is vitatott terhesség-előrejelző algoritmusáig.

## 8. Szintézis — jó KPI-rendszer vagy mikromenedzsment?

(forrás: 6.9.html)

### 8. Szintézis — jó KPI-rendszer vagy mikromenedzsment?

## Szintézis: hol a határ a jó KPI-rendszer és a mikromenedzsment között?

### Eszköz marad-e a mutató, vagy döntéshozóvá válik?

Térjünk vissza a nyitó dilemmához: a 22 KPI-t egyszerre megjelenítő dashboard nem azért volt rossz megoldás, mert a mutatók hibásak lettek volna egyenként — hanem mert a rendszer egésze nem tett különbséget a fontos és a kevésbé fontos között.

Amit ez a lecke végigvitt:

- A Goodhart-törvény megmutatja, hogy bármelyik jól megtervezett KPI elromolhat, ha céllá válik — és ez a jelenség az AI-rendszerekben is megjelenik.

- Az OEE technikai pontossága nem garancia a manipuláció ellen — a "gaming" mindig a helyi optimalizálás és a rendszerszintű cél közötti feszültségből fakad.

- A Balanced Scorecard csak akkor marad stratégiai eszköz, ha nem engedik bürokratikus rituálévá silányulni.

- A dashboard-tervezés sosem "semleges" — akár ember, akár AI választja ki, mit emeljen ki, ez mindig tartalmaz értékítéletet.

🏭 Záró tanulság

Egy jó KPI-rendszer arra való, hogy támogassa a döntéshozó ítélőképességét — nem arra, hogy helyettesítse azt. Amikor egy vezető minden döntését kizárólag a dashboardra hivatkozva hozza meg, és nem meri megkérdőjelezni a mutatót, az már nem adatvezérelt vezetés, hanem mikromenedzsment automatizált álruhában.

🤔 Záró reflektív kérdés

Hol húznád meg a határt a saját munkahelyeden — mettől kezdve válik egy KPI-alapú vezetési stílus mikromenedzsmenté?

Kitekintés a következő előadásra: a 7. előadásban azt vizsgáljuk, mi történik, amikor a mutatók mögötti mintázatokat nem az ember, hanem a gép fedezi fel — az OLAP-tól a valódi adatbányászatig, egészen a Target-cég híres, etikailag is vitatott terhesség-előrejelző algoritmusáig.

## 1. 6. előadás: Alapfogalmak — Opcionális Könyv

(forrás: 6.10.html)

### 1. 6. előadás: Alapfogalmak — Opcionális Könyv

## 2. A BI-rendszer hat eleme

(forrás: 6.11.html)

### 2. A BI-rendszer hat eleme

## A BI-rendszer hat eleme

### Alapfogalmak — mielőtt belevágnánk a kritikába

Egy teljes üzleti intelligencia (BI) környezet hat, egymásra épülő elemből áll:

- Üzleti környezet adatai — a nyersanyag, amiből minden más épül

- BI-infrastruktúra — adatbázisok, adattárházak, adatpiacok

- BA-eszközkészlet — az elemző szoftverek (pl. Power BI)

- Menedzseri módszerek — hogyan használják a vezetők mindezt (pl. Balanced Scorecard)

- Szállítási platform — MIS, DSS vagy ESS, a felhasználó szintjétől függően

- Felhasználói felület — dashboard, riport, amit ténylegesen látunk

[kép]Ábra helye: BI környezet

Érdemes megjegyezni: a Power BI-labor gyakorlatilag a 3. és a 6. elemmel foglalkozik a legtöbbet — de ez az egész csak akkor működik jól, ha az 1. és 2. elem (adat és infrastruktúra) is rendben van.

Forrás: Laudon & Laudon, Ch.12 (Fig. 12.3)

## 3. Riport-példák funkcionálisan

(forrás: 6.12.html)

### 3. Riport-példák funkcionálisan

## Riport-példák funkcionálisan

### Alapfogalmak — mielőtt belevágnánk a kritikába

A BI-rendszerek nem elvont fogalmak — konkrét, előre definiált riportokat generálnak minden vállalati funkcionális területen:

Terület | 
Tipikus riportok | 

Értékesítés | Forgalom-előrejelzés, értékesítési csapatteljesítmény, kereszt-értékesítés, értékesítési ciklusidő | 

Ügyfélszolgálat | Ügyfél-elégedettség, szolgáltatási költség, megoldási arány, churn-ráta | 

Marketing | Kampányhatékonyság, hűség és lemorzsolódás, kosárelemzés | 

Beszerzés | Közvetlen/közvetett kiadások, szerződésen kívüli beszerzés, beszállítói teljesítmény | 

Ellátási lánc | Hátralék, teljesítési státusz, rendelési ciklusidő | 

Pénzügy | Főkönyv, vevő-/szállítóállomány, cash flow, jövedelmezőség | 

HR | Alkalmazotti termelékenység, kompenzáció, munkaerő-demográfia, megtartás | 

Ez a lista jól mutatja: a BI nem egy elszigetelt eszköz, hanem minden vállalati funkcióba beépül — ezért is fontos, hogy a KPI-tervezés (következő oldal) ne csak a gyártási területre korlátozódjon a fejedben.

Forrás: Laudon & Laudon, Ch.12

## 4. KPI-tervezés alapszinten

(forrás: 6.13.html)

### 4. KPI-tervezés alapszinten

## KPI-tervezés alapszinten

### Alapfogalmak — mielőtt belevágnánk a kritikába

Egy jó KPI (Key Performance Indicator) megtervezéséhez két alapfogalmat érdemes felidézni:

SMART-kritériumok — egy jó mutató legyen:

- Specifikus (konkrét, egyértelmű, mit mér)

- Mérhető (számszerűsíthető)

- Achievable / elérhető (reális célérték)

- Relevant / releváns (valóban a stratégiai célhoz kapcsolódik)

- Time-bound / időhöz kötött (van határidő vagy mérési periódus)

Lag- és lead-mutatók megkülönböztetése:

- Lag-mutató (késleltetett, "utólagos" mutató): a már megtörtént eredményt méri — pl. havi árbevétel, negyedéves selejtarány. Könnyen mérhető, de már nem lehet rajta változtatni.

- Lead-mutató (előrejelző, "vezető" mutató): a jövőbeli eredményt előre jelző tényezőt méri — pl. karbantartási gyakoriság, munkatársi képzési óraszám. Nehezebben mérhető, de még lehet rajta beavatkozni.

Példa: ha a cél a selejtarány (lag-mutató) csökkentése, egy jó lead-mutató lehet a gépkarbantartási ütemterv betartása — mert ez az, amin ma még lehet változtatni, mielőtt a selejtarány romlana.

Forrás: saját anyag (ÜIA-ismétlés)

## 5. Az OEE alapképlete

(forrás: 6.14.html)

### 5. Az OEE alapképlete

## Az OEE alapképlete

### Alapfogalmak — mielőtt belevágnánk a kritikába

Az OEE (Overall Equipment Effectiveness) a gyáripar egyik legelterjedtebb összetett hatékonysági mutatója:

OEE = Rendelkezésre állás × Teljesítmény × Minőség

- Rendelkezésre állás = tényleges üzemidő ÷ tervezett üzemidő

- Teljesítmény = (ciklusidő × legyártott darabszám) ÷ tényleges üzemidő

- Minőség = jó darabszám ÷ összes legyártott darabszám

Egyszerű számpélda: ha egy gép a tervezett üzemidejének 90%-át üzemel, e közben a névleges kapacitás 85%-át hozza, és a legyártott darabok 98%-a megfelelő minőségű:

OEE = 0,90 × 0,85 × 0,98 ≈ 0,75, azaz 75%

A "world class" OEE-érték a szakirodalom szerint kb. 85% körül van — a legtöbb üzem valós OEE-je jellemzően 40–60% között mozog.
[kép]

Ábra: OEE három komponensének vizuális szemléltetése

Forrás: saját anyag (ÜIA-ismétlés)

## 6. Balanced Scorecard alapok

(forrás: 6.15.html)

### 6. Balanced Scorecard alapok

## Balanced Scorecard alapok

### Alapfogalmak — mielőtt belevágnánk a kritikába

A Balanced Scorecard (BSC) Kaplan és Norton (1996) módszertana, amely a vállalati teljesítményt négy perspektívából vizsgálja egyszerre, nem csak pénzügyi szempontból:

Perspektíva | 
Alapkérdés | 

Pénzügyi | Hogyan látnak minket a tulajdonosok/befektetők? | 

Vevői | Hogyan látnak minket a vevőink? | 

Belső folyamat | Miben kell kiválónak lennünk? | 

Tanulás-fejlődés | Hogyan tudjuk fenntartani a képességünket a változásra és fejlődésre? | 

A négy perspektíva vizuálisan egy stratégiai térképen (Strategy Map) jeleníthető meg, amely megmutatja az oksági kapcsolatot: a tanulás-fejlődési beruházások → javítják a belső folyamatokat → ami javítja a vevői elégedettséget → ami végül pénzügyi eredményben csapódik le.
[kép]

Ábra: Strategy Map for BSC

Forrás: Kaplan, R. S., & Norton, D. P. (1996); Laudon & Laudon, Ch.12

## 7. Dashboard-tervezés alapszabályai

(forrás: 6.16.html)

### 7. Dashboard-tervezés alapszabályai

## Dashboard-tervezés alapszabályai

### Alapfogalmak — mielőtt belevágnánk a kritikába

Két klasszikus szerző alapelvei segítenek abban, hogy egy dashboard valóban informatív legyen, ne csak dekoratív:

Tufte "data-ink ratio" elve: minden vizuális elemnek (szín, vonal, keret) információt kell hordoznia — ami nem hordoz információt, az felesleges "zaj", és elvonja a figyelmet a lényegtől.

Few néhány gyakori dashboard-hibája:

- túlzsúfoltság — túl sok mutató egy felületen (emlékeztető: lásd a fejezet nyitó dilemmáját!)

- félrevezető skálázás (pl. y-tengely nem nulláról indul)

- felesleges 3D-effektek, díszítőelemek, amelyek torzítják az adat leolvasását

- rossz színhasználat (pl. piros-zöld kontraszt, ami színtévesztőknek nem olvasható)

Alapszabály: egy jó dashboard első pillantásra megmutatja, mi a legfontosabb — nem igényel magyarázatot, és nem hagy teret a félreértésnek.
[kép]

Ábra: "jó" és "rossz" dashboard

Forrás: Tufte, E. R.; Few, S. (saját anyag alapján, ÜIA-ismétlés)
