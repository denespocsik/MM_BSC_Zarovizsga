# 4. előadás: 4. előadás Mit ér az adat és ki felelős érte? - Kötelező tananyag

## 1. Nyitó dilemma — Knight Capital, 2012

(forrás: 4.1.html)

### 1. Nyitó dilemma — Knight Capital, 2012

## Mit ér az adat és ki felelős érte?

### Nyitó dilemma — Knight Capital, 2012

[kép]

Ábra: tőzsdei kereskedési terem ésalgoritmikus kereskedés

🔴 Döntés előtt — Ön az IT-igazgató

2012. augusztus 1., New York. Ön a Knight Capital Group — az egyik legnagyobb amerikai tőzsdei kereskedő cég — informatikai igazgatója. A csapata az éjszaka folyamán egy új kereskedési algoritmust telepített nyolc szerverre. Reggel 9:30-kor megnyílik a piac.

Hét szerverre sikeresen felkerült az új kód. A nyolcadik szerveren azonban egy 2003 óta használaton kívüli, elfeledett funkció ("Power Peg") aktiválódott újra — egy régi, ott felejtett kódrészlet miatt. A rendszer ettől kezdve úgy viselkedett, mintha minden szerver ugyanazt a logikát futtatná — pedig nem így volt.

45 perc alatt a hibás szerver 154 részvényben, 397 millió darab részvényt érintő, 4 millió tranzakciót hajtott végre — vásárolt drágán, eladott olcsón, gazdaságilag értelmetlen mintázatban. Mire a csapat rájött, mi történik, és leállította a rendszert, a veszteség 440 millió dollár volt. A cég részvényárfolyama két nap alatt 75%-ot esett, és végül felvásárolták.

Kérdés, mielőtt tovább olvasna:

- Hogyan lehetséges, hogy egy cég nem tudja biztosan, mi fut a saját szerverein?

- Mi az, ami miatt senki nem vette észre azonnal, hogy valami nincs rendben?

- Ha Ön lett volna az IT-igazgató, mit tett volna másképp — azelőtt, hogy ez megtörtént?

Ezt a dilemmát a fejezet 7. oldalán oldjuk fel részletesen — beleértve azt is, hogy pontosan mit jelent a "single source of truth" hiánya, és mi történik, ha egy szervezet ezt jól oldja meg.

💡 Tanulási eredmények

A fejezet elvégzése után Ön képes:

- elhelyezni egy adatminőségi problémát a DIKW-lánc megfelelő pontján, és azonosítani, hol "törik el" a lánc

- értékelni az adatminőség valós pénzügyi kockázatát vállalati példákkal alátámasztva

- megkülönböztetni az OLTP és OLAP rendszerek célját és jellemzőit

- megmagyarázni, miért menedzseri, nem IT-feladat az adattárház/adatpiac kialakítása

- azonosítani a data governance-ért felelős szerepköröket (CIO, CSO, CPO, CKO, CDO) és feladataikat

- alkalmazni a "single source of truth" elvét mint döntési logikát valós vállalati helyzetekben — nagyvállalati és KKV-léptékben egyaránt

📚 A fejezet térképe

2. oldal: DIKW mint diagnosztikai lánc → 3. oldal: az adatminőség mint pénzügyi kockázat → 4. oldal: OLTP vs. OLAP → 5. oldal: adattárház/adatpiac (Société Générale) → 6. oldal: data governance és a CDO → 7. oldal: "single source of truth" — vissza Knight Capitalhoz + Siemens Amberg → 8. oldal: hazai kitekintő — Bosch és a magyar KKV-valóság.

Forrás: SEC Order — Knight Capital; Henrico Dolfing esettanulmány (részletes hivatkozások a 7. oldalon)

## 2. A DIKW-lánc: hol törik el?

(forrás: 4.2.html)

### 2. A DIKW-lánc: hol törik el?

## A DIKW-lánc: hol törik el?

### Nem definíció — diagnózis

A DIKW-modellt (adat → információ → tudás → bölcsesség) valószínűleg már ismeri egy korábbi tárgyból. Ez a fejezet nem a fogalmakat definiálja újra, hanem egy diagnosztikai eszközként használja: minden komoly IT-katasztrófa mögött megtalálható, hogy a lánc melyik pontján szakadt meg a megbízható átmenet.
[kép]

Ábra: DIKW

A Knight Capital-eset a DIKW-lánc mentén:

Szint | 
Mi történt a Knight Capital-esetben | 

Adat | 
A 8. szerveren lévő kód-állapot eltért a többi hét szerverétől — ez már itt "rossz adat" volt: a rendszer állapotáról szóló tény nem egyezett a valósággal | 

Információ | 
Senki nem alakította ezt az eltérést látható, értelmezhető információvá — nem volt automatikus riasztás arról, hogy "a 8. szerver más kódot futtat, mint a többi" | 

Tudás | 
Még ha lett volna is riasztás, a csapatnak fel kellett volna ismernie, hogy ez kritikus, nem apró eltérés — ehhez kontextus és tapasztalat kell | 

Bölcsesség | 
A megfelelő döntés — azonnali leállítás — csak akkor születhetett volna meg időben, ha az előző három szint mind működik. Knight Capitalnál ez 45 percig nem történt meg | 

A tanulság: a bölcsesség szintjén hozott rossz döntés szinte mindig egy korábbi, észrevétlen töréspontra vezethető vissza — leggyakrabban az adat→információ átmenetre, ahol a nyers tény nem alakul át időben látható, cselekvésre ösztönző jelzéssé.

💡 Műszaki analógia

Gondoljon a DIKW-láncra úgy, mint egy érzékelő-jelfeldolgozó láncra egy ipari vezérlőrendszerben: az érzékelő adatot mér (adat), a jelfeldolgozó egység ezt értelmezhető mértékegységgé alakítja (információ), a vezérlőalgoritmus felismeri, hogy ez a mérték kritikus tartományban van-e (tudás), és ez alapján avatkozik be vagy riaszt (bölcsesség). Ha bármelyik lépés kimarad vagy hibás — pl. az érzékelő jó adatot küld, de a vezérlő nem ismeri fel a kritikus tartományt —, a rendszer katasztrofálisan viselkedhet, még ha az eredeti adat teljesen helyes volt is.

🤔 Reflektív kérdés

Gondoljon egy helyzetre a saját munkahelyén, amikor egy probléma "tudati" szinten (felismerésben) csúszott el, annak ellenére, hogy az alapadat rendelkezésre állt. Mi hiányzott — a riasztás, a kontextus, vagy a döntéshozatali jogkör?

Forrás: SEC Order — Knight Capital

## 3. Az adatminőség mint pénzügyi kockázat

(forrás: 4.3.html)

### 3. Az adatminőség mint pénzügyi kockázat

## Az adatminőség mint pénzügyi kockázat

### Nem csak a Knight Capital — ez rendszerszintű probléma

[kép]

Ábra: A probléma nem múlt el, csak mérete változott

📊 Kemény számok

- Az IBM 2016-os, azóta is széles körben idézett becslése szerint a rossz adatminőség évente 3,1 billió dollárba kerül az amerikai gazdaságnak — ez akkoriban az amerikai GDP kb. 18%-a volt

- A 2025-ös IBM Institute for Business Value jelentés szerint a vállalati adatvezetők (COO-k) 43%-a az adatminőséget nevezi meg legfontosabb adatpriorításként

- A szervezetek több mint negyede évi 5 millió dollár feletti veszteséget becsül az adatminőségi problémákból, 7%-uk 25 millió dollár felettit

Ez azt jelenti: a Knight Capital nem egy egyedi rémtörténet, hanem egy szélsőséges, de tipikus példája egy folyamatosan jelenlévő kockázatnak.

#### Honnan ered technikailag a rossz adatminőség?

[kép]

Ábra: Hagyományos fájlkörnyezet vs Relációs adatbázis"

A hagyományos, fájlalapú rendszerkörnyezetben (amikor minden részleg saját fájljait kezeli, egymástól függetlenül) négy jellegzetes probléma jelentkezik:

Probléma | 
Mit jelent | 

Adatredundancia | 
Ugyanaz az adat (pl. egy ügyfél neve) több helyen, eltérő formában tárolva | 

Adatinkonzisztencia | 
Ugyanannak az adatnak eltérő értékei a különböző rendszerekben (pl. "M" vs. "medium" méretkód) | 

Program-adat függőség | 
A programkód szorosan összefonódik az adat fizikai elrendezésével — egy apró változtatás az adatszerkezetben az összes hozzá kapcsolódó programot elronthatja | 

Korlátozott adatmegosztás | 
Az egyes részlegek nem férnek hozzá egymás adataihoz, még ha szükségük lenne is rá | 

A válasz: a relációs adatbázis. Ahelyett, hogy minden alkalmazás saját fájlt kezelne, a relációs adatbázis egyetlen, közös, logikailag rendezett adatállományt biztosít, ahol minden adatelemnek egyetlen, azonosítható helye van (kulcsmező), és a kapcsolódó adatok összekapcsolhatók anélkül, hogy másolniuk kellene egymást. Ez alapvetően, technikai szinten oldja meg a fenti négy problémát — nem szünteti meg az adatminőségi kockázatot, de megteremti az alapfeltételét annak, hogy egyáltalán kezelhető legyen.

🤔 Menedzseri kérdés

Ha az Ön szervezeténél 25%-kal csökkenne az adatminőségi hibák száma, melyik üzleti területen (pénzügy, ügyfélkapcsolat, termelés) várná a legnagyobb, mérhető hatást — és miért?

Forrás: IBM (2016, Thomas C. Redman/HBR); IBM Institute for Business Value (2025); Laudon Ch.6

## 4. OLTP vs. OLAP

(forrás: 4.4.html)

### 4. OLTP vs. OLAP

## OLTP vs. OLAP: különböző kérdések, különböző rendszerek

### Két teljesen más logika

Amikor adatról beszélünk, fontos különbséget tenni: más rendszer kell ahhoz, hogy egy tranzakciót rögzítsünk, mint ahhoz, hogy trendeket elemezzünk belőle.
[kép]

Ábra: OLTP vs OLAP

Tulajdonság | 
OLTP (Online Transaction Processing) | 
OLAP (Online Analytical Processing) | 

Felhasználó | 
ügyintéző | 
elemző | 

Használat | 
rendszeresen ismétlődő | 
alkalmi | 

Adatok | 
naprakész, aktuális állapot | 
történeti, archivált | 

Összegzés szintje | 
nagyon részletes | 
összesített | 

Elérés | 
írás/olvasás | 
főleg olvasás | 

Elért rekordszám | 
tízes nagyságrend | 
milliós nagyságrend | 

Adatbázis szerkezete | 
relációs | 
csillag vagy hópehely séma | 

Teljesítménymutató | 
tranzakciós idő | 
lekérdezési idő | 

Funkció | 
operatív feldolgozás | 
döntéstámogatás | 

Ezt a különbséget újabban a FASMI (Fast Analysis of Shared Multidimensional Information) betűszóval szokták összefoglalni az OLAP elvárásaira: gyors, megosztott, többdimenziós, elemzésre optimalizált hozzáférés.

💡 Műszaki analógia

Gondoljon az OLTP-re úgy, mint egy gyártósor valós idejű PLC-vezérlésére — minden másodpercben pontos, aktuális állapotot kell rögzítenie és azonnal reagálnia. Az OLAP ezzel szemben olyan, mint a havi termelési riport elemzése: nem érdekel, mi történt pontosan 14:03:12-kor egy adott szenzorral, hanem az, hogy milyen trend rajzolódik ki hetek, hónapok alatt. Ha valaki megpróbálná az OLTP-rendszeren futtatni az OLAP-jellegű, milliós rekordokat összesítő lekérdezéseket, az lelassítaná vagy leállítaná a napi működést — pontosan ezért kell a kettőt külön rendszerben tartani.

✨ Előretekintés

Érdemes megjegyezni: a big data és az AI szoros kölcsönhatásban állnak egymással — az AI-modellek betanításához hatalmas mennyiségű adatra van szükség, a gépi tanulás pedig a big data-ból nyert információt használja fel értékesebb üzleti meglátások előállítására. Ezt a kapcsolatot a Big Data-fejezetben (8. fejezet) dolgozzuk fel részletesen.

Forrás: (OLTP/OLAP táblázat, FASMI-kritériumok)

## 5. Adattárház és adatpiac

(forrás: 4.5.html)

### 5. Adattárház és adatpiac

## Adattárház és adatpiac: menedzseri infrastruktúra, nem IT-projekt

### Miért nem elég "megvenni egy szoftvert"?

Az adattárház (data warehouse) és a kisebb, területspecifikus adatpiac (data mart) technikailag "csak" egy nagy, elemzésre optimalizált adatbázis. A valóságban azonban a sikeres kialakításuk elsősorban menedzseri, nem technikai kihívás — az alábbi valós eset pontosan ezt mutatja be.

Mi a különbség a kettő között?

Az adattárház a teljes vállalat összes releváns adatát egyesíti — minden részleg, minden funkcionális terület adatai egy helyen, hosszú távú, elemzésre optimalizált formában. Az adatpiac ennek egy kisebb, célzott alegysége: csak egyetlen üzleti terület (pl. csak az értékesítés, vagy csak a HR) adatait tartalmazza, ezért gyorsabban felépíthető és olcsóbb, mint egy teljes adattárház — cserébe szűkebb rálátást ad.

[kép]

Ábra: a Société Générale-eset

🏦 Valós eset: Société Générale

A Société Générale — Franciaország legnagyobb, az EU harmadik legnagyobb bankja, 76 országban, 33+ millió ügyféllel — naponta tízmillió tranzakciót generál, több mint 1500 fájlban tárolva, mielőtt ezek frissítenék a fő adatbázisokat.

A probléma: mielőtt ezek az adatok a fő rendszerekbe kerülnének, ellenőrizni kell őket — mert az adat gyakran "koszos": a rekordszámok és összegek megváltozhatnak, ahogy az adat rendszerek között áramlik, duplikált fájlok keletkeznek, vagy hiányzó/rossz sorrendű fájlok downstream alkalmazások leállásához vezetnek.

A régi megoldás: több száz alkalmazott manuálisan ellenőrizte a fájlokat. Az új megoldás egy "intelligens rendszer" (Infogix platform) volt — de ennek a lényege nem a szoftver volt, hanem az, hogy a bank vezetése explicit módon fel kellett térképezze és kodifikálja azt a 220+ üzleti szabályt, amit az alkalmazottai évek tapasztalatából alakítottak ki. Csak ezután lehetett ezeket a szabályokat automatizálni.

A tanulság: az adattárház/adatpiac sikere nem azon múlik, milyen szoftvert vásárolnak, hanem azon, hogy a vezetés fel tudja-e térképezni és tudatosítani a saját szervezeti tudását az adatokról — ez menedzseri feladat, amit semmilyen technológia nem helyettesíthet.

Forrás: Laudon Ch.6, "Interactive Session: Management — Societe Generale Builds an Intelligent System to Manage Information Flow"

## 6. Data governance és a CDO szerepe

(forrás: 4.6.html)

### 6. Data governance és a CDO szerepe

## Data governance és a CDO szerepe

### Ki felelős az adatért a vállalatnál?

Ahogy egy vállalat mérete és adatmennyisége nő, egyre világosabbá válik, hogy valakinek felelősséget kell vállalnia a vállalati adatvagyonért — nem lehet minden részleg saját belátása szerint kezelje a saját adatait.

[kép]

Ábra helye: CIO szerepe és felelőssége

A vezetői szerepkörök, amelyek ma egy nagyvállalatnál a CIO mellett dolgoznak:

Szerepkör | 
Felelősségi terület | 

CIO (Chief Information Officer) | 
az IT-stratégia egésze, a technológia integrálása az üzleti stratégiába | 

CSO/CISO (Chief Security Officer) | 
információbiztonsági szabályzat kikényszerítése, biztonsági fenyegetések kezelése | 

CPO (Chief Privacy Officer) | 
adatvédelmi jogszabályoknak való megfelelés | 

CKO (Chief Knowledge Officer) | 
a vállalati tudásmenedzsment-program | 

CDO (Chief Data Officer) | 
a vállalati szintű adatirányítás és -hasznosítás, hogy a szervezet a lehető legtöbb értéket nyerje ki az adataiból | 

A CDO szerepköre viszonylag új — pontosan azért jött létre, mert a szervezetek egyre nagyobb mennyiségű adatot gyűjtenek és állítanak elő, és valakinek biztosítania kell, hogy (1) a megfelelő adatot gyűjtik, (2) a megfelelő technológiákkal elemzik, és (3) az eredményeket ténylegesen felhasználják üzleti döntésekhez.

🤔 Reflektív kérdés

Gondolja végig a saját szervezetét (vagy egy korábbi munkahelyét): van-e valaki, aki explicit módon felelős az adatminőségért és az adatirányításért — vagy ez "mindenkié és senkié"? Mi történne, ha holnaptól kineveznének egy CDO-t — mi lenne az első három dolog, amit tennie kellene?

Forrás: Laudon Ch.2, Ch.6 (CDO fogalma és szerepköre)

## 7. "Single source of truth" mint döntési logika

(forrás: 4.7.html)

### 7. "Single source of truth" mint döntési logika

## "Single source of truth" mint döntési logika

### Vissza a nyitó dilemmához

Az 1. oldalon feltett kérdésre — hogyan lehetséges, hogy egy cég nem tudja biztosan, mi fut a saját szerverein — most már pontos válasz adható: a Knight Capital esetében nem volt "single source of truth" — nem volt egyetlen, megbízhatóan ellenőrzött hely, ahol valaki biztosan tudhatta volna, hogy mind a nyolc szerver ugyanazt a kódot futtatja. A csapat 20 percen át tévesen azt hitte, hogy a probléma forrása egy másik szerver — és ez alatt az idő alatt rontott a helyzeten, mert az elavult kódot minden szerverre visszaállította.
[kép]

Ábra: Knight Capital vs Siemens Amberg

✅ Az ellenpélda: Siemens Amberg (Németország)

A Siemens Amberg-gyár (Electronic Works Amberg) a világ egyik legismertebb "digitális gyára" — évi 6 millió SIMATIC automatizálási terméket gyárt, 1200 termékváltozatban, napi 350 átállással a gyártósorokon. Naponta kb. 50 millió darab folyamatadat keletkezik — és ez a hatalmas adatmennyiség egyetlen, közös adatmodellben él, amelyben minden gép és termék "kommunikál" egymással.

Az eredmény: 99,99885%-os minőségi mutató (kb. 11 hibás darab millióként). 2025–2026-ban a gyár egy lépéssel tovább ment: mesterséges intelligencia-alapú minőségellenőrzést vezettek be, amivel elkerültek egy 500 000 eurós beruházást egy röntgenalapú vizsgálóberendezésre — mert a megfelelően strukturált, megbízható adat helyettesíteni tudta a drága fizikai ellenőrzést.

A közös elv mindkét esetben: amikor egy szervezet egyetlen, megbízhatóan karbantartott, mindenki által ugyanúgy látott adatforrásra támaszkodik, a döntések (legyen szó kereskedési algoritmusról vagy gyártósori minőségellenőrzésről) gyorsak és pontosak lehetnek. Amikor ez hiányzik — mint Knight Capitalnál —, még a legjobb szándékú csapat is rossz irányba korrigál.

💡 Műszaki analógia

Ez pontosan az elosztott rendszerek konszenzus-problémája: ha egy rendszer több, egymástól függetlenül működő csomópontból (szerver, gép, adatbázis-példány) áll, valamilyen mechanizmusnak biztosítania kell, hogy mindegyik csomópont ugyanazt az állapotot lássa — különben a rendszer egyes részei ellentmondó információ alapján döntenek.

Forrás: SEC Order — Knight Capital; Henrico Dolfing esettanulmány; Siemens Amberg (Harvard Business School Case 518-054; Information Systems Journal, 2026)

## 8. Hazai kitekintő: két magyar valóság

(forrás: 4.8.html)

### 8. Hazai kitekintő: két magyar valóság

## Hazai kitekintő: két magyar valóság

### Ugyanaz a probléma, két különböző lépték

A Siemens Amberg lenyűgöző, de érdemes tudni: ugyanez a fajta adatvezérelt fejlesztés zajlik magyar gyárakban is — miközben a magyar vállalkozások túlnyomó többsége számára a valóság egészen más képet mutat.

[kép: 🇭🇺 Hungary Emoji | Flagpedia.net]  A) Amikor a nagyvállalat teszi jól: Bosch Hatvan — "Plant Digital Twin"

[kép]

Ábra: gyártósor/digitális iker illusztráció

A Robert Bosch Elektronika Kft. hatvani gyára 2025-ben vezette be a "Plant Digital Twin" (digitális iker) megoldást, amely valós idejű képet ad a teljes gyártási folyamatról — elektromos meghajtású járművekhez használt komponensek gyártásához kapcsolódóan. A projekt elnyerte a Gyártástrend magazin "Az Év Gyári Projektje" díját az ipari digitalizációs kategóriában.

A maklári gyár (Robert Bosch Automotive Steering Kft.) ugyanebben az évben AI-alapú minőségellenőrző rendszereket vezetett be, és több Shainin Dorian-díjat kapott a minőségfejlesztésért.

🏢 B) Amikor nincs CDO: az adatprobléma KKV-méretben

A Bosch-gyárak lenyűgözőek — de a magyar gazdaság gerincét nem a multinacionális nagyvállalatok, hanem a KKV-szektor adja. Mi történik itt?

Egy 2023-ban hazai KKV-k és mikrovállalkozások körében folytatott kérdőíves kutatás (2022: N=161, 2023: N=72 vállalkozás) megkérdezte: mi hátráltatja leginkább a digitális átállásukat?
[kép]

Ábra: KKV-k digitális átalakulása - hátráltató tényezők

A válasz mindkét évben ugyanaz volt — és nem a pénz, nem a technológia, nem is a digitális készségek hiánya állt az élen:

Hátráltató tényező | 
2022 | 
2023 | 

Információhiány | 
3,36 (1. hely) | 
3,14 (1. hely) | 

Szakképzett munkaerő hiánya | 
3,27 | 
2,90 | 

Pénzügyi problémák | 
3,18 | 
3,12 | 

Technológiai hiányosságok | 
3,01 | 
2,94 | 

Digitális készségek hiánya | 
2,61 | 
2,47 | 

(1–5 skála, ahol 1 = egyáltalán nem hátráltató)

A kutatók szó szerint megfogalmazzák a lényeget: "nem elegendő csupán a készség vagy a digitális infrastruktúra megléte — azt jól kell tudni használni, illetve alkalmazni is." Vagyis a magyar KKV-k saját magukat a probléma gyökereként pontosan azt nevezték meg, amiről ez a fejezet szól: nem az eszköz hiányzik, hanem a megbízható, időben rendelkezésre álló információ.

Egy további érdekes eredmény: a kutatás statisztikailag igazolta (ANOVA, sig=0,915), hogy a vállalkozás mérete nem befolyásolja szignifikánsan az információhiány súlyosságát — ez tehát nem csak a legkisebb mikrovállalkozásokat érinti, hanem egyformán minden KKV-t.

Mit jelent a governance KKV-méretben, ha nincs CDO? Nem egy szerepkör kell, hanem egy tudatos döntés: valaki (a tulajdonos, egy irodavezető) explicit módon felelős legyen az adatokért, és a szervezet egyetlen közös, megbízható adatforrásra álljon át a szétszórt táblázatok és papíralapú nyilvántartás helyett — ugyanaz a "single source of truth" elv, amit a 7. oldalon láttunk, csak nulla CDO-büdzséből megvalósítva.

🤔 Záró gondolkodtató kérdés

Gondoljon a saját szervezetére (vagy egy jövőbeli munkahelyére): ha valakit megkérdeznének, mi hátráltatja leginkább a napi működést, vajon Önöknél is az "információhiány" lenne az első helyen — vagy valami más? Mit jelentene ez a felismerés a gyakorlatban, ha Ön lenne a döntéshozó?

Forrás: Garai-Fodor, Varga, Csiszárik-Kocsir (2023). "A digitális átállás nehézségei és a magyar KKV-szektorban alkalmazott megoldások." Vállalkozásfejlesztés a XXI. században, 2023/1., Óbudai Egyetem KGK; Technokrata.hu (2026, Bosch Magyarország)

## 9. Elmélyítő Kiegészítő

(forrás: 4.9.html)

### 9. Elmélyítő Kiegészítő

Turban, E., Pollard, C., & Wood, G. (2023). Information Technology for Management: Driving Digital Transformation to Increase Local and Global Performance, Growth and Sustainability (12th ed.). Wiley.
A könyv 3. fejezete — "Data Management, Data Warehouses, and Data Governance" — szó szerint ugyanazt a témát dolgozza fel, mint a mi 4. fejezetünk. Jó kiegészítő olvasmány azoknak, akik a Laudon mellett egy másik szemszögből is át szeretnék tekinteni ugyanezt az anyagot — ez a könyv szerepelt eredetileg is a tárgy ajánlott szakirodalmában.

Xiao, J., Ding, H., & Zhang, H. (2024). How chief data officers promote data-driven innovation: an empirical investigation. European Journal of Innovation Management, ahead-of-print. DOI: 10.1108/EJIM-12-2023-1046
261 CDO bevonásával készült kérdőíves kutatás — azt vizsgálja, hogyan (nem csak mit) csinálnak a CDO-k, hogy adatvezérelt innovációt segítsenek elő a szervezetükben. Közvetlenül kapcsolódik a 6. oldal CDO-témájához, és túlmutat a Laudon-tankönyv alapszintű szerepkör-leírásán.

IBM Institute for Business Value & Oxford Economics (2023). Turning data into value: How top Chief Data Officers deliver outsize results while spending less.
Nagymintás felmérés arról, mit csinálnak másképp a legsikeresebb CDO-k — konkrét, gyakorlati adatokkal (pl. hogy az adatbiztonság a CDO-k 52%-a szerint még mindig a legkritikusabb felelősség). Jó, gyakorlatias kiegészítés a 6. oldal elméleti CDO-bemutatása mellé.

Tick, A. (2023). Industry 4.0 narratives through the eyes of SMEs in V4 countries, Serbia and Bulgaria. Acta Polytechnica Hungarica, 20(2), 83–104. DOI: 10.12700/APH.20.2.2023.2.5
A V4-országok (köztük Magyarország), Szerbia és Bulgária KKV-inak Ipar 4.0-hoz való viszonyulását, "narratíváit" vizsgálja — 47 független idéző közleménnyel. Közvetlenül elmélyíti a 8. oldal hazai KKV-témáját.

Garai-Fodor, M., Varga, J., & Csiszárik-Kocsir, Á. (2023). A digitális átállás nehézségei és a magyar KKV-szektorban alkalmazott megoldások. Vállalkozásfejlesztés a XXI. században, 2023/1., Óbudai Egyetem KGK.

## 1. Mi az a DIKW-lánc?

(forrás: 4.10.html)

### 1. Mi az a DIKW-lánc?

## Mit ér az adat és ki felelős érte? — fogalmi alapok

### 1. Mi az a DIKW-lánc?

A DIKW egy egyszerű modell arra, hogyan alakul a nyers tény egyre használhatóbb tudássá:
[kép]

Ábra:  Adat, Információ, Tudás, Bölcsesség

Adat | 
egy nyers tény vagy szám, önmagában — pl. "37" | 

Információ | 
az adat kontextusban — pl. "37°C-os testhőmérséklet" | 

Tudás | 
annak felismerése, hogy ez mit jelent — pl. "ez normális testhőmérséklet, nincs láz" | 

Bölcsesség | 
a helyes döntés meghozatala ez alapján — pl. "nem kell orvoshoz menni" | 

A fejezet Kötelező Könyve ezt a modellt arra használja, hogy megmutassa: egy rossz üzleti döntés mögött szinte mindig egy korábbi, észrevétlen hiba áll — valahol a láncban elromlik valami, mielőtt a döntéshez érnénk.

## 2. Miért számít az adatminőség?

(forrás: 4.11.html)

### 2. Miért számít az adatminőség?

### 2. Miért számít az adatminőség?

Képzeljünk el egy egyszerű helyzetet: egy webshopban a raktárkészlet-adat szerint van 50 darab egy termékből, de a valóságban csak 10 van. Ez az eltérés rossz adatminőség — és minden ebből fakadó döntés (pl. hogy hány rendelést fogadjunk el) hibás lesz.
[kép]

Honnan ered a rossz adatminőség? Leggyakrabban abból, hogy több rendszer külön-külön, egymástól függetlenül tárolja ugyanazt az adatot — és ezek idővel elkezdenek eltérni egymástól. Ezt hívjuk adatredundanciának és adatinkonzisztenciának.

A Kötelező Könyvben bemutatott Knight Capital-eset egy szélsőséges példa erre: egy apró eltérés (a szerverek nem ugyanazt a kódot futtatták) 45 perc alatt 440 millió dolláros veszteséghez vezetett.

Forrás: Laudon Ch.6, saját összefoglalás

## 3. OLTP vs. OLAP — mi a különbség?

(forrás: 4.12.html)

### 3. OLTP vs. OLAP — mi a különbség?

### 3. OLTP vs. OLAP — mi a különbség?

Két teljesen más célra használunk adatrendszereket:

OLTP

a napi működést rögzíti — pl. amikor egy pénztárgép beüti egy vásárlás adatait. Sok, gyors, apró művelet.

OLAP

a felhalmozott adatot elemzi — pl. amikor megnézzük, hogyan alakult a havi forgalom. Kevesebb, de nagyobb, összetettebb lekérdezés.

[kép]

Ábra: OLTP vs OLAP

Egy egyszerű hüvelykujjszabály: ha a kérdés "mi történt most?" — az OLTP. Ha a kérdés "mi történt az elmúlt fél évben, és mi a trend?" — az OLAP.

Forrás: EA3 saját előadásanyag

## 4. Adattárház és adatpiac egyszerűen

(forrás: 4.13.html)

### 4. Adattárház és adatpiac egyszerűen

### 4. Adattárház és adatpiac egyszerűen

Amikor egy vállalatnak sok, különböző rendszerből származó adata van, és ezt mind egy helyen szeretné elemezni, két megoldás közül választhat:

- Adattárház (data warehouse): a teljes vállalat összes adata egy helyen — nagy, átfogó, de drágább és lassabb felépíteni

- Adatpiac (data mart): csak egy terület (pl. csak az értékesítés) adatai — kisebb, olcsóbb, gyorsabban elkészül

[kép]

Ábra : Adattárház és adatpiacok: Értékesítés, HR, Pénzügy]

A Kötelező Könyvben bemutatott Société Générale-eset jól mutatja: nem elég megvenni egy ilyen rendszert — a vállalatnak előbb tudnia kell, milyen szabályok szerint szeretné rendezni és ellenőrizni az adatait.

Forrás: Laudon Ch.6

## 5. Ki felelős az adatért?

(forrás: 4.14.html)

### 5. Ki felelős az adatért?

### 5. Ki felelős az adatért?

Minél nagyobb egy vállalat, annál fontosabb, hogy valaki egyértelműen felelős legyen az adatokért — ne legyen "mindenkié és senkié" a kérdés.

A nagyvállalatoknál ma már gyakran külön szerepkör foglalkozik ezzel: a CDO (Chief Data Officer), akinek a feladata, hogy a vállalat a lehető legtöbb értéket nyerje ki az adataiból — biztosítva, hogy a megfelelő adatot gyűjtsék, jól elemezzék, és ténylegesen fel is használják döntésekhez.

[kép]

Ábra: Ki a felelős? 

Kisebb vállalatoknál nincs erre külön szerepkör — de az alapelv ugyanaz: valakinek tudatosan felelősséget kell vállalnia az adatokért, még ha ez "csak" annyit jelent, hogy egy közös, megbízható rendszerre állnak át a szétszórt táblázatok helyett.

Forrás: Laudon Ch.2, Ch.6
