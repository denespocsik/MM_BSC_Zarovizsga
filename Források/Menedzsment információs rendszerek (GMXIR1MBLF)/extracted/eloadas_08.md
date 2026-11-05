# 8. előadás: 8. előadás Big Data: Hogyan nyerjünk értéket? - Kötelező tananyag

## 1. 8. fejezet: Big Data — hogyan nyerjünk belőle valódi értéket?

(forrás: 8.1.html)

### 1. 8. fejezet: Big Data — hogyan nyerjünk belőle valódi értéket?

## 2. Nyitó dilemma: a GE és a Predix

(forrás: 8.2.html)

### 2. Nyitó dilemma: a GE és a Predix

## Big Data: hogyan nyerjünk belőle valódi értéket?

### Miért fektet be mégis mindenki, ha a legtöbb projekt megbukik?

🔴 Döntés előtt — Ön az IT-vezető

Ön egy középvállalat IT-vezetője. A vezérigazgató a legutóbbi igazgatósági ülésről visszatérve bejelenti: "A versenytársaink Big Data-ba fektetnek. Nekünk is lépnünk kell, különben lemaradunk. Indítsunk el egy hasonló projektet — mennyi idő alatt tudunk platformot választani?"

Mit tenne elsőként?

- A) Elkezdi felmérni a piacon elérhető Big Data-platformokat, és összeállít egy rövid listát.

- B) Visszakérdez: "Milyen konkrét üzleti problémát oldana meg ez?" — és csak ez után kezd technológiai tervezésbe.

- C) Javasolja, hogy egy külső tanácsadó céget bízzanak meg a teljes projekt megtervezésével és kivitelezésével.

(A választ a fejezet 3. és 9. oldalán elemezzük — egy valós, nagyvállalati zászlóshajó-projekt fényében.)

#### A tét nem elméleti

[kép]

Ábra: Digitális projektek sikeraránya

Egy 2015-ös elemzői előrejelzés szerint a Big Data-projektek 60%-a nem jut túl a kísérleti (pilot) fázison — a fő ok a régi vállalati gondolkodásmód és szervezeti kultúra, nem a technológia hiányossága. Két évvel később a becslést felülvizsgálták: a valós bukási arány közelebb áll a 85%-hoz, és a felülvizsgálat szerint "a probléma nem a technológia", hanem az üzleti folyamatokba illesztés nehézsége, a vezetői ellenállás, a belső politika, a szakemberhiány és a hiányos adat-governance. Egy független vállalati felmérés ezt megerősíti: a válaszadó cégek 85%-a indított célzottan adatvezérelt kultúra-programot, de mindössze 37%-uk számolt be tényleges sikerről.

Ez ellentmond a józan észnek: ha ilyen magas a kudarcráta, és a szakértők egyöntetűen szervezeti okokra mutatnak, miért fektet bele mégis szinte minden nagyvállalat évről évre egyre több erőforrást? A válasz kulcsa abban rejlik, hogy a Big Data nem informatikai projekt, hanem szervezeti-stratégiai döntés. Ennek a fejezetnek a gerincét egy olyan vállalat esete adja, amely a 2010-es évek közepén a Big Data és IoT egyik legambiciózusabb zászlóshajó-projektjét indította el — és amelynek sorsa azóta gyökeresen átértékelődött.

💡 Tanulási eredmények

A fejezet elvégzése után Ön képes:

- kritikusan értékelni, miért nem hoz automatikusan üzleti értéket egy Big Data-beruházás, és felismerni az érték-realizálás tipikus akadályait (Gartner, 2015, 2017; NewVantage Partners, é. n.)

- megkülönböztetni, mikor elegendő a hagyományos ("kis") adatelemzés, és mikor indokolt a Big Data-infrastruktúra kiépítése — build/buy/outsource döntési logika mentén (McAfee & Brynjolfsson, 2012)

- kritikusan elemezni egy valós, nagy volumenű vállalati Big Data-kezdeményezés sikerét és kudarcát, és azonosítani a stratégiai, nem technikai bukási okokat

- értékelni, hogyan változtatja meg a mesterséges intelligencia és a generatív AI a Big Data-ból nyerhető érték jellegét és mértékét

- mérlegelni az edge computing és a centralizált felhő-feldolgozás közötti stratégiai választást ipari/műszaki kontextusban (Achouch et al., 2022)

- alkalmazni az adatosítás fogalmát (Mayer-Schönberger & Cukier, 2013), és felismerni, mikor válik egy szervezetben az adat a döntéshozatal középpontjává

📚 A fejezet térképe

2. oldal: építsünk, vásároljunk, vagy szervezzünk ki? → 3. oldal: a GE és a Predix — egy zászlóshajó-projekt két olvasata → 4. oldal: Big Data és a mesterséges intelligencia → 5. oldal: edge computing és a centralizáció kockázata → 6. oldal: amikor az adat kerül a döntés középpontjába (Moneyball, Zara, Tesco Clubcard) → 7. oldal: az adatvezérelt szervezet érettségi lépései → 8. oldal: Big Data ROI és TCO → 9. oldal: vissza a nyitó dilemmához.

🤔 Gondolkodtató kérdés

A fenti A/B/C döntési helyzetben melyik választás csökkentené leginkább annak esélyét, hogy Ön is a fent említett bukási arányhoz tartozzon?

Forrás: Gartner (2015, Business Intelligence & Analytics Summit) és felülvizsgálata (2017); NewVantage Partners vállalati felmérése az adatvezérelt kultúra-programok sikerességéről; McAfee, A., & Brynjolfsson, E. (2012). Big Data: The management revolution. Harvard Business Review, 90(10), 60–68.

## 3. Big Data mint szervezeti döntés

(forrás: 8.3.html)

### 3. Big Data mint szervezeti döntés

## Építsünk, vásároljunk, vagy szervezzünk ki?

### Big Data mint szervezeti döntés, nem technológiai divat

Mielőtt bármilyen technológiai kérdést feltennénk, egy alapvetőbb, menedzseri kérdést kell megválaszolni: egyáltalán szükségünk van-e Big Data-ra? Sok szervezet abba a hibába esik, hogy a "Big Data" kifejezés presztízse miatt épít ki drága infrastruktúrát olyan problémákra, amelyeket egy jól megtervezett, hagyományos ("kis") adatelemzés is megoldana. Egy klasszikus, azóta is sokat idézett menedzsment-elemzés éppen ezt a döntési logikát fogalmazza meg (McAfee & Brynjolfsson, 2012): a kérdés nem az, hogy "van-e elég adatunk ahhoz, hogy Big Data-nak nevezzük", hanem hogy a probléma jellege igényli-e a nagy volumenű, nagy sebességű vagy nagy változatosságú adatok kezelését.

[kép]

Ábra: döntési fa —  "hagyományos BI elég" vs. "Big Data indokolt" . 

#### A build/buy/outsource döntési keret

Opció | 
Mikor indokolt | 
Fő kockázat | 

Build (saját fejlesztés) | 
az adatelemzés a versenyelőny megkülönböztető eleme | 
magas költség, hosszú átfutási idő, technológiai versenyhelyzet | 

Buy (kész platform) | 
az adatelemzés támogató funkció, nem fő tevékenység | 
vendor lock-in, testreszabhatóság korlátai | 

Outsource (kiszervezés) | 
gyors indulás, korlátozott belső szakértelem | 
függőség, adatbiztonsági kérdések, tudás nem épül be a szervezetbe | 

Ez a döntés nem technikai, hanem stratégiai: attól függ, hogy az adatelemzési képesség a vállalat versenyelőnyének kritikus, megkülönböztető eleme-e, vagy csak támogató funkció. Egy olyan cégnél, ahol az adatelemzés csak támogatja a fő tevékenységet (pl. egy gyártó cég karbantartás-tervezését), a kész platform vagy a kiszervezés jellemzően alacsonyabb kockázatú és gyorsabban megtérülő út.

⚠️ A GIGO-elv és a 80–20-as arány mint erőforrás-allokációs döntés

A "garbage in, garbage out" (GIGO) elv a Big Data-kontextusban élesebben jelentkezik, mint a hagyományos üzleti intelligenciánál, mert a volumen és a változatosság miatt az adattisztítás technikailag is nehezebb. A gyakorlatban az adatelemzők munkaidejük jelentős részét — becslések szerint akár 50–80%-át — adattisztítással és -előkészítéssel töltik, nem magával az elemzéssel. Ez nem technikai részletkérdés, hanem menedzseri döntés tárgya: a vezetésnek explicit módon kell allokálnia erőforrást (adatmérnöki létszám, idő, költségvetés) az adatminőségi munkára.

💡 Műszaki analógia: a Big Data-infrastruktúra kiépítése olyan, mint egy új gyártósor beruházása — nem azért érdemes megépíteni, mert technológiailag lehetséges, hanem mert a megtermelt volumen és a minőségi követelmények indokolják.

🤔 Kritikai kérdés — menedzseri szemmel

Gondoljon egy saját szervezetére vagy egy ismert vállalatra. Az adatelemzés ott a versenyelőny megkülönböztető eleme, vagy csak támogató funkció? Ez a válasz hogyan befolyásolná a build/buy/outsource döntést?

Forrás: McAfee, A., & Brynjolfsson, E. (2012). Big Data: The management revolution. Harvard Business Review, 90(10), 60–68.

## 4. Esettanulmány: a GE és a Predix

(forrás: 8.4.html)

### 4. Esettanulmány: a GE és a Predix

## Egy zászlóshajó-projekt két olvasata

### 2016: minden idők egyik legnagyobb ígérete. 2024: figyelmeztető példa.

🔴 Az első olvasat — a 2016-os siker-narratíva

A General Electric a 2010-es évek közepén radikális stratégiai fordulatot hirdetett: a hagyományos ipari gyártó (repülőgép-hajtóművek, mozdonyok, erőművi turbinák) szoftvercéggé kívánt átalakulni. Ennek középpontjában a Predix platform állt — egy ipari IoT-alapú felhőszolgáltatás, amely a berendezésekbe épített szenzorok (hőmérséklet, vibráció, nyomás, fordulatszám) adatait gyűjtötte és elemezte, hogy előre jelezze a meghibásodásokat, és optimalizálja a karbantartást. A vezetés kinyilvánított célja az volt, hogy a GE 2020-ra a top 10 amerikai szoftvercég közé kerüljön, és évi több milliárd dolláros bevételt termeljen a Predix-alapú szolgáltatásokból.

#### A második olvasat — amit a 2016-os elemzések még nem tudhattak

Év | 
Esemény | 

2013–2014 | 
A Predix platform elindul, saját felhő-adatközponttal | 

2016 | 
Csúcs-narratíva: GE Digital, top 10 szoftvercég ambíció | 

2018–2019 | 
A bevételi célok elmaradnak; a GE elkezdi leépíteni a digitális üzletágat | 

2024 | 
A GE konglomerátum szétválik — a Predix-kudarc az elemzők szerint ebben is szerepet játszott | 

A vállalat összesen több mint 7 milliárd dollárt fektetett a platform fejlesztésébe és a kapcsolódó tanácsadói csapatokba, a bevételi célok azonban jelentősen elmaradtak a tervezettől. A kudarc a szakértői elemzések szerint nem technikai, hanem stratégiai és kulturális eredetű volt, három fő ok mentén:

1. Saját infrastruktúra-építés versenyhelyzetben

A GE saját felhő-adatközpontot épített a Predix kiszolgálására, ahelyett hogy meglévő felhőszolgáltatásra (Amazon, Microsoft, Google) épített volna — versenybe kényszerítve magát a nála jóval nagyobb erőforrásokkal rendelkező technológiai vállalatokkal.

2. Univerzális platform diffúz stratégiával

A Predix minden ipari szektorhoz (repülőgépgyártás, energiatermelés, egészségügy) egyetlen platformot próbált nyújtani, holott egy szélturbina és egy MRI-berendezés üzemeltetési logikája és szabályozási környezete gyökeresen eltérő.

3. Termékközpontú, nem szolgáltatásközpontú szemlélet

A GE mint hagyományos gyártó vállalat nem tudott átállni a szoftveripari szereplőkre jellemző szolgáltatás-központú gondolkodásmódra — fejlesztői közösség, felhasználói élmény, iterációs sebesség terén jelentős lemaradásban volt.

🔑 A tanulság

Ha a fejezet elején az A) opciót választotta — azonnal technológiai szállítót keresni —, érdemes újragondolni: a GE pontosan ezt tette, és ez volt az egyik fő bukási ok. A B) opció — előbb az üzleti problémát tisztázni, majd a technológiát hozzáigazítani — sokkal közelebb áll ahhoz, amit a szakirodalom sikeres megközelítésként azonosít. Egy Big Data/IoT-kezdeményezés sikeréhez nem elég a technológiai képesség és a tőke — szükséges a fókuszált, a saját szakértelemre épülő stratégia és a szervezeti kultúra tényleges átalakítása.

🤔 Reflektív kérdés

Ha a GE 2014-ben nem saját adatközpontot épít, hanem egy meglévő felhőszolgáltatóra alapozza a Predixet, és kevesebb iparágra koncentrál — vajon a technikai koncepció önmagában életképes lett volna? Mi választja el a jó ötletet a jó stratégiától?

Élő, ellenőrizhető források:

- Predix (szoftver) — háttér és fejlődéstörténet: en.wikipedia.org/wiki/Predix_(software)

- Elemzés a bukás okairól (Panorama Consulting): panorama-consulting.com/ge-digital-transformation-failure

Forrás: Laudon, K. C., & Laudon, J. P. (2017). Management information systems (15th ed.). Pearson. Ch.12 (GE Predix esettanulmány); utólagos kritikai elemzések a Predix platform sorsáról (2018–2024, ipari elemzések és üzleti sajtó).

## 5. Big Data és a mesterséges intelligencia

(forrás: 8.5.html)

### 5. Big Data és a mesterséges intelligencia

## Ki kinek a "tápláléka"?

### A Big Data és az AI kölcsönös, nem egyirányú kapcsolata

Az AI-nak Big Data-ra van szüksége

A modern gépi tanulási és mélytanulási modellek — beleértve a generatív AI-t is — annál pontosabb mintázatokat ismernek fel, minél nagyobb és változatosabb adathalmazon tanulnak. Egy prediktív karbantartási modell, amely egyetlen gép néhány hónapos szenzoradatán tanul, jóval kevésbé megbízható, mint amely több ezer hasonló berendezés több éves adatán épül fel. A Big Data az AI "üzemanyaga" — enélkül a legkifinomultabb algoritmus is csak találgat.

A Big Data-nak AI-ra van szüksége

A puszta adatmennyiség önmagában nem termel értéket, ha nincs, ami értelmet ad neki. A hagyományos statisztikai módszerek (7. fejezet: OLAP, klasszikus adatbányászat) jól működnek strukturált, kisebb adathalmazokon, de a nagy volumenű, gyorsan változó, vegyes formátumú adatok esetén a gépi tanulás ismer fel mintázatokat ott, ahol az ember csak zajt látna.

#### Mit tenne ma a generatív AI a Predix helyén?

A GE 2014-es Predix-koncepciója — szenzoradatok gyűjtése, szabályalapú küszöbértékek, emberi elemzők jelentései — ma jelentősen automatizálhatóbb lenne. Egy modern rendszerben a gépi tanulási modellek nemcsak küszöbérték-átlépést jeleznének, hanem anomáliát ismernének fel olyan mintázatokban is, amelyeket előre nem definiáltak. A generatív AI ezen felül a nyers szenzoradatokból természetes nyelvű karbantartási jelentéseket is összeállíthatna a technikusok számára.

⚠️ A kritikai fenntartás — az AI nem oldja meg a szervezeti problémát

Egy 2018-as elemzői előrejelzés szerint 2022-ig az AI-projektek 85%-a téves vagy hasznavehetetlen eredményt szolgáltat majd — ugyanaz a szervezeti-kulturális minta, amit az 1. oldalon a Big Data-nál láttunk. Az AI felerősíti a jó adatstratégia előnyeit, de nem helyettesíti azt — egy rosszul megtervezett, rossz minőségű adatokra épülő projektet az AI sem menti meg, sőt, a hibás mintázatokat nagyobb magabiztossággal, nagyobb léptékben termeli újra.

💡 Műszaki analógia: az AI olyan, mint egy rendkívül tapasztalt géplakatos, aki apró rezgésmintázatokból következtet a meghibásodásra — de ha soha nem látott elég gépet működés közben, a megérzése is megbízhatatlan lesz.

🤔 Gondolkodtató kérdés

Ha egy vállalat AI-alapú prediktív karbantartást vezet be, de a mögöttes adatgyűjtési folyamat hibás, mi történik gyorsabban és nagyobb léptékben — a hibás döntés, vagy a hibás döntés felismerése?

✅ Gyors ellenőrző kérdés

Egy vállalat prediktív karbantartási AI-modellt vezet be, de a szenzorai rosszul vannak kalibrálva. Az AI bevezetése ebben az esetben...

A) javítani fog a helyzeten, mert az AI kiszűri a hibás adatokat

B) ronthat a helyzeten, mert nagyobb magabiztossággal és léptékben termeli újra a hibás mintázatokat

C) nem lesz hatással a döntések minőségére

(Helyes válasz: B)

[kép]

Ábra: "Big Data → AI" és "AI → Big Data"

Forrás: Gartner (2018). CIO Agenda Survey.

## 6. Edge computing és a centralizáció kockázata

(forrás: 8.6.html)

### 6. Edge computing és a centralizáció kockázata

## Amikor a milliszekundum számít

### Edge computing: stratégiai válasz a centralizáció kockázatára

A GE/Predix-eset egyik bukási oka (3. oldal) az volt, hogy a vállalat saját, centralizált felhő-adatközpontot épített az összes szenzoradat feldolgozására. Ez egy alapvetőbb műszaki-stratégiai kérdést is felvetett: valóban minden adatot érdemes-e a felhőbe küldeni feldolgozásra?

#### Az edge computing alaplogikája

Az edge computing (peremhálózati számítás) azt jelenti, hogy az adatfeldolgozás egy része nem a távoli felhőszerveren, hanem közvetlenül a berendezés mellett, helyben történik.

Architektúra | 
Jellemző válaszidő | 
Mire alkalmas | 

Felhő (cloud) | 
~100–500 ezredmásodperc | 
hosszú távú, komplex elemzés, modell-tanítás | 

Edge (gép melletti) | 
egyszámjegyű – alacsony kétjegyű ezredmásodperc | 
azonnali riasztás, kritikus beavatkozás | 

Egy nagy sebességű forgó alkatrész (pl. turbina) csapágyhibája másodperceken belül kialakulhat — ekkor egy 100–500 ezredmásodperces késleltetésű felhő-alapú riasztás egyszerűen elkésett. Az ipari edge-megoldások ezzel szemben a döntést ott hozzák meg, ahol az adat keletkezik (Achouch et al., 2022).

Mikor éri meg edge-re építeni, és mikor a felhőre?

A döntés nem "vagy-vagy", hanem tipikusan hibrid architektúra kérdése: az edge réteg végzi a valós idejű, azonnali reakciót igénylő szűrést és riasztást, míg a felhő réteg végzi a hosszú távú, komplex elemzést és a modellek tanítását. Egy ipari IoT-kontextusban végzett kutatás szerint a sikeres prediktív karbantartási rendszerek jellemzően ezt a réteges — edge, fog és felhő komponenseket egyaránt tartalmazó — architektúrát alkalmazzák, nem egyetlen, mindenre kiterjedő centralizált megoldást.

🔑 Visszakötés a GE/Predix-esethez

Ha a GE 2014-ben eleve hibrid, edge-alapú architektúrában gondolkodik, valószínűleg nem kényszerült volna arra a stratégiai hibára, hogy egy saját, mindenre elegendő centralizált adatközpontot építsen a technológiai óriásokkal versenyezve. Az edge computing nem csak technikai optimalizálás, hanem stratégiai kockázatcsökkentés — kevesebb függés egy centralizált infrastruktúrától, alacsonyabb sávszélesség-költség, és működőképesség hálózati kimaradás esetén is.

💡 Műszaki analógia: az edge computing olyan, mint amikor egy gyártósoron a minőségellenőrzést nem a központi irodában, hanem közvetlenül a gép mellett végzik — mire az adat "felérne" a központba, a hibás termék már rég legördült volna a szalagról.

🤔 Reflektív kérdés

Egy magyar KKV gyártó üzem, amely 15 régi CNC-gépet üzemeltet, fontolgatja az IoT-alapú állapotfigyelés bevezetését. Milyen szempontok alapján döntené el, hogy edge-alapú helyi feldolgozásra, vagy egyszerűbb, felhő-alapú megoldásra van szüksége?

Forrás: Achouch, M., Dimitrova, M., Ziane, K., Sattarpanah Karganroudi, S., Dhouib, R., Ibrahim, H., & Adda, M. (2022). On predictive maintenance in industry 4.0: Overview, models, and challenges. Applied Sciences, 12(16), 8081.; Analyzing the impact of edge, fog and cloud computing on predictive maintenance in the Industrial Internet of Things (2025). Discover Computing.

## 7. Adatosítás: három példa három világból

(forrás: 8.7.html)

### 7. Adatosítás: három példa három világból

## Amikor az adat kerül a döntés középpontjába

### Három példa három világból

A Big Data mögötti valódi paradigmaváltás nem a technológiában, hanem a gondolkodásmódban rejlik.

Small Data vs. Big Data — okság vs. korreláció

A hagyományos statisztikai megközelítés kevés, pontos adatra épül, és oksági összefüggéseket keres — azt, hogy miért történik valami. A Big Data-szemlélet ezzel szemben gyakran kusza, hatalmas mennyiségű adatból dolgozik, és elsősorban korrelációkat keres — azt, hogy mi jár együtt mivel, anélkül hogy megértené, miért. Ez tudatos kompromisszum: bizonyos kérdéseknél a megbízható korreláció is elegendő cselekvéshez (Mayer-Schönberger & Cukier, 2013).

Adatosítás (datafication)

Egyre több, korábban nem számszerűsíthetőnek tartott dolog válik adattá (Mayer-Schönberger & Cukier, 2013). A szavakból keresési adat lesz, a helymeghatározásból GPS-adat, az emberi kapcsolatokból hálózatelemzési adat. Az adat önmagában árucikké válik, amelynek elsődleges és másodlagos értéke egyaránt lehet.

#### Első példa: Moneyball

Egy 2003-as könyv és az abból készült 2011-es film az Oakland Athletics baseballcsapat történetét dolgozza fel, amely — korlátozott költségvetéssel — radikálisan új megközelítést vezetett be a játékosértékelésben: a scoutok megérzése helyett szisztematikus statisztikai elemzést (sabermetrics). A történet lényege a szervezeti ellenállás: a tapasztalt szakemberek kezdetben elutasították, mert az adat szembement a bevett szakértői tapasztalattal.

🎬 Elérhetőség (folyamatosan frissülő aggregátor): justwatch.com/hu/film/moneyball

#### Második példa: Zara

Egy Harvard Business School esettanulmány szerint a Zara (Inditex-csoport) a divatipar hagyományos, előre tervező logikáját valós idejű adatvisszacsatolási hurokkal váltotta fel. A boltvezetők kézi eszközökkel rögzítik, mit próbálnak fel a vásárlók, de nem vásárolnak meg — maguk is "adatgyűjtővé" válnak.

#### Harmadik példa: a Tesco Clubcard

A Tesco 1995-ben indította el hűségkártya-programját, amely az Egyesült Királyság első nagy áruházlánci lojalitásprogramja volt. A tesztidőszak eredményeit bemutató ülésen a Tesco akkori elnöke állítólag ezt mondta:

"Ami megrémiszt ebben, hogy három hónap alatt többet tudtok meg a vásárlóimról, mint én harminc év alatt."

— Lord MacLaurin, a Tesco akkori elnöke, idézi: Emerald Publishing (2004)

A hűségkártya itt nem elsősorban jutalmazási eszköz, hanem adatgyűjtő infrastruktúra: minden vásárlás adatosítva, egyénhez köthetően rögzítve.

A közös tanulság

Mindhárom eset ugyanazt mutatja: az adat nem attól válik értékessé, hogy sok van belőle, hanem attól, hogy egy korábban megérzés-alapú döntést szisztematikussá és megismételhetővé tesz.

[kép]

Ábra: Adatosítás  — baseball-scout, divattervező és boltvezető "megérzés-alapú" folyamata

🤔 Reflektív kérdés

Az Ön saját szakterületén (mérnöki/műszaki menedzsment) hol létezik ma olyan döntés, amelyet még mindig döntően megérzés vagy tapasztalat alapján hoznak meg, és amelyet szisztematikus adatelemzéssel lehetne alátámasztani?

Forrás: Mayer-Schönberger, V., & Cukier, K. (2013). Big data: A revolution that will transform how we live, work, and think. Houghton Mifflin Harcourt.; Lewis, M. (2003). Moneyball: The art of winning an unfair game. W. W. Norton & Company.; Miller, B. (rendező). (2011). Moneyball [film]. Columbia Pictures.; McAfee, A. P., Dessain, V., & Sjoman, A. (2007). Zara: IT for fast fashion (Harvard Business School Case 604-081).; Interjú Clive Humbyval (2004). The success of the Tesco Clubcard in winning customer loyalty. International Journal of Retail & Distribution Management, Emerald Publishing.

## 8. Az adatvezérelt szervezet érettségi modellje

(forrás: 8.8.html)

### 8. Az adatvezérelt szervezet érettségi modellje

## Négy lépés az adatvezérelt szervezetig

### Az adatvezérelt szervezet érettségi modellje

Az eddigi oldalak mind ugyanahhoz a következtetéshez vezettek: a Big Data önmagában nem hoz üzleti értéket — csak akkor, ha a szervezet kultúrája és struktúrája képes befogadni és hasznosítani azt. Ez fokozatos érettségi folyamat (Davenport & Harris, 2007, 2017 nyomán, leegyszerűsítve).

Lépés | 
Jellemző | 
Kapcsolódó eset | 

1. Szórványos kísérletezés | 
izolált próbálkozások, nincs vezetői mandátum | 
a legtöbb elbukó projekt (1. oldal) | 

2. Technológiai befektetés mandátum nélkül | 
megvan a technológia, hiányzik a "miért" | 
GE/Predix (3. oldal) | 

3. Adatvezérelt döntés egy területen | 
mérhető eredmény egy konkrét problémán | 
Moneyball, Zara, Tesco (6. oldal) | 

4. Szervezeti kultúra átalakítása | 
adatvezérelt döntés az alapértelmezett elvárás | 
BICC-érettség (5. fejezet) | 

⚠️ Magyar kontextus

Egy hazai közepes méretű gyártó vállalat (pl. a 7. fejezetben megismert üzemi környezet) tipikusan a 2–3. lépés között helyezkedik el: van szenzoros adatgyűjtés egy-egy gépsoron, de a szervezet egésze még nem tekinti alapértelmezettnek az adatalapú döntéshozatalt minden területen. A modell éppen azt segít átlátni, hogy egy KKV-nak nem kell egyből a 4. lépésre ugrania — a 3. lépés, egy jól kiválasztott pilot-terület, jóval reálisabb belépési pont.

💡 Műszaki analógia: az adatvezérelt szervezet felépítése olyan, mint a minőségbiztosítási rendszer bevezetése egy gyártó üzemben — a valódi érték akkor jelentkezik, amikor a minőségi gondolkodás az egész szervezet alapértelmezett működési módjává válik.

[kép]

Ábra: Az adatvezérelt szervezet érettségi modellje

Forrás: Davenport, T. H., & Harris, J. G. (2017). Competing on analytics: The new science of winning (frissített kiadás). Harvard Business Review Press.

## 9. Big Data ROI és TCO

(forrás: 8.9.html)

### 9. Big Data ROI és TCO

## Mikor éri meg, mikor nem

### Big Data ROI és TCO

A build/buy/outsource döntés (2. oldal) csak a kiindulópont — a tényleges pénzügyi mérlegelés két fogalom köré épül: a megtérülés (ROI) és a teljes birtoklási költség (TCO, Total Cost of Ownership; Ellram, 1993).

[kép]

Ábra: TCO-jéghegy, Ellram (1993)

TCO-elem | 
Miért marad gyakran figyelmen kívül | 

Adatmérnöki/adatelemzői létszám | 
a 2. oldalon látott 50–80%-os adattisztítási arány rejtve marad a licenc-árban | 

Integráció a meglévő rendszerekkel | 
gyakran csak a bevezetés közben derül ki a valós mérték | 

Stratégiai lehetőségköltség | 
a GE/Predix-eset (3. oldal) élesen megmutatta: az erőforrás, amit rossz irányba fektetünk, máshol hiányzik | 

⚠️ A ROI-számítás csapdája: mit mérünk?

Sok szervezet a Big Data-projekt megtérülését olyan mutatókkal próbálja igazolni, amelyek a technológiai aktivitást mérik, nem az üzleti értéket (pl. "hány terabájt adatot dolgozunk fel naponta"). Ez a hiba rokon a Goodhart-törvénnyel (5–6. fejezet): a mérőszám maga válik céllá. A helyes megközelítés fordított logikájú: először azonosítjuk a konkrét üzleti döntést, amit a Big Data-elemzés jobbá tehet, és csak utána számoljuk ki, mennyit ér ez pénzben.

Mikor NEM éri meg? Ha egy szervezet nem tudja megfogalmazni, milyen konkrét, jelenleg rosszul meghozott döntést javítana a beruházás, a ROI-számítás eleve légből kapott lesz. Ha a probléma mérete nem indokolja a Big Data-szintű infrastruktúrát (2. oldal döntési fája), a TCO szinte garantáltan meghaladja a realizálható hasznot.

🤔 Gondolkodtató kérdés

Egy vállalat vezetése azzal érvel, hogy "a versenytársunk már bevezette a Big Data-elemzést, nekünk is kell, különben lemaradunk" — ez önmagában elég indoklás egy pozitív ROI-hoz? Mi hiányzik ebből az érvelésből?

Forrás: Ellram, L. M. (1993). Total cost of ownership: Elements and implementation. International Journal of Purchasing and Materials Management, 29(4), 3–11.

## 10. Összefoglalás és a nyitó dilemma feloldása

(forrás: 8.10.html)

### 10. Összefoglalás és a nyitó dilemma feloldása

## Vissza a nyitó dilemmához

### Amit a fejezet nyolc oldala egyetlen üzenetté sűrít

Térjünk vissza a fejezet elején feltett döntési helyzethez: a vezérigazgató bejelenti, hogy Big Data-ba kell fektetni, és Öntől várja az első lépést.

Az üzenet, sokféle nézőpontból

A Big Data-projektek sikere és kudarca nem a technológián, hanem a szervezeti gondolkodáson múlik. A bevezető statisztikák (1. oldal) ezt számszerűen mutatták meg; a GE/Predix-eset (3. oldal) egy konkrét, nagy léptékű illusztrációval; a Moneyball, Zara és Tesco Clubcard (6. oldal) azzal, hogy megmutatták, milyen a sikeres átállás egy megérzés-alapú döntésről egy adatalapúra; az érettségi modell és a TCO/ROI-logika (7–8. oldal) pedig gyakorlati keretet adott ahhoz, hogyan tervezze meg egy műszaki menedzser ezt az átállást felelősségteljesen.

Az AI és a generatív AI (4. oldal), valamint az edge computing (5. oldal) ehhez a képhez azt teszik hozzá, hogy a technológiai eszköztár folyamatosan bővül és erősödik — de egyik sem old meg egy rosszul definiált üzleti problémát vagy egy adatellenes szervezeti kultúrát. Az AI felerősíti a jó adatstratégiát, és felerősíti a rosszat is.

🔑 Záró reflektív kérdés

Ha Ön most, a fejezet végén, újra feltehetné a kérdést a vezérigazgatónak a nyitó dilemmából — milyen egyetlen kérdéssel kezdené a választ, mielőtt bármilyen technológiai döntést meghozna?

#### Kitekintés a 9. fejezetre

A következő fejezetben a Tudásmenedzsment és intelligens szervezet témájára térünk át — ahol ismét visszatér egy hasonló alapkérdés: hogyan őrizhető meg és hasznosítható a szervezetben felhalmozott tudás, amikor a tapasztalt szakemberek távoznak, és mennyiben helyettesítheti (vagy nem helyettesítheti) ezt a mesterséges intelligencia.

Forrás: a fejezet teljes forrásjegyzéke az 1–8. oldalon, oldalanként feltüntetve.

## 11. Elmélyítő kiegészítő

(forrás: 8.11.html)

### 11. Elmélyítő kiegészítő

- Achouch, M., Dimitrova, M., Ziane, K., Sattarpanah Karganroudi, S., Dhouib, R., Ibrahim, H., & Adda, M. (2022). On predictive maintenance in Industry 4.0: Overview, models, and challenges. Applied Sciences, 12(16), 8081. https://doi.org/10.3390/app12168081
- NewVantage Partners. (2023). Data and AI leadership executive survey. NewVantage Partners LLC. https://www.newvantage.com
- Fodor, Z., & Kosztyi, D. (2020). Big data: Valós lehetőség a vállalati hatékonyság növelésére? In dBEM Conference Proceedings (pp. 27–36). Óbudai Egyetem. https://doi.org/10.18515/dBEM.M2020.n01.ch02

## 1. 8. fejezet: Big Data — Opcionális Könyv (fogalmi felidézés)

(forrás: 8.12.html)

### 1. 8. fejezet: Big Data — Opcionális Könyv (fogalmi felidézés)

## 2. Big Data alapfogalma és az 5V/7V-modell

(forrás: 8.13.html)

### 2. Big Data alapfogalma és az 5V/7V-modell

## Big Data — fogalmi felidézés

### Big Data alapfogalma és az 5V/7V-modell

A Big Data fogalma olyan adathalmazokat jelöl, amelyek mérete, keletkezési sebessége vagy formátumbeli változatossága meghaladja a hagyományos adatbázis-kezelő rendszerek (DBMS) kapacitását. A jelenség jellemzésére leggyakrabban használt keret az 5V-modell:

Volume (mennyiség) — az adatok mérete terabájtos, petabájtos vagy exabájtos nagyságrendben.

Velocity (sebesség) — az adatok keletkezésének és feldolgozásának üteme, gyakran valós időben vagy ahhoz közeli sebességgel.

Variety (változatosság) — strukturált, félig strukturált és strukturálatlan adatok együttes jelenléte (szöveg, kép, szenzoradat, tranzakciós adat).

Veracity (megbízhatóság) — az adatok minősége és pontossága; a nagy mennyiség önmagában nem garantálja a jó minőséget.

Value (érték) — az adatokból ténylegesen kinyerhető üzleti haszon; ez a dimenzió köti össze a fogalmat a Kötelező Könyv érték-realizálási problémájával.

Egyes szerzők további két dimenzióval egészítik ki a modellt (7V): a Variability (az adatok jelentésének kontextusfüggő változékonysága) és a Visualization (az eredmények érthető megjelenítésének képessége).

Ha ezek a fogalmak nem ismerősek vagy felfrissítésre szorulnak, az Üzleti Informatikai Alkalmazások tárgy "Big Data és prediktív analitika" előadása részletes, ábrákkal illusztrált bevezetést ad az 5V/7V-modellbe.

Forrás: Laudon, K. C., & Laudon, J. P. (2017). Management information systems (15th ed.). Pearson. Ch.6; Tick, A. Big data — saját előadásanyag.

## 3. Adattárolási architektúrák

(forrás: 8.14.html)

### 3. Adattárolási architektúrák

## Adattárház, adattó, adattó-ház

### Adattárolási architektúrák

A Big Data-korszak két alapvető adattárolási megközelítést hozott létre a hagyományos relációs adatbázis mellett.

Architektúra | 
Séma-elv | 
Jellemző | 

Data Warehouse (adattárház) | 
schema-on-write | 
előre definiált struktúra; jól illeszkedik ismételt, tervezett riportokhoz | 

Data Lake (adattó) | 
schema-on-read | 
natív formátumú tárolás, rugalmas, de nagyobb governance-fegyelmet igényel | 

Data Lakehouse | 
hibrid | 
a Data Lake rugalmassága + az adattárház strukturáltsága és teljesítménye | 

A három architektúra közötti technikai különbségek részletes bemutatása az Üzleti Informatikai Alkalmazások tárgy "Big Data és prediktív analitika" előadásában található.

Forrás: Tick, A. Big data — saját előadásanyag.

## 4. Feldolgozási paradigmák

(forrás: 8.15.html)

### 4. Feldolgozási paradigmák

## Batch vagy stream?

### Feldolgozási paradigmák

A Big Data feldolgozása két alapvető paradigma szerint történhet:

Batch feldolgozás — az adatokat nagyobb kötegekben, meghatározott időközönként dolgozzák fel (pl. éjszakai futtatás). Jól skálázható, de nem ad azonnali választ.

Stream processing (folyamfeldolgozás) — az adatokat érkezésükkor, valós időben dolgozzák fel; ez szükséges a Kötelező Könyv edge computing-alkalmazásaihoz (pl. azonnali anomáliadetektálás).

E két paradigma egységes rendszerbe foglalására két architekturális megoldás terjedt el:

Architektúra | 
Lényeg | 
Hátránya / előnye | 

Lambda | 
külön batch- és speed-réteg, egy serving-réteg egyesíti | 
az üzleti logikát kétszer kell implementálni | 

Kappa | 
egyszerűsítés — minden feldolgozás streaming-alapon | 
egyszerűbb, de mindig streaming-infrastruktúrát igényel | 

A két architektúra részletes működése az Üzleti Informatikai Alkalmazások tárgy "Big Data és prediktív analitika" előadásában található.

Forrás: Tick, A. Big data — saját előadásanyag.

## 5. Big Data technológiai ökoszisztéma

(forrás: 8.16.html)

### 5. Big Data technológiai ökoszisztéma

## Hadoop, NoSQL, Spark

### Big Data-technológiai ökoszisztéma — rövid áttekintés

Technológia | 
Szerepe | 

Hadoop (HDFS, MapReduce, YARN) | 
Elosztott fájlrendszer és feldolgozási keretrendszer nagy adathalmazok tárolására és kötegelt elemzésére | 

NoSQL adatbázisok | 
Dokumentum-orientált (pl. MongoDB), kulcs-érték (pl. Redis), oszlopcentrikus (pl. Cassandra) és gráf-adatbázisok (pl. Neo4j) — rugalmas séma, nagy skálázhatóság | 

Apache Spark | 
Memóriaalapú feldolgozás, jelentősen gyorsabb a hagyományos MapReduce-nál, alkalmas gépi tanulási munkafolyamatokra is | 

A technológiák részletes működése, előnyei és korlátai az Üzleti Informatikai Alkalmazások tárgy "Big Data és prediktív analitika" előadásában olvashatók.

Forrás: Tick, A. Big data — saját előadásanyag.

## 6. Prediktív modellek értékelési mutatói

(forrás: 8.17.html)

### 6. Prediktív modellek értékelési mutatói

## Mennyire jó egy előrejelzés?

### Prediktív modellek értékelési mutatói — fogalmi felidézés

A prediktív modellek teljesítményét leggyakrabban a következő hibametrikákkal mérik:

Mutató | 
Mit fejez ki | 

MAE (Mean Absolute Error) | 
az előrejelzett és a valós értékek közötti abszolút eltérések átlaga — az eredeti adat egységében fejezi ki a hibát | 

MAPE (Mean Absolute Percentage Error) | 
a hibát százalékos formában fejezi ki, ami megkönnyíti eltérő nagyságrendű előrejelzések összehasonlítását | 

RMSE (Root Mean Squared Error) | 
nagyobb súlyt ad a nagy hibáknak, ezért hasznos, ha a kiugró tévedések különösen károsak | 

A modellezés két tipikus buktatója a túlillesztés (a modell "megjegyzi" a tréningadatot, de rosszul általánosít) és az alulillesztés (a modell túl egyszerű ahhoz, hogy megragadja az adatban rejlő mintázatokat). Ezek kockázatát a keresztvalidálás csökkenti.

A metrikák pontos képletei és számítási példái az Üzleti Informatikai Alkalmazások tárgy "Big Data és prediktív analitika" előadásában megtalálhatók.

Forrás: Tick, A. Big data — saját előadásanyag.

## 7. Rendszerszemléletű modellezés

(forrás: 8.18.html)

### 7. Rendszerszemléletű modellezés

## Amikor a lineáris előrejelzés félrevezet

### Rendszerszemléletű modellezés — rövid felidézés

A komplex üzleti rendszerek (pl. ellátási láncok) modellezésénél a lineáris előrejelzés gyakran félrevezető, mert nem veszi figyelembe a visszacsatolásokat.

Bullwhip-effektus (ostor-hatás)

Ennek klasszikus példája a bullwhip-effektus, amellyel már a 3. fejezetben (ERP/SCM) találkoztunk: egy kis kereslet-ingadozás az ellátási lánc mentén felfelé haladva egyre nagyobb készlet-ingadozássá erősödik.

A rendszerszemléletű modellezés (pl. szimulációs szoftverekkel) ezekre a visszacsatolásokra, késleltetésekre és nem-lineáris hatásokra is választ ad, szemben az egyszerű, egyváltozós előrejelzési modellekkel.

A bullwhip-effektus és a rendszerszemléletű szimuláció részletes bemutatása (esettanulmánnyal illusztrálva) az Üzleti Informatikai Alkalmazások tárgy "Big Data és prediktív analitika" előadásában található.

Forrás: Tick, A. Big data — saját előadásanyag.
