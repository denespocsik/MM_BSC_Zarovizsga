# Menedzsment információs rendszerek (GMXIR1MBLF) — Kontextus és forrástérkép

## A fájl jellege

Ez a fájl **navigációs segéd, nem forrás**: megmutatja, melyik forrásfájl melyik szakasza releváns a V6–V10 tételekhez. A tételekben csak az állítható, amit a megengedett forrás eredeti szövege is tartalmaz. **Egyetlen kötelező érvényű szakasza a „Döntési napló”.** A szakasz- és fájlhivatkozások a `Források/Menedzsment információs rendszerek (GMXIR1MBLF)/` mappa 2026-10-02-i állapotára vonatkoznak.

## Tantárgy adatok

- **Kód:** GMXIR1MBLF — Menedzsment információs rendszerek
- **Kredit:** 4
- **Tagozat / nyelv / félév:** levelező / magyar / 2026/27/1
- **Szak:** Műszaki menedzser
- **Intézet:** Üzleti Tudományok és Digitális Ismeretek Intézet (1084 Budapest, Tavaszmező u. 17.)
- **Tantárgyfelelős:** Prof. Dr. Tick Andrea (a HTML-ek szerzőjeként nem nevezhető meg)
- **Óraszám (syllabus, „F” = féléves jelölés):** előadás 5, tantermi gyakorlat 0, labor 10
- **Félévzárás:** évközi jegy, írásbeli
- **Félévközi követelmény:** egy beadandó feladat, félévzáró elméleti teszt és 1 ZH
- **Pontozás:** elmélet 25, ZH 25, beadandó 25; a ZH max. 50 pont (25 elmélet + 25 gyakorlat), részenként min. 20% az aláírás feltétele
- **Jegy:** 0–50% elégtelen (1), 51–62% elégséges (2), 63–74% közepes (3), 75–86% jó (4), 87–100% jeles (5)
- **Megjegyzés:** a ZH-n az MI és a GenMI használata tilos (syllabus)

## Forrásleltár

| Csoport | Darab | Szint / állapot |
|---|---|---|
| `1_01`–`1_12` Kötelező tananyag (HTML) | 12 | **elsődleges forrás**; mind olvasható; kb. 41 800 szó; az `1_10`–`1_12` nem tartalmaz beágyazott képet |
| `2_01`–`2_12` Opcionális Fogalmi Alapkönyv (HTML) | 12 | `CSAK OPCIONÁLIS`; kb. 11 500 szó; a K1=A döntés szerint a tételekben **nem használható** |
| `3_07` Opcionális Haladó Könyv (HTML, adatbányászati számítások) | 1 | `CSAK OPCIONÁLIS`; kb. 1 700 szó; K1=A szerint **nem használható** |
| Syllabus (PDF), tételsor | 2 | hivatalos, szöveges; a syllabus a zip `01_General/1_MIR_levelező_2026_27_1.pdf` fájljával tartalmilag azonos (hash-egyezés), más néven |
| Ábrák (PNG/JPG) | kb. 80 | a tartalmilag releváns ábrákat megnéztem; illusztratív: Target-logó, magyar zászló |
| Zip | 1 | hash-összevetés szerint azonos a mappával, két `image.png` variáns kivételével (K9/1: elég jelezni, külön vizsgálat nem kell) |

**Ábrák állapota:**
- Hivatkozatlan, a hivatkozott ábrától eltérő: `Vállalati piramos_egyszerűbb.png`, `1. előadás döntési lépcső csak.png` (és `…_1`). **Nem használható** (K7).
- A hivatkozott IS-piramis: `Vállalati piramis.png` (1_01 §3).
- `ChatGPT Image 2026. júl. 13. 20_12_40.png` (OEE lebontása a dashboardokon): K9/2 szerint **tananyag**.
- A gyakorlati órák anyaga (Excel dashboard, Power BI, Looker Studio, Tableau, Fabric) **nincs a mappában**.

## Syllabus-hét ↔ előadásfájl

A fájlnév előadásszáma **nem azonos** a syllabus heti sorszámával.

| Syllabus-hét | Témakör | HTML |
|---|---|---|
| 1 | A MIS valódi szerepe | `1_01` |
| 2 | Versenyképesség, IT-stratégia (Porter, értéklánc, platform) | `1_02` |
| 3 | Az integrált vállalat: ERP, CRM, SCM | `1_03` |
| 4 | Mit ér az adat és ki felelős érte? | `1_04` |
| 5 | Üzleti intelligencia: kultúra, nem eszköz | `1_05` |
| 6 | OLAP és adatbányászat | `1_07` (az `1_06` „BI a gyakorlatban I.” — KPI-tervezés — önálló syllabus-héthez nem köthető) |
| 7 | nincs előadás (-) | |
| 8 | Tudásmenedzsment és intelligens szervezet | `1_09` |
| 9 | Big Data | `1_08` (az `1_08`/`1_09` sorrendje felcserélt) |
| 10 | Felhő és IT-infrastruktúra | `1_10` |
| 11 | E-kereskedelem és platform-gazdaság | **nincs HTML** |
| 12 | Etika, algoritmusok, felelős AI | `1_11` |
| 13 | Kiberbiztonság, digitális transzformáció | `1_12` |
| 14 | ZH | |

## Tétel ↔ forrás leképezés

Állapot: ✅ lefedett / ⚠️ gyenge / ❌ hiányzik / `CSAK OPCIONÁLIS`. A szakaszszámok a HTML saját tartalomjegyzéke szerintiek. A `CSAK OPCIONÁLIS` jelölésű sorokban a K1=A miatt a tétel nem használhatja az opcionális szintet.

### V6 — VIR fogalma, IS-típusok, VIR szerepe, funkciók, mutatószámok, műszaki menedzser

| R | Részkérdés | Forrás (fájl §) | Állapot |
|---|---|---|---|
| R1 | A VIR fogalmának meghatározása | `1_01` §3–4 („MIR/VIR”; önálló definíció nincs) | ⚠️ |
| R2 | Az IS-ek főbb típusai | `1_01` §3 (TPS, MIS, DSS, ESS/EIS; K7) | ✅ |
| R3 | A VIR szerepe a vállalati irányítási struktúrában | `1_01` §3–4; `1_05` §6 | ✅ |
| R4 | A VIR legfontosabb funkciói | `1_01` §4 (alkalmazási célok, KST/KPI, kivételkezelés, szerepkörök) | ✅ |
| R5 | Pénzügyi mutatószámok felsorolása | `1_01` §7 (PV, NPV, IRR, ROI); TCO (`1_08` §9, `1_10`); KPI (`1_06` §2–3) | ⚠️ |
| R6 | Összetett mutatószámrendszerek (pl. EVA, Z-score) | – | ❌ |
| R7 | A műszaki menedzser célja és ismereti mélysége a VIR programcsomagoknál | `1_06` §8, `1_07` §8 (általános szintézis) | ⚠️ |

### V7 — BSC, hazai VIR/BI programcsomagok, rendszerválasztás

| R | Részkérdés | Forrás (fájl §) | Állapot |
|---|---|---|---|
| R1 | A BSC filozófiája | `1_06` §5 (kritikai nézet); részletek csak `2_06` | ⚠️ + `CSAK OPCIONÁLIS` |
| R2 | A négy nézőpont | `1_06` §5 (a négy nézőpont fel van sorolva); részletek csak `2_06` | ⚠️ + `CSAK OPCIONÁLIS` |
| R3 | A stratégiai térkép logikája | `1_06` §5 (ábra: `BSC_2`/stratégiai térkép; magyarázó szöveg gyenge) | ⚠️ |
| R4 | A hazai VIR/BI programcsomagok áttekintése | – | ❌ |
| R5 | Sorbaállítás: elterjedtség, ár, komplexitás, BSC-támogatás | – | ❌ |
| R6 | Melyik rendszer alkalmaz beépítetten BSC-t | – | ❌ |
| R7 | Miért meghatározó ez a rendszerválasztásnál | `1_03` §9 (általános integrációs döntés; BSC-szempont nincs) | ⚠️ |

### V8 — BI, VIR–BI, BICC, vezetési szintek

| R | Részkérdés | Forrás (fájl §) | Állapot |
|---|---|---|---|
| R1 | A BI fogalma és funkciói | `1_05` §2–3; a definíció csak `2_05` | ⚠️ + `CSAK OPCIONÁLIS` |
| R2 | A VIR–BI kapcsolat és különbségek | – | ❌ |
| R3 | A BICC fogalma, kialakítási szempontjai, szervezeti szerepe | `1_05` §2 (szöveg: 3 kompetenciaterület; ábra: 6; K8) | ⚠️ |
| R4 | A BICC szerepe a döntéshozatalban és az adatvezérelt kultúrában | `1_05` §2, §4; `1_08` §8 | ✅ |
| R5 | A BI illeszkedése az operatív, taktikai, stratégiai szintekhez | `1_01` §4; `1_05` §3, §6 (BI-felhasználók megoszlása, menedzser szerepek) | ✅ |

### V9 — dashboard, KPI, DAX, megosztás, jogosultság

| R | Részkérdés | Forrás (fájl §) | Állapot |
|---|---|---|---|
| R1 | A dashboard fogalma | `1_06` §6; `1_01` §3 | ⚠️ |
| R2 | Típusai | – | ❌ |
| R3 | Felépítése | `1_06` §6 (tervezési elvek: Tufte, Few, Lie Factor) | ⚠️ |
| R4 | Információszolgáltatás: valós idejű adat, drill-down, szűrők | drill-down: `1_07` §3; valós idejű adat csak említés; szűrő nincs | ⚠️ |
| R5 | Alkalmazás a vezetési szinteken | `1_01` §3–4; `1_05` §6 | ⚠️ |
| R6 | A KPI fogalma | `1_01` §4; `1_06` §2–3 | ✅ |
| R7 | KPI-alapú jelentés készítése BI rendszerben | `1_06` §7 (Power BI; nem a jelentéskészítés lépései) | ⚠️ |
| R8 | A DAX-kifejezések szerepe | – | ❌ |
| R9 | Egyéni és vállalati vizualizációk | `1_06` §6 (általános); egyéni vizualizáció nincs | ⚠️ |
| R10 | Megosztás vállalaton belül és kívül | – | ❌ |
| R11 | Adminisztrációs jogosultságok és engedélyezés | – | ❌ |

### V10 — OLTP/OLAP, adattárház, KDD, adatbányászat, szakértői rendszerek, tudás, Big Data

| R | Részkérdés | Forrás (fájl §) | Állapot |
|---|---|---|---|
| R1 | Az OLTP–OLAP különbség | `1_04` §4 (táblázat, FASMI) | ✅ |
| R2 | Az adattárház szerepe és jelentősége | `1_04` §5, §7 | ✅ |
| R3 | A KDD iteratív folyamata | `1_07` §4 (lépések); az „iteratív” jelleg csak `2_07` | ⚠️ + `CSAK OPCIONÁLIS` |
| R4 | A tudásfeltárás és az adatbányászat kapcsolata | `1_07` §4–5 | ✅ |
| R5 | A leggyakoribb adatbányászati technikák | `1_07` §5–6 (a számítások csak `3_07`) | ✅ |
| R6 | A szakértői rendszerek struktúrája | `1_09` §7 (az architektúra csak szöveges helyőrző) | ⚠️ |
| R7 | A tudás informatikai kezelésének módszerei | `1_09` §3–6 | ✅ |
| R8 | A VIR-hez kapcsolódó szakértői rendszerek előnyei és korlátai | `1_09` §7 (VIR-kapcsolat nem explicit) | ⚠️ |
| R9 | A Big Data lehetőségei és kihívásai | `1_08` §3–9; a szöveges definíció csak `2_08` (a 3V a döntési fa ábrán) | ⚠️ + `CSAK OPCIONÁLIS` |

## Tartalmi hiányok

A „nincs” megállapítás teljes szöveges keresésre épül (mind a 25 HTML, ékezetes/ékezet nélküli alak, szóhatáron). **Jóváhagyott kezelés: A) beszerzés** mindegyik sorra (Döntési napló, K3).

| # | Tétel / R | Mit kér | Mit találtam | Keresett kifejezések | Állapot / kezelés |
|---|---|---|---|---|---|
| G1 | V6 R5 | pénzügyi mutatószámok | PV, NPV, IRR, ROI (`1_01` §7), TCO, KPI/OEE | `penzugyi mutato` (3), `roi` (15), `roe`, `du pont` (0) | ⚠️ — A (beszerzés) |
| G2 | V6 R6 | EVA, Z-score, mutatószámrendszer | semmi | `eva`, `economic value added`, `gazdasagi hozzaadott`, `z-score`, `z score`, `altman`, `csod`, `mutatoszam`, `mutatoszamrendszer`: mind 0 | ❌ — A (AVIR) |
| G3 | V6 R7 | műszaki menedzseri célok, mélység | csak általános szintézis (`1_06` §8, `1_07` §8) | `programcsomag` (0) | ⚠️ — A |
| G4 | V7 R1–R2 | BSC filozófia, négy nézőpont | `1_06` §5 kritika; részletek csak `2_06` | `balanced scorecard` (12), `bsc` (10), `kaplan`, `nezopont` (7) | ⚠️ — A (K1=A: `2_06` nem használható) |
| G5 | V7 R4–R5 | hazai programcsomagok, sorbaállítás | semmi | `programcsomag`, `qlik`, `tableau`, `cognos`, `sap bw`: 0; `hazai` (34, esettanulmányok), `elterjedt`, `licenc` (nem összevetés) | ❌ — A |
| G6 | V7 R6–R7 | beépített BSC, rendszerválasztási szempont | semmi (a SAP-említések ERP-esetekben: `1_01`, `1_03`) | `bsc`, `strategiai terkep` (2), `sap`, `power bi` kontextusa | ❌ — A |
| G7 | V8 R2 | VIR–BI különbség | semmi (külön-külön szerepelnek) | `vezetoi informacios` (5), `vir` (22), `business intelligence`, `uzleti intelligencia` együtt | ❌ — A |
| G8 | V9 R2, R4 | dashboard-típusok, szűrők | semmi | `dashboard` (45), `muszerfal` (0), `szuro` (3, nem szűrő-kontextus) | ❌ — A |
| G9 | V9 R8 | DAX | semmi | `dax` (0) | ❌ — A (Power BI doc) |
| G10 | V9 R9–R11 | egyéni/vállalati vizualizáció, megosztás, jogosultság | semmi | `custom visual`, `power bi service`, `row-level`, `rls`, `publikal` (3), `megosztas` (4), `jogosultsag` (1, felhő-kontextus), `engedelyez` (4) | ❌ — A (Power BI doc) |
| G11 | V10 R6 | szakértői rendszer struktúrája | szöveges helyőrző (`1_09` §7) | `szakertoi rendszer`, `tudasbazis`, `kovetkeztet` | ⚠️ — A |

A K1=A következménye: a `CSAK OPCIONÁLIS` jelölésű sorok (V7 R1–R2, V8 R1, V10 R3, V10 R9) hiányként kezelendők, amíg kötelező szintű forrás nem érkezik.

## Beszerzendő anyagok (összesítve)

| Szerző | Mű | Jelleg | Indoklás / érintett rész |
|---|---|---|---|
| Bángi-Magyar, A. et al. | AVIR kézikönyv (Digitális Tankönyvtár) | ajánlott irodalom | V6 R6 (G2); V7 R1–R3 (G4). A tartalom nem ellenőrzött, a syllabus-cím alapján feltételezett. |
| Microsoft | Power BI documentation | kötelező irodalom | V9 R8 (G9), R9–R11 (G10) |
| Óbudai Egyetem (gyakorlatvezető) | Power BI gyakorlati anyagok, Excel dashboard | gyakorlati anyag | V9 R3–R4, R7 (G8) |
| Bencsik, A. | Tudásmenedzsment elméletben és gyakorlatban (2015, 2024) | ajánlott irodalom | V10 R6–R8 (G11) |

G1, G3, G5–G7 pótlására a syllabus egyik műve sem rendelhető egyértelműen; a K3=A szerint ezekhez a felhasználó helyez be anyagot (forrás megnevezése nyitott).

## A HTML-ekben hivatkozott külső művek és kiadás-eltérések

A hivatkozott művek tartalma **nem használható**; másodlagos hivatkozásként a szerző és az év megadható (K6=A).

- **Laudon & Laudon:** a HTML-ek a 15. (2017/2018) és a 18. (2025) kiadásra hivatkoznak (`1_01`, `1_02`, `1_06`, `1_08`, `1_09`, `1_10`, `1_11`, `1_12`), a syllabus a 17. kiadást (2022) nevezi meg. **Forrásütközés**, nem oldható fel: kiadás-specifikus szám-, ábra- és fejezetszám nem vehető át.
- **Turban:** `1_03` a 3. kiadásra (2002) hivatkozik; a syllabus a 11. kiadást (2018) nevezi meg. Ugyanez a szabály.
- **V6–V10-hez kapcsolódó külső hivatkozások:** Kaplan & Norton (1996), Goodhart (1975), Thomas & Uminsky (2022) — `1_06`; Tokola et al. (2016), Fayyad, Piatetsky-Shapiro & Smyth (1996), Chapman et al. (2000, CRISP-DM), Press (2016) — `1_07`; McAfee & Brynjolfsson (2012), Gartner (2015/2018), Mayer-Schönberger & Cukier (2013), Davenport & Harris (2017), Ellram (1993) — `1_08`; Nonaka & Takeuchi (1995), Grieves & Vickers (2017) — `1_09`; Gartner BI- és BICC-modell — `1_05`.
- **„Saját anyag” típusú hivatkozások** (a HTML-re adandó, a külső mű nem nevezhető meg): `1_05` („EA2 saját anyag”, „saját dilemma”, „saját szintézis”), `1_06` („OEE gyáripari szakirodalom”), `1_07` („saját anyag (MIS_BIG_DATA.pdf)”, „saját üzleti forgatókönyv”), `1_09` (Iván Cs., Tick A. előadásanyag), `1_11` (MIS_KMS.pdf).
- A teljes „Forrás:” sorjegyzék az `1_01`–`1_12` HTML-ek végén és szakaszaiban található.

## Terminológia

- Az `1_01` „MIR/VIR” megfogalmazást használ (§4); az `1_01` §3 táblázata szerint a MIS a taktikai szint rendszere („menedzsment IS”), a DSS taktikai/stratégiai, az ESS/EIS stratégiai. Önálló VIR-definíció nincs.
- A VIR-rövidítés ütközik a **V11–V15 tárggyal** (GMXIV2MBLF; a rövidítés ottani jelentését ez a fájl nem rögzíti): a V6–V10 tételekben a VIR kizárólag a GMXIR1MBLF anyaga szerint értelmezhető; V11–V15 anyagából tartalom nem vehető át, csak utalás („lásd V12”).
- **K4=C szerint:** a V6-ban a „MIR/VIR” együttes megfogalmazás marad, a kapcsolat külön jelölve; egyenlőségjelet a tétel nem tesz, amit a forrás nem mond ki.
- **K7 szerint:** az IS-típusok szintezése az `1_01` §3 szövegét és táblázatát követi.

## Döntési napló

| Dátum | Kérdés | A felhasználó válasza |
|---|---|---|
| 2026-10-02 | K1 — Opcionális források | **A:** csak a kötelező tananyag (`1_NN`); a `2_NN` és a `3_07` a tételekben nem használható. |
| 2026-10-02 | K2 — Hivatkozási forma | Válasz: **„C”**. A K2 lehetséges válaszai: A) jóváhagyás, B) módosítás — **a C nem definiált opció: NYITOTT, tisztázandó, a tételek írása előtt kötelező.** |
| 2026-10-02 | K3 — Tartalmi hiányok kezelése | **A:** beszerzés (G1–G11, az A2 jelentés számozása szerint). |
| 2026-10-02 | K4 — Terminológia | **C:** a V6-ban a „MIR/VIR” együttes megfogalmazás marad, a kapcsolat külön jelölve. |
| 2026-10-02 | K5 — Terjedelem (V8–V10) | **B:** táblázatos tömörítés az irányérték megtartásával. |
| 2026-10-02 | K6 — Másodlagos hivatkozások | **A:** használhatók `(szerző, év, idézi: <HTML-forrás>, <év>, <szakasz>)` formában; az Irodalomban csak a HTML-forrás szerepel. |
| 2026-10-02 | K7 — IS-típusok szintezése (forrásütközés) | **Elfogadom:** az `1_01` §3 szövege és táblázata a mérvadó; a hivatkozatlan képek nem használhatók. |
| 2026-10-02 | K8 — BICC kompetenciaterületei (forrásütközés) | **Elfogadom:** a szöveg (három kompetenciaterület) követendő, az ábra eltérését jelezni kell. |
| 2026-10-02 | K9/1 — két zip-only `image.png` | **Elég jelezni:** külön vizsgálat nem szükséges. |
| 2026-10-02 | K9/2 — ChatGPT-kép (OEE dashboardok) | **Tananyag.** |
| 2026-10-02 | K10 — hiányzó promptfájl | A `Tétel revíziós prompt - GMXIR1MBLF tananyag-feldolgozás.md` fájlt a felhasználó visszahelyezte; a README-hivatkozás javítása nem szükséges. |
