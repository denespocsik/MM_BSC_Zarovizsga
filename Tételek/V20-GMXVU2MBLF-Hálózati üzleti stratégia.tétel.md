## V20 – Hálózati üzleti stratégia

### Beszerzendő anyagok

| Szerző | Mű | Jelleg | Indoklás / érintett rész |
|---|---|---|---|
| Håkansson, H. | *Határtalan hálózatok.* Alinea Kiadó, 2010. | ajánlott irodalom | A syllabus ajánlott irodalma; a tétel szervezeti határokra (R2) és eredményességre (R3) vonatkozó részkérdése a tárgy üzletihálózat-vonalához tartozik. A forrásmappában 2026-11-06-tól a Håkansson & Snehota (szerk., 2017) IMP-összegző kötet áll rendelkezésre, amely R2-t és R3-at elsődleges forrásként lefedi (20.3–20.4); a 2010-es mű saját tárgyalásának ellenőrzéséhez a mű továbbra is szükséges. |
| Szilágyi, G. A. | A 10–12. oktatási hét előadásanyaga (robosztusság és reziliencia, hálózatrengések; hálózati menedzsment, stratégia és menedzsment a hálózatokban; fejlődő vállalati hálózatok) | előadás-prezentáció | Az `Előadás_ppt1.pdf` a Mastenbroek-résznél véget ér; a syllabus 11. hete („Stratégia és menedzsment a hálózatokban”) a tétel témája, és mindhárom részkérdést (R1–R3) érinti. |

**Tétel:** Hálózati üzleti stratégia. Mutassa be az üzleti stratégiaalkotás hálózati megközelítését! Hogyan értelmezi a hálózati stratégiát: a szervezeti határokat és a szervezeti eredményességet.

---

*A kötelező irodalom (Barabási: Behálózva) angol eredetije (Linked, 2014) 2026-11-06-tól a forrásmappában van; a hubokra, a preferenciális kapcsolódásra és a robosztusságra vonatkozó állítások a Network Science tankönyv (Barabási, 2012) mellett erre is hivatkoznak. A szervezeti határok és az eredményesség hálózati értelmezését (20.3–20.4) az IMP 2017-es összegző kötete (Håkansson & Snehota, szerk., 2017) és a Linked 14. fejezete alapján egészítettük ki.*

### 20.1. A hálózati szemlélet a stratégiaalkotásban

A hálózattudomány (network science) kiindulópontja a tárgyban az, hogy a szervezet **nem gép, hanem hálózat** – sőt egyszerre több, egymásra rakódó hálózat (Szilágyi, 2026). A gép komplikált (complicated) rendszer: sok alkatrésze van, de viselkedése a részekből kiszámítható, és nem rendeződik át spontán. A szervezet ezzel szemben komplex (complex) rendszer: részei megjelennek és eltűnnek, visszacsatolásai részben véletlenszerűek, és viselkedése a részek ismeretéből nem vezethető le (Szilágyi, 2026). Ebből következik a stratégiaalkotás hálózati megközelítésének alapgondolata: a vállalat teljesítményét nem csak a belső erőforrásai, hanem a kapcsolatainak szerkezete – a hálózatban elfoglalt pozíciója – határozza meg.

Az előadás ezt gazdasági tételként fogalmazza meg: **a sikeres vállalatok a hálózatra építik üzleti stratégiájukat**, és a kapcsolatokkal rendelkező (linked) vállalatok robosztusabbak, mint az önállóak; a nagyobb kapcsolatsűrűség nagyobb véletlenhiba- és támadástűrést ad a vállalatnak (Szilágyi, 2026). Barabási ugyanezt a 21. század legsikeresebb cégein mutatja be: a Google, a Facebook, a Cisco, az Apple vagy az Akamai technológiája és üzleti modellje hálózatokra épül – a Google például nemcsak a web legnagyobb feltérképezője, hanem keresőtechnológiája is a web hálózati tulajdonságaira támaszkodik (Barabási, 2012, 1. fej.).

A hagyományos és a hálózati szemlélet különbsége a vezetés nézőpontjában ragadható meg. A hagyományos menedzsment a szervezetet a **hivatalos parancslánc** (organigram) alapján érti meg. A hálózati szemlélet szerint viszont a vállalat sikere szempontjából az **informális hálózat** – ki kivel kommunikál valójában – még fontosabb: ennek térképe feltárja a kulcsegységek közötti kommunikációhiányt, és megmutatja, kik azok, akik a részlegeket és a termékeket ténylegesen összekötik (Barabási, 2012, 1. fej.). Ez a gondolat a tárgy elejéig nyúlik vissza: már Moreno szociometriája (1933) azt mutatta ki, hogy a szervezetben kialakuló kapcsolathálózat eltér a hivatalos szervezeti ábrától (Szilágyi, 2026).

```mermaid
flowchart TD
    subgraph HAGY["Hagyományos szemlélet"]
        K1["<b>Organigram</b><br/>hivatalos parancslánc"]:::szurke --> K2["<b>A szervezet mint gép</b><br/>komplikált rendszer"]:::szurke --> K3["<b>Belső optimalizálás</b><br/>erőforrások, folyamatok"]:::szurke
    end
    subgraph HAL["Hálózati szemlélet"]
        H1["<b>Valódi, informális hálózat</b><br/>ki kivel kommunikál"]:::kek --> H2["<b>A szervezet mint hálózat</b><br/>komplex, többrétegű rendszer"]:::kek --> H3["<b>Stratégia a hálózatra építve</b><br/>pozíció, kapcsolatsűrűség, robosztusság"]:::zold
    end

    classDef kek    fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef zold   fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef szurke fill:#eceff1,stroke:#546e7a,stroke-width:2px,color:#263238,rx:10,ry:10;

    style HAGY fill:#f7f9fa,stroke:#b0bec5,stroke-width:1.5px,color:#546e7a;
    style HAL  fill:#f5f9ff,stroke:#90caf9,stroke-width:1.5px,color:#1565c0;

    linkStyle default stroke:#546e7a,stroke-width:2px;
```

---

### 20.2. Hálózati pozíció mint stratégiai alap: hubok és preferenciális kapcsolódás

A hálózati pozíció stratégiai jelentőségét a valós hálózatok topológiája magyarázza. A véletlen (Erdős–Rényi) hálózat fokszámeloszlása Poisson-eloszlás, haranggörbéhez hasonló: a legtöbb csomópontnak hasonló számú kapcsolata van, hubok nincsenek. A valós, nagy hálózatok azonban nem ilyenek: fokszámeloszlásuk hatványfüggvényt (power-law) követ, ezért **skálafüggetlenek** (scale-free). Bennük a legtöbb csomópontnak csak kevés kapcsolata van, és ezt a sok kis csomópontot néhány, rendkívül sok kapcsolattal rendelkező **hub** tartja össze (Szilágyi, 2026). Buchanan ezért nevezi az ilyen hálózatokat „arisztokratikusnak”, szemben az „egalitárius” hálózatokkal, amelyekben a kapcsolatok nagyjából egyenletesen oszlanak el (Buchanan, 2003, 7. fej.). Barabási a hubokat Gladwell „connectorai” általánosításának tekinti: a társadalomban kevés ember ismer kiugróan sokakat, és ugyanilyen kiugróan kapcsolt csomópontok vannak a webtől a sejtig minden komplex rendszerben; a hatványfüggvény mögött a Pareto-féle 80/20 szabály húzódik (Barabási, 2014, 5–6. fej.).

```mermaid
%%{init: {'theme':'base','themeVariables':{'xyChart':{'backgroundColor':'#ffffff','titleColor':'#263238','xAxisLabelColor':'#546e7a','xAxisTitleColor':'#263238','xAxisTickColor':'#90a4ae','xAxisLineColor':'#546e7a','yAxisLabelColor':'#546e7a','yAxisTitleColor':'#263238','yAxisTickColor':'#90a4ae','yAxisLineColor':'#546e7a','plotColorPalette':'#1565c0,#c2185b'}}}}%%
xychart-beta
    title "Sematikus fokszámeloszlás skálafüggetlen hálózatban (nem mért adat)"
    x-axis ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10+"]
    y-axis "Csomópontok száma" 0 --> 100
    bar [100, 55, 30, 18, 11, 7, 4, 3, 2, 1]
```

A hubok keletkezését a Barabási–Albert-modell két, együtt ható mechanizmussal magyarázza (Szilágyi, 2026; Barabási, 2012, 5. fej.):

1. **Növekedés (growth):** a valós hálózatok nem statikusak – a csomópontok száma új belépőkkel folyamatosan nő, míg a véletlen hálózat modellje rögzített csomópontszámmal, statikusan számol.
2. **Preferenciális kapcsolódás (preferential attachment):** az új csomópontok nem véletlenszerűen, hanem nagyobb valószínűséggel a már jól kapcsolt csomópontokhoz kötődnek.

A két mechanizmus együtt „a gazdag gazdagodik” (rich-gets-richer) dinamikát hozza létre: aki korábban lépett be és több kapcsolatot gyűjtött, az aránytalanul több újat vonz. A hubok tehát nem azért nagyok, mert gyorsabban nőnek, hanem mert **korábban érkeztek** – ezt nevezi a marketing- és üzleti irodalom az első belépő előnyének (first-mover advantage) (Barabási, 2012, 5. fej.; Barabási, 2014, 7. fej.; Buchanan, 2003, 7. fej.). Hogy a növekedés önmagában nem elég, Barabási a saját „A modelljével” mutatja meg: növekedés *véletlen* kapcsolódással exponenciális, nem hatványfüggvény-eloszlást ad, hubok nélkül (Barabási, 2014, 7. fej.). Üzleti példája a biotech szövetségi hálózat: már 79 szervezet és 31 kapcsolat mellett is két nagy komponens alakult ki a korai belépők (Genzyme, Chiron, Genentech) körül, és 3973 K+F-megállapodás elemzése hatványfüggvény-eloszlást adott – a stratégiai szövetségek hálózata skálafüggetlen (Barabási, 2014, 14. fej.).

**Stratégiai következmény – és a korlátja.** A modellből az következne, hogy a korai, tudatos pozicionálás önerősítő előnyt ad, és a legrégebbi szereplő mindig a legnagyobb hub marad. A valóság ennél árnyaltabb. A Google harmadik belépőként nemcsak vezető kereső lett, hanem 2000-re a web legjobban kapcsolt csomópontja is – pozíciója azonban nem bizonyult tartósnak: 2011-ben a még később induló Facebook vette át a web legnagyobb hubjának szerepét. Az Apple 1987-es Newton kéziszámítógépét a Palm söpörte le a piacról, majd egy évtizeddel később az iPaddel az Apple hódította vissza a vásárlókat (Barabási, 2012, 6. fej.). A magyarázat a **rátermettség (fitness)**: a csomópontok nem csak a koruk, hanem belső tulajdonságaik alapján is eltérő ütemben gyűjtenek kapcsolatokat. Egy vállalat esetében a fitness a vásárlók megszerzésére való képesség a versenytársakhoz képest, amely a menedzsment minőségével és az innovativitással függhet össze (Barabási, 2012, 6. fej.; Barabási, 2014, 8. fej.). A hub-pozíció tehát stratégiai cél, de nem tartja fenn önmagát: a korai belépés előnyét a rátermett késői belépő megfordíthatja. Barabási a hálózati gazdaság egy másik következményét is kiemeli: a hálózat növekedésével **a huboknak nagyobbra kell nőniük**, és az üzleti háló csomópontjai ezt – más hálózatoktól eltérően – a kisebb csomópontok felvásárlásával érik el; a fúziós hullámok ebben az értelemben a növekvő hálózati gazdaság természetes következményei (Barabási, 2014, 14. fej.).

**A pozíció mérése.** A hálózati pozíció két alapmutatója az előadásban a **fokszám** (degree) – a csomópont kapcsolatainak száma, a csomópont legfontosabb tulajdonsága – és a **közbeesettségi centralitás** (betweenness centrality), amely azt mutatja meg, hogy a hálózat összes legrövidebb útjából hány halad át az adott csomóponton (Szilágyi, 2026). A magas fokszám a hub ismérve; a magas közbeesettség azt jelzi, hogy a csomópont egymástól távoli hálózatrészeket köt össze. Buchanan szerint a hubok a sok kapcsolatuk révén természetes módon töltik be a Granovetter-féle hidak szerepét (Buchanan, 2003, 7. fej.).

---

### 20.3. A szervezeti határok hálózati értelmezése

A hálózati stratégia a szervezet határait is másképp értelmezi, mint a hagyományos szemlélet. A mainstream közgazdaságtan a vállalat határát a **tulajdoni egység** határaként látja, és ezt jogi, számviteli és intézményi eszközök erősítik meg; ha azonban a vállalatok közötti interakciót és kölcsönös függőségeket helyezzük a fókuszba, „ez a kép elpárolog”: a határ **többdimenziós, mozgatható és vitatható** lesz. A határkérdés „az IMP genomjának része”: a kutatás abból indult, hogy a két cég közötti *kapcsolatot* legalább olyan fontosnak tekinti, mint a cégeket magukat (Munksgaard, Olsen & Prenkert, 2017). Négy állítás bontja ki a hálózati határfogalmat.

**Először: a szervezet határa nem az organigram.** A szociometria óta tudjuk, hogy a tényleges kapcsolathálózat eltér a hivatalos szervezeti ábrától (Szilágyi, 2026), és a vezetés számára a hivatalos parancslánc helyett az informális hálózat a releváns egység (Barabási, 2012, 1. fej.). Barabási szerint a 20. századi vállalat **fa** – a vezérigazgató a gyökér, az ágak az egyre specializáltabb feladatok –, amely az információt rosszul szűri és merevvé teszi a szervezetet; az információs gazdaságban a vállalat **fából hálóvá** alakul: lapos, keresztkapcsolatos, projektcsapatokkal, külső szövetségekkel és kiszervezéssel, vertikális helyett virtuális integrációval (Barabási, 2014, 14. fej.).

**Másodszor: a szervezet többrétegű (multiplex) hálózat.** Ugyanazon személyek között egyszerre létezik hatalmi, szakmai utasítási, tudásmegosztási, helyettesítési, folyamat-, térbeli, preferencia- és pletykaréteg, és ezek topológiája eltér egymástól (Szilágyi, 2026). A határ ezért rétegenként más: egy dolgozó a hivatalos hierarchiában a periférián lehet, miközben a tudásmegosztási rétegben központi szereplő. Az IMP ugyanezt mondja a határ **helyéről**: az nem csak a tulajdon szerint, hanem a tevékenységek, az erőforrások és a szereplők rétege szerint is máshol húzódik (Gadde, 2014, idézi Munksgaard, Olsen & Prenkert, 2017).

**Harmadszor: a határ stratégiai választás – két archetípus.** Gadde (2014) a határok két ellentétes stratégiáját írja le (idézi Munksgaard, Olsen & Prenkert, 2017):

| Jellemző | Integrált hierarchia | Kapcsolt vállalat (connected company) |
|---|---|---|
| Alapstratégia | **pufferelés** (buffering): védekezés a külső ingadozás ellen | **hídépítés** (bridging): kapcsolódás a változó külső tényezőkhöz |
| Határmozgatás | **szélesítés** – a korábban külső tevékenységek bevonása (a korai Ford, General Electric) | **szűkítés** – a cég „zsugorodik”, interakciói nőnek (kiszervezés) |
| Függőségek | erős belső, gyenge külső | jelentős függőségek a tulajdoni határon át |
| Interfészek, interakció | kevés, egyoldalú adaptáció; a pufferelés korlátozza az interakciót | kölcsönös adaptáció; intenzív, hosszú távú kapcsolatok |
| Befolyási és tudatossági határ | az internalizálás „megoldja” a mások befolyásolását; korlátozott rálátás a hierarchián kívülre | az interakció lehetőséget ad mások befolyásolására; a megosztott tudás tágítja a rálátást |

A két archetípus a gyakorlatban egy cégen belül, időszakonként váltakozva van jelen. A határ **áteresztőképessége** (permeability) attól függ, pufferként vagy hídként használják-e; a határ három dimenziója a **tudatossági** (awareness: mit tud a cég mások tevékenységéről), a **befolyási** (influence) és a **kontroll-** (control) határ (Dubois, 1998; Gadde, 2014, idézi Munksgaard, Olsen & Prenkert, 2017). „Egyetlen szereplő sincs teljes kontrollban a határ fölött”: a határ mozgatását a partnerek ellenlépései is alakítják (Munksgaard, Olsen & Prenkert, 2017).

**Negyedszer: a határ kinyitásának ára.** A kapcsolt vállalat a partnerei zavarait is örökli. Barabási példája a kiszervezés: a Cisco „nem gyártott semmit, amit eladott”, hanem gyártók sűrű hálóját kötötte magához; a Compaq Pocket PC-je a beszállítói kapacitor- és flash-hiány miatt 600–700 ezer kielégítetlen rendelésnél akadt el, a Cisco nem állította le időben az ellátási láncát, és 12 kiszervező nagyvállalat piaci értékvesztése 2000–2001-ben meghaladta az 1,2 billió dollárt. Barabási diagnózisa szerint nem a hálózati gazdaság hibázott, hanem a **hierarchikus gondolkodás** átvitele hálózati üzleti modellre: a hierarchiában a veszteség a szervezet más részére átterhelhető, a hálózati gazdaságban „minden csomópontnak profitábilisnak kell lennie” (Barabási, 2014, 14. fej.). Ez összhangban van az előadás tételével: a kapcsolatsűrűség növeli a hiba- és támadástűrést (Szilágyi, 2026), de a hálózati határ tudatos kezelést kíván.

---

### 20.4. Szervezeti eredményesség: a hálózati pozíció és a valódi hálózat feltárása

A hálózati megközelítés az eredményességet a kapcsolatszerkezethez köti. A menedzsment-szakirodalomban egyre több bizonyíték van arra, hogy **a dolgozó pozíciója az informális hálózatban összefügg a termelékenységével** (Barabási, 2012, 1. fej.). Ezért alakult ki egy tanácsadói iparág – az IBM-től az SAP-ig – a szervezet valódi struktúrájának feltérképezésére: véleményvezérek azonosítására, a fluktuáció megelőzésére, egy feladatra optimális csoportok kijelölésére, termékek terjedésének modellezésére (Barabási, 2012, 1. fej.). Barabási megfogalmazásában a hálózattudomány „mikroszkóp” a felső vezetés kezében, amely a valódi hálózat feltárásával javítja a vállalat eredményességét (effectiveness).

Ezt egy magyar vállalat esettanulmánya szemlélteti (Barabási, 2012, 1. fej.). A három telephelyű cégnek súlyos belső kommunikációs problémája volt: a dolgozókhoz eljutó információ eltért a vezetés szándékától. A Maven 7 tanácsadó cég online kérdőívvel térképezte fel, hogy a dolgozók kitől kérnek tanácsot a vállalatot érintő döntésekben. A térkép néhány rendkívül befolyásos egyént – a szervezet hubjait – azonosított, és kiderült: **egyikük sem a vezetés tagja**. Sem az igazgatók, sem a vezérigazgató, sem a felső vezetők nem voltak hubok; a legnagyobb hub egy beosztott, a cég munkavédelmi és környezetvédelmi szakértője volt, akinek a munkája minden telephely bejárása. A dolgozók jelentős része egy-két lépésre volt tőle, a felső vezetéssel viszont nem volt kapcsolata, így az útja során összegyűjtött információkat adta tovább, pletykaközpontként működve.

A tanulság stratégiai: a megoldás nem a hub elbocsátása – ez a problémát csak súlyosbítaná. A valódi hiba az volt, hogy a vezetés nem épített ki megfelelő kommunikációs csatornákat, és **strukturális lyukat** (structural hole) hagyott maga és a dolgozók között, amelyet a hálózat természetes módon a munkavédelmi szakértővel töltött be. Ha a vezetés neki és a többi hubnak hozzáférést ad a valós információkhoz, az alapvetően megváltoztatja a vállalaton belüli információ megbízhatóságát (Barabási, 2012, 1. fej.).

**Az eredményesség IMP-oldali értelmezése: epizód → kapcsolat → hálózati pozíció.** Az IMP szerint az érték három szinten keletkezik. Az **epizódok** (egy szállítás, egy ajánlat) önmagukban jelentéktelenek, de mindegyik szűkíti és tágítja a jövőbeli lehetőségeket; a **kapcsolat** értéke az epizódok láncából és a jövőbeli potenciálból fakad, és a kulcskapcsolatok jelentős, **a pénzügyi kimutatásokban meg nem jelenő, kapcsolat-specifikus eszközöket** hordoznak; a **hálózati pozíciót** a vállalat összes kapcsolata adja (Johanson & Mattsson, 1992), és jogok és kötelezettségek halmazát jelenti a jövőbeli interakcióra. Ezért minden epizódot a kapcsolat, minden kapcsolatot a pozíció fejlődésére tekintettel kell kezelni; a kapcsolatok „a vállalat elsődleges eszközei”, amelyek nélkül nem tud kereskedni, mások erőforrásaihoz hozzáférni és saját beruházásait kiaknázni (Ford, Mattsson & Snehota, 2017). Két mérési következmény: a közösen teremtett érték mérése és felosztása a függőségek miatt mindig részben önkényes (Baraldi & Lind, 2017), és az interakcióban „a költség megelőzi a bevételt” – az eredményesség hálózati mutatóit ezért hosszabb időtávon kell nézni (Håkansson & Snehota, 2017).

```mermaid
flowchart TB
    subgraph VEZ["Felső vezetés"]
        CEO["<b>Vezérigazgató</b>"]:::szurke
        IG1["<b>Igazgató</b>"]:::szurke
        IG2["<b>Igazgató</b>"]:::szurke
        CEO --- IG1
        CEO --- IG2
    end

    NOTE(["Nincs kapcsolat a vezetés és a hub között:<br/><b>strukturális lyuk</b>, amelyet a hub<br/>pletykaközpontként tölt be"]):::rozsa

    subgraph DOLG["Dolgozók és csoportvezetők – három telephely"]
        HUB(["<b>Munkavédelmi szakértő</b><br/>a legnagyobb hub"]):::lilaH
        D1["●"]:::kek
        D2["●"]:::kek
        D3["●"]:::zold
        D4["●"]:::zold
        D5["●"]:::narancs
        D6["●"]:::narancs
        HUB --- D1
        HUB --- D2
        HUB --- D3
        HUB --- D4
        HUB --- D5
        HUB --- D6
        D1 --- D2
        D3 --- D4
        D5 --- D6
    end

    VEZ ~~~ NOTE
    NOTE ~~~ DOLG

    classDef kek     fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef zold    fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef narancs fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;
    classDef rozsa   fill:#fce4ec,stroke:#c2185b,stroke-width:2px,color:#880e4f,rx:10,ry:10;
    classDef lilaH   fill:#f3e5f5,stroke:#7b1fa2,stroke-width:3px,color:#4a148c,rx:10,ry:10;
    classDef szurke  fill:#eceff1,stroke:#546e7a,stroke-width:2px,color:#263238,rx:10,ry:10;

    style VEZ  fill:#f7f9fa,stroke:#b0bec5,stroke-width:1.5px,color:#546e7a;
    style DOLG fill:#f5f9ff,stroke:#90caf9,stroke-width:1.5px,color:#1565c0;

    linkStyle default stroke:#546e7a,stroke-width:2px;
    linkStyle 11,12 stroke:transparent,stroke-width:0px;
```

---

### 20.5. Eredményesség és robosztusság: a hálózat zavartűrő képessége

Az eredményesség hálózati értelmezésének másik pillére a **robosztusság** (robustness): az a képesség, hogy a rendszer egyes elemeinek kiesése ellenére is fenntartja az alapfunkcióit. Sok természeti és társadalmi rendszer működik tovább alkotóelemeinek meghibásodása után is, és ennek forrása a hálózati szerkezet (Szilágyi, 2026). A **perkolációs elmélet** (percolation theory) kérdése: hány csomópontot kell eltávolítani ahhoz, hogy a hálózat izolált komponensekre essen szét? Egyetlen csomópont eltávolítása csak korlátozottan hat a hálózat egységére, több csomóponté viszont széttördelheti (Szilágyi, 2026).

Az előadás két hibatípust különböztet meg: a **véletlen hibát** (failure) és a **célzott támadást** (attack); a robosztusság a hálózat topológiájától függ, és a skálafüggetlen hálózat másként viselkedik, mint a véletlen (Szilágyi, 2026). Ez a skálafüggetlen hálózatok „Achilles-sarka” (Albert, Jeong és Barabási 2000-es Nature-cikke nyomán): a valós hálózatok **robosztusak a véletlen hibákkal szemben, de sérülékenyek a célzott támadással szemben** (Barabási, 2012, 8. fej.). Buchanan ezt számszerűsíti: az internet szerkezetű hálózatban a csomópontok 5%-ának véletlen kiesése nem változtatja meg a hálózat átmérőjét, mert a véletlen hiba szinte mindig kis fokszámú elemet talál el, a hubok pedig „ragasztóként” tartják össze a hálózatot; ha viszont a legnagyobb hubokat távolítjuk el, már 1%-uk eltávolítása 12%-kal növeli az átmérőt, 5% megduplázza, 18% pedig apró töredékekre szakítja a hálózatot (Buchanan, 2003, 8. fej.).

A vállalatra ebből két következmény adódik. Egyrészt a hub-pozíció előny és kockázat egyszerre: ha a vállalat működése egy-két kulcsszereplőre vagy kulcspartnerre (hubra) épül, a véletlen zavarokat jól tűri, de e hubok célzott kiesése szétszakíthatja. Másrészt a robosztusság **tervezhető, de költséges**: a küllős (hub-and-spoke) hálózat a véletlen hibával szemben robosztus, a központ kiesésére viszont szétesik; ha a perifériás csomópontokat is összekötjük egymással, a támadástűrés nő – de a hálózat fenntartásának költsége, amely az átlagos fokszámmal arányos, a tankönyv példájában megduplázódik (Barabási, 2012, 8. fej.). A magas kapcsolatsűrűség tehát egyszerre növeli a vállalat hiba- és támadástűrését (Szilágyi, 2026) és a kapcsolatok fenntartásának költségét; a stratégiai döntés a kettő közötti egyensúly megtalálása.

A robosztusság dinamikus oldala a **kaszkádhiba** (cascading failure): ha egy csomópont kiesik, a terhelése a szomszédaira kerül, és ha azok nem bírják, ők is kiesnek vagy továbbadják a terhet. Így terjedt a 2003-as észak-amerikai áramszünet, amely nyolc amerikai államban 45 millió, Ontarióban további 10 millió embert hagyott áram nélkül, és Barabási szerint kaszkádhiba állt a 2009–2011-es pénzügyi válság mögött is, amikor az amerikai hitelválság bankokat, vállalatokat és államokat sodort csődbe (Barabási, 2012, 1. fej.). A kötelező irodalom makrogazdasági példája az 1997-es ázsiai válság: egy thai ingatlancég 3,1 millió dolláros kamatfizetési mulasztásától a malajziai és koreai pénzügyi szektor megrendülésén és a baht feladásán át a Dow Jones 554 pontos eséséig terjedt a kaszkád – ami „nem magyarázható olyan keretben, ahol minden szervezet csak egy mitikus piaccal interaktál”, a kaszkádhiba a hálózati gazdaság közvetlen következménye (Barabási, 2014, 14. fej.). A hálózati stratégia ezért a kapcsolódásból fakadó sérülékenységgel (vulnerability due to interconnectivity) is számol: a hálózatba kapcsolt vállalat a partnerei zavarait is „örökli”. Barabási szerint a hálózati gondolkodás egyben a védekezés eszköze: segít azonosítani és megerősíteni azokat a csomópontokat, amelyek a „makrogazdasági tűz” terjedését megállíthatják (Barabási, 2014, 14. fej.).

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#e3f2fd','primaryBorderColor':'#1565c0','primaryTextColor':'#0d47a1','lineColor':'#546e7a','fontFamily':'inherit'}}}%%
mindmap
  root((Szervezeti<br/>eredményesség<br/>hálózatban))
    A valódi hálózat feltárása
      Pozíció és termelékenység
      Rejtett hubok a vezetésen kívül
      Kommunikációs rések, strukturális lyuk
    A hálózati pozíció mutatói
      Fokszám
      Közbeesettségi centralitás
    Robosztusság
      Véletlen hiba és célzott támadás
      Kapcsolatsűrűség – tűrés és költség
      Kaszkádhiba
```

---

**Összegzés:** A hálózati üzleti stratégia abból indul ki, hogy a szervezet nem gép, hanem komplex, többrétegű hálózat, és a sikeres vállalatok a hálózatra építik a stratégiájukat. A stratégiai alap a hálózati pozíció: a skálafüggetlen hálózatokban a növekedés és a preferenciális kapcsolódás hubokat hoz létre, a korai belépő előnye önerősítő, de a rátermett késői belépő megfordíthatja. A szervezeti határ hálózati szemléletben nem az organigram és nem a tulajdon, hanem a valódi, rétegenként eltérő és a vállalaton túlnyúló kapcsolathálózat; a határ stratégiai választás a pufferelő-szélesítő integrált hierarchia és a hídépítő-szűkítő kapcsolt vállalat között, és a határ áteresztőképességét a tudatossági, befolyási és kontrolldimenzióban kell beállítani (Gadde, 2014, idézi Munksgaard, Olsen & Prenkert, 2017). A kinyitott határ ára, hogy a vállalat a partnerei zavarait is örökli, és a hálózati gazdaságban minden csomópontnak profitábilisnak kell lennie (Barabási, 2014, 14. fej.). Az eredményesség IMP-oldalról epizód → kapcsolat → hálózati pozíció szinten keletkezik, a kapcsolatok mérlegen kívüli eszközök (Ford, Mattsson & Snehota, 2017). Az eredményesség a hálózati pozícióból (fokszám, közbeesettség), a valódi hálózat feltárásából (rejtett hubok, strukturális lyukak) és a robosztusságból fakad: a kapcsolatsűrűség növeli a hiba- és támadástűrést, de a hub-függőség célzott támadásra sérülékennyé tesz, és a robosztusság növelésének költsége van.

---

### Várható vizsgáztatói kérdések

1. **Mi a különbség az integrált hierarchia és a kapcsolt vállalat határstratégiája között, és miért nem „vagy-vagy”?** — Az integrált hierarchia pufferel és szélesít: a külső ingadozás ellen belső integrációval védekezik, a korábban külső tevékenységeket bevonja (a korai Ford, GE), erős belső és gyenge külső függőségekkel, kevés interfésszel; a kapcsolt vállalat hidat épít és szűkít: tevékenységeit kiszervezi, függőségei a tulajdoni határon át húzódnak, interakciói intenzívek, és a megosztott tudás tágítja a rálátását (Gadde, 2014, idézi Munksgaard, Olsen & Prenkert, 2017). A gyakorlatban mindkettő jelen van egy cégen belül, időszakonként váltakozva; a stratégiai kérdés a határ helye és áteresztőképessége, nem a típusválasztás. Barabási Cisco–Compaq példája mutatja az árát: aki hálózati modellre hierarchikus gondolkodással vált, a kapcsolódás kockázatát viseli az előnye nélkül (Barabási, 2014, 14. fej.).
2. **Elég-e a preferenciális kapcsolódás a hubok keletkezésének magyarázatához?** — Nem. A Barabási–Albert-modell két mechanizmust tételez: a növekedést (a csomópontok száma folyamatosan nő, szemben a véletlen modell rögzített, statikus csomópontszámával) és a preferenciális kapcsolódást (az új csomópont a jól kapcsoltakhoz köt). A kettő együtt adja a hatványfüggvény-eloszlást és a hubokat (Szilágyi, 2026; Barabási, 2012, 5. fej.).
3. **Ha a korai belépő előnye önerősítő, miért nem mindig a legrégebbi szereplő a legnagyobb hub?** — A rátermettség (fitness) miatt: a csomópontok belső tulajdonságaik szerint eltérő ütemben gyűjtenek kapcsolatokat. A Google harmadik belépőként lett a web legnagyobb hubja 2000-re, 2011-ben pedig a még később induló Facebook vette át a helyét; az Apple Newtonját a Palm szorította ki, majd az iPad hódította vissza a piacot. Vállalatnál a fitness a vásárlók megszerzésének képessége, amely a menedzsment minőségével és az innovativitással függhet össze (Barabási, 2012, 6. fej.).
4. **Mi a különbség a fokszám és a közbeesettségi centralitás között, és melyik mikor fontos?** — A fokszám a csomópont kapcsolatainak száma, a csomópont legfontosabb tulajdonsága; a közbeesettségi centralitás azt mutatja, hogy a hálózat legrövidebb útjaiból hány halad át a csomóponton (Szilágyi, 2026). A fokszám a hub-jelleget, a közbeesettség a hídszerepet méri; a hubok nagy fokszámuk révén gyakran egyben hidak is (Buchanan, 2003, 7. fej.).
5. **Mit jelent a skálafüggetlen hálózat „Achilles-sarka”, és mi következik belőle a vállalati stratégiára?** — A valós hálózatok robosztusak a véletlen hibákkal, de sérülékenyek a célzott támadással szemben (Barabási, 2012, 8. fej.): a csomópontok 5%-ának véletlen kiesése nem változtatja meg az átmérőt, a legnagyobb hubok 1%-ának eltávolítása viszont 12%-kal növeli, 18%-uké pedig széttöredezi a hálózatot (Buchanan, 2003, 8. fej.). A vállalatnak ezért kezelnie kell a hub-függőséget; a perifériás csomópontok összekötése növeli a támadástűrést, de a fenntartás költségét is (Barabási, 2012, 8. fej.).
6. **A Maven 7 esettanulmányban miért nem megoldás a legnagyobb hub elbocsátása?** — Mert nem a hub a probléma, hanem a vezetés által hagyott strukturális lyuk: a felső vezetés nem épített ki kommunikációs csatornát a dolgozók felé, és ezt a rést töltötte be a sok telephelyet bejáró munkavédelmi szakértő. Elbocsátása a problémát súlyosbítaná; a megoldás az, hogy a vezetés a huboknak hozzáférést ad a valós információkhoz (Barabási, 2012, 1. fej.).

---

## Irodalom

* Barabási, A.-L. (2012). *Network science* [Elektronikus tankönyv, előzetes kiadás, PDF Version: November 2012]. barabasilab.com/networksciencebook
* Barabási, A.-L. (2014). *Linked: The new science of networks.* Basic Books. (Magyar kiadás: *Behálózva.* Open Books, 2022 — a syllabus kötelező irodalma.)
* Baraldi, E., & Lind, J. (2017). Value measuring and value appropriation in business networks. In H. Håkansson & I. Snehota (szerk.), *No business is an island: Making sense of the interactive business world* (3. fej.). Emerald.
* Buchanan, M. (2003). *Nexus: Small worlds and the groundbreaking science of networks.* W. W. Norton.
* Dubois, A. (1998). *Organising industrial activities across firm boundaries.* Routledge. (Idézi: Munksgaard, Olsen & Prenkert, 2017.)
* Ford, D., Mattsson, L.-G., & Snehota, I. (2017). Management in the interactive business world. In H. Håkansson & I. Snehota (szerk.), *No business is an island: Making sense of the interactive business world* (2. fej.). Emerald.
* Gadde, L.-E. (2014). Strategizing at the boundaries of firms. *IMP Journal, 8*(2), 51–63. (Idézi: Munksgaard, Olsen & Prenkert, 2017.)
* Håkansson, H., & Snehota, I. (2017). The significance of business relationships. In H. Håkansson & I. Snehota (szerk.), *No business is an island: Making sense of the interactive business world* (1. fej.). Emerald.
* Johanson, J., & Mattsson, L.-G. (1992). Network positions and strategic action: An analytical framework. In B. Axelsson & G. Easton (szerk.), *Industrial networks: A new view of reality* (205–217. o.). Routledge. (Idézi: Ford, Mattsson & Snehota, 2017.)
* Munksgaard, K. B., Olsen, P. I., & Prenkert, F. (2017). Boundaries of business actors and networks – theoretical and methodological reflections. In H. Håkansson & I. Snehota (szerk.), *No business is an island: Making sense of the interactive business world* (12. fej.). Emerald.
* Óbudai Egyetem, Keleti Károly Gazdasági Kar. (2026). *Vállalati és üzleti hálózatmenedzsment (GMXVU2MBLF) — Syllabus* [Syllabus].
* Szilágyi, G. A. (2026). *Organizational networks* [Előadás-prezentáció]. Óbudai Egyetem, Keleti Károly Gazdasági Kar.
