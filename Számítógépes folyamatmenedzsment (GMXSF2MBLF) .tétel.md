# Számítógépes folyamatmenedzsment (GMXSF2MBLF) — Tételkidolgozás

**Tételsor:** Vállalatirányítási szakirány (V1–V5)  
**Forrás:** Novák Géza: Számítógépes folyamatmenedzsment (2026); OMG BPMN 2.0 specifikáció

---

## V1 – Az üzleti folyamatmenedzsment (BPM) életciklusa és a BPMS rendszerek felépítése

**Tételkérdés:** Ismertesse a folyamatmenedzsment életciklusának szakaszait és a támogató informatikai rendszerek (BPMS) alapvető összetevőit! Értelmezze a BPMS hídszerepét az üzleti és informatikai oldal között!

---

### 1.1. A BPM fogalma

Az üzleti folyamatmenedzsment (Business Process Management, BPM) olyan irányítási szemlélet, amely a szervezet működését egymáshoz kapcsolódó folyamatok rendszereként vizsgálja és fejleszti. A BPM nemcsak folyamatábrák készítését jelenti, hanem teljes irányítási ciklust: a folyamatok azonosítását, modellezését, végrehajtását, mérését és folyamatos javítását (Dumas et al., 2018).

A modern szervezetekben a BPM szorosan összekapcsolódik az informatikával: a folyamatok zöme ERP-, CRM-, raktárkezelő vagy dokumentumkezelő rendszerekben zajlik. A BPM informatikai támogatására fejlesztették ki a BPMS-rendszereket.

### 1.2. A BPM életciklusa

A BPM életciklusa nem egyszeri projektet, hanem ismétlődő fejlesztési kört jelent. Az alábbi öt szakasz épül egymásra:

```
  ┌─────────────────────────────────────────┐
  │                                         │
  ▼                                         │
TERVEZÉS ──► MODELLEZÉS ──► VÉGREHAJTÁS     │
                                │           │
                          MONITOROZÁS       │
                                │           │
                          OPTIMALIZÁLÁS ────┘
```

| Szakasz | Fő feladatok |
|---|---|
| **Tervezés** | Folyamatok azonosítása; folyamatgazdák kijelölése; stratégiai célok és KPI-k meghatározása |
| **Modellezés** | Vizuális folyamatleírás (BPMN, folyamatábra, értékáram-térkép); szimuláció |
| **Végrehajtás** | Manuális, félautomata vagy teljesen automatizált működtetés; BPMS-ben való indítás |
| **Monitorozás** | KPI-adatok gyűjtése; dashboardok; valós idejű felügyelet; eltérések azonosítása |
| **Optimalizálás** | Szűk keresztmetszetek megszüntetése; TO-BE folyamat bevezetése; Lean, Six Sigma, RPA |

A ciklus alapelve: az optimalizálás befejezése után a folyamat visszakerülhet a tervezési vagy modellezési szakaszba. Ez biztosítja a folyamatos fejlesztést, amely a BPM egyik sarokköve (Harmon, 2019).

### 1.3. BPMS – a BPM informatikai eszköztára

A Business Process Management Suite (BPMS) olyan integrált szoftverkörnyezet, amely az összes életciklus-szakaszt támogatja. Négy fő komponensből áll:

```
┌──────────────────────────────────────────────────┐
│                    BPMS                          │
│  ┌─────────────┐  ┌─────────────┐               │
│  │Folyamat-    │  │ Végrehajtó  │               │
│  │modellező    │  │   motor     │               │
│  │ eszköz      │  │(process     │               │
│  │(BPMN 2.0)  │  │ engine)     │               │
│  └─────────────┘  └─────────────┘               │
│  ┌─────────────┐  ┌─────────────┐               │
│  │  Üzleti     │  │ Szabály-    │               │
│  │  analitika  │  │ kezelő      │               │
│  │(dashboards) │  │  modul      │               │
│  └─────────────┘  └─────────────┘               │
└──────────────────────────────────────────────────┘
```

**Folyamatmodellező eszköz:** Grafikus felületen teszi lehetővé a BPMN 2.0-alapú modellek létrehozását. Az üzleti szakemberek programozói tudás nélkül is részt vehetnek a folyamatok tervezésében.

**Végrehajtó motor (process engine):** A folyamatmodell „lelke": elindítja a példányokat, kiosztja a feladatokat, kezeli a határidőket és döntési pontokat, kapcsolódik más rendszerekhez.

**Üzleti analitika:** KPI-mérés, riportok, dashboardok, trendek és eltérések elemzése. Ebből indul ki az optimalizálás.

**Szabálykezelő modul (Business Rules Management):** Az üzleti döntési logika (pl. értékhatár-alapú jóváhagyás) elkülönítése a programkódtól, rugalmas módosíthatóság érdekében.

### 1.4. A BPMS hídszerepe

A BPMS kulcsértéke, hogy összekötő szerepet tölt be az üzleti és IT oldal között. Az üzleti oldal folyamatalapú igényeket fogalmaz meg (gyorsabb ügyintézés, kevesebb hiba), az IT pedig rendszerekben gondolkodik. A folyamatmodell mindkét fél számára érthető közös nyelv: az üzleti oldal validálja a logikát, az IT oldal megvalósítja automatizálva.

**Összegzés:** A BPM életciklus (Tervezés→Modellezés→Végrehajtás→Monitorozás→Optimalizálás) ciklikus és folyamatos. A BPMS ennek informatikai infrastruktúrája, amelynek négy komponense (modellező, motor, analitika, szabálykezelő) együttesen teszi lehetővé a folyamatok irányítását, mérését és fejlesztését.

---

## V2 – Üzleti folyamatok modellezése BPMN 2.0 szabvány szerint

**Tételkérdés:** Mutassa be a BPMN 2.0 jelölésrendszer legfontosabb elemeit és a folyamatok strukturálásának lehetőségeit! Ismertesse az alapvető objektumtípusokat, a szervezési elemeket és az összekötő elemeket!

---

### 2.1. A BPMN célja és szerepe

A BPMN (Business Process Model and Notation) az Object Management Group (OMG) által standardizált folyamatmodellezési jelölésrendszer. Célja, hogy egységes vizuális nyelvet biztosítson az üzleti elemzők, folyamatgazdák és informatikusok között. A 2.0-s verzió (2011) végrehajtható modellek készítését is lehetővé teszi.

### 2.2. Alapvető objektumtípusok

#### Események

Az események valamilyen történést jelölnek és körrel ábrázolhatók:

| Eseménytípus | Jelölés | Példa |
|---|---|---|
| Start esemény | Vékony vonalú kör | „Vevői rendelés beérkezett" |
| Közbenső esemény | Kettős vonalú kör | „Aláírt szerződés megérkezett" |
| Vég esemény | Vastag vonalú kör | „Rendelés teljesítve" |

Speciális start/vég típusok: üzenet, időzítő, hiba, jel, eszkaláció.

#### Tevékenységek

A tevékenységek lekerekített sarkú téglalappal ábrázolt munkalépések:

- **Feladat (Task):** A folyamat legkisebb önálló munkalépése (pl. „Számla ellenőrzése")
- **Alfolyamat (Sub-process):** Több lépésből álló tevékenység, amely kibontható; az áttekinthetőség megőrzése érdekében hasznos

A tevékenység neve mindig cselekvést fejezzen ki (ige + főnév, pl. „Rendelés rögzítése").

#### Átjárók (Kapuk)

Az átjárók rombusz alakú döntési, elágazási vagy összesítési pontok:

| Átjárótípus | Jelölés | Logika |
|---|---|---|
| Exkluzív (XOR) | Rombusz (X jel) | Pontosan egy ág fut le |
| Párhuzamos (AND) | Rombusz (+ jel) | Minden ág egyszerre fut |
| Inkluzív (OR) | Rombusz (O jel) | Egy vagy több ág futhat le |

**Példa – rendelés feldolgozása:**
```
[Rendelés beérkezett] ──► [Rendelés ellenőrzése] ──► <Készleten van?>
                                                        │           │
                                                      IGEN         NEM
                                                        │           │
                                              [Kiszállítás]  [Beszerzés]
                                                        │           │
                                                        └─────┬─────┘
                                                       [Rendelés lezárva]
```

### 2.3. Szervezési elemek: medencék és sávok

**Medence (Pool):** Egy önálló résztvevőt vagy szervezetet jelöl. Pl. „Vállalat", „Ügyfél", „Beszállító". Külön medencékbe kerülnek azok a felek, amelyek egymással kommunikálnak, de belső folyamataik egymástól függetlenek.

**Sáv (Lane):** A medencén belüli felelősségi köröket jelöli. Pl. Értékesítés | Pénzügy | Raktár | Logisztika. Megmutatja, hogy melyik szervezeti egység felel az egyes tevékenységekért.

```
┌─────────────────────────────────────────────────┐
│ VÁLLALAT                                        │
│  ┌───────────────────────────────────────────┐  │
│  │ Értékesítés  │ [Rendelés rögzítése]       │  │
│  ├──────────────┼───────────────────────────┤  │
│  │ Raktár       │ [Készlet ellenőrzése]      │  │
│  ├──────────────┼───────────────────────────┤  │
│  │ Pénzügy      │ [Számla kiállítása]        │  │
│  └───────────────────────────────────────────┘  │
└─────────────────────────────────────────────────┘
```

### 2.4. Összekötő elemek és használati szabályaik

| Összekötő | Jelölés | Hol használható | Mire való |
|---|---|---|---|
| **Szekvenciafolyam** | Folytonos nyíl | Medencén belül | A folyamatlépések sorrendje |
| **Üzenetfolyam** | Szaggatott nyíl | Medencék között | Szervezetek közötti kommunikáció |
| **Asszociáció** | Pontozott vonal | Bárhol | Dokumentumok, adatok, megjegyzések csatolása |

Alapszabály: szekvenciafolyam nem léphet át medencehatárokon; medencék között csak üzenetfolyamot szabad használni.

### 2.5. Strukturálási lehetőségek

A BPMN lehetővé teszi a folyamatok hierarchikus strukturálását: főfolyamat + alfolyamatok, különböző részletezettségi szintek (vezetői szintű áttekintés vs. operatív munkautasítás). Jó BPMN-modell ismérvei: áttekinthető, egységes elnevezések, feliratozottak az átjárók, jól meghatározott kezdet és vég.

**Összegzés:** A BPMN 2.0 három alapobjektum-típusból épül fel: esemény (kör), tevékenység (lekerekített téglalap), átjáró (rombusz). A szervezési elemek (medence, sáv) a felelősségi köröket mutatják, az összekötők (szekvencia, üzenet, asszociáció) az elemek kapcsolatait adják meg.

---

## V3 – Üzleti folyamatok mérése és optimalizálása

**Tételkérdés:** Elemezze a folyamatok hatékonyságának mérési lehetőségeit és az optimalizáláshoz vezető módszertani lépéseket! Értelmezze a KPI meghatározásának szerepét, a szimuláció jelentőségét és az AS-IS/TO-BE elemzés logikáját!

---

### 3.1. Miért kell mérni?

Amit nem mérünk, nem tudjuk irányítani. A mindennapi szervezeti életben megjelenő szubjektív megállapítások („lassú az ügyintézés", „sok a hiba") önmagukban nem elegendők fejlesztési döntések megalapozásához. Szükség van számszerű, célértékkel összehasonlítható mutatókra.

### 3.2. KPI – kulcsfontosságú teljesítménymutató

A KPI (Key Performance Indicator) olyan mérhető mutató, amely a folyamat kritikus teljesítményterületeire vonatkozik. Jó KPI jellemzői:

- kapcsolódik a folyamat céljához
- mérhető, célértékkel összehasonlítható
- felelőshöz rendelhető
- fejlesztési intézkedést válthat ki

**KPI-típusok és példák:**

| Kategória | Példa KPI-k |
|---|---|
| **Időalapú** | Ciklusidő, átfutási idő, várakozási idő, jóváhagyási idő |
| **Minőségi** | Hibaarány, selejtarány, újramunka aránya, visszaküldött rendelések |
| **Hatékonysági** | Egy ügyre jutó munkaidő, egy ügyre jutó költség, kapacitáskihasználtság |
| **Ügyfélközpontú** | Ügyfél-elégedettség, határidőre teljesítés aránya, panaszok száma, SLA-teljesülés |

KPI akkor igazán hasznos, ha célérték is kapcsolódik hozzá: pl. „a panaszok 95%-át 5 munkanapon belül le kell zárni."

### 3.3. Szűk keresztmetszetek és folyamatszimuláció

A **szűk keresztmetszet (bottleneck)** olyan folyamatlépés, ahol torlódás alakul ki, és amely az egész folyamat teljesítményét korlátozza. Azonosítása monitorozási adatokból (átfutási idők, feladatvárakozási listák) vagy szimulációból történhet.

A **folyamatszimuláció** lehetővé teszi a folyamat előzetes modellezését különböző feltételek mellett (mennyiség, kapacitás, valószínűségek megadásával), anélkül hogy a valós rendszert meg kellene változtatni. Kérdések, amelyekre választ adhat:

- Mi történik, ha 20%-kal nő a beérkező ügyek száma?
- Hány ügyintéző szükséges a határidők teljesítéséhez?
- Csökken-e az átfutási idő, ha egy lépést automatizálunk?

### 3.4. Az optimalizálás lépései

```
AS-IS elemzés          Problémaelemzés        TO-BE tervezés
(jelenlegi állapot) ──► (gyökérokok)      ──► (jövőbeli modell)
        │                                            │
        └──────────────────────────────────────────►┘
                    Visszamérés (KPI-összehasonlítás)
```

**1. AS-IS elemzés:** A jelenlegi folyamat feltárása: lépések, felelősök, döntési pontok, dokumentumok, időadatok, problémák. Fontos a munkatársak bevonása.

**2. Problémaelemzés és gyökérokok:** Az 5 Miért (5 Why) módszer alkalmazásával a tünettől eljutunk az okig. Pl.: „Késnek a jóváhagyások → manuális e-mail-továbbítás → nincs standardizált workflow → nincs folyamatgazda."

**3. TO-BE folyamat:** A javított folyamat modellje, amelybe beépíthetők: felesleges lépések elhagyása, párhuzamosítás, automatizálás, rendszerintegráció, egyszerűsített jóváhagyás.

**4. Visszamérés:**

| Mutató | AS-IS | TO-BE cél | Mért eredmény |
|---|---|---|---|
| Átlagos átfutási idő | 6 nap | 3 nap | 3,2 nap |
| Hibaarány | 5% | 2% | 1,8% |
| Határidőre teljesítés | 78% | 95% | 93% |
| Egy ügyre jutó költség | 4200 Ft | 3000 Ft | 3100 Ft |

Ha az eredmények eltérnek a céltól, újabb elemzési kör indul – ez biztosítja a BPM ciklikus jellegét.

**Összegzés:** A folyamatmérés KPI-kon alapul, amelyek idő-, minőségi, hatékonysági és ügyfélközpontú dimenziókban értékelhetők. Az optimalizálás az AS-IS elemzéstől a gyökérok-azonosításon és TO-BE modelltervezésen át a visszaméréssel zárul.

---

## V4 – Kockázatkezelés és hibamód-elemzés (FMEA) a folyamatokban

**Tételkérdés:** Mutassa be a folyamatokhoz kapcsolódó kockázatok elemzésének módszertanát, különös tekintettel az FMEA alkalmazására! Ismertesse az RPN számítási módját és a kockázatcsökkentő intézkedések logikáját!

---

### 4.1. Kockázat a folyamatmenedzsmentben

A kockázat olyan bizonytalan esemény, amely bekövetkezése esetén negatívan befolyásolja a folyamat eredményét. A folyamatkockázat azt jelenti, hogy a folyamat nem a tervezett minőségben, nem időben vagy nem a várt költségen teljesít.

### 4.2. Az FMEA módszer

Az FMEA (Failure Mode and Effects Analysis – hibamód- és hatáselemzés) szisztematikus, proaktív kockázatkezelési módszer. Célja a hibák előzetes azonosítása, hatásaik értékelése és kockázatcsökkentő intézkedések kidolgozása — mielőtt a hiba bekövetkezne.

**Két fő típus:**
- **DFMEA** (Design FMEA): Termék vagy szolgáltatás tervezési kockázatai
- **PFMEA** (Process FMEA): Folyamatlépések lehetséges hibái → **a folyamatmenedzsmentben ez az elsődleges**

### 4.3. Az FMEA módszertani lépései

```
Folyamat    Hibamódok    Hibahatások    Hibaokok
kijelölése ──► azonosítása ──► meghatározása ──► azonosítása
                                                     │
                                             Kontrollok feltárása
                                                     │
                                              RPN számítás
                                                     │
                                       Intézkedések kidolgozása
                                                     │
                                            Visszamérés (új RPN)
```

### 4.4. A kockázati prioritási szám (RPN)

Az FMEA értékelési mutatója az RPN (Risk Priority Number – kockázati prioritási szám):

$$\text{RPN} = S \times O \times D$$

| Tényező | Angol | Tartalom | Skála |
|---|---|---|---|
| **S** | Severity (Súlyosság) | A hiba következménye, ha bekövetkezik | 1–10 |
| **O** | Occurrence (Előfordulás) | Milyen valószínűséggel fordulhat elő | 1–10 |
| **D** | Detection (Észlelhetőség) | Mennyire nehéz időben észlelni (10 = szinte észrevehetetlen) | 1–10 |

**Skálák összefoglalása:**

| Értéktartomány | Súlyosság (S) | Előfordulás (O) | Észlelhetőség (D) |
|---|---|---|---|
| 1–2 | Csekély hatás | Ritka, kivételes | Szinte biztosan észlelhető |
| 5–6 | Érezhető probléma, ügyfél érintett | Közepes valószínűség | Részleges kontroll |
| 9–10 | Kritikus, jogi/biztonsági kár | Rendszeresen előfordul | Szinte felismerhetetlen |

### 4.5. Az FMEA táblázat

| Folyamatlépés | Hibamód | Hibahatás | Hibaok | Kontroll | S | O | D | RPN | Intézkedés |
|---|---|---|---|---|---|---|---|---|---|
| Panasz rögzítése | Hiányos adatok | Kivizsgálás késik, ügyfél elégedetlen | Nem kötelező mezők | Ügyintézői ellenőrzés | 6 | 7 | 5 | **210** | Kötelező mezők + auto figyelmeztetés |
| Számla rögzítése | Rossz költséghely | Pénzügyi eltérés | Manuális kiválasztás | Utólagos ellenőrzés | 7 | 5 | 6 | **210** | Legördülő lista, validáció |
| Belső űrlap kitöltése | Kisebb formai hiba | Adminisztratív javítás | Nincs sablon | Kézi ellenőrzés | 2 | 6 | 3 | **36** | Sablon bevezetése |

### 4.6. Kockázatcsökkentő intézkedések és visszamérés

Az intézkedések három irányban hatnak:
- **O csökkentése:** Automatizálás, képzés, szabványosítás, rendszerintegráció
- **D javítása:** Automatikus validáció, ellenőrzőlista, jóváhagyási pontok, audit
- **S csökkentése:** Ritkán csökkenthető, a következmény adott (pl. egészségügyi kockázatnál)

Az intézkedések után az S, O, D értékeket újra kell becsülni, és kiszámítani az új RPN-t. Ha pl. az eredeti RPN = 210, az intézkedések után (S=6, O=3, D=3) → **RPN = 54**, a kockázat jelentősen csökkent.

**Fontos:** Az RPN mechanikusan nem alkalmazható. Ha S = 10, az a hiba kritikus figyelmet igényel alacsony RPN esetén is.

**Az FMEA és BPM kapcsolata:** Az FMEA beépül a BPM életciklusba: tervezésnél a kockázatok előzetes azonosítása, végrehajtásnál kontrollpontok, monitorozásnál kockázati KPI-k, optimalizálásnál intézkedések.

**Összegzés:** Az FMEA proaktív kockázatkezelési módszer. Az RPN = S × O × D képlet alapján rangsorolja a kockázatokat. A kockázatcsökkentő intézkedések végrehajtása és visszamérése zárja le a ciklust.

---

## V5 – Folyamatszemléletű irányítási rendszerek és dokumentáció

**Tételkérdés:** Értelmezze a folyamatközpontú megközelítést a minőségirányítási rendszerekben (MIR) és a kapcsolódó dokumentációs követelményeket! Mutassa be a teknős-elemzést, a folyamatleltárt, a KPI és PDCA ciklus összefüggését!

---

### 5.1. Folyamatszemlélet a minőségirányításban

A minőségirányítási rendszer (MIR) – legismertebb szabványa az ISO 9001:2015 – a folyamatszemléletű megközelítést alapelvként rögzíti. Lényege: a szervezet tevékenységeit nem osztályok elszigetelt feladataiként, hanem egymáshoz kapcsolódó folyamatok rendszereként értelmezi.

Egy vevői rendelés teljesítése például érinti az ügyfélszolgálatot, értékesítést, pénzügyet, raktárt, logisztikát és számlázást. Ha minden szervezeti egység csak a saját részfeladatát optimalizálja, az nem feltétlenül javítja a teljes folyamatot.

**A folyamatok négy fő kategóriája MIR-ben:**

| Típus | Példák |
|---|---|
| Vezetési folyamatok | Stratégiai tervezés, célok meghatározása, vezetőségi átvizsgálás |
| Főfolyamatok | Termékfejlesztés, gyártás, rendelésfeldolgozás, kiszállítás |
| Támogató folyamatok | HR, IT, pénzügy, karbantartás, dokumentumkezelés |
| Mérési és fejlesztési folyamatok | Belső audit, vevői elégedettség mérése, helyesbítő intézkedések |

### 5.2. A folyamatleltár

A folyamatleltár a szervezet folyamatainak rendszerezett felsorolása – az egész MIR kiindulópontja. Megmutatja, milyen folyamatok léteznek, milyen kategóriába tartoznak, és ki felel értük.

| Folyamat neve | Típus | Folyamatgazda | Fő kimenet |
|---|---|---|---|
| Vevői rendelés kezelése | Főfolyamat | Értékesítési vezető | Teljesített rendelés |
| Belső audit | Fejlesztési folyamat | Minőségügyi vezető | Auditjelentés |
| Munkatársak képzése | Támogató folyamat | HR vezető | Képzett munkatárs |
| Vezetőségi átvizsgálás | Vezetési folyamat | Ügyvezető | Fejlesztési döntések |

### 5.3. A teknős-elemzés (Turtle Diagram)

A teknős-elemzés a folyamatok átfogó szabályozási és elemzési eszköze. A diagram középen a vizsgált folyamatot tartalmazza, körülötte hat dimenzió helyezkedik el:

```
                    ┌─────────────┐
                    │  BEMENETEK  │
                    │ (Mi indítja?)│
                    └──────┬──────┘
                           │
  ┌──────────────┐         ▼         ┌──────────────┐
  │  KIKKEL?     │  ┌────────────┐   │   MIVEL?     │
  │ (Szereplők,  ├─►│ FOLYAMAT  │◄──┤ (Erőforrások,│
  │ felelősök)  │  │  NEVE      │   │  rendszerek) │
  └──────────────┘  └─────┬──────┘   └──────────────┘
                           │
  ┌──────────────┐         ▼         ┌──────────────┐
  │  HOGYAN?     │         │         │  MÉRÉSEK?    │
  │ (Módszerek,  │    ┌────┴─────┐   │  (KPI-k)     │
  │ szabályzatok)│    │ KIMENETEK│   └──────────────┘
  └──────────────┘    └──────────┘
```

**Panaszkezelési folyamat teknős-elemzése:**

| Elem | Tartalom |
|---|---|
| **Folyamat** | Ügyfélpanasz kezelése |
| **Bemenetek** | Beérkezett panasz, ügyféladatok, vásárlási adatok |
| **Kimenetek** | Kivizsgált panasz, ügyfélválasz, helyesbítő intézkedés, lezárt ügy |
| **Kikkel?** | Ügyfélszolgálat, minőségügy, szakmai terület, folyamatgazda |
| **Mivel?** | CRM rendszer, dokumentumkezelő, e-mail, panaszűrlap |
| **Hogyan?** | Panaszkezelési szabályzat, adatvédelmi előírás, határidő-szabály |
| **Mérések** | Átfutási idő, határidőre lezárt ügyek aránya, ismételt panaszok száma |

A teknős-elemzés nem helyettesíti a BPMN-modellt, de kiváló kiegészítője: a BPMN a sorrendet, a teknős az operatív feltételrendszert mutatja meg.

### 5.4. KPI és a PDCA ciklus kapcsolata

A **PDCA (Plan–Do–Check–Act)** Deming ciklusa a folyamatos fejlesztés alapmodellje a MIR-ben:

```
         ┌────────────────────────────────────────┐
         │                                        │
    PLAN ──► DO ──► CHECK ──► ACT ─────────────────┘
    (Tervez)  (Végrehajt)  (Ellenőriz)  (Beavatkozik)
```

| PDCA szakasz | KPI-k szerepe |
|---|---|
| **Plan** | KPI-célértékek meghatározása (pl. 95% határidőn belüli panaszlezárás) |
| **Do** | Folyamat működik, KPI-adatok gyűlnek |
| **Check** | KPI-mérés: tényleges értékek összehasonlítása a céllal |
| **Act** | Ha az eltérés fennáll: helyesbítő intézkedés, folyamatmódosítás, új ciklus |

### 5.5. Dokumentációs követelmények

A MIR dokumentáció két rétegből áll:

**Szabályozó dokumentumok** (mit kell tenni):
- Folyamatleltár, folyamatleírás, munkautasítás, szabályzat, ellenőrzőlista, BPMN-modell

**Bizonyító feljegyzések** (mit tettünk):
- KPI-riportok, auditjelentések, helyesbítő intézkedések nyilvántartása, vezetőségi átvizsgálási jegyzőkönyvek

A dokumentáció leggyakoribb hibái: túlzott formalizmus (csak auditon elővett papírok), túlzott részletezettség (senki nem használja), elavult tartalom (változás után nem frissítik).

**Összegzés:** A folyamatszemléletű MIR a folyamatokat rendszerként kezeli. A folyamatleltár adja az áttekintést, a teknős-elemzés az operatív feltételeket, a KPI-k a mérhetőséget, a PDCA ciklus pedig a folyamatos fejlesztés keretét biztosítja.

---

*Forrás: Novák Géza – Számítógépes folyamatmenedzsment, oktatási segédanyag (2026); Dumas, M. et al.: Fundamentals of Business Process Management (2018, Springer); OMG: BPMN 2.0 specifikáció (2013)*
