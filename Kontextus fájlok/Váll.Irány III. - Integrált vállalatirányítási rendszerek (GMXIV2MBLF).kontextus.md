# Integrált vállalatirányítási rendszerek (GMXIV2MBLF) — Kontextus

**Tantárgy:** Integrált vállalatirányítási rendszerek  
**Neptun kód:** GMXIV2MBLF  
**Tételek:** V11–V15 (Vállalatirányítási szakirány tételsor)  
**Tantárgyfelelős:** Prof. Dr. habil. Tick Andrea | **Oktató:** Novák Géza  
**Kreditérték:** 4 | **Félév:** 2025/26-2

---

## 1. A tantárgy tárgya és célja

A tárgy az integrált vállalatirányítási rendszerek – elsősorban az SAP S/4HANA – elméletét és gyakorlatát dolgozza fel. A hallgatók megismerik az ERP rendszerek fogalmát, fejlődéstörténetét, szervezeti szerepét, bevezetési módszertanát és üzemeltetési elveit. Kiemelt hangsúlyt kap az SAP moduláris felépítése, az integrált adatáramlás logikája, a projektmenedzsment-támogatás és az ITIL-alapú üzemeltetési szemlélet. A tárgy elvégzéséhez szükséges a SAP Fiori/GUI alapszintű ismerete és 2 SAP challenge teljesítése.

---

## 2. Feldolgozott forrásanyagok

### 2.1. HTML oktatási segédanyagok (ERP rendszerek mappa)

| Fájl | Témakör |
|---|---|
| Integrált vállalatirányítási rendszer fogalma és alapjai.html | ERP definíció, integráltság lényege, MRP→S/4HANA fejlődés, SAP-történet, Fiori navigáció, adattípusok |
| Vállalatirányítási rendszerek.html | ERP evolúció, SAP mérföldkövek, adattípusok (szervezeti, törzs-, tranzakciós), S/4HANA újítások |
| Az integrált VIR szerepe a vállalatok életében.html | Folyamatok racionalizálása, valós idejű adathasználat, új üzleti modellek, „Segment of One", Run Simple filozófia |
| SAP S/4HANA struktúra, felépítés és modulok.html | HANA architektúra, szervezeti egységek, moduláris felépítés (SD, MM, PP, FI, CO, HCM, WM), Intelligent Enterprise vízió |
| Az ERP rendszerek szerepe a szervezeti felépítésben és kultúrájában.html | Folyamatorientált szervezet, hierarchia laposítása, SAP Fiori UX, WM modul esettanulmány |
| BPR az ERP rendszerben.html | BPR fogalma, S/4HANA optimalizációs emelők (Efficiency, Effectiveness, Agility), greenfield vs. brownfield, MRP/PP esettanulmányok |
| Integrált VIR a vállalati információ rendszerében.html | Digitális mag, bizonylati elv, bizonylatfolyam, FI/CO/MM esettanulmányok |
| Projektmenedzsment az ERP rendszerben.html | PS modul, WBS, hálózati tervek, projekt életciklusa, lezárás-settlement, Global Bike esetpélda |
| SAP Leonardo – A digitális innovációs rendszer.html | IoT, ML, Blockchain, Big Data, Design Thinking, iparági megoldások, HCM modul |
| Üzleti Intelligencia kialakítása az ERP rendszerben.html | Embedded Analytics, OLTP vs. OLAP, valós idejű elemzés, CRM/CSM folyamat, prediktív analitika |
| Minőségügymenedzsment integrálása vállalati rendszerekben.html | QM modul, minőségtervezés/ellenőrzés/irányítás, vizsgálati tétel életciklusa |

### 2.2. Oktatási segédanyag PDF

Az „Oktatási segédanyag.pdf" (ERP rendszerek mappa) a tantárgy elméleti keretét adja meg, a HTML anyagok tartalmi alapjaként szolgál. Magába foglalja az ERP architektúra, a modulintegráció és az SAP esetgyakorlatok leírásait.

### 2.3. Gyakorlati_anyag – SAP University Alliance tananyag (Global Bike v4.3)

Az SAP UCC Magdeburg által gondozott „Intro to SAP S/4HANA Using Global Bike" v4.3 (2025. július) kurzuscsomag 16 modult tartalmaz. Szoftverkörnyezet: S/4HANA 2023, Fiori 3.0. Modelltársaság: **Global Bike Group** (GBI) – fiktív kerékpárgyártó, két vállalattal (Global Bike Inc., US; Global Bike Germany GmbH, DE) és több telephellyel (Dallas, Miami, San Diego, Heidelberg, Hamburg, Perth).

| Mappa | Modul | Tartalom |
|---|---|---|
| 01 Introduction | Introduction to SAP S/4HANA | SAP történet, Intelligent Enterprise vízió, adattípusok, szervezeti egységek, deployment (cloud/on-premise), Fiori, átállási forgatókönyvek |
| 02 Navigation | Navigation | Fiori Launchpad, SAP GUI navigáció |
| 03 Global Bike | Global Bike Story | Vállalattörténet, szervezeti felépítés, kulcsfolyamatok (Idea-to-Market, Order-to-Cash, Build-to-Stock) |
| 04 SD | Sales and Distribution | Order-to-Cash folyamat, Sales Area, Customer Master, Material Master, Pricing, Output |
| 05 MM | Materials Management | Procure-to-Pay folyamat, Vendor Master, Purchasing Info Record, Goods Receipt, Invoice Verification |
| 06 PP | Production Planning | MRP, gyártási rendelések, kapacitástervezés |
| 07 FI | Financial Accounting | Szervezeti struktúra (Company Code, CoA, Credit Control Area), G/L, AR, AP, Balance Sheet, Income Statement, Document Principle |
| 08 CO | Controlling | Controlling Area, Operating Concern, Cost Center, Profit Center, Internal Order, Cost Elements (Primary/Secondary) |
| 09 HCM | Human Capital Management | Szervezeti felépítés, személyügyi adminisztráció, bérszámfejtés |
| 10 WM | Warehouse Management | Raktárstruktúra, tárhelyszintű kezelés |
| 11 PS | Project System | WBS-elemek, tevékenységtípusok, mérföldkövek, projekt életciklus, settlement típusok |
| 12 EAM | Enterprise Asset Management | Karbantartásmenedzsment |
| 13 CS | Customer Service | Ügyfélszolgálati folyamatok |
| 14 QM | Quality Management | Minőségtervezés, vizsgálati tételek |
| 15 EHS | Environment, Health & Safety | EHS folyamatok |
| 20 Integrative Case Study | MM + PP + SD | Teljes gyártási és értékesítési folyamat integrált esettanulmánya |

**Kulcstartalmak tételszempontból:**
- **Adattípusok:** Szervezeti adat (Client, Company Code, Plant) / Törzadat (Material, Customer, Vendor) / Tranzakciós adat (Sales Order, PO, Invoice)
- **Bizonylati elv:** Minden tranzakció egyedi sorszámú elektronikus bizonylatot hoz létre, amely nem törölhető
- **Bizonylatfolyam:** A bizonylatok egymáshoz láncolódnak (pl. PO → GR → Invoice → Payment)
- **Adattömörítés:** Hagyományos DB: 593 GB → HANA: 118,6 GB → S/4HANA: 42,4 GB
- **Fiori alkalmazástípusok:** Tranzakciós (create/change/display), Analitikai (vizuális áttekintés), Factsheet (objektum-részletek)
- **S/4HANA átállási forgatókönyvek:** New Implementation (greenfield), System Conversion (brownfield), Landscape Transformation (több forrásrendszer összevonása)
- **PS projekttípusok:** Vevői projekt (Customer project), Általános költségprojekt (Overhead cost project), Beruházási projekt (Investment project)
- **WBS-elem státuszok:** Released (tényleges költség rögzíthető), Unlocked, Technically Complete, Closed (logisztika és FI zárva), Deletion flag, Fully Invoiced
- **Settlement típusok:** Közvetlen elszámolás (Direct: WBS → külső cost object) / Többszintű elszámolás (Multi-level: részelemek → magasabb WBS → végső fogadó)
- **Tevékenységtípusok PS-ben:** Belsőleg feldolgozott (Internally processed), Külső megrendelés (Externally processed), Általános költségtevékenység (General costs)
- **CO Cost Elements:** Elsődleges (Primary – FI kiadásszámlákból eredő), Másodlagos (Secondary – kizárólag CO-ban használt belső átterhelésekhez)
- **Global Bike vállalati struktúra:** Client: GBI → Company Code: US00 / DE00 → Plant: DL00, MI00, SD00, HD00, HH00, PE00 → Sales Organization: US West (UW00), US East (UE00), DE North (DN00), DE South (DS00)

### 2.4. Syllabus – tantárgynyilvántartó (GMXIV2MBLF)

Az ÓE KGK tantárgynyilvántartója alapján az oktatás témái: ERP fogalom, SAP S/4HANA struktúra, VIR szervezeti szerepe, VIR az információs rendszerben, BPR, szervezeti kultúra, BI, QM, projektmenedzsment, SAP Leonardo/HCM, komplex esetpélda.

---

## 3. A tételek forrásainak leképezése

| Tétel | Fő forrás |
|---|---|
| V11 – Informatikai fejlődés és szigetrendszerek | Vállalatirányítási rendszerek.html; VIR fogalma és alapjai.html; Introduction to SAP S/4HANA slides (v4.3) |
| V12 – ERP fogalma és fejlődéstörténete | VIR fogalma és alapjai.html; VIR szerepe a vállalatok életében.html; ERP szervezeti kultúra.html; Introduction slides + Global Bike Story (v4.3) |
| V13 – ERP bevezetése és BPR | BPR az ERP rendszerben.html; VIR fogalma és alapjai.html; Introduction slides – átállási forgatókönyvek (v4.3) |
| V14 – SAP S/4HANA struktúra és modulok | SAP S/4HANA struktúra.html; VIR az információs rendszerben.html; FI, CO, MM, SD, PS slides (v4.3) |
| V15 – ERP projektmenedzsment és üzemeltetés | Projektmenedzsment az ERP rendszerben.html; BI az ERP rendszerben.html; PS slides (v4.3) |

---

## 4. A forrásokban hivatkozott és ajánlott szakirodalom

### 4.1. Kötelező irodalom (syllabus szerint)

- **Hetyei József** (21. sz.): *ERP rendszerek Magyarországon a 21. században.* — A hazai ERP-piac és bevezetési tapasztalatok áttekintése.
- **Tasi Miklós** (2011): *Vállalatirányítási rendszerek.* Edutus Főiskola. [online] dtk.tankonyvtar.hu — Alapvető magyar nyelvű ERP tankönyv, az MRP-től az ERP II-ig.
- **Molnár Bálint** (2014): *Vállalatirányítási rendszerek gazdaságinformatikai megközelítésben.* — Gazdaságinformatikai szemszögből tárgyalja az ERP architektúrát és az integrációs kérdéseket.
- SAP Handbook; support.sap.com; help.sap.com — Hivatalos SAP dokumentáció, modulleírások, best practice útmutatók.

### 4.2. Ajánlott és hivatkozott szakirodalom

#### ERP elmélet és bevezetés

- **Monk, E., Wagner, B.** (2012): *Concepts in Enterprise Resource Planning.* 4th ed. Cengage Learning. — Az ERP fogalmak és a moduláris felépítés leggyakrabban idézett angol tankönyve.
- **Klaus, H., Rosemann, M., Gable, G.G.** (2000): „What is ERP?" *Information Systems Frontiers*, 2(2), 141–162. — Az ERP fogalom tudományos megalapozása.
- **Davenport, T.H.** (1998): „Putting the Enterprise into the Enterprise System." *Harvard Business Review*, 76(4), 121–131. — Az ERP bevezetés szervezeti hatásainak klasszikus elemzése.

#### BPR és folyamatátalakítás

- **Hammer, M., Champy, J.** (1993): *Reengineering the Corporation: A Manifesto for Business Revolution.* HarperBusiness. — A BPR alapmű; a folyamatok gyökeres újratervezésének elmélete.
- **Hammer, M.** (1990): „Reengineering Work: Don't Automate, Obliterate." *Harvard Business Review*, 68(4), 104–112. — A BPR forrása; az automatizálás helyett az újratervezés szükségességét hirdeti.

#### SAP S/4HANA és in-memory technológia

- **Russel, D., Hartley, N.** (2019): *SAP S/4HANA: An Introduction.* SAP Press. — Az S/4HANA architektúra, modulok és a HANA adatbázis ismertetése.
- **Plattner, H., Zeier, A.** (2012): *In-Memory Data Management: Technology and Applications.* Springer. — Az in-memory adatbázis-technológia elméleti alapjai és üzleti alkalmazásai.

#### Projektmenedzsment és ITIL

- **PMI** (2021): *A Guide to the Project Management Body of Knowledge (PMBOK® Guide).* 7th ed. Project Management Institute. — A projektmenedzsment globális szabványa; a PS modul tervezési logikájának alapja.
- **Axelos** (2019): *ITIL 4 Foundation.* TSO. — Az ITIL 4 keretrendszer, az ERP üzemeltetési és szolgáltatásmenedzsment alapja.

#### Információs rendszerek tervezése

- **IBM** (1984): *Business Systems Planning (BSP).* IBM Corporation. — Az információs rendszerek vállalati stratégiához igazításának klasszikus módszertana.
- **Rockart, J.F.** (1979): „Chief Executives Define Their Own Data Needs." *Harvard Business Review*, 57(2), 81–93. — A Critical Success Factors (CSF) módszer alapja, az ERP stratégiai tervezés kiindulópontja.

#### Felhőalapú ERP és digitális transzformáció

- **Gartner** (2023): *Magic Quadrant for Cloud ERP for Product-Centric Enterprises.* Gartner Research. — A felhőalapú ERP piaci szereplők és trendek összehasonlítása.
- **SAP SE** (2023): *Intelligent Enterprise Framework.* SAP Whitepaper. — Az SAP jövőképe: az IoT, ML és S/4HANA integrációja az „Intelligens Vállalat" megvalósításához.

---

## 5. Kulcsfogalmak gyűjteménye

| Fogalom | Rövid definíció |
|---|---|
| ERP | Enterprise Resource Planning – integrált vállalatirányítási rendszer |
| MRP | Material Requirements Planning – anyagszükséglet-tervezés (1960-as évek) |
| MRP II | Manufacturing Resource Planning – gyártási erőforrás-tervezés (1980-as évek) |
| Szigetrendszer | Önálló, nem integrált részlegszintű alkalmazás; adatredundanciát okoz |
| S/4HANA | SAP negyedik generációs ERP platformja, in-memory HANA adatbázison |
| Fiori | SAP szerepkör-alapú, csempe-alapú webes felhasználói felülete |
| WBS | Work Breakdown Structure – munkalebontási struktúra a projektmenedzsmentben |
| BPR | Business Process Reengineering – üzleti folyamatok gyökeres újratervezése |
| ITIL | IT Infrastructure Library – IT-szolgáltatásmenedzsment keretrendszer |
| BSP | Business Systems Planning – vállalati informatikai stratégiatervezési módszertan |
| Embedded Analytics | S/4HANA beágyazott analitika: OLTP és OLAP egy rendszerben, valós időben |
| Greenfield | ERP bevezetés nulla alapról, meglévő folyamatok mellőzésével |
| Brownfield | ERP bevezetés meglévő rendszer migrálásával |
| Digital Core | Az S/4HANA digitális mag: az összes vállalati folyamat integrációs középpontja |
| Global Bike (GBI) | SAP University Alliance oktatási modelltársaság – kerékpárgyártó; US (Dallas) + DE (Heidelberg) telephelyekkel |
| Bizonylati elv | Minden SAP-tranzakció egyedi sorszámú, nem törölhető elektronikus bizonylatot hoz létre |
| Bizonylatfolyam | A bizonylatok láncolata (pl. PO → GR → Szállítói számla → Kifizetés) |
| Sales Area | Értékesítési szervezet + Értékesítési csatorna + Divízió hármasa; az SD-ben az árazás és feltételek kerete |
| Company Code | Önálló jogi számviteli egység az SAP-ban; ezen a szinten készül mérleg és eredménykimutatás |
| Controlling Area | CO szervezeti egység, amely egy vagy több Company Code-ot fog át; a vezetői számvitel kerete |
| Operating Concern | A piaci szegmentáció CO szintű egysége; profitabilitáselemzés alapja (PA) |
| Cost Center | Csak kiadásokért felelős szervezeti egység (pl. karbantartás, másolóközpont) |
| Profit Center | Bevételért és kiadásért egyaránt felelős egység; ROI-alapon értékelt |
| Primary Cost Element | Elsődleges költségelem – FI kiadásszámlából eredő; párhuzamos CO-beli megfelelője |
| Secondary Cost Element | Másodlagos költségelem – kizárólag CO-n belüli belső átterhelésekhez (pl. assessment) |
| WBS-elem (PSP-elem) | A projekt hierarchiájának alapegysége; állapotaival (Released, Closed stb.) nyomkövetés lehetséges |
| Settlement | Projektköltségek elszámolása/átvezetése a végső fogadó cost object-re (közvetlen vagy többszintű) |
| Procurement (P2P) | Procure-to-Pay – a teljes MM-FI folyamatlánc: PR → PO → GR → Invoice → Payment |
| Order-to-Cash (O2C) | Az SD teljes folyamatlánca: Inquiry → Quotation → Sales Order → Delivery → Billing → Payment |
| Purchasing Info Record | MM törzadat: szállító–anyag kapcsolat, árak, szállítási feltételek, utolsó rendelési adatok |
| Greenfield (New Implementation) | ERP bevezetés nulláról; az S/4HANA best practice folyamataira épít; data migration szükséges |
| Brownfield (System Conversion) | Meglévő SAP ECC-rendszer konvertálása S/4HANA-ra; üzleti folyamatok nem szakadnak meg |
| Landscape Transformation | Több forrásrendszer (pl. régiós ERP-ek) összevonása egyetlen S/4HANA-rendszerbe |

---

*Összeállította: Claude (2026-05-09); frissítve: 2026-05-10 – Gyakorlati_anyag (SAP University Alliance v4.3) feldolgozva* – forrás: GMXIV2MBLF oktatási anyagok, tantárgynyilvántartó, kötelező és ajánlott szakirodalom*
