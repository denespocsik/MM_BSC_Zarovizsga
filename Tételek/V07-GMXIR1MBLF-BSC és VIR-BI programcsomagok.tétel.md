## V7 – Balanced Scorecard és VIR/BI programcsomagok

### Beszerzendő anyagok

| Szerző | Mű | Jelleg | Indoklás / érintett rész |
|---|---|---|---|
| Bángi-Magyar, A. et al. | AVIR kézikönyv: Stratégiaalkotás, VIR, stratégiai mutató, adattár, felsőoktatási menedzsment (Digitális Tankönyvtár) | ajánlott irodalom | A syllabus ajánlott irodalomként nevezi meg; címe szerint a BSC/VIR-témát fedi, az R1–R3 elmélyítésére. Tartalmát nem ellenőriztem, az R4–R6 pótlására való alkalmasságáról nincs információm. |
| Óbudai Egyetem (gyakorlatvezető) | 12. heti gyakorlat: „Alternatív BI-eszközök: Looker Studio, Tableau, Fabric” (és a Power BI gyakorlatok anyaga) | gyakorlati anyag | A syllabus egyetlen olyan eleme, amely több BI-eszközt állít egymás mellé; az R4–R5 (programcsomagok áttekintése, sorbaállítás) pótlásához. A „hazai elterjedtség, ár, BSC-támogatás” szempontokat (R5–R6) a syllabus egyik műve sem fedi bizonyíthatóan. |

**Tétel:** Ismertesse a Balanced Scorecard (BSC) filozófiáját, mutassa be annak négy nézőpontját és a stratégiai térkép logikáját! Tekintse át a hazánkban elterjedt VIR és BI programcsomagokat és állítsa sorba azokat elterjedtség, ár, komplexitás és BSC-támogatás szempontjából! Térjen ki arra, hogy mely rendszerek alkalmazzák beépítetten a Balanced Scorecard mutatószámrendszert, és indokolja, miért meghatározó szempont ez egy vállalati rendszerválasztás során!

---

### 7.1. A BSC filozófiája

A Balanced Scorecard (BSC) Kaplan és Norton (1996) módszertana, amely a vállalati teljesítményt négy perspektívából (nézőpontból) vizsgálja egyszerre, nem csak pénzügyi szempontból (Kaplan & Norton, 1996, idézi: Óbudai Egyetem, Keleti Károly Gazdasági Kar, Üzleti Tudományok és Digitális Ismeretek Intézet [ÓE KGK ÜTDI], 2026d, 15. szakasz). A tananyag a BSC-t a menedzsment információs rendszer (MIR) alrendszereinek fejlődési idővonalán helyezi el: az 1980-as évek EIS- és DSS-rendszerei, majd az 1990-es évek adattárháza és üzleti intelligenciája (BI) után a 2000-es évek jellemzője a „dashboards and scorecards, performance management” (Turban et al., 2002, idézi: ÓE KGK ÜTDI, 2026a, 2. szakasz).

A négy perspektíva – pénzügyi, vevői, belső folyamat, tanulás-fejlődés – a kötelező tananyag szerint is alapfogalom. Kaplan és Norton eredeti szándéka szerint a BSC nem egyszerű mutatólista, hanem **oksági lánc**: a tanulás-fejlődési beruházások javítják a belső folyamatokat, azok javítják a vevői elégedettséget, ami végül pénzügyi eredményben csapódik le (Kaplan & Norton, 1996, idézi: ÓE KGK ÜTDI, 2026c, 5. szakasz).

A BSC tehát stratégiai gondolkodási eszköz, nem pusztán jelentés. Ha a mutatók kitöltése önmagáért való céllá válik, a BSC elveszti stratégiai funkcióját (ÓE KGK ÜTDI, 2026c, 5. szakasz). Ez a jelenség rokon a Goodhart-csapdával: amikor egy mutató célponttá válik, megszűnik jó mutatónak lenni (Goodhart, 1975, idézi: ÓE KGK ÜTDI, 2026c, 3. szakasz). A tananyag példája: egy call centerben az átlagos hívásidő lett az egyetlen mutató; a hívások gyorsabban zárultak, de az ismételt hívások aránya drasztikusan nőtt, vagyis a mutató javult, a valódi cél romlott (ÓE KGK ÜTDI, 2026c, 3. szakasz). A tananyag szintézise szerint a BSC csak akkor marad stratégiai eszköz, ha nem engedik bürokratikus rituálévá silányulni (ÓE KGK ÜTDI, 2026c, 8. szakasz).

A 6. előadás tanulási eredménye szerint a hallgatónak a BSC erősségeit és korlátait kell tudnia értékelni egy adott vállalati helyzetben, kritikai szemszögből (ÓE KGK ÜTDI, 2026c, 2. szakasz). Ezért a „filozófia” itt az oksági stratégiai eszköz gondolata és annak kritikája.

*(A BSC definíciója és a nézőpontok alapkérdései a 6. előadás opcionális könyvéből származnak – a K1=A döntés alóli, a V7-re jóváhagyott kivétel; a kötelező rész a BSC-t csak kritikai nézőpontból tárgyalja.)*

---

### 7.2. A négy nézőpont

Minden nézőponthoz egy alapkérdés tartozik (Kaplan & Norton, 1996, idézi: ÓE KGK ÜTDI, 2026d, 15. szakasz), a stratégiai térkép ábrája pedig célkitűzésekkel tölti meg őket (ÓE KGK ÜTDI, 2026c, 5. szakasz, ábra):

| Nézőpont | Alapkérdés | Mit jelent | Célkitűzések az ábra szerint |
|---|---|---|---|
| 1. Pénzügyi | Hogyan látnak minket a tulajdonosok, befektetők? | a stratégia végső céljait tükröző pénzügyi eredmények | hosszú távú pénzügyi érték; a bevétel növelése; a költséghatékonyság javítása |
| 2. Vevői | Hogyan látnak minket a vevőink? | a vevői érték létrehozása, amely a pénzügyi célok eléréséhez vezet | vevői elégedettség és érték; vevői elégedettség; vevői hűség és megtartás; a piaci részesedés növelése |
| 3. Belső folyamatok | Miben kell kiválónak lennünk? | a kulcsfolyamatok kiválósága, amelyek értéket teremtenek a vevők számára | hatékony és kiváló belső folyamatok; működési hatékonyság; minőségbiztosítás; innovációs folyamatok; ügyfélkapcsolat-menedzsment |
| 4. Tanulás és fejlődés | Hogyan tudjuk fenntartani a képességünket a változásra és fejlődésre? | az emberek, rendszerek és kultúra fejlesztése, amely megalapozza a stratégia végrehajtását | képességek és motiváció a fejlődéshez; humán tőke fejlesztése; információs rendszerek; szervezeti kultúra és elkötelezettség; vezetői képességek |

Az ábra szerint az **információs rendszerek a tanulás és fejlődés nézőpontban** szerepelnek: a BSC logikájában az IS az oksági lánc alapja, nem a vége. Konkrét mutatókat (KPI-kat) nézőpontonként a tananyag nem nevez meg.

---

### 7.3. A stratégiai térkép logikája

A stratégiai térkép (strategy map) a négy nézőpontot oksági láncként kapcsolja össze. Alulról felfelé olvasandó: a beruházások és képességek (tanulás és fejlődés) javítják a belső folyamatokat, azok növelik a vevői értéket, ez vezet végül jobb pénzügyi eredményhez (ÓE KGK ÜTDI, 2026c, 5. szakasz, ábra).

```mermaid
flowchart BT
    L("<b>4. Tanulás és fejlődés</b><br/>képességek és motiváció:<br/>humán tőke, információs rendszerek,<br/>szervezeti kultúra, vezetői képességek"):::lila --> B("<b>3. Belső folyamatok</b><br/>hatékony és kiváló folyamatok:<br/>működési hatékonyság, minőségbiztosítás,<br/>innováció, ügyfélkapcsolat-menedzsment"):::sarga
    B --> V("<b>2. Vevői</b><br/>vevői elégedettség és érték:<br/>hűség és megtartás,<br/>piaci részesedés növelése"):::kek
    V --> P("<b>1. Pénzügyi</b><br/>hosszú távú pénzügyi érték:<br/>bevétel növelése,<br/>költséghatékonyság javítása"):::zoldH

    classDef kek     fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef sarga   fill:#fffde7,stroke:#f9a825,stroke-width:2px,color:#f57f17,rx:10,ry:10;
    classDef lila    fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px,color:#4a148c,rx:10,ry:10;
    classDef zoldH   fill:#e8f5e9,stroke:#2e7d32,stroke-width:3px,color:#1b5e20,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
```

*(Az ábra a ÓE KGK ÜTDI, 2026c, 5. szakasz stratégiaitérkép-ábrája alapján készült.)*

A pénzügyi nézőpont az eredmény, a másik három az eredményt előidéző ok. A négy nézőpont ezért egymásra épülő lánc, nem négy külön siló. A kritikai szakirodalom szerint a gyakorlatban a szervezetek gyakran (ÓE KGK ÜTDI, 2026c, 5. szakasz):

- utólag illesztik a mutatókat a már meglévő jelentési struktúrához, ahelyett hogy valódi oksági stratégiai térképet építenének;
- a négy perspektívát négy külön silóként kezelik;
- a rendszer idővel bürokratikus rituálévá válik: negyedévente kitöltött táblázat, amelyet senki nem használ tényleges döntéshozatalra.

A stratégiai térkép tehát az, ami a BSC-t megkülönbözteti egy mutatólistától: a mutató értelmét a láncban elfoglalt helye adja.

---

### ⚠️ Tartalmi hiány — a hazai VIR- és BI-programcsomagok és sorbaállításuk (R4, R5)

A tételsor a hazánkban elterjedt VIR- és BI-programcsomagok áttekintését, és sorbaállításukat kéri elterjedtség, ár, komplexitás és BSC-támogatás szerint. A megengedett forrásokban ilyen áttekintés vagy sorbaállítás nem szerepel. Keresett kifejezések (a 12 előadás Kötelező Könyvében, `extracted/eloadas_01–12.md`, ékezetes és ékezet nélküli alak; 2026-11-06-án megismételve): programcsomag, szoftvercsomag, Qlik, Tableau, Cognos, Hyperion, BusinessObjects, MicroStrategy, SAP BW, SAP Analytics, Oracle BI, Looker, Fabric, Dynamics 365, Navision, Infor, Jedox, Pentaho, Targit, Anaplan, piaci részesedés, market share: mind 0 találat. Forráson kívüli tartalmat nem írok be. Az R4 és az R5 kitöltetlen; pótlás: lásd a Beszerzendő anyagokat.

**Név szerint szereplő rendszerek (nem rangsor, nem hazai elterjedtség).** Az alábbi lista csak azt rögzíti, mi fordul elő a tananyagban; a tételsor kérdésére nem válasz.

| Rendszer | Hol és milyen minőségben szerepel |
|---|---|
| Power BI | BI-eszközként: egy Power BI-alapú vezetői információs rendszer bevezetése a nyitó dilemmában (ÓE KGK ÜTDI, 2026f, 1. szakasz); a Key Influencers és az Anomaly Detection funkció (ÓE KGK ÜTDI, 2026c, 7. szakasz) |
| SAP (S/4HANA) | vállalatirányítási rendszerként: a MOL brownfield átállása (ÓE KGK ÜTDI, 2026a, 9. szakasz) |
| Oracle NetSuite | cloud ERP-ként, a tananyag szerint a KKV-szegmens piacvezetője (ÓE KGK ÜTDI, 2026a, 9. szakasz) |
| Salesforce | cloud CRM-ként (ÓE KGK ÜTDI, 2026a, 9. szakasz) |

A Power BI kivételével ezek ERP- vagy CRM-rendszerek, nem VIR/BI-csomagok, és egyikhez sem tartozik ár-, komplexitás- vagy BSC-támogatási adat.

---

### ⚠️ Tartalmi hiány — a beépített BSC-támogatás (R6)

A tételsor azt kéri, hogy mely rendszerek alkalmazzák beépítetten a BSC mutatószámrendszert. A megengedett forrásokban egyetlen rendszer sem szerepel beépített BSC-támogatással. A „scorecard” kifejezés csak a MIR alrendszereinek idővonalán fordul elő: a 2000-es évek jellemzője a „dashboards and scorecards, performance management” (Turban et al., 2002, idézi: ÓE KGK ÜTDI, 2026a, 2. szakasz). A BSC-re vonatkozó kifejezések (BSC, Balanced Scorecard, scorecard, stratégiai térkép) a módszertan kritikai tárgyalásában fordulnak elő (ÓE KGK ÜTDI, 2026c, 5. szakasz), szoftverhez kötve egyikben sem. Keresett kifejezések (a 12 előadás Kötelező Könyvében, `extracted/eloadas_01–12.md`, ékezetes és ékezet nélküli alak; 2026-11-06-án megismételve): BSC, Balanced Scorecard, scorecard, stratégiai térkép, pontozókártya, mutatórendszer; a fenti és a R4–R5 szakaszban keresett szoftvernevek BSC-vel együtt említve: 0 találat. Az R6 kitöltetlen; pótlás: lásd a Beszerzendő anyagokat.

---

### 7.4. Miért szempont a rendszerválasztásnál? (R7)

*(Tananyag-alapú szintézis. A megengedett források nem mondják ki, hogy a BSC-támogatás meghatározó szempont a rendszerválasztásnál; az alábbiak azt gyűjtik össze, mi támasztható alá a rendszerválasztás és a BSC kapcsán.)*

- **Stratégiai illeszkedés.** A tananyag szerint a kérdés nem az, hogy „milyen rendszert vegyünk”, hanem az, hogy „hol fáj a legjobban”; az IT és az üzleti stratégia összehangolása a legjövedelmezőbb vállalatok közös jellemzője (ÓE KGK ÜTDI, 2026e, 8. szakasz). A BSC ugyanezt a logikát a mérés oldalán adja: a mutatók a stratégia oksági láncából következnek (ÓE KGK ÜTDI, 2026c, 5. szakasz).
- **Stratégiai üzleti célkitűzés.** A tananyag szerint hat stratégiai üzleti célkitűzés áll az IS-befektetések mögött: működési kiválóság; új termékek és üzleti modellek; vevői és szállítói intimitás; jobb döntéshozatal; versenyelőny; túlélés (Laudon & Laudon, 2025, idézi: ÓE KGK ÜTDI, 2026b, 6. szakasz). A rendszerválasztás ezek közül elsősorban a „jobb döntéshozatal” (valós idejű adatok, nem találgatás) célkitűzéshez kapcsolható.
- **Beszerzési opciók.** A tananyag az ERP/CRM/SCM kapcsán négy opciót tárgyal: saját fejlesztés (build), kész szoftver (buy), felhő (cloud) és a legjobb egyedi megoldások összekötése (best-of-breed). Mindegyiknél megadja, mikor éri meg (ÓE KGK ÜTDI, 2026a, 9. szakasz).
- **Gazdaságosság.** A beruházást NPV, IRR és ROI mutatja; a TCO szerint a hardver- és szoftverbeszerzés a teljes költségnek csak kb. 20%-a, a többi rejtett tétel (Laudon & Laudon, 2018, idézi: ÓE KGK ÜTDI, 2026b, 7. szakasz). A megtérülést a komplementer szervezeti, menedzsment- és társadalmi befektetések határozzák meg (Brynjolfsson & Hitt, 2000, idézi: ÓE KGK ÜTDI, 2026b, 6. szakasz): a megtérülési mátrix szerint a magas IT-befektetés alacsony komplementer befektetéssel semmi vagy negatív megtérülést hoz, az alacsony IT-befektetés magas komplementer befektetéssel viszont meglepően jót; ezért érhet el egy kis vállalat olcsó felhőalapú CRM-mel jobbat, mint egy nagyvállalat milliárdos SAP-implementációval (Laudon & Laudon, 2017, idézi: ÓE KGK ÜTDI, 2026b, 6. szakasz).
- **Szervezeti érettség.** A Gartner ötszintű BI-érettségi modelljében (Unaware → Tactical → Focused → Strategic → Pervasive) a Focused → Strategic átmenethez nem újabb szoftver, hanem a siló-struktúrán átívelő szervezeti egység, a BI Kompetencia Központ (BICC) kell; ha a vállalat bevezeti a technológiát, de koordináló egységet nem hoz létre, a probléma nem a szoftverrel van, hanem a hiányzó szervezeti híddal (Gartner, idézi: ÓE KGK ÜTDI, 2026f, 2. szakasz). A tananyag nyitó dilemmája – egy 50 millió forintos, Power BI-alapú vezetői információs rendszer, amelyet a középvezetők nem használnak – a feloldás szerint koordinációs probléma (H3), nem eszköz- vagy képzési probléma (ÓE KGK ÜTDI, 2026f, 1. és 8. szakasz).
- **Kritikai szempont.** A BSC-bevezetések tipikus hibája, hogy a mutatókat utólag illesztik a meglévő jelentési struktúrához, és a rendszer rituálévá válik (ÓE KGK ÜTDI, 2026c, 5. szakasz). A tananyag a szoftvermodulokról nem mondja ki, de az előző pontokból következő logika az, hogy a beépített BSC-támogatás önmagában nem garantálja a stratégiai használatot.

⚠️ A tételsor ezzel szemben a BSC-támogatást meghatározó szempontnak tekinti. A megengedett források ezt sem megerősíteni, sem cáfolni nem tudják; az indoklást a Beszerzendő anyagok pótlása után lehet kiegészíteni.

---

### 7.5. Összegzés és tárgyon belüli kapcsolódások

A BSC a stratégiát négy nézőpont oksági láncává bontja, és a mutatók értelmét a láncban elfoglalt helyük adja. Ereje a stratégiai térkép, gyengesége a rituálévá válás. A tételsor második fele (programcsomagok, sorbaállítás, beépített BSC) a megengedett forrásokból nem készíthető fel; ezt a ⚠️ szakaszok nyíltan jelzik.

Kapcsolódások:
- **V6:** a KST és a KPI a VIR információszervezésének eszköze (ÓE KGK ÜTDI, 2026b, 4. szakasz). A tananyag a BSC-t és a KST/KPI-t külön tárgyalja, közvetlen kapcsolatot nem mond ki.
- **V8:** a BI-érettség és a BICC mint a szervezeti híd (ÓE KGK ÜTDI, 2026f, 2. szakasz).
- **V9:** a KPI-tervezés, a Goodhart-csapda és a dashboard-tervezés (ÓE KGK ÜTDI, 2026c, 2–6. szakasz).
- **1. előadás (saját összekapcsolás):** a VIR tíz gazdasági hatása közül egyik sem közvetlenül pénzügyi mutató, mégis mindegyik pénzügyi hatással jár, ezért a VIR-beruházás megtérülését nem elég egyetlen mutatóval mérni (ÓE KGK ÜTDI, 2026b, 7. szakasz). Ez a gondolat rokon a BSC többnézőpontú logikájával, amelyben a pénzügyi eredmény a nem pénzügyi okok következménye; a tananyag a két helyet nem köti össze.
- A BSC controlling-szemléletű tárgyalását lásd K20, az ERP-rendszerek témáját lásd V12 (csak utalás).

---

### Várható vizsgáztatói kérdések

1. **Miért nem „csak mutatólista” a BSC?** — Kaplan és Norton szándéka szerint oksági lánc: a tanulás-fejlődési beruházások javítják a belső folyamatokat, azok a vevői elégedettséget, ami pénzügyi eredményben csapódik le (Kaplan & Norton, 1996, idézi: ÓE KGK ÜTDI, 2026c, 5. szakasz).
2. **Miben különbözik a BSC egy 22 KPI-t mutató dashboardtól?** — A 22 KPI-s dashboard elemzési bénultsághoz vezet, mert nem tesz különbséget a fontos és a kevésbé fontos mutató között (ÓE KGK ÜTDI, 2026c, 2. és 8. szakasz). A BSC-ben a mutató helyét az oksági lánc adja, de a BSC is elromolhat, ha a mutatókat utólag illesztik a jelentési struktúrához (ÓE KGK ÜTDI, 2026c, 5. szakasz).
3. **Melyek a BSC bevezetésének tipikus hibái?** — Utólag illesztett mutatók valódi stratégiai térkép helyett, a négy nézőpont négy külön silóként kezelése, és a negyedéves kitöltési rituálé (ÓE KGK ÜTDI, 2026c, 5. szakasz).
4. **Mit jelent az, hogy az információs rendszerek a tanulás és fejlődés nézőpontban szerepelnek?** — Az ábra szerint az IS a képességek és a kultúra mellett az oksági lánc alapját képezi, amelyre a belső folyamatok, a vevői érték és a pénzügyi eredmény épül (ÓE KGK ÜTDI, 2026c, 5. szakasz, ábra).
5. **Mit mérlegel a vállalat egy új rendszer beszerzésekor?** — A build, buy, cloud és best-of-breed opciót, a TCO-t (a vételár kb. 20%-a) és a komplementer befektetéseket (ÓE KGK ÜTDI, 2026a, 9. szakasz; Laudon & Laudon, 2018, idézi: ÓE KGK ÜTDI, 2026b, 7. szakasz; Brynjolfsson & Hitt, 2000, idézi: ÓE KGK ÜTDI, 2026b, 6. szakasz).
6. **Hol helyezkedik el a BSC a menedzsment információs rendszerek fejlődésében?** — A MIR alrendszereinek idővonalán az 1980-as évek EIS- és DSS-rendszerei és az 1990-es évek adattárháza és BI-je után a 2000-es évek jellemzője a „dashboards and scorecards, performance management”; a 2010 utáni korszakot a tananyag nyitva hagyja (Turban et al., 2002, idézi: ÓE KGK ÜTDI, 2026a, 2. szakasz).

---

## Irodalom

* Óbudai Egyetem, Keleti Károly Gazdasági Kar, Üzleti Tudományok és Digitális Ismeretek Intézet. (2026a). *Az integrált vállalat: ERP, CRM, SCM* [Kötelező tananyag, 3. ea.].
* Óbudai Egyetem, Keleti Károly Gazdasági Kar, Üzleti Tudományok és Digitális Ismeretek Intézet. (2026b). *AZ MIS valódi szerepe* [Kötelező tananyag, 1. ea.].
* Óbudai Egyetem, Keleti Károly Gazdasági Kar, Üzleti Tudományok és Digitális Ismeretek Intézet. (2026c). *BI a gyakorlatban I.* [Kötelező tananyag, 6. ea.].
* Óbudai Egyetem, Keleti Károly Gazdasági Kar, Üzleti Tudományok és Digitális Ismeretek Intézet. (2026d). *BI a gyakorlatban I.* [Opcionális könyv, 6. ea.].
* Óbudai Egyetem, Keleti Károly Gazdasági Kar, Üzleti Tudományok és Digitális Ismeretek Intézet. (2026e). *Hogyan teremt versenyelőnyt az IT* [Kötelező tananyag, 2. ea.].
* Óbudai Egyetem, Keleti Károly Gazdasági Kar, Üzleti Tudományok és Digitális Ismeretek Intézet. (2026f). *Üzleti intelligencia: kultúra, nem eszköz* [Kötelező tananyag, 5. ea.].
