# Menedzsment információs rendszerek (GMXIR1MBLF) — Kontextus és forrástérkép

## A fájl jellege

Ez a fájl **navigációs segéd, nem forrás**: megmutatja, melyik forrásfájl melyik szakasza releváns a V6–V10 tételekhez. A tételekben csak az állítható, amit a megengedett forrás eredeti szövege is tartalmaz. **Egyetlen kötelező érvényű szakasza a „Döntési napló”.** A fájl- és szakaszhivatkozások a `Források/Menedzsment információs rendszerek (GMXIR1MBLF)/` mappa **2026-11-06-i állapotára** vonatkoznak (az előző állapot: 2026-10-02, `1_NN`/`2_NN` HTML-ek és zip; ez a szerkezet megszűnt).

**Jelölés:** `eloadas_NN §K` = az `extracted/eloadas_NN.md` kivonatban a `(forrás: N.K.html)` jelölővel kezdődő szakasz; a K a Kötelező Könyv saját oldalszáma, ez egyezik a tételekben használt `K. szakasz` hivatkozással. A régi `1_NN §K` hivatkozások tartalmilag ugyanezeknek felelnek meg (az `1_NN` = `eloadas_NN`).

## Tantárgy adatok

- **Kód:** GMXIR1MBLF — Menedzsment információs rendszerek
- **Kredit:** 4
- **Tagozat / nyelv / félév:** levelező / magyar / 2026/27/1
- **Szak:** Műszaki menedzser
- **Intézet:** Üzleti Tudományok és Digitális Ismeretek Intézet (1084 Budapest, Tavaszmező u. 17.)
- **Tantárgyfelelős:** Prof. Dr. Tick Andrea (a kivonatok szerzőjeként nem nevezhető meg)
- **Óraszám (syllabus, „F” = féléves jelölés):** előadás 5, tantermi gyakorlat 0, labor 10
- **Félévzárás:** évközi jegy, írásbeli
- **Félévközi követelmény:** egy beadandó feladat, félévzáró elméleti teszt és 1 ZH
- **Pontozás:** elmélet 25, ZH 25, beadandó 25; a ZH max. 50 pont (25 elmélet + 25 gyakorlat), részenként min. 20% az aláírás feltétele
- **Jegy:** 0–50% elégtelen (1), 51–62% elégséges (2), 63–74% közepes (3), 75–86% jó (4), 87–100% jeles (5)
- **Megjegyzés:** a ZH-n az MI és a GenMI használata tilos (syllabus)
- **Syllabus-irodalom:** kötelező — Laudon & Laudon (2022, 17. kiad.); Turban, Pollard & Wood (2018, 11. kiad.); Microsoft (2025) Power BI documentation. Ajánlott — Bángi-Magyar et al. (é. n.) AVIR kézikönyv; Bencsik (2015; 2024) Tudásmenedzsment; Chikán (2008) Vállalatgazdaságtan. **Egyik sincs a mappában.**

## Forrásleltár (2026-11-06)

| Elem | Állapot / használhatóság |
|---|---|
| `extracted/eloadas_01.md` … `eloadas_12.md` | a 12 Moodle-előadás kivonata; **elsődleges forrás**, de **csak a Kötelező Könyv rész** (határok: lásd alább). Az ábrák helyén `[kép]` jelölő áll — ábra tartalma csak a felirat szövegéből használható. |
| `extracted/targyi_adatlap.txt` | a hivatalos Tantárgynyilvántartó adatlap (syllabus) szövege; hivatalos forrás |
| `site prints/N. előadás/N.K.html` (+ `_files/`) | az eredeti HTML-nyomatok és a beágyazott képek (2026-10-22: 1–3. ea.; 2026-11-05: 4–12. ea.); a kivonat ellenőrzésére, ábrák megtekintésére |
| `Menedzsment információs rendszerek (GMXIR1MBLF).pdf` | a tételsor (V6–V10) PDF-je |
| `MIR_jegyzet.md`, `MIR_study_guide.md/.docx/.pdf`, `MIR_checklist.md` | **hallgatói jegyzetek — NEM tananyag**, a tételekben nem hivatkozhatók (a HR „Cheat sheet” analógiájára; a V08–V10 futtatásnál hozott döntés, Dénes utólag felülbírálhatja) |
| Gyakorlati órák anyaga (Excel dashboard, Power BI, Looker Studio, Tableau, Fabric, Power BI Service) | **nincs a mappában** |
| A korábbi `1_NN`/`2_NN`/`3_07` HTML-ek, zip | **megszűntek**; helyüket a fenti kivonatok és nyomatok vették át |

### Kötelező / opcionális határ (K1=A alkalmazása)

A tételekben **csak a „Kötelező Könyv”** használható. Az „Opcionális Könyv” és (a 7. ea.-n) a „Haladó Könyv” oldalai a Kötelező Könyv után, a számozás újraindulásával kezdődnek (az 1. ea.-nál számozatlan oldalak).

| Előadás | Kötelező oldalak | „Elmélyítő kiegészítő” (átvezető, lényegében irodalomjegyzék; tartalom nem vehető át) | **Nem használható** (Opcionális / Haladó) |
|---|---|---|---|
| 1 | 1.1–1.8 | 1.9 („Tovább az anyagon”) | 1.10–1.13 (konzervatív értelmezés: önmagukat előolvasmányként azonosítják) |
| 2 | 2.1–2.10 | 2.11 | 2.12–2.16 |
| 3 | 3.1–3.10 | 3.11 | 3.12–3.17 |
| 4 | 4.1–4.8 | 4.9 | 4.10–4.14 |
| 5 | 5.1–5.8 | 5.9 | 5.10–5.15 |
| 6 | 6.1–6.9 (a 6.8 és 6.9 azonos című szintézis) | – | 6.10–6.16 |
| 7 | 7.1–7.8 | 7.9 | 7.10–7.15 (Opcionális), 7.16–7.22 (Haladó: Bayes, konfúziós mátrix, F1, ROC/AUC) |
| 8 | 8.1–8.10 | 8.11 | 8.12–8.18 |
| 9 | 9.1–9.10 | 9.11 | 9.12–9.16 |
| 10 | 10.1–10.10 | 10.11 | 10.12–10.16 |
| 11 | 11.1–11.11 | 11.12 | 11.13–11.16 |
| 12 | 12.1–12.10 | 12.11 | 12.12–12.16 |

**Ábrák állapota:**
- A hivatkozott IS-piramis: `1.3_files/Vállalati piramis.png` (`eloadas_01` §3).
- Hivatkozatlan, a hivatkozott ábrától eltérő: `1.12_files/Vállalati piramos_egyszerűbb.png`, `1.13_files/1. előadás döntési lépcső csak.png` (mindkettő az opcionális oldalakon). **Nem használható** (K7).
- `7.2_files/ChatGPT Image 2026. júl. 13. 20_12_40.png` (OEE lebontása a hierarchia szintjein dashboardokká): K9/2 szerint **tananyag**; **a 7. előadás 2. szakaszához tartozik** (nem a 6.-hoz), a kivonatban csak a felirata szerepel.

## Syllabus-hét ↔ előadásfájl

A fájlnév előadásszáma **nem azonos** a syllabus heti sorszámával (a 6–7. hétnél eltér).

| Syllabus-hét | Témakör | Kivonat |
|---|---|---|
| 1 | A MIS valódi szerepe | `eloadas_01` |
| 2 | Versenyképesség, IT-stratégia (Porter, értéklánc, platform) | `eloadas_02` |
| 3 | Az integrált vállalat: ERP, CRM, SCM | `eloadas_03` |
| 4 | Mit ér az adat és ki felelős érte? | `eloadas_04` |
| 5 | Üzleti intelligencia: kultúra, nem eszköz | `eloadas_05` |
| 6 | OLAP és adatbányászat | `eloadas_07` (az `eloadas_06` „BI a gyakorlatban I.” — KPI-tervezés — önálló syllabus-héthez nem köthető) |
| 7 | nincs előadás (-) | |
| 8 | Tudásmenedzsment és intelligens szervezet | `eloadas_09` |
| 9 | Big Data | `eloadas_08` (a 8./9. sorrend felcserélt) |
| 10 | Felhő és IT-infrastruktúra | `eloadas_10` |
| 11 | E-kereskedelem és platform-gazdaság | **nincs előadásfájl** (platform-gazdaság érintőlegesen: `eloadas_02` §7) |
| 12 | Etika, algoritmusok, felelős AI | `eloadas_11` |
| 13 | Kiberbiztonság, digitális transzformáció | `eloadas_12` |
| 14 | ZH | |

## Tétel ↔ forrás leképezés

Állapot: ✅ lefedett / ⚠️ gyenge / ❌ hiányzik / `CSAK OPCIONÁLIS`. A szakaszszámok a kivonat `(forrás: N.K.html)` jelölői szerintiek. A `CSAK OPCIONÁLIS` jelölésű sorokban a K1=A miatt a tétel nem használhatja az opcionális szintet. A „+” jelű források a V8–V10 sub-agentek jelentései alapján kerültek a térképre (korábban hiányoztak).

### V6 — VIR fogalma, IS-típusok, VIR szerepe, funkciók, mutatószámok, műszaki menedzser

| R | Részkérdés | Forrás (fájl §) | Állapot |
|---|---|---|---|
| R1 | A VIR fogalmának meghatározása | `eloadas_01` §3–4 („MIR/VIR”; önálló definíció nincs; „VIR” kizárólag az 1. ea.-ban fordul elő) | ⚠️ |
| R2 | Az IS-ek főbb típusai | `eloadas_01` §3 (TPS, MIS, DSS, ESS/EIS; K7) | ✅ |
| R3 | A VIR szerepe a vállalati irányítási struktúrában | `eloadas_01` §3–4; `eloadas_05` §6 | ✅ |
| R4 | A VIR legfontosabb funkciói | `eloadas_01` §4 (alkalmazási célok, KST/KPI, kivételkezelés, szerepkörök) | ✅ |
| R5 | Pénzügyi mutatószámok felsorolása | `eloadas_01` §7 (PV, NPV, IRR, ROI); TCO (`eloadas_01` §7, `eloadas_08` §9, `eloadas_10` §8); KPI (`eloadas_06` §2–3) | ⚠️ |
| R6 | Összetett mutatószámrendszerek (pl. EVA, Z-score) | – | ❌ |
| R7 | A műszaki menedzser célja és ismereti mélysége a VIR programcsomagoknál | `eloadas_06` §8, `eloadas_07` §8 (általános szintézis) | ⚠️ |

### V7 — BSC, hazai VIR/BI programcsomagok, rendszerválasztás

| R | Részkérdés | Forrás (fájl §) | Állapot |
|---|---|---|---|
| R1 | A BSC filozófiája | `eloadas_06` §5 (a négy perspektíva megnevezve, Kaplan–Norton oksági lánc, kritikai nézet); a részletes tárgyalás csak az opcionális 6.15-ben | ⚠️ + `CSAK OPCIONÁLIS` |
| R2 | A négy nézőpont | `eloadas_06` §5 (felsorolás: pénzügyi, vevői, belső folyamat, tanulás-fejlődés); részletek csak 6.15 | ⚠️ + `CSAK OPCIONÁLIS` |
| R3 | A stratégiai térkép logikája | `eloadas_06` §5 (strategy map említése, ábra csak `[kép]`; magyarázó szöveg gyenge) | ⚠️ |
| R4 | A hazai VIR/BI programcsomagok áttekintése | – | ❌ |
| R5 | Sorbaállítás: elterjedtség, ár, komplexitás, BSC-támogatás | – | ❌ |
| R6 | Melyik rendszer alkalmaz beépítetten BSC-t | – | ❌ |
| R7 | Miért meghatározó ez a rendszerválasztásnál | `eloadas_03` §9 (általános integrációs döntés; BSC-szempont nincs) | ⚠️ |

### V8 — BI, VIR–BI, BICC, vezetési szintek

| R | Részkérdés | Forrás (fájl §) | Állapot |
|---|---|---|---|
| R1 | A BI fogalma és funkciói | `eloadas_05` §1–5, §8; `eloadas_03` §2–3 (BI mint MIR-alrendszer); `eloadas_07` §3–6; `eloadas_06` §8; **szó szerinti definíció a kötelező részben nincs** (csak 5.10, opcionális) → munkadefiníció | ⚠️ + `CSAK OPCIONÁLIS` |
| R2 | A VIR–BI kapcsolat és különbségek | – (a két fogalom külön szerepel; együtt csak `eloadas_05` §1 „Power BI-alapú vezetői információs rendszer” és `eloadas_03` §2 kronológia; összehasonlítás sehol) | ❌ |
| R3 | A BICC fogalma, kialakítási szempontjai, szervezeti szerepe | `eloadas_05` §2 (szöveg: 3 kompetenciaterület; ábra: 6; K8), **+** §4 (self-service vs. IT-centrikus, Managed Self-Service), §8 (BICC-szerű funkció felelősségei); kialakítási lépéssor/elhelyezés/létszám nincs | ⚠️ |
| R4 | A BICC szerepe a döntéshozatalban és az adatvezérelt kultúrában | `eloadas_05` §2, §4, §8; `eloadas_08` §8 | ✅ |
| R5 | A BI illeszkedése az operatív, taktikai, stratégiai szintekhez | `eloadas_01` §3–4; `eloadas_05` §3, §4 (BI-felhasználók megoszlása, ábrafelirat), §6; `eloadas_07` §2 | ✅ |

### V9 — dashboard, KPI, DAX, megosztás, jogosultság

| R | Részkérdés | Forrás (fájl §) | Állapot |
|---|---|---|---|
| R1 | A dashboard fogalma | `eloadas_01` §3 (ESS/EIS: dashboard); `eloadas_03` §2; `eloadas_06` §2, §6, §8; `eloadas_07` §2 (Tokola); definíció nincs | ⚠️ |
| R2 | Típusai | – (kapcsolódó: `eloadas_07` §2 ábrafelirat — OEE lebontása hierarchia-szintenként; tipológia nincs) | ❌ |
| R3 | Felépítése | `eloadas_06` §6 (Tufte, Few, Lie Factor), §8; `eloadas_07` §2 (tervezési elvek, nem komponens-felépítés) | ⚠️ |
| R4 | Információszolgáltatás: valós idejű adat, drill-down, szűrők | valós idő: `eloadas_05` §3 (időszerűség–pontosság), `eloadas_01` §3, `eloadas_07` §8; drill-down: `eloadas_07` §3, `eloadas_01` §4; szűrés: `eloadas_01` §3–4 (szűrt riport, kivételkezelés), `eloadas_07` §3 (slice/dice); dashboard-vezérlő (slicer) nincs | ✅ valós idő, ✅ drill-down, ⚠️ szűrők |
| R5 | Alkalmazás a vezetési szinteken | `eloadas_01` §3–4; `eloadas_05` §3–4, §6; `eloadas_07` §2 | ✅ |
| R6 | A KPI fogalma | `eloadas_01` §4; `eloadas_06` §2–4, §8 (Goodhart, OEE) | ✅ |
| R7 | KPI-alapú jelentés készítése BI rendszerben | `eloadas_07` §2 (Tokola); `eloadas_05` §4 (self-service vs. IT-centrikus), §1, §8; `eloadas_06` §6–7 (Power BI-funkciók, GE Predix); eszközszintű lépések nincsenek | ⚠️ |
| R8 | A DAX-kifejezések szerepe | – | ❌ |
| R9 | Egyéni és vállalati vizualizációk | – (kapcsolódó, nem válasz: `eloadas_05` §4 self-service vs. IT-centrikus; az R9 értelmezése nyitott, lásd lent) | ❌ |
| R10 | Megosztás vállalaton belül és kívül | – (kapcsolódó: `eloadas_03` §7 intranet/extranet; `eloadas_04` §4 FASMI „shared”) | ❌ |
| R11 | Adminisztrációs jogosultságok és engedélyezés | – (kapcsolódó: `eloadas_05` §4 „ki mit lát”; `eloadas_04` §6 CIO/CSO/CPO/CKO/CDO, §7 single source of truth) | ❌ |

### V10 — OLTP/OLAP, adattárház, KDD, adatbányászat, szakértői rendszerek, tudás, Big Data

| R | Részkérdés | Forrás (fájl §) | Állapot |
|---|---|---|---|
| R1 | Az OLTP–OLAP különbség | `eloadas_04` §4 (táblázat, FASMI); `eloadas_07` §3 | ✅ |
| R2 | Az adattárház szerepe és jelentősége (R2a döntéstámogatás ✅; R2b BI-architektúra ⚠️) | `eloadas_04` §5, §7, §2, §6; **+** `eloadas_05` §2 (adatpiac = Focused, EDW = Strategic; ETL a BICC IT-kompetenciái között); réteges architektúra-leírás nincs | ✅ / ⚠️ |
| R3 | A KDD iteratív folyamata | `eloadas_07` §4 (lépések, GIGO); az „iteratív” jelleg nincs a kötelező részben (csak 7.13, opcionális) | ⚠️ + `CSAK OPCIONÁLIS` |
| R4 | A tudásfeltárás és az adatbányászat kapcsolata | `eloadas_07` §3–4, §6 (CRISP-DM mint a KDD ipari változata), §9; `eloadas_08` §5 | ✅ |
| R5 | A leggyakoribb adatbányászati technikák | `eloadas_07` §4–8 (számítások/Bayes/F1/ROC csak a Haladó Könyvben) | ✅ |
| R6 | A szakértői rendszerek struktúrája | `eloadas_09` §7 (szöveges ábra-helyőrző: felhasználói felület – következtető motor – tudásbázis, a tudásbázis négy típusa); **+** `eloadas_11` §3; működés nincs kifejtve | ⚠️ |
| R7 | A tudás informatikai kezelésének módszerei | `eloadas_09` §3–6, §8–10 | ✅ |
| R8 | A VIR-hez kapcsolódó szakértői rendszerek előnyei és korlátai | `eloadas_09` §7–8; **+** `eloadas_11` §3 (átláthatóság, szabályba írt torzítás); VIR-kapcsolatot egyik előadás sem mondja ki | ⚠️ |
| R9 | A Big Data lehetőségei és kihívásai | `eloadas_08` §2–10; a három dimenzió (volumen, sebesség, változatosság) szövegesen §3 és §5; a „3V” címke/definíció csak 8.13 (opcionális) | ✅ lehetőségek/kihívások, ⚠️ definíció + `CSAK OPCIONÁLIS` |

## Tartalmi hiányok

A „nincs” megállapítás teljes szöveges keresésre épül (mind a 12 előadás **kötelező része**, ékezetes/ékezet nélküli alak, szóhatáron; 2026-11-06-án az új kivonatokon újra lefuttatva — a korábbi, 25 HTML-re épülő eredmény változatlan). **Jóváhagyott kezelés: A) beszerzés** mindegyik sorra (Döntési napló, K3).

| # | Tétel / R | Mit kér | Mit találtam | Keresett kifejezések (kötelező rész) | Állapot / kezelés |
|---|---|---|---|---|---|
| G1 | V6 R5 | pénzügyi mutatók | PV, NPV, IRR, ROI (`eloadas_01` §7), TCO, KPI/OEE | `penzugyi mutato` (1: ea01 §7), `roi`, `npv`, `irr`, `tco` (több), `du pont` (0) | ⚠️ — A (beszerzés) |
| G2 | V6 R6 | EVA, Z-score, mutatószámrendszer | semmi | `eva`, `z-score`, `altman`, `mutatoszam`, `du pont`: mind 0 | ❌ — A (AVIR) |
| G3 | V6 R7 | műszaki menedzseri célok, mélység | csak általános szintézis (`eloadas_06` §8, `eloadas_07` §8) | `programcsomag` (0) | ⚠️ — A |
| G4 | V7 R1–R2 | BSC filozófia, négy nézőpont | `eloadas_06` §5: négy perspektíva megnevezve + kritika; a részletes tárgyalás csak 6.15 (K1=A: nem használható) | `balanced scorecard`/`bsc` (6.2, 6.4, 6.5, 6.8, 6.9, 7.2, 7.8), `nezopont` | ⚠️ — A |
| G5 | V7 R4–R5 | hazai programcsomagok, sorbaállítás | semmi | `programcsomag`, `qlik`, `tableau`, `cognos`, `looker`, `fabric`, `sap bw`: 0 (a `sap` ERP-esetekben: ea01, ea03) | ❌ — A |
| G6 | V7 R6–R7 | beépített BSC, rendszerválasztási szempont | semmi | `bsc` + rendszer-kontextus: 0; `strategiai terkep` (6.5: 1) | ❌ — A |
| G7 | V8 R2 | VIR–BI különbség | semmi (külön-külön szerepelnek) | `vir` (11 sor, mind ea01), `vezetoi informacios` (5), `business intelligence`/`uzleti intelligencia` (11); VIR/MIS/EIS/ESS és BI egy sorban: 2 | ❌ — A |
| G7b | V8 R1 | a BI szó szerinti definíciója | nincs a kötelező részben (csak 5.10, opcionális) | `business analytics` (0) | ⚠️ — munkadefiníció + A |
| G7c | V8 R3 | BICC kialakítási szempontjai | mikor kell, mit felel, három terület, self-service/IT-centrikus határ; lépéssor, elhelyezés, létszám nincs | `data steward` (0), `uzleti elemzo` (0) | ⚠️ — A |
| G8 | V9 R2, R4 | dashboard-típusok, szűrők | semmi tipológia; szűrés csak szűrt riport / slice-dice formában | `dashboard` (37 sor), `muszerfal`/`iranyitopult` (0), `slicer` (0) | ❌ / ⚠️ — A (gyakorlati anyag) |
| G9 | V9 R8 | DAX | semmi | `dax` (0), `calculated`, `calculate`, `sumx` (0) | ❌ — A (Power BI doc) |
| G10 | V9 R9–R11 | egyéni/vállalati vizualizáció, megosztás, jogosultság | semmi Power BI-kontextusban | `custom visual`, `row-level`, `rls`, `workspace`, `munkaterulet`, `tenant` (0); `jogosultsag` (1: `eloadas_10` §8, felhő) | ❌ — A (Power BI doc) |
| G11 | V10 R6, R8 | szakértői rendszer struktúrája, VIR-kapcsolat | szöveges ábra-helyőrző (`eloadas_09` §7); VIR-kapcsolat nincs | `szakertoi rendszer`, `tudasbazis` (4), `kovetkeztet` | ⚠️ — A (Bencsik) |
| G12 | V10 R3 | a KDD iteratív jellege | a lépések megvannak; „iteratív” csak 7.13 (opcionális) | `iterativ`, `ciklikus`, `spiral` (0 KDD-kontextusban) | ⚠️ — dőlt megjegyzés + A |
| G13 | V10 R9 | Big Data definíció, 3V | három dimenzió szövegesen; „3V” és definíció csak 8.13 (opcionális) | `3v` (0), `velocity`, `variety` (0) | ⚠️ — dőlt megjegyzés + A |
| G14 | V10 R2b | BI-architektúra | elemei külön; réteges leírás nincs | `adattarhaz` (9), `etl` (1: BICC) | ⚠️ — dőlt megjegyzés |

A K1=A következménye: a `CSAK OPCIONÁLIS` jelölésű sorok (V7 R1–R2, V8 R1, V10 R3, V10 R9) hiányként kezelendők, amíg kötelező szintű forrás nem érkezik.

**Nyitott értelmezési kérdések (a V9 kidolgozásból):** (a) R9 „egyéni és vállalati vizualizációk” — szűk (Power BI custom/organizational visuals, hiány) vagy tág (self-service vs. IT-központi jelentés, részben fedett az `eloadas_05` §4-ben) értelmezés; a V9 a szűkebbet választotta. (b) `eloadas_06` §4: a 75%-os OEE-t a szöveg „világszínvonalúnak” mondja, miközben a „world class” OEE ugyanott ~85% — forráson belüli feszültség, a tétel nem veszi át a 75%-os minősítést.

## Beszerzendő anyagok (összesítve)

| Szerző | Mű | Jelleg | Indoklás / érintett rész |
|---|---|---|---|
| Bángi-Magyar, A. et al. | AVIR kézikönyv (Digitális Tankönyvtár) | ajánlott irodalom | V6 R6 (G2); V7 R1–R3 (G4). A tartalom nem ellenőrzött, a syllabus-cím alapján feltételezett. |
| Microsoft | Power BI documentation (2025) | kötelező irodalom | V9 R8 (G9), R9–R11 (G10) |
| Óbudai Egyetem (gyakorlatvezető) | Power BI gyakorlati anyagok, Excel dashboard, Power BI Service | gyakorlati anyag | V9 R2–R4, R7, R9–R11 (G8, G10) |
| Bencsik, A. | Tudásmenedzsment elméletben és gyakorlatban (2015, 2024) | ajánlott irodalom | V10 R6–R8 (G11) |
| Laudon, K. C., & Laudon, J. P. | Management information systems: Managing the digital firm (17th ed., 2022) | kötelező irodalom | V8 R1–R2 (BI-definíció, VIR–BI); V10 R2b, R3, R9 (G12–G14). Tartalma nem ellenőrzött. |
| Turban, E., Pollard, C., & Wood, G. | Information technology for management (11th ed., 2018) | kötelező irodalom | V8 R1–R2. Tartalma nem ellenőrzött. |

G1, G3, G5–G7 pótlására a syllabus egyik műve sem rendelhető egyértelműen; a K3=A szerint ezekhez a felhasználó helyez be anyagot (forrás megnevezése nyitott). A Chikán (2008) *Vállalatgazdaságtan* ajánlott irodalom egyik részkérdéshez sincs rendelve (tartalma nem ellenőrzött).

## A kivonatokban hivatkozott külső művek és kiadás-eltérések

A hivatkozott művek tartalma **nem használható**; másodlagos hivatkozásként a szerző és az év megadható (K6=A); ha a kivonat évszámot nem ad, „é. n.”.

- **Laudon & Laudon:** a kivonatok a 15. (2017/2018) és a 18. (2025) kiadásra hivatkoznak (`eloadas_01`, `02`, `06`–`12`), a syllabus a 17. kiadást (2022) nevezi meg. **Forrásütközés**, nem oldható fel: kiadás-specifikus szám-, ábra- és fejezetszám nem vehető át.
- **Turban:** `eloadas_03` a 3. kiadásra (2002) hivatkozik; a syllabus a 11. kiadást (2018) nevezi meg. Ugyanez a szabály.
- **V6–V10-hez kapcsolódó külső hivatkozások:** Kaplan & Norton (1996), Goodhart (1975), Thomas & Uminsky (2022) — `eloadas_06`; Tokola et al. (2016), Fayyad, Piatetsky-Shapiro & Smyth (1996), Chapman et al. (2000, CRISP-DM; a 7.9 átvezetőben), Press (2016) — `eloadas_07`; McAfee & Brynjolfsson (2012), Gartner (2015/2018), Mayer-Schönberger & Cukier (2013), Davenport & Harris (2017), Ellram (1993) — `eloadas_08`; Nonaka & Takeuchi (1995; a SECI név és a kvadránsok csak 9.13-ban, opcionális), Grieves & Vickers (2017) — `eloadas_09`; Gartner BI- és BICC-modell, bimodális IT, Dietvorst et al. (2015) — `eloadas_05`.
- **„Saját anyag” típusú hivatkozások** (a kivonatra adandó, a külső mű nem nevezhető meg): `eloadas_05` („EA2 saját anyag”, „saját dilemma”, „saját szintézis”), `eloadas_06` („OEE gyáripari szakirodalom”), `eloadas_07` („saját anyag (MIS_BIG_DATA.pdf)”, „saját üzleti forgatókönyv”), `eloadas_09` (Iván Cs., Tick A. előadásanyag), `eloadas_11` (MIS_KMS.pdf).
- A „Forrás:” sorok az egyes szakaszok végén találhatók.

## Terminológia

- Az `eloadas_01` „MIR/VIR” megfogalmazást használ (§4); a §3 táblázata szerint a MIS a taktikai szint rendszere („menedzsment IS”), a DSS taktikai/stratégiai, az ESS/EIS stratégiai. Önálló VIR-definíció nincs; a „VIR” szó a kötelező részben kizárólag az 1. előadásban fordul elő (§4, §5, §7).
- A VIR-rövidítés ütközik a **V11–V15 tárggyal** (GMXIV2MBLF; a rövidítés ottani jelentését ez a fájl nem rögzíti): a V6–V10 tételekben a VIR kizárólag a GMXIR1MBLF anyaga szerint értelmezhető; V11–V15 anyagából tartalom nem vehető át, csak utalás („lásd V12”).
- **K4=C szerint:** a V6-ban a „MIR/VIR” együttes megfogalmazás marad, a kapcsolat külön jelölve; egyenlőségjelet a tétel nem tesz, amit a forrás nem mond ki.
- **K7 szerint:** az IS-típusok szintezése az `eloadas_01` §3 szövegét és táblázatát követi.

## Hivatkozás a tételekben (K2 szerint)

Szerző: Óbudai Egyetem, Keleti Károly Gazdasági Kar, Üzleti Tudományok és Digitális Ismeretek Intézet (első előfordulásnál `[ÓE KGK ÜTDI]`, utána `ÓE KGK ÜTDI`). Szövegközi: `(ÓE KGK ÜTDI, 2026c, 5. szakasz)` — a betű az Irodalomban címsorrendben tételfájlon belül oszlik ki; `K. szakasz` = a `(forrás: N.K.html)` szerinti oldalszám. Másodlagos hivatkozás: `(Kaplan & Norton, 1996, idézi: ÓE KGK ÜTDI, 2026c, 5. szakasz)`; az Irodalomban csak a kivonat-forrás szerepel (`[Kötelező tananyag, N. ea.]`). Részletes szabály: `Tétel kidolgozó sub-agent prompt - GMXIR1MBLF V08-V10.md` 3.3.

## Döntési napló

| Dátum | Kérdés | A felhasználó válasza |
|---|---|---|
| 2026-10-02 | K1 — Opcionális források | **A:** csak a kötelező tananyag (Kötelező Könyv); az Opcionális és a Haladó Könyv a tételekben nem használható. |
| 2026-10-02 | K2 — Hivatkozási forma | Válasz: „C” (a K2 lehetséges válaszai: A) jóváhagyás, B) módosítás — a C nem definiált). **Rendezve:** a hivatkozási forma a V06/V07 kidolgozásakor jóváhagyásra került (sub-agent prompt 3.3, „jóváhagyott, kötelező”); lásd az előző szakaszt. |
| 2026-10-02 | K3 — Tartalmi hiányok kezelése | **A:** beszerzés (G1–G11, az A2 jelentés számozása szerint; G7b–G14 a 2026-11-06-i kiegészítés, ugyanezen kezeléssel). |
| 2026-10-02 | K4 — Terminológia | **C:** a V6-ban a „MIR/VIR” együttes megfogalmazás marad, a kapcsolat külön jelölve. |
| 2026-10-02 | K5 — Terjedelem (V8–V10) | **B:** táblázatos tömörítés az irányérték megtartásával. |
| 2026-10-02 | K6 — Másodlagos hivatkozások | **A:** használhatók `(szerző, év, idézi: <forrás>, <év>, <szakasz>)` formában; az Irodalomban csak a kivonat-forrás szerepel. |
| 2026-10-02 | K7 — IS-típusok szintezése (forrásütközés) | **Elfogadom:** az `eloadas_01` §3 szövege és táblázata a mérvadó; a hivatkozatlan képek nem használhatók. |
| 2026-10-02 | K8 — BICC kompetenciaterületei (forrásütközés) | **Elfogadom:** a szöveg (három kompetenciaterület) követendő, az ábra eltérését jelezni kell (a kivonatban az ábra csak `[kép]`; a hat terület szövegből nem ellenőrizhető). |
| 2026-10-02 | K9/1 — két zip-only `image.png` | **Elég jelezni:** külön vizsgálat nem szükséges. *(2026-11-06: a zip és a két variáns a mappából megszűnt, a pont tárgytalan.)* |
| 2026-10-02 | K9/2 — ChatGPT-kép (OEE dashboardok) | **Tananyag.** *(2026-11-06 pontosítás: a kép a `7.2_files/` mappában van, a 7. előadás 2. szakaszához tartozik.)* |
| 2026-10-02 | K10 — hiányzó promptfájl | A `Tétel revíziós prompt - GMXIR1MBLF tananyag-feldolgozás.md` fájlt a felhasználó visszahelyezte; a README-hivatkozás javítása nem szükséges. |
| 2026-11-06 | `MIR_*` hallgatói jegyzetek | **Nem tananyag** (a V08–V10 futtatásnál hozott döntés; Dénes utólag felülbírálhatja). |
| 2026-11-06 | Az 1. előadás 1.10–1.13 oldalai | **Opcionálisként kezelve** (a V09 D1 döntése; Dénes utólag felülbírálhatja — ha kötelezőnek minősül, a V9 R5 és a V6 R2 forrásbázisa bővül). |
