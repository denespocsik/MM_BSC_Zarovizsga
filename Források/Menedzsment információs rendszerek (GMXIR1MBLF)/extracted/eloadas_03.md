# 3. előadás: 3. előadás Az integrált vállalat: ERP, CRM, SCM — Kötelező tananyag

## 1. Nyitó dilemma — Target Canada, 2013

(forrás: 3.1.html)

### 1. Nyitó dilemma — Target Canada, 2013

## Az integrált vállalat: ERP, CRM, SCM

### Nyitó dilemma — [kép] Target Canada, 2013

🔴 Döntés előtt — Ön a vezetőségben ül

2013-at írunk. Ön a Target Corporation vezetőségének tagja. Éppen most hagyták jóvá minden idők legnagyobb nemzetközi terjeszkedését: 133 áruházat nyitnak Kanadában, két éven belül — a cég első lépése az Egyesült Államok határain túl.

A tervek szerint mindehhez egy vadonatúj, a nulláról felépített SAP ERP-rendszert kell bevezetni, amely körülbelül 75 000 termék adatait fogja kezelni: készletet, beszerzést, elosztást, árazást — az összes áruházban egyszerre. A rendelkezésre álló idő: 18 hónap. Az iparági szakértők egy ekkora projekthez jellemzően 3–4 évet javasolnak.

Kérdés, mielőtt tovább olvasna:

- Ön szerint sikerülni fog a bevezetés ilyen ütemterv mellett?

- Mi az, amit ilyen tempó mellett a leginkább kockáztatnak?

- Ha most megkérdeznék, mire figyelmeztetné a projektcsapatot?

Ezt a dilemmát a fejezet végén, a 9. oldalon oldjuk fel — a tényleges kimenetellel és élő, ellenőrizhető forrásokkal együtt. Addig azonban végig kell járnunk az utat: honnan jött a MIR, hogyan illeszkedik bele az ERP, és milyen más rendszerek (CRM, SCM) kapcsolódnak hozzá — hogy a 9. oldalon már szakmai fogalmakkal tudjuk elemezni, mi történt valójában.

💡 Tanulási eredmények

A fejezet elvégzése után Ön képes:

- elhelyezni az ERP-t a MIR tágabb, kronologikus fejlődésében, és megmagyarázni, mi különbözteti meg a MIR korábbi generációit (adatfeldolgozás, vezetői információk, stratégiai IS) az ERP-generációtól

- megkülönböztetni a szigetrendszert és az integrált vállalati rendszert, és megmagyarázni, miért jelent üzleti kockázatot az előbbi

- felismerni az MRP → MRP II → ERP → ERP II fejlődési szakaszait és azok korlátait

- bemutatni az ERP, CRM és SCM rendszerek szerepét és kapcsolódási pontjait egy közös vállalati architektúrában

- elemezni a bullwhip-effektus okait, és javaslatot tenni SCM-alapú megoldásra

- mérlegelni a build/buy/cloud/best-of-breed beszerzési döntés szempontjait egy adott vállalati helyzetben

- értékelni a bevezetési stratégiák (big bang, phased, parallel, pilot) kockázatait valós esetek alapján

📚 A fejezet térképe

2. oldal: a MIR kronologikus fejlődése — a nagy kép → 3. oldal: ezen belül az ERP-ág fejlődése (MRP → ERP II) → 4. oldal: mit ígér az ERP és hol bukik el → 5–6. oldal: CRM és SCM, az ERP-ág két folytatása → 7. oldal: hogyan kapcsolódik mind egy architektúrában → 8. oldal: hogyan szerezzük be → 9. oldal: hogyan vezessük be — és mi történt Target Canadával.

Forrás: Panorama Consulting Solutions, Canadian Business, Henrico Dolfing esettanulmány (részletes hivatkozások a 9. oldalon)

## 2. A MIR kronologikus fejlődése

(forrás: 3.2.html)

### 2. A MIR kronologikus fejlődése

## A MIR kronologikus fejlődése

### Mielőtt az ERP-hez érnénk — a nagy kép

A menedzsment információs rendszer (MIR) nem egyetlen technológia, hanem egy közel hetven éves fejlődési folyamat eredménye. Mielőtt rátérnénk az ERP, CRM és SCM részleteire — amelyek, ahogy a következő oldalon látni fogjuk, csak egy konkrét ága ennek a fejlődésnek —, nézzük meg a teljes képet: hogyan jutott el a MIR az egyszerű adatfeldolgozástól a mai intelligens, adatvezérelt rendszerekig.

#### A MIR négy nagy korszaka

[kép]

Ábra MIR kronologikus fejlődés Forrás: Turban et al. 2002

Korszak | 
Időszak | 
Cél | 

Az adatfeldolgozás korszaka | 
'60-as évek | 
Működési hatékonyság növelése | 

A vezetői információk korszaka | 
'70-es évek | 
A vezetői munka hatékonyságának növelése | 

A stratégiai információs rendszerek korszaka | 
'80-as–'90-es évek | 
Üzleti előnyök szerzése | 

Intelligens on-line megoldások korszaka | 
2000-es évektől | 
A tudásalapú társadalom megteremtése | 

#### A MIR alrendszereinek kronologikus fejlődése

- 1980-as évek: Executive Information Systems (EIS), Decision Support Systems (DSS)

- 1990-es évek: Data Warehousing (DW), Business Intelligence (BI)

- 2000-es évek: Dashboards and scorecards, Performance management

- 2010+ …?

🤔 Gondolkodtató kérdés

Az eredeti lista szándékosan nyitva hagyja a 2010 utáni korszakot ("2010+ …??"). Ön szerint mi került volna a listára, ha ma írnánk tovább? Gondoljon a saját munkahelyén használt eszközökre — mesterséges intelligencia alapú előrejelzés, valós idejű dashboardok, automatizált riportok? A 7–8. oldalon (build/buy/cloud, illetve a magyar vállalati példa) visszatérünk erre a kérdésre.

#### Funkcionális és üzemeltetési fejlődés — a MIR alkalmazásának változó kontextusa

Funkcionális fejlődés

e-Commerce → m-Commerce → c-Commerce — a MIR egyre inkább nem egy irodai, hanem egy mindenütt jelenlévő eszközzé vált

Üzemeltetési fejlődés

on-premise → on-demand / SaaS — a MIR-hez való hozzáférés módja is átalakult, ahogy azt a 7–8. oldalon (cloud ERP/CRM) részletesen látni fogjuk

Mindez egy új típusú felhasználóhoz igazodik: a modern munkavállalóhoz, aki állandóan mozgásban van, csapatban, projekt alapon dolgozik, és készségszinten ismeri a közösségi hálózatokat. A MIR fejlődése tehát nemcsak technológiai, hanem a munkavégzés jellegének változásához is igazodó folyamat.

Hova illeszkedik ide az ERP, CRM és SCM? A következő oldalon pontosan ezt nézzük meg: az ERP-CRM-SCM vonulat a fenti nagy képnek egy konkrét, de nagyon fontos ága — az, amelyik a vállalaton belüli és a vállalatok közötti erőforrás-integrációra fókuszál.

Forrás: Turban, E., McLean, E., & Wetherbe, J. (2002). Information Technology for Management: Transforming Business in the Digital Economy (3rd ed.). John Wiley & Sons.

## 3. Az ERP-ág fejlődése a MIR-en belül

(forrás: 3.3.html)

### 3. Az ERP-ág fejlődése a MIR-en belül

## Az ERP-ág fejlődése a MIR-en belül

### MRP-től ERP II-ig — egy konkrét ág a nagy képen belül

Az előző oldalon látott MIR-kronológia egyik konkrét, de a mai vállalati gyakorlatban meghatározó ága az, amelyik a vállalaton belüli és a vállalatok közötti erőforrás-integrációra fókuszál. Ez az ág négy lépésben írható le — és minden lépés ugyanarra a kérdésre válaszol egyre szélesebb körben: ki lát mit, és mikor?

[kép]

Ábra ERP fejlődési szakaszai Turban et al. (2002) modellje alapján

Év | 
Alap | 
+ Hozzáadva | 
→ Eredmény | 

1960 | 
Beszerzés + Raktározás | 
Gyártástervezés | 
→ MRP | 

1970 | 
MRP | 
Pénzügy | 
→ MRP II | 

1980 | 
MRP II | 
Minden belső forrás kezelése | 
→ ERP | 

1990 | 
ERP | 
Vevők és szállítók integrálása | 
→ Internal ERP/SCM | 

2000 | 
Internal ERP/SCM | 
Üzleti intelligencia | 
→ ERP II | 

Érdemes megfigyelni: az 1990-es sor ("ERP + Vevők és szállítók integrálása") az, ahonnan a fejezet következő két oldalán tárgyalt CRM (vevők) és SCM (szállítók) rendszerek erednek — ezek tehát nem külön történetek, hanem ugyanennek az ágnak a folytatásai. A 2000-es sor ("Üzleti intelligencia") pedig már előrevetíti a 7. oldalon tárgyalt Enterprise Application Architecture logikáját.

Miért nem elég a szigetrendszerek kommunikációja? Mert minden rendszernek megvan a saját adatstruktúrája, saját "igazsága". Ha az értékesítési rendszer és a pénzügyi rendszer nem ugyanazt az ügyféladatot látja, a vezető két különböző valóság között kénytelen dönteni — és rendszerint az egyeztetésre fordított idő emészti fel a versenyelőnyt.

💡 Műszaki analógia

Gondoljon úgy az MRP → ERP fejlődésre, mint egy gyárban arra, amikor minden gépet külön PLC (programozható logikai vezérlő) irányított, egymástól függetlenül — majd bevezettek egy központi SCADA-rendszert, ami mindet egyetlen felületen látja és vezérli. A gépek önmagukban nem lettek jobbak vagy gyorsabbak — de a rendszerszintű átláthatóság minőségi ugrást hozott: most már látni lehet az összefüggéseket, amik korábban rejtve maradtak.

Forrás: Turban, E. et al. (2002)

## 4. ERP mint válasz — és mint új probléma

(forrás: 3.4.html)

### 4. ERP mint válasz — és mint új probléma

## ERP mint válasz — és mint új probléma

### Az ígéret és a valóság közötti szakadék

Az ERP-rendszer ígérete egyértelmű: egységes adatbázis, egységes folyamatok, valós idejű átláthatóság az egész vállalatra. A valóság azonban jóval árnyaltabb — és a számok ezt kíméletlenül megmutatják.
[kép]

Ábra ERP-projekt életciklusa Forrás: Panorama Consulting Group, 2025 ERP Report; Gartner-elemzés

📊 Kemény számok (Panorama Consulting 2025 ERP Report + Gartner)

- a Gartner szerint az ERP-projektek 70%-a nem éri el a kitűzött célokat

- az átlagos költségtúllépés 189%, a feldolgozóiparban 215%

- csak 30% fejeződik be időben és a tervezett költségvetésen belül

- a projektek 50%-a elbukik már az első nekifutásra

- 41% a várt hasznoknak még a felét sem éri el

- az átlagos bevezetési költség 2025-ben: 450 000 dollár

Forrás: Panorama Consulting Group, 2025 ERP Report; Gartner-elemzés

Három figyelmeztető eset:

- Kmart: az i2 Technologies SCM-szoftvere nem illett a cég promóció-vezérelt üzleti modelljéhez, ami éles keresleti kilengéseket okozott — a szoftver egyszerűen nem volt felkészülve rá.

- Overstock.com: egy házon belül fejlesztett rendszer Oracle enterprise rendszerre cserélésekor a megrendelés-követés egy teljes hétre leállt, mert a visszatérítési folyamatot nem szinkronizálták megfelelően a követelés-nyilvántartással.

- Kennametal (2 milliárd dolláros szerszámgyártó): 13 éven át, 6400 egyedi testreszabással tartott fenn egy ERP-rendszert — végül lecserélték egy "plain-vanilla", testreszabás nélküli SAP-verzióra, és inkább a saját folyamataikat igazították a szoftverhez.

🤔 Reflektív kérdés

Gondoljon egy rendszerre a saját munkahelyén, amit "testreszabtak" az Ön igényeihez. Ki döntött úgy, hogy megéri a testreszabás? Visszamenőleg, a Kennametal-eset fényében, jó döntés volt — vagy inkább egy lassan felhalmozódó teher lett belőle?

A tanulság, amit a fejezet később (8. oldal) még visszaidéz: minél több az egyedi testreszabás, annál törékenyebb és drágább a rendszer. Ez a szál a fejezet végén a Target Canada-esettel is összekapcsolódik — ahol nem a testreszabás, hanem a sietség okozta ugyanazt a fajta törékenységet.

Forrás: Laudon Ch.9 (Enterprise Application Challenges)

## 5. CRM — az ügyfélkapcsolatok információs rendszere

(forrás: 3.5.html)

### 5. CRM — az ügyfélkapcsolatok információs rendszere

## CRM — az ügyfélkapcsolatok információs rendszere

### Aki "birtokolja" az ügyfelet, az nyer

A CRM (Customer Relationship Management) rendszer célja, hogy a vállalat egységes, 360 fokos képet kapjon minden ügyfélről — függetlenül attól, hogy az ügyfél az értékesítéssel, a marketinggel vagy az ügyfélszolgálattal lépett kapcsolatba.

Emlékezzen a 3. oldal táblázatára: az 1990-es sor pontosan azt mutatta, hogy az ERP "vevők és szállítók integrálásával" bővült. A CRM ennek az integrációnak a vevői oldala — az SCM (6. oldal) pedig a szállítói oldala.

#### Két alaptípus

Operational CRM

a napi ügyfélkapcsolati folyamatokat támogatja: értékesítés-automatizálás (SFA — Sales Force Automation), marketingkampányok, ügyfélszolgálati esetek kezelése

Analytical CRM

az ügyféladatok elemzésére épül: kik a legértékesebb ügyfelek, kik hagyják el a szolgáltatást, mi a mintázat a vásárlásokban

#### Kulcsfogalmak

- Churn rate (lemorzsolódási ráta): milyen arányban veszítjük el az ügyfeleket — az egyik legfontosabb korai figyelmeztető jelzés

- CLTV (Customer Lifetime Value): mennyit ér egy ügyfél a teljes kapcsolat során — nem csak az aktuális vásárlás

- PRM (Partner Relationship Management) és ERM (Employee Relationship Management): a CRM-logika kiterjesztése partnerekre és alkalmazottakra

- Social CRM: közösségimédia-adatok beépítése az ügyfélkapcsolatba (hangulatelemzés, gyorsabb reagálás)

Miért lett stratégiai kérdés? Mert a versenyelőny, ami egy új termékből fakad, gyorsan lemásolható — de az ügyfélkapcsolat tartósabb versenyelőnyt jelent. Ma már nem az nyer, aki a legtöbb terméket adja el, hanem aki "birtokolja" az ügyfelet.

💡 Műszaki analógia

Gondoljon úgy a CRM-re, mint egy ipari monitoring/telemetriai rendszerre: minden érintkezési pont (touchpoint — értékesítés, marketing, ügyfélszolgálat) olyan, mint egy külön érzékelő, amely folyamatosan adatot küld. CRM nélkül minden "érzékelőt" külön kellene leolvasni, és senki nem látja az egészet egyben. Egy jó CRM pontosan azt csinálja, amit egy központi vezérlőpult (dashboard): az összes érzékelő adatát egyetlen, valós idejű képpé állítja össze — így az ügyfélkapcsolat "állapota" egy pillantásra átlátható, ahelyett hogy három különböző rendszerben kellene keresgélni.

🤔 Reflektív kérdés

Gondoljon egy ügyfélre (vagy partnerre) a saját munkahelyén, akivel több részleg is kapcsolatban áll — mondjuk az értékesítés, az ügyfélszolgálat és a pénzügy egyaránt. Ha mindhárom terület pontosan ugyanazt az adatot látná róla valós időben, mi változna a döntéseikben? Előfordult már, hogy két részleg egymásnak ellentmondó információt adott ugyanarról az ügyfélről?

[kép]

✨ AI for CRM

A legújabb CRM-rendszerekbe már gépi tanulás és generatív AI épül be, hogy automatizálja, javítsa és optimalizálja az ügyfélkapcsolati folyamatokat. Ennek köszönhetően a vállalatok valós időben tudják elemezni a hatalmas mennyiségű ügyféladatot — például automatikusan felismerve, mely ügyfelek állnak a lemorzsolódás (churn) szélén, vagy milyen ajánlat illik leginkább egy adott vásárlóhoz, még mielőtt egy ügyintéző egyáltalán ránézne az adatokra.

Ez nem váltja le az operatív/analitikai CRM korábban megismert logikáját — felgyorsítja és élesebbé teszi azt: amit korábban egy elemzőnek kellett kézzel kibányásznia az adatokból, azt ma egyre inkább az AI végzi el elsőre, az ember pedig a kivételekre és a stratégiai döntésekre koncentrálhat.

Forrás: Laudon Ch.9 (9.3)

## 6. SCM — az ellátási lánc irányítása adatokkal

(forrás: 3.6.html)

### 6. SCM — az ellátási lánc irányítása adatokkal

## SCM — az ellátási lánc irányítása adatokkal

### Nem az áru mozog — az információ

A supply chain management (SCM) lényege nem a fizikai áru mozgatása, hanem az információ mozgatása — pontosabban: minél pontosabb információ minél gyorsabban jusson el minden szereplőhöz a láncban.

Ahogy az 5. oldalon (CRM) is jeleztük: a 3. oldal táblázatának 1990-es sora ("ERP + vevők és szállítók integrálása") két ágra bomlik — a CRM a vevői oldal, az SCM pedig a szállítói oldal.

[kép]

Ábra: klasszikus bullwhip-diagram Forrás Laudon&Laudon, 2025

#### A bullwhip-effektus (ostorcsapás-hatás)

Egy apró keresletnövekedés a lánc mentén felerősödik: a kiskereskedő kicsit többet rendel, a nagykereskedő ebből "biztonsági" többletet rendel, a gyártó még többet termel "hátha" — mire a hatás visszaér, elképesztő túlkészletezés alakul ki.

📦 Valós példa: Procter & Gamble Pampers

A boltokban a vásárlás stabil volt, de amikor a P&G árakciókat hirdetett, a nagykereskedői rendelések kiugrottak — a lánc mentén felhalmozódott pelenka-készlet olyan keresletet szolgált ki, ami valójában nem is létezett. A megoldás: pontosabb keresleti előrejelzés és megosztott, valós idejű adatok a lánc minden szereplője között.

#### Push vs. pull modell

- Push (build-to-stock): a termelés előrejelzésre épül — "gyártsuk le, aztán eladjuk"

- Pull (build-to-order, demand-driven): a tényleges vevői rendelés indítja el a láncot — "Make what we sell, not sell what we make." (Walmart folyamatos utánpótlási rendszere klasszikus példa erre.)

Két szoftvertípus: a supply chain planning (mit, mennyit, hol gyártsunk/tároljunk — előrejelzés-alapú) és a supply chain execution (a fizikai áramlás nyomon követése raktárból raktárba).

💡 Műszaki analógia

A bullwhip-effektus pontosan az, amit egy szabályozástechnikai rendszerben késleltetett visszacsatolásnak (feedback delay) nevezünk: ha egy szabályozókör információja késve érkezik, a rendszer túllő a célon, majd túlkorrigál — oszcillációt okozva. Minél hosszabb a lánc (több beszállítói szint), annál nagyobb a késleltetés, és annál durvább a kilengés. A megoldás ugyanaz, mint a szabályozástechnikában: gyorsabb, pontosabb visszacsatolás — vagyis valós idejű adatmegosztás a lánc minden tagja között.

[kép]

✨ AI for SCM

Az AI ma már kulcsszerepet játszik a modern globális ellátási láncok által termelt, egyre növekvő mennyiségű adat elemzésében — pontosabb keresleti előrejelzések készítésére, működési összefüggések feltárására, valamint a raktározási és szállítási folyamatok hatékonyságának javítására használják, akár több partnert is átfogó, kiterjedt logisztikai hálózatokon keresztül.

Ez közvetlenül kapcsolódik a fent bemutatott bullwhip-effektushoz: minél pontosabb az AI-alapú előrejelzés, annál kevésbé kell a lánc egyes szereplőinek "biztonsági ráhagyással" rendelniük — vagyis az AI a pontosabb információ eszközeként ugyanazt a problémát oldja, amit a valós idejű adatmegosztás is old, csak egy fokkal kifinomultabb szinten.

Forrás: Laudon Ch.9 (9.2)

## 7. Enterprise Application Architecture

(forrás: 3.7.html)

### 7. Enterprise Application Architecture

## Enterprise Application Architecture

### Hogyan kapcsolódnak egymáshoz?

Eddig külön-külön néztük az ERP-t, CRM-et, SCM-et — ez az oldal az egészet egyben mutatja meg, a Laudon-tankönyv 2.6-os ábrájának logikája szerint.

Ez az architektúra tulajdonképpen a 3. oldal táblázatának 2000-es sora ("Internal ERP/SCM + Üzleti intelligencia → ERP II") vizuális kibontása: az ERP II generáció pontosan ezt a fajta, minden irányba nyitott architektúrát jelenti.
[kép]

Ábra: ERP architektúra

A négy rendszer nem versenyez egymással, hanem kiegészíti egymást:

ERP — befelé integrál (gyártás, pénzügy, HR)

SCM — kifelé, a beszállítók irányába

CRM — kifelé, a vevők irányába

KMS — a vállalati tudást fogja össze és teszi elérhetővé, ahol szükség van rá

💡 Műszaki analógia

Az architektúra-ábra pontosan úgy néz ki, mint egy hálózati topológia-diagram: az ERP a központi csomópont (hub), a CRM és SCM pedig kifelé mutató kapcsolatok — nem egy lapos, mindenkivel-mindenki (mesh) hálózat, hanem egy tudatosan központosított architektúra, ahol a hub minden adatot lát, és onnan irányítja a forgalmat a megfelelő irányba.

Alternatíva kisebb büdzsére: intranet (belső, csak alkalmazottaknak elérhető céges háló) és extranet (kiterjesztett hozzáférés partnereknek) — olcsóbb, gyorsabb megoldás, ha egy teljes enterprise-rendszer bevezetése még nem indokolt vagy nem elérhető méretű a vállalat számára.

Forrás: Laudon Ch.2

## 8.  A kiterjesztett vállalat: ipari B2B piacterek

(forrás: 3.8.html)

### 8. A kiterjesztett vállalat: ipari B2B piacterek

## Ipari piacterek: hosszú távú kapcsolat vagy azonnali beszerzés?

### A kiterjesztett vállalat továbbgondolva

A 7. oldalon látott architektúra-ábra már megmutatta, hogy egy vállalat nemcsak befelé (ERP), hanem kifelé is kapcsolódik: vevőkhöz (CRM), beszállítókhoz (SCM), sőt üzleti és stratégiai partnerekhez is. De mi történik, ha ezek a kapcsolatok nem kétoldalúak maradnak, hanem egy közös piactéren zajlanak, ahol egyszerre sok vevő és sok eladó találkozik?
[kép]

Ábra: Net marketplace vs Exchange

📖 Fogalmi alap (Laudon Ch.10)

A B2B online kapcsolatoknak három fő típusa van: private industrial network (egy nagy cég saját, zárt hálózata a beszállítóihoz — pl. a VW Group Supply, amelyen a Volkswagen globális beszerzésének 90%-a zajlik), net marketplace (sok vevő és sok eladó közös, hosszabb távú, gyakran iparág-tulajdonú piactere) és exchange (független harmadik fél piactere, azonnali, „spot" vásárlásra). Az utóbbi kettő ugyanarra a kérdésre ad eltérő választ: hogyan szerezzünk be gyártási kapacitást vagy alkatrészt, ha nem akarunk — vagy nem tudunk — saját zárt hálózatot építeni?

 | 
Net marketplace — Exostar | 
Exchange — Go2Paper | 

Kapcsolat jellege | 
hosszú távú, szerződéses, együttműködő | 
rövid távú, azonnali („spot") | 

Tulajdonos | 
maga az iparág (BAE Systems, Boeing, Lockheed Martin, Raytheon, Rolls-Royce közösen alapította) | 
független közvetítő cég | 

Mire jó | 
tervezés, fejlesztés, gyártásütemezés megosztása 100 000+ beszállítóval a védelmi/repülőgépipari láncban | 
pillanatnyi szükséglet gyors kielégítése, ár-összehasonlítás | 

Kockázat | 
erős függés, lassabb rugalmasság | 
árverseny lenyomja az árakat, nincs hosszú távú garancia a beszállítóra | 

Emlékezzen a 6. oldal bullwhip-hatására: minél pontosabb és korábbi az információ a lánc mentén, annál kisebb a torzítás. Egy net marketplace — mint az Exostar — pontosan ezt szolgálja: hosszú távú, megosztott tervezési adatokkal csökkenti a bizonytalanságot. Egy exchange — mint a Go2Paper — ezzel szemben nem tervezésre, hanem a pillanatnyi hiány gyors pótlására való.

💡 Műszaki analógia

Gondoljon úgy a net marketplace-re, mint egy szabványosított iparági csatlakozóra (pl. egy USB-portra): mindenki ugyanahhoz a felülethez illeszkedik, nem kell egyedi interfészt fejleszteni minden egyes partnerhez — de a szabvány kialakítása és fenntartása hosszú távú elköteleződést igényel minden résztvevőtől. Az exchange ezzel szemben inkább egy nyílt piactér: bárki bárkivel egyszeri tranzakciót köthet, gyorsan, de szabványosított, tartós kapcsolat nélkül.

🤔 Reflektív kérdés

Ha az Ön vállalatánál egy kritikus alkatrész gyártási kapacitását kellene biztosítani: egy hosszú távú, iparági net marketplace-hez csatlakozna — kiszámítható, de lassabb és mélyebb elköteleződést kívánó megoldás —, vagy egy azonnali exchange-en keresne megoldást — gyors, de bizonytalanabb minőségű/árú? Mitől függ a döntése?

Forrás: Laudon Ch.10 (10.4) — B2B e-commerce: private industrial networks, net marketplaces, exchanges

## 9. Az integrációs döntés

(forrás: 3.9.html)

### 9. Az integrációs döntés

## Az integrációs döntés

### Build vs. buy vs. cloud vs. best-of-breed

Miután láttuk, mi az ERP/CRM/SCM, jön a gyakorlati kérdés: hogyan szerezze be egy vállalat?

Opció | 
Lényeg | 
Mikor éri meg | 

Build (saját fejlesztés) | 
egyedi rendszer a nulláról | 
csak nagyon specifikus, versenyelőnyt adó folyamatoknál | 

Buy (kész szoftver, on-premise) | 
bevált csomag, testreszabással | 
stabil, kiforrott folyamatoknál, ahol a testreszabás vállalható | 

Cloud | 
előfizetéses, gyorsan bevezethető, kevés testreszabás | 
KKV-knak, gyors növekedésnél, ahol a sebesség fontosabb, mint a teljes testreszabhatóság | 

Best-of-breed | 
különböző területekre a legjobb egyedi megoldás, összekötve | 
ha egyetlen "all-in-one" rendszer egyik területen sem elég erős | 

☁️ Két aktuális cloud-példa

- Oracle NetSuite — jelenleg a piacvezető cloud ERP a KKV-szegmensben, előre konfigurált modulokkal és gyors bevezetéssel

- Salesforce — a cloud CRM egyértelmű piacvezetője, 100 000+ ügyféllel, webes és mobil elérésű szolgáltatásként

[kép: 🇭🇺 Hungary Emoji | Flagpedia.net] Magyar vállalati példa: MOL Csoport vs. Kometa 99

Egy 2024-es SAP S/4HANA-konferencián Svébis András, a MOL Csoport csoportszintű CIO-ja nyíltan elmondta: a MOL számára a "zöldmezős" (greenfield) átállás — egy teljesen új rendszer felépítése a nulláról — nem opció. A vállalat földrajzilag és szervezetileg annyira komplex, annyi egyedi fejlesztéssel, hogy egy ilyen projekt 3–4 évig tartana — eközben pedig nem állhatnak le, mert folyamatosan zajlanak felvásárlások, változik az üzleti környezet. Ezért "barnamezős" (brownfield) átállást választottak: technikai frissítés, alapvető üzleti transzformáció nélkül.

Ezzel szemben egy másik hazai vállalat, a Kometa 99 pont az ellenkező döntést hozta: ők a zöldmezős váltás mellett döntöttek — mert az ő rendszerük "szét volt fejlesztve", töredezett, sok egyedi megoldással. Ez pontosan a fejezet 1. oldalán látott szigetrendszer-probléma hazai változata.

Forrás: ITBUSINESS.hu, "SAP-konferencia az S/4HANA körül" (2024) https://itbusiness.hu/technology/sap-konferencia-az-s-4hana-korul/

Vissza a 4. oldalhoz: a NetSuite és a Salesforce sikerének kulcsa pontosan az, amit a Kennametal-eset a rossz oldalán mutatott meg: kevés testreszabás, gyors bevezetés — szemben a Kennametal 13 évével és 6400 testreszabásával egy elavuló rendszeren.

Ez egyben válasz is a 2. oldal nyitva hagyott kérdésére ("2010+ …??"): a felhő-alapú, gyorsan bevezethető, kevés testreszabású megoldások (NetSuite, Salesforce) éppen a MIR-fejlődés jelenlegi, még nevesítetlen korszakát testesítik meg.

🤔 Reflektív kérdés — menedzseri döntés

Ha Ön döntene a saját vállalatánál egy új vállalatirányítási rendszerről: build, buy, cloud vagy best-of-breed mellett érvelne? Mi lenne a legnagyobb kockázat, amit vállalna — és mi az, amit semmiképp nem kockáztatna?

Forrás: Laudon Ch.9 (Next-Generation Enterprise Applications)

## 10. Big bang vs. phased rollout + Target Canada feloldása

(forrás: 3.10.html)

### 10. Big bang vs. phased rollout + Target Canada feloldása

## „Big bang" vs. „phased rollout"

### És mi történt valójában Target Canadával?

#### A négy klasszikus bevezetési (konverziós) stratégia

Stratégia | 
Leírás | 
Kockázat | 

Parallel | 
régi és új rendszer egyszerre fut egy ideig | 
biztonságos, de drága és erőforrás-igényes | 

Direct cutover ("big bang") | 
egy kijelölt napon a régi rendszert teljesen lecseréli az új | 
kockázatos — nincs visszaút hiba esetén | 

Pilot study | 
egy részlegen/egységen tesztelik, majd terjesztik ki | 
fokozatos tanulás, kisebb kockázat | 

Phased approach | 
funkciónként vagy egységenként, lépcsőzetesen vezetik be | 
lassabb, de kontrollált | 

[kép]

Ábra Crocs fázisos rollout (Ausztrália) vs Target Canada "big bang" 

✅ Valós ellenpélda — Crocs (SAP, fázisos globális rollout)

Ausztráliában indították, majd fokozatosan, régiónként terjesztették ki. A cél kimondottan az volt, hogy a problémák egyetlen régióra korlátozódjanak, mielőtt a következőre lépnének. Eredmény: 17 hónap alatt sikeres bevezetés, 24 elavult legacy rendszer megszüntetése.

#### A Target Canada feloldása — az 1. oldal dilemmájának válasza

Target Canada nem fázisos bevezetést, hanem gyakorlatilag egy irányított "big bang"-et választott: 133 áruház egyszerre, 18 hónap alatt, ott, ahol a szakértők 3–4 évet javasoltak volna. Mi történt ténylegesen?

- a 75 000 termék adatait kézzel, sietve vitték fel a rendszerbe — egyes becslések szerint a termékadatok akár 70%-a volt hibás (rossz mértékegység, hiányzó adat, elírás)

- a POS (pénztári) rendszer és az automatikus utánrendelési rendszer emiatt megbízhatatlanul működött — az áruházak polcai kongtak az ürességtől, miközben a raktárakban állt a készlet

- 2015. január 15-én a Target bejelentette mind a 133 kanadai áruház bezárását — a teljes veszteség kb. 7 milliárd dollár, 17 600 alkalmazott vesztette el az állását

🔑 A tanulság

A bukás oka nem a SAP szoftver minősége volt (ugyanezt a rendszert világszerte sikeresen használják) — hanem az, hogy a vezetőség technikai projektként kezelte azt, ami valójában egy mélyreható szervezeti változás volt, és a sebesség érdekében feláldozta az adatminőséget és a felkészülési időt.

🤔 Döntési kérdés — kapcsolódik az 1. oldal dilemmájához

Most, hogy ismeri a kimenetelt: ha Ön lett volna 2013-ban a Target Canada projektvezetője, és a vezetőség ragaszkodik a 2 éves határidőhöz, melyik konverziós stratégiát javasolta volna helyette — és mit mondott volna a vezetőségnek, amikor közölték, hogy nincs idő a fokozatos bevezetésre?

Források:

- Panorama Consulting Solutions: panorama-consulting.com/target-canada-supply-chain-failure

- Canadian Business — "The Last Days of Target Canada": canadianbusiness.com/ideas/the-last-days-of-target-canada

- Henrico Dolfing esettanulmány: henricodolfing.ch — Case Study 7

Forrás: Laudon Ch.13 (Conversion) + Ch.9 esettanulmányok + friss webes források

## 11. Elmélyítő kiegészítések

(forrás: 3.11.html)

### 11. Elmélyítő kiegészítések

##### 📚 Klasszikus alapmunkák

1. A bullwhip-effektus — az eredeti tanulmány

Lee, H. L., Padmanabhan, V., & Whang, S. (1997). Information Distortion in a Supply Chain: The Bullwhip Effect. Management Science, 43(4), 546–558.

DOI: 10.1287/mnsc.43.4.546

Ingyenesen olvasható változat: MIT Sloan Management Review — sloanreview.mit.edu/article/the-bullwhip-effect-in-supply-chains

Ez a tanulmány vezette be magát a "bullwhip effect" elnevezést.

2. ERP kritikus sikertényezők — átfogó szakirodalmi összegzés

Finney, S., & Corbett, M. (2007). ERP implementation: a compilation and analysis of critical success factors. Business Process Management Journal, 13(3), 329–347.

DOI: 10.1108/14637150710752272

45 tanulmány alapján összegzi, mely tényezők tűnnek fel újra és újra ERP-bevezetéseknél.

3. ERP-bevezetés kritikus sikertényezői — KKV-kontextusban

Ahmad, M. M., & Pinedo Cuenca, R. (2013). Critical success factors for ERP implementation in SMEs. Robotics and Computer-Integrated Manufacturing, 29(3), 104–111.

DOI: 10.1016/j.rcim.2012.04.019

Kifejezetten azt vizsgálja, mitől sikeres egy ERP-bevezetés kis- és középvállalatoknál.

##### 🆕 Friss kiegészítések (2024)

4. Bullwhip-effektus — friss szisztematikus áttekintés

Brauch, M., Mohaghegh, M., & Größler, A. (2024). Causes of the bullwhip effect: A systematic review and categorization. Management Research Review, 47, 1127–1149.

DOI: 10.1108/MRR-05-2023-0392

Megmutatja, hogyan fejlődött tovább a kutatás az 1997-es klasszikus tanulmány óta.

5. Cloud ERP KKV-knál — 2024-es, nyílt hozzáférésű kutatás

Hong, P. W., Dorasamy, M., Hong, L. J., & Malarvizhi, C. A. N. (2024). Exploring cloud enterprise resource planning and open innovation for small and medium enterprises: Insights from practitioners. Journal of Open Innovation: Technology, Market, and Complexity, 10(4), 100418.

DOI: 10.1016/j.joitmc.2024.100418

## 1. Mi az a MIR, és hogyan fejlődött?

(forrás: 3.12.html)

### 1. Mi az a MIR, és hogyan fejlődött?

## Az integrált vállalat — fogalmi alapok

### 1. Mi az a MIR, és hogyan fejlődött?

A MIR (menedzsment információs rendszer) gyűjtőfogalom: mindent jelöl, ami a vezetőket adatokkal, jelentésekkel és döntéstámogatással segíti. A MIR nem egyik napról a másikra alakult ki — fokozatosan, évtizedeken át fejlődött.

[kép]

Ábra: MIR kronologikus fejlődése

'60-as évek | 
egyszerű adatfeldolgozás — a cél a napi működés gyorsítása | 

'70-es évek | 
rendszeres, strukturált jelentések a vezetőknek | 

'80–90-es évek | 
stratégiai döntéstámogató rendszerek — innentől beszélünk ERP-ről is | 

2000-es évektől | 
intelligens, valós idejű, adatvezérelt megoldások | 

Ez a fejezet a harmadik szakaszra fókuszál: arra, amikor a vállalatok rájöttek, hogy a különböző rendszereiket (gyártás, pénzügy, ügyfélkapcsolat) össze kell kapcsolni. Ekkor jelent meg az ERP — és ebből nőtt ki a CRM és az SCM is.

Forrás: EA1 saját előadásanyag, saját összefoglalás

## 2. Mi az a szigetrendszer, és miért probléma?

(forrás: 3.13.html)

### 2. Mi az a szigetrendszer, és miért probléma?

## Az integrált vállalat — fogalmi alapok

### 2. Mi az a szigetrendszer, és miért probléma?

Képzeljünk el egy vállalatot, ahol az értékesítés Excelben dolgozik, a raktár egy másik, régi szoftvert használ, a pénzügy pedig egy harmadikat. Ezek a rendszerek nem "beszélnek" egymással — ez a szigetrendszer.
[kép]

Ábra: Sziget rendszerek vs Integrált rendszerek

Mi a baj ezzel?

- ugyanazt az ügyfelet vagy terméket többször, eltérő adatokkal rögzítik

- a vezető nem kap egységes, megbízható képet

- minden egyeztetés (pl. hónap végi zárás) kézi munkával, sok hibalehetőséggel jár

A megoldás egy közös, mindenki által látott adatbázis — ez az alapötlete minden integrált vállalati rendszernek, amiről a következő oldalakon lesz szó.

Forrás: Laudon Ch.2,

## 3. ERP, CRM, SCM — alapfogalmak röviden

(forrás: 3.14.html)

### 3. ERP, CRM, SCM — alapfogalmak röviden

### 3. ERP, CRM, SCM — alapfogalmak röviden

Rövidítés | 
Mit jelent | 
Egyszerű példa | 

ERP
(Enterprise Resource Planning) | 
egységes rendszer, ami összeköti a gyártást, pénzügyet, HR-t, értékesítést | 
egy gyár mindent egy rendszerben lát: mennyi alapanyag van, mennyi a bevétel, ki dolgozik ma | 

CRM
(Customer Relationship Management) | 
az ügyfélkapcsolatokat kezelő rendszer | 
a call center látja, hogy az ügyfél korábban mit vásárolt és milyen panasza volt | 

SCM
(Supply Chain Management) | 
a beszállítóktól a vevőig tartó lánc irányítása | 
egy bolt automatikusan jelez a gyártónak, ha fogy a készlet | 

Mindhárom rendszer ugyanarra a problémára válaszol: hogyan lássuk egységesen azt, ami korábban több, egymástól elszigetelt helyen volt szétszórva.

Forrás: Laudon Ch.2, Ch.9,

## 4. Hogyan függenek össze?

(forrás: 3.15.html)

### 4. Hogyan függenek össze?

### 4. Hogyan függenek össze?

Ez a három rendszer nem külön-külön, hanem együtt adja a modern vállalat gerincét.
[kép]

Az SCM a beszállítók felé, a CRM a vevők felé nyit — az ERP pedig mindkettőt összeköti a vállalaton belüli folyamatokkal (gyártás, pénzügy, HR).

Ha bármelyik hiányzik vagy nincs összekapcsolva, visszatér a szigetrendszer-probléma — csak most már nagyobb léptékben: nemcsak a vállalaton belül, hanem a beszállítók vagy a vevők irányában is.

Forrás: Laudon Ch.2

## 5. Bevezetési stratégiák dióhéjban

(forrás: 3.16.html)

### 5. Bevezetési stratégiák dióhéjban

### 5. Bevezetési stratégiák dióhéjban

Ha egy vállalat ilyen rendszert szeretne, alapvetően két kérdést kell eldöntenie.

1. Honnan szerezze be?

- Build — megépítjük magunknak (drága, de teljesen ránk szabott)

- Buy — megvesszük egy kész szoftvert (gyorsabb, olcsóbb, de kompromisszumokkal jár)

- Cloud — előfizetünk rá az interneten keresztül (leggyorsabb bevezetés, kevés testreszabás)

2. Hogyan vezessük be?

- "Big bang" — egyszerre, egy adott napon mindenki átáll az új rendszerre (gyors, de kockázatos)

- Fokozatos (phased) — lépésről lépésre, részlegenként vagy funkciónként (lassabb, de biztonságosabb)

Egy mondatos összefoglaló: minél nagyobb és összetettebb a vállalat, annál inkább megéri a fokozatos bevezetés — a sietség komoly kockázatot hordoz, ahogy azt a Kötelező Könyvben a Target Canada-eset is megmutatja.

Forrás: Laudon Ch.13, saját összefoglalás

## 6. Mi az a piactér, és mi köze az ERP-hez?

(forrás: 3.17.html)

### 6. Mi az a piactér, és mi köze az ERP-hez?

### 6. Mi az a piactér, és mi köze az ERP-hez?

Az előző oldalon látott build/buy/cloud döntés mellett van egy negyedik lehetőség is: nem építünk, nem veszünk és nem is bérlünk egy saját rendszert, hanem csatlakozunk egy már létező, iparági piactérhez, ahol sok vevő és sok eladó találkozik.

- Net marketplace — hosszú távú, iparág-tulajdonú piactér (pl. Exostar, a repülőgépipari/védelmi beszállítói hálózat)

- Exchange — független, azonnali („spot") piactér egyszeri beszerzésre (pl. Go2Paper, a papíripar piactere)

Egy mondatos összefoglaló: a választás azon múlik, hogy hosszú távú, kiszámítható kapcsolatot keresünk-e egy iparági közösségben, vagy csak egy pillanatnyi szükségletet kell gyorsan, egyszeri alkalommal kielégítenünk.

Forrás: Laudon Ch.10,
