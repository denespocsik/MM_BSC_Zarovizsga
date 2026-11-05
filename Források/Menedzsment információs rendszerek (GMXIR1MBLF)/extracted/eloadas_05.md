# 5. előadás: 5.előadás  Üzleti intelligencia: kultúra, nem eszköz - Kötelező tananyag

## 1. Nyitó dilemma

(forrás: 5.1.html)

### 1. Nyitó dilemma

## Üzleti intelligencia: kultúra és stratégia

### Nyitó dilemma

🔴 Döntés előtt — Ön a cég ügyvezetője

Egy középvállalat ügyvezetőjeként tavaly 50 millió forintot fektetett be egy vadonatúj Power BI-alapú vezetői információs rendszerbe. A rendszer működik, a dashboardok szépek, a riportok pontosak. Hat hónappal a bevezetés után azonban azt tapasztalja: a középvezetők többsége továbbra is Excel-táblázatokban dolgozik, és csak akkor nyitják meg a Power BI-t, ha Ön kifejezetten rákérdez egy számra egy megbeszélésen.

Három versengő magyarázat lehetséges — melyik igaz?

Hipotézis | 
Mit jelentene | 

H1 — Felületi/képzési probléma | 
A rendszer túl bonyolult, a felhasználók nem kaptak elég képzést | 

H2 — Bizalmi probléma | 
A vezetők nem bíznak az adat forrásában vagy pontosságában | 

H3 — Koordinációs probléma | 
Nincs, aki felelős lenne a BI szervezeti bevezetéséért — a rendszer technikailag kész, szervezetileg nem | 

Ezt a három hipotézist a fejezet további oldalai sorban vizsgálják — a végleges diagnózist a 8. oldalon adjuk meg, konkrét indoklással, hogy melyik (vagy melyik kombináció) áll fenn ilyen esetekben leggyakrabban.

Kérdés, mielőtt tovább olvasna: Ön szerint melyik hipotézis a legvalószínűbb — és milyen konkrét jelet keresne a vállalatnál, hogy eldöntse, melyik igaz?

💡 Tanulási eredmények

A fejezet elvégzése után Ön képes:

- elhelyezni egy szervezetet a BI-érettségi modell szintjein, és azonosítani a strukturális/politikai okokat, amiért a legtöbb szervezet alacsony szinten reked

- kritikusan értékelni a self-service és az IT-centrikus BI-stratégia közötti feszültséget egy tágabb szervezetelméleti kereten (bimodális IT) keresztül

- megkülönböztetni a kognitív torzítást és az algoritmus-averziót mint két, egymással ellentétes döntéshozatali kockázatot

- elemezni, mely vezetői szerepeket támogat és melyeket nem támogat érdemben egy BI-rendszer

- többtényezős, oksági elemzést végezni egy valós BI-bukáson, versengő magyarázatokat mérlegelve

- diagnosztizálni egy valós szervezeti dilemmát a fejezet fogalmi eszközeivel

📚 A fejezet térképe

2. oldal: hol tart a szervezetünk, és ki koordinálja → 3. oldal: mitől jó az adat, és milyen döntéseket támogat → 4. oldal: kié legyen a BI → 5. oldal: miért torzít a legjobb vezető is → 6. oldal: mit támogat és mit nem támogat egy rendszer → 7. oldal: valós bukás, többtényezős elemzéssel → 8. oldal: mindez itthon — és a dilemma feloldása.

Forrás: saját dilemma, Laudon Ch.12 szellemében

## 2. BI-érettségi modell és a BICC

(forrás: 5.2.html)

### 2. BI-érettségi modell és a BICC

## Hol tart a szervezetünk — és ki koordinálja?

### BI-érettségi modell és a BICC

Egy széles körben használt öt szintű érettségi modell írja le, hol tarthat egy szervezet a BI-ban (Gartner): Unaware → Tactical → Focused → Strategic → Pervasive.

[kép]

Ábra: 5 lépcsős BI érettségi

Szint | 
Jellemző | 

Unaware | nincs formális BI-folyamat, mindenki a kéznél lévő eszközzel (Excel) dolgozik | 

Tactical | alkalmi elemzés, elszigetelt rendszerek és adatforrások | 

Focused | kidolgozott elemzési módszertan egyes területeken, adatpiacok jelennek meg | 

Strategic | egységes vállalati adattárház (EDW), prediktív technikák, a BI a tervezést is támogatja | 

Pervasive | BI-kompetenciaközpontok működnek, kollaboratív, adatvezérelt vállalati kultúra | 

📊 Megdöbbentő statisztika

Egy 2019-es felmérés szerint a szervezetek 87%-a még mindig az alsó két szinten (Unaware/Tactical) ragadt (Gartner).

A modell önmagában leíró — megmondja, hol tartunk, de nem magyarázza meg, miért nem lépünk tovább. A válasz jellemzően nem technikai, hanem strukturális: a Focused → Strategic átmenethez olyan szervezeti egység kell, amely átível a hagyományos siló-struktúrán. Ezt az egységet nevezik BI Kompetencia Központnak (BICC — Business Intelligence Competency Center).

A BICC — mit csinál, és mit nem

A BICC egy olyan szervezeti egység, amely a legmagasabb (Strategic/Pervasive) BI-érettségi szinten jelenik meg, és három kompetenciaterületet fog össze: üzleti kompetenciák (vízió, finanszírozás, prioritások), elemző kompetenciák (módszertan, szabványok, adatdefiníciók) és IT-kompetenciák (infrastruktúra, adatminőség, ETL). Fontos korlát: a BICC nem helyettesíti a döntéshozót — csak a döntéshozatali folyamatot támogatja.

Ha egy vállalat bevezeti a technológiát (Focused szint jellemzője), de nem hoz létre semmilyen koordináló egységet, aki felelős lenne a szabványokért és a bizalomépítésért, a szervezet technikailag éretlenebbnek tűnik, mint amilyen valójában — a probléma nem a szoftverrel van, hanem a hiányzó szervezeti híddal.

✨ AI — mikor automatizálódik a BI?

A legérettebb (Pervasive) szinten a BI túllép a leíró és prediktív elemzésen: preskriptív analitikává válik — a rendszer nemcsak megjósolja a jövőt, hanem konkrét cselekvést vagy döntést is javasol. Egy online lottószolgáltató (ZEAL Network) prediktív modelleket épített ügyféladatokból, hogy valós időben személyre szabja ajánlatait, és előre jelezze, mely ügyfelek válnak inaktívvá. Minél automatizáltabb a döntés, annál nagyobb a tét, ha a mögöttes adat vagy szervezeti bizalom hibás — ez köti össze ezt a fejezetet a 4. fejezet "single source of truth" témájával.

🤔 Reflektív kérdés

Gondolja végig a saját szervezetét: van-e olyan személy vagy csoport, aki explicit módon felel az adatszabványokért és a BI-koordinációért — vagy ez szét van szórva, esetleg senkié? Mi történne, ha holnaptól kineveznének egy BICC-felelőst?

Forrás: Gartner BI and Performance Management Maturity Model; Gartner BICC-modell

## 3. Mitől jó az adat, és milyen döntést támogat?

(forrás: 5.3.html)

### 3. Mitől jó az adat, és milyen döntést támogat?

## Mitől jó az adat, és milyen döntést támogat?

### Az adatminőség dimenziói döntéshozatali kontextusban

A 4. fejezetben már megismert adatminőségi problémák itt, döntéshozatali szemszögből térnek vissza. Az adatminőségnek hét jellemző dimenziója van (Laudon):

Dimenzió | 
Kérdés | 

Pontosság | Az adat a valóságot tükrözi? | 

Integritás | Az adatszerkezet és a kapcsolatok konzisztensek? | 

Konzisztencia | Az adatelemek egységesen vannak definiálva? | 

Teljesség | Minden szükséges adat rendelkezésre áll? | 

Érvényesség | Az értékek a megengedett tartományban vannak? | 

Időszerűség | Az adat akkor áll rendelkezésre, amikor kell? | 

Hozzáférhetőség | Az adat elérhető, érthető, használható? | 

💡 Műszaki kötődés

Egy gyártósori érzékelő-hálózatnál a hét dimenzió nem egyformán fontos. Egy vezérlőkörnél az időszerűség kritikus — egy másodperces késés balesetet vagy selejtet okozhat. Egy minőségbiztosítási jelentésnél a pontosság az elsődleges. Egy éves stratégiai riportnál a teljesség számít leginkább. Konkrét példa: egy CNC-gép hőmérséklet-érzékelője lehet tökéletesen pontos, mégis gyakorlatilag használhatatlan, ha 10 perces késéssel érkezik az adat a vezérlőrendszerbe — mire megérkezik, már megtörtént a szerszámtörés.

A dimenziók közötti trade-off: a hét dimenzió nem egyszerre optimalizálható. Minél gyorsabban (időszerűbben) akarunk adatot, jellemzően annál kevesebb validáció fér bele a folyamatba — tehát csökken a pontosság. Ez nem tervezési hiba, hanem tudatos döntés: egy valós idejű gyártási dashboard szándékosan elfogad kisebb pontossági kockázatot a sebességért cserébe, míg egy pénzügyi zárás fordítva dönt — inkább vár, de garantáltan pontos legyen.

#### Három döntéstípus, amit a BI-rendszer másképp szolgál ki

Strukturált döntés

pl. napi rendelési mennyiség → MIS, rutinjelentések

Félig strukturált döntés

pl. "mi történne, ha 5%-kal emelnénk az árat?" → DSS, what-if elemzés

Strukturálatlan döntés

pl. lépjünk-e be egy új piacra? → ESS, vezetői ítélőképesség

🤔 Reflektív kérdés

Gondoljon egy adatra a saját munkahelyén, amit rendszeresen használ egy döntéshez. Melyik a hét dimenzió közül, amelyik leggyakrabban sérül — és okozott-e ez már konkrét problémát? Volt-e olyan eset, amikor tudatosan feláldozták az egyik dimenziót a másikért (pl. gyorsaságot a pontosság rovására)?

Forrás: Laudon Ch.12 (Table 12.3)

## 4. Kié legyen a BI?

(forrás: 5.4.html)

### 4. Kié legyen a BI?

## Kié legyen a BI?

### Self-service vs. IT-centrikus BI

Két alapvetően eltérő filozófia létezik egy vállalati BI-rendszer üzemeltetésére:

IT-centrikus BI

az IT-osztály tervezi, építi és karbantartja a jelentéseket — megbízható, konzisztens, de lassú és rugalmatlan

Self-service BI

a felhasználók maguk építik jelentéseiket — gyors, rugalmas, de a konzisztencia és a "ki mit lát" kérdése bonyolultabbá válik

A self-service BI jellemzői (saját anyag):

- együttdolgozik a felhasználókkal, nem helyettük dolgozik

- kulcsadatok grafikus megjelenítése, figyelmeztetés, egy kattintásos lefúrás

- adatokban "gazdag": különböző forrásokból vegyített, aggregált és részletes, historikus és valós idejű adat

- felhatalmazott, beavatott dolgozók: a felhasználók a fontos dolgokra figyelhetnek, célokkal és versennyel motiválva, proaktívan

Ez a lista jól mutatja, hogy a self-service BI nem egyszerűen "kevesebb IT-kontroll", hanem egy tudatosan megtervezett felhasználói élmény — ha ez a négy jellemző hiányzik, a self-service BI könnyen inkonzisztenciához és "árnyék-IT"-hez vezet, ahogy az alábbi eset is mutatja.

A self-service vs. IT-centrikus vita egy tágabb, elismert szervezetelméleti keret konkrét esete: a bimodális IT koncepciója (Gartner). Mode 1 stabil, megbízhatóság-fókuszú, IT-vezérelt működést jelent; Mode 2 gyors, kísérletező, üzleti oldal által vezérelt működést. Ugyanez a mintázat jelenik meg minden gyors technológiai változásnál — pl. a felhőalapú infrastruktúra bevezetésénél is, amivel a 9. fejezetben találkozunk majd.

✅ Valós eset: Microsoft "Starlight/KPI Lake" belső BI-átalakítás

A Microsoft szervezeti kultúrája korábban arra ösztönözte az egyéneket, hogy teljes körűen "birtokolják" saját adataikat és elemzéseiket. Az eredmény: inkonzisztens adatdefiníciók régiónként, az elemzők idejük 75%-át adatgyűjtéssel töltötték, a jelentések 78%-a "offline környezetben" készült, és évi ~30 millió dolláros költség az "árnyék-alkalmazásokra". A megoldás egy "felügyelt önkiszolgáló BI" (Managed Self-Service BI) modell lett — nem visszatérés a tiszta IT-centrikus modellhez, hanem középút: közös adatszabványok, önkiszolgáló hozzáférés.

[kép]

Ábra: BI-felhasználók megoszlása — 80%+ alkalmi felhasználó (kész jelentések), felső vezetők (dashboard), középvezetők/elemzők ("power user", lekérdez és szeletel), Forrás: Laudon Fig. 12.4 logikája alapján
👔 Menedzseri kérdés — döntési szituáció

Ön egy 200 fős gyártó részleg vezetője. A csapata sürgeti, hogy mindenki önállóan építhessen Power BI-jelentést, mert az IT-osztály 3 hetes várólistával dolgozik. Ön engedélyezi — fél évvel később három különböző "hivatalos" selejt-arány kering a cégnél, mert mindenki máshogy számolja. Mi volt az Ön eredeti döntésének kockázata, amit nem mért fel? Mit tenne most — visszavonja az önkiszolgálást, vagy máshogy oldja meg?

🤔 Saját reflexió

Gondolja végig a saját (jelenlegi vagy egy korábbi) munkahelyét: ott inkább az IT-centrikus vagy az önkiszolgáló modell jellemző? Melyik probléma jelentkezett ebből — lassúság vagy inkonzisztencia? Ha Ön dönthetne, hol húzná meg a határt: mely jelentéseket szabványosítana központilag, és melyeket engedne szabadon?

Forrás: EA2 saját anyag; Microsoft Power BI hivatalos dokumentáció; Gartner bimodális IT-koncepció

## 5. Miért torzít a legjobb vezető is?

(forrás: 5.5.html)

### 5. Miért torzít a legjobb vezető is?

## Miért torzít a legjobb vezető is?

### A "Management Filters" jelenség

Még ha a BI-rendszer tökéletes, naprakész adatot szolgáltat is, a döntéshozó torzított szűrőkön keresztül dolgozza fel azt. Kognitív kutatások szerint (Kahneman, 2011; Tversky és Kahneman, 1986) az emberek — vezetők is — rosszul mérik fel a kockázatot, mintázatokat látnak ott is, ahol nincs, és megérzés, érzelem és a probléma "keretezése" alapján döntenek, nem tiszta empirikus adat alapján.

✅ Valós eset: Bear Stearns és Lehman Brothers, 2008

Ezek a Wall Street-i cégek azért omlottak össze, mert alábecsülték a komplex jelzálogpapírokba fektetett tőkéjük kockázatát. A kockázatkezelő modelljeik túl optimista feltételezésekre épültek — a rendszerek pontosan azt az eredményt adták, amit a vezetés hallani akart, nem a valós kockázatot.

✅ Intel

Egy strukturálatlan, stratégiai döntési helyzetben az adatfolyam minden lépése rendben zajlik: adatok keresése (OLAP, adatbányászat) → feldolgozás → tálalás (vizualizáció) — de a lánc végén ott áll a "vezetők korlátozottsága". Még egy tökéletesen felépített adatfolyam is a döntéshozó befogadóképességén akad el (saját anyag).

A kognitív torzítás csak az érem egyik oldala. Egy 2015-ös, széles körben idézett kutatás szerint (Dietvorst, Simmons és Massey, 2015) a döntéshozók gyakran elutasítják egy jó DSS/algoritmus javaslatát is — ezt hívják algoritmus-averziónak: ha egyszer látják, hogy egy algoritmus hibázott, még akkor sem bíznak benne újra, ha összességében jobban teljesít, mint az emberi becslés. Ennek pontosan az ellentéte az automation bias: amikor a döntéshozó túlzottan megbízik az automatizált javaslatban, és nem kérdőjelezi meg, még akkor sem, ha az nyilvánvalóan hibás. A jó döntéstámogatás tehát két, egymással ellentétes kockázat között egyensúlyoz: se ne utasítsuk el reflexből a gépi javaslatot, se ne fogadjuk el automatikusan, kritika nélkül.

💡 Műszaki analógia

Gondoljon erre úgy, mint egy precíz mérőműszerre, aminek hibás a kijelzője: hiába pontos a szenzor, ha az, aki leolvassa, szisztematikusan félreérti a mutatott értéket — vagy soha többé nem bízik a műszerben, miután egyszer tévedett, még akkor sem, ha időközben megjavították.

🤔 Reflektív kérdés

Emlékszik olyan esetre, amikor Ön (vagy egy vezetője) figyelmen kívül hagyott egy adatot vagy egy rendszerjavaslatot, mert nem illett a várt eredménybe? Vagy fordítva — túlzottan megbízott egy automatizált kimenetben, amiről utólag kiderült, hogy hibás volt?

Forrás: Laudon Ch.12 (Real-World Decision Making); EA2 saját anyag (Intel-példa); Dietvorst, Simmons & Massey (2015), Journal of Experimental Psychology: General

## 6. Mit támogat és mit nem támogat egy rendszer?

(forrás: 5.6.html)

### 6. Mit támogat és mit nem támogat egy rendszer?

## Mit támogat és mit nem támogat egy rendszer?

### A Mintzberg-szerepek — alkalmazási szinten

Egy klasszikus modell szerint egy vezető tíz szerepet tölt be (Mintzberg, 1971). Ez azért fontos, mert megmutatja: egy információs rendszer nem minden szerepet támogat egyformán jól.

(A teljes 10 szerepes táblázat az Opcionális Könyvben található, részletes bontásban.)

A lényeg alkalmazási szinten

- Az "erőforrás-elosztó" szerepet a BI/DSS kifejezetten jól szolgálja (adatalapú allokációs döntések)

- A "vállalkozó" és a "tárgyaló" szerephez semmilyen rendszer nem ad támogatást — ezek tisztán emberi, kapcsolati, kreatív feladatok

[kép]

Ábra: Rendszer által jól támogatott szerepek vs kizárólag emberi szerepek, Laudon Table 12.2 logikája alapján

Egy műszaki menedzser napi munkájában mind a tíz szerep megjelenhet, de eltérő súllyal, mint egy pénzügyi vezetőnél: a "zavarelhárító" szerep (pl. váratlan géphiba kezelése) és az "erőforrás-elosztó" szerep (kapacitás- és karbantartás-ütemezés) különösen gyakori. Ha egy BI-projekt indoklása az, hogy "csökkenteni fogja a zavarelhárítás idejét", érdemes megkérdezni: valóban a zavarelhárítás döntési szakaszát gyorsítja, vagy csak az információgyűjtést — mert a kettő nem ugyanaz. Ha egy vezetőség a "vállalkozó" szerepet (pl. új piac felfedezése, innovációs kezdeményezés) próbálja BI-eszközzel helyettesíteni, a projekt eleve kudarcra van ítélve, mert olyan feladatot delegál a technológiának, amit az strukturálisan nem tud ellátni.

A tanulság: amikor valaki azt mondja, "vezessünk be egy rendszert, ami mindent megold", érdemes megkérdezni: pontosan melyik vezetői szerepet szeretnénk támogatni — mert van, amit egy rendszer soha nem fog helyettesíteni.

Forrás: Laudon Ch.12 (Table 12.2, Mintzberg 1971)

## 7. Valós bukás: NHS Choose and Book

(forrás: 5.7.html)

### 7. Valós bukás: NHS Choose and Book

## Valós bukás: NHS "Choose and Book"

### Többtényezős elemzés

[kép]

Ábra helye: brit kórház vagy egészségügyi rendszer illusztráció

2004-ben a brit Nemzeti Egészségügyi Szolgálat (NHS) bevezetett egy 200 millió fontos rendszert ("Choose and Book"), ami lehetővé tette volna a betegeknek, hogy online válasszanak kórházat és időpontot háziorvosi beutaló alapján. 2014-re a költség 356 millió fontra duzzadt, a tervezett évi 51 millió font megtakarítás soha nem valósult meg.

#### Három versengő magyarázat — melyik volt a domináns ok?

Magyarázat | 
Bizonyíték mellette | 
Korlátja mint magyarázat | 

(1) Rossz alapfeltevés | 
A rendszer a kórházválasztást helyezte középpontba — de a betegek/háziorvosok gyors, helyi ellátást akartak, nem választási lehetőséget | 
Önmagában nem magyarázza, miért nem korrigálták a célt idővel | 

(2) Hiányzó ösztönzők | 
A háziorvosoknak nem volt anyagi vagy szakmai érdekük a rendszer aktív használatára | 
Nem magyarázza, miért nem alakítottak ki utólagos ösztönzőrendszert | 

(3) Technikai inkompatibilitás | 
A kórházi és háziorvosi rendszerek nem kommunikáltak megbízhatóan egymással | 
Technikai probléma orvosolható lett volna — mégsem történt meg időben | 

A legvalószínűbb válasz: mindhárom együtt, egymást erősítve.

A rossz alapfeltevés (1) miatt a felhasználók motiválatlanok voltak; a motiválatlanság (2) miatt senki nem nyomott a technikai hibák (3) sürgős javítására; a javítatlan technikai hibák pedig tovább erősítették a kezdeti bizalmatlanságot. Ez a tanulság fontosabb, mint bármelyik ok önmagában: egy komplex rendszerbukásnál ritkán van egyetlen "gyökérok" — a valódi kérdés az, hogyan erősítik egymást a különböző szintű problémák.

Forrás: Laudon Ch.12, "Interactive Session: Management — Britain's National Health Service Jettisons Choose and Book System"

## 8. Hazai kitekintő és a dilemma feloldása

(forrás: 5.8.html)

### 8. Hazai kitekintő és a dilemma feloldása

## Hazai kitekintő és a nyitó dilemma feloldása

### OTP Mobilbank — BI mindenkinek

Az OTP Bank egy személyes pénzügyi asszisztensként működő mobilbanki platformot épített, valós idejű elemzésekkel: automatikus tranzakció-kategorizálás gépi tanulással (90%-os pontossággal), kiadásfigyelő dashboard, célalapú megtakarítási funkció. Az eredmény: közel 2 millió aktív felhasználó havonta, a megtakarítási funkciót használók 20–30%-kal többet takarítanak meg. A siker kulcsa: a bonyolult analitikai koncepciók intuitív felületbe csomagolása — ez a BICC-elv gyakorlati alkalmazása lakossági kontextusban: a technológia nem helyettesíti, hanem eszközzé teszi az elemzést a laikus felhasználó számára is.

#### A nyitó dilemma (1. oldal) tényleges feloldása

Térjünk vissza a három hipotézishez:

Hipotézis | 
Diagnózis | 

H1 — Felületi/képzési probléma | 
Önmagában ritkán elégséges magyarázat — a modern BI-eszközök (Power BI) felhasználóbarátok; ha ez lenne az egyetlen ok, célzott képzéssel gyorsan megoldódna | 

H2 — Bizalmi probléma | 
Gyakori, de tünet, nem gyökérok — a bizalmatlanság onnan ered, hogy nincs, aki garantálja az adat konzisztenciáját (lásd Microsoft Starlight-eset, 4. oldal) | 

H3 — Koordinációs probléma | 
Ez a leggyakoribb, legmélyebb ok — technikailag kész rendszer, de nincs BICC-szerű szervezeti egység, aki felelős lenne a szabványokért, a bizalomépítésért és a felhasználói bevonásért | 

🔑 A válasz

A válasz tehát jellemzően H3, ami H2-t okozza, ami H1-ként jelenik meg a felszínen — a vezetők "nem tudják használni" (H1), mert nem bíznak benne (H2), mert senki nem garantálja a mögötte álló adat és folyamat megbízhatóságát (H3). A megoldás nem több képzés, hanem egy BICC-szerű koordináló funkció létrehozása.

🤔 Záró gondolkodtató kérdés

Ha Ön lenne az 1. oldal cégének ügyvezetője, és most, e diagnózis birtokában kellene lépnie: mi lenne az első konkrét intézkedése — és hogyan mérné le fél év múlva, hogy sikerült-e?

Forrás: OTP Mobilbank esettanulmány; saját szintézis

## 9. Elmélyítő kiegészítő

(forrás: 5.9.html)

### 9. Elmélyítő kiegészítő

Dietvorst, B. J., Simmons, J. P., & Massey, C. (2015). Algorithm aversion: People erroneously avoid algorithms after seeing them err. Journal of Experimental Psychology: General, 144(1), 114–126. https://doi.org/10.1037/xge0000033

Martins, A., Bianchi de Aguiar, M. T., Sambento, M., & Castelo Branco, M. (2024). Business intelligence system adoption and the leveraging of reporting process capabilities. Journal of Accounting & Organizational Change, 21(3), 506–534. https://doi.org/10.1108/JAOC-11-2023-0204
Alzghoul, A., Khaddam, A. A., Abousweilem, F., Irtaimeh, H. J., & Alshaar, Q. (2024). How business intelligence capability impacts decision-making speed, comprehensiveness, and firm performance. Information Development. https://doi.org/10.1177/02666669221108438
Theodorakopoulos, L., Theodoropoulou, A., & Halkiopoulos, C. (2025). Cognitive bias mitigation in executive decision-making: A data-driven approach integrating big data analytics, AI, and explainable systems. Electronics, 14(19), 3930. https://doi.org/10.3390/electronics14193930 (nyílt hozzáférésű)

## 1. Mi az a BI és BA?

(forrás: 5.10.html)

### 1. Mi az a BI és BA?

## Üzleti intelligencia — fogalmi alapok

### 1. Mi az a BI és BA?

Két, gyakran együtt emlegetett, de nem ugyanazt jelentő fogalom:

- Business Intelligence (BI): az az infrastruktúra, ami összegyűjti, tárolja és elemzi a vállalat által termelt adatokat — adatbázisok, adattárházak, adatpiacok

- Business Analytics (BA): az eszközök és technikák, amikkel ezt az adatot ténylegesen elemezzük — OLAP, statisztika, modellek, adatbányászat

[kép]

Ábra: BI és BA

Egyszerűen: a BI a "hol tárolunk", a BA a "hogyan elemzünk" kérdésre válaszol. A kettő együtt adja azt, amit a hallgatók a Power BI-laboron gyakorlatban is használni fognak.

Forrás: Laudon Ch.12

## 2. Döntéstípusok egyszerűen

(forrás: 5.11.html)

### 2. Döntéstípusok egyszerűen

### 2. Döntéstípusok egyszerűen

Nem minden döntés egyforma — háromféle típust érdemes megkülönböztetni:

Strukturált | 
van rá bevált eljárás — pl. "mennyi alapanyagot rendeljünk a jövő hétre?" | 

Félig strukturált | 
részben van eljárás, részben mérlegelés kell — pl. "melyik beszállítóval szerződjünk?" | 

Strukturálatlan | 
nincs bevált eljárás, tiszta vezetői ítélőképesség kell — pl. "lépjünk-e be egy új piacra?" | 

[Ábra helye: piramis-ábra — alul strukturált döntések (sok, gyakori), felül strukturálatlan döntések (kevés, ritka, nagy tét)]

Minél feljebb megyünk a szervezeti hierarchiában, annál inkább strukturálatlanná válnak a döntések — ez az oka, hogy a felső vezetőknek más típusú rendszer kell (ESS), mint egy operatív dolgozónak (MIS).

Forrás: Laudon Ch.12

## 3. Mi az a BICC egyszerűen?

(forrás: 5.12.html)

### 3. Mi az a BICC egyszerűen?

### 3. Mi az a BICC egyszerűen?

A Kötelező Könyv 2. oldala bevezeti a BICC (BI Kompetencia Központ) fogalmát. Ha ez elsőre bonyolultnak tűnt, itt egy egyszerűbb megközelítés.

Egyszerű analógia: képzelje el a BICC-et úgy, mint egy fordítóirodát a vállalaton belül. Az üzleti oldal a saját "nyelvén" beszél (bevétel, ügyfél, piac), az IT a sajátján (adatbázis, szerver, kód). Ha nincs, aki fordít a kettő között, a két oldal elbeszél egymás mellett — az üzleti igény nem jut el technikailag pontos formában az IT-hez, és az IT megoldása nem szolgálja valójában az üzleti célt.

A BICC pontosan ezt a "fordítói" szerepet tölti be, három területen egyszerre:

Üzleti oldal

mit szeretnénk elérni

Elemző oldal

hogyan mérjük és definiáljuk

IT oldal

hogyan valósítjuk meg technikailag

Fontos: a BICC nem dönt a vezető helyett — csak biztosítja, hogy mindenki ugyanarról a megbízható adatról beszéljen, amikor döntést hoz.

Forrás: Gartner BICC-modell, saját összefoglalás

## 4. Korlátozott racionalitás

(forrás: 5.13.html)

### 4. Korlátozott racionalitás

### 4. Korlátozott racionalitás — miért nem tudunk "tökéletesen" dönteni?

A Kötelező Könyv 5. oldala bemutatja a kognitív torzításokat — de honnan erednek egyáltalán ezek a torzítások? A választ Herbert Simon (közgazdasági Nobel-díjas, 1978) adta meg.

Korlátozott racionalitás (bounded rationality): Simon kimutatta, hogy az emberek nem optimalizálnak egy döntés meghozatalakor, hanem "satisfice-lnek" — megelégszenek az első "elég jó" megoldással. Ennek oka nem hanyagság, hanem az, hogy korlátozott az idejük, az információjuk és a mentális kapacitásuk egy valóban tökéletes döntéshez.

[kép]

Ábra: Korlátozott racionalitás

Egyszerű példa: amikor egy cég beszállítót választ, nem hasonlítja össze az összes lehetséges beszállítót a világon — megnéz 3-4-et, és azt választja, amelyik megfelel egy minimumkövetelménynek. Ez ésszerű alkalmazkodás a korlátozott erőforrásokhoz, nem hiba.

Miért fontos ez a BI szempontjából? Egy BI-rendszer nem azért hasznos, mert "tökéletessé" teszi a döntést, hanem mert csökkenti a rést az elméletileg elérhető legjobb döntés és a korlátozott emberi kapacitás között — sosem szünteti meg teljesen.

Forrás: Simon, H. A. (1957). Models of Man; Kötelező Könyv 5. oldala

## 5. Algoritmikus torzítás vs. algoritmus-averzió

(forrás: 5.14.html)

### 5. Algoritmikus torzítás vs. algoritmus-averzió

### 5. Algoritmikus torzítás vs. algoritmus-averzió

Két, gyakran összekevert fogalom — pedig ellentétes irányú problémákról van szó.

Algoritmikus torzítás

maga az algoritmus/modell torz — pl. egy toborzó-algoritmus, amit korábbi, elfogult emberi döntésekből tanítottak be, tovább örökíti azt. Ez adat/modell-probléma.

Algoritmus-averzió

az algoritmus jó, jobban teljesít, mint az ember — mégis nem bíznak benne, miután egyszer hibázni látták (Kötelező Könyv, 5. oldal). Ez pszichológiai probléma

[kép]

Ábra: Algoritmikus torzítás vs algoritmus-averzió

Egyszerű példa

Egy gyártó cég minőségellenőrző algoritmusa szisztematikusan több hibát jelez az éjszakai műszak termékeinél. Két teljesen eltérő magyarázat lehetséges:

- az éjszakai műszak tényleg rosszabb minőséget termel (az algoritmus jól működik)

- az algoritmust olyan adaton tanították, ahol az éjszakai műszak megvilágítása rosszabb volt, és ez tévesen "hibaként" tanulta meg (az algoritmus torz)

Csak alapos vizsgálattal dönthető el, melyik áll fenn.

Miért fontos megkülönböztetni? A két probléma ellentétes megoldást igényel. Algoritmikus torzításnál a megoldás technikai: jobb tréningadat, rendszeres auditálás. Algoritmus-averziónál a megoldás emberi/szervezeti: bizalomépítés, fokozatos bevezetés. Ha felcseréljük a kettőt — pl. bizalomépítő tréninget tartunk egy ténylegesen torz algoritmusra —, a probléma nem oldódik meg, csak elfedjük.

Forrás: Dietvorst, Simmons & Massey (2015); saját összefoglalás

## 6. Mintzberg vezetői szerepek — teljes táblázat

(forrás: 5.15.html)

### 6. Mintzberg vezetői szerepek — teljes táblázat

### 6. Mintzberg vezetői szerepek — teljes táblázat

A Kötelező Könyv 6. oldala röviden említi ezt a modellt — itt a teljes, tíz szerepes táblázat található, azzal is jelezve, mely informatikai rendszer támogatja (vagy nem támogatja) az adott szerepet.

Csoport | 
Szerep | 
Támogató rendszer | 

Interperszonális | Névleges vezető (figurehead) | telepresence rendszerek | 

Vezető (leader) | telepresence, közösségi hálózatok | 

Kapcsolattartó (liaison) | okostelefon, közösségi hálózatok | 

Informális | Információs központ (nerve center) | MIS, ESS | 

Terjesztő (disseminator) | e-mail, közösségi hálózatok | 

Szóvivő (spokesperson) | webinárium, telepresence | 

Döntési | Vállalkozó (entrepreneur) | nincs támogató rendszer | 

Zavarelhárító (disturbance handler) | nincs támogató rendszer | 

Erőforrás-elosztó (resource allocator) | BI, DSS | 

Tárgyaló (negotiator) | nincs támogató rendszer | 

Jól látható: a döntési szerepek közül csak az "erőforrás-elosztót" támogatja igazán a BI/DSS — a másik három (vállalkozó, zavarelhárító, tárgyaló) tisztán emberi, kapcsolati készség.

Forrás: Laudon Ch.12 (Table 12.2), Mintzberg (1971)
