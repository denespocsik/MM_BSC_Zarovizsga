## V15 – ERP rendszer és projektmenedzsment, BSP módszertan, ITIL és döntéstámogatás

**Tételkérdés:** Ismertesse, hogyan támogatja az ERP rendszer a projektmenedzsmentet, milyen funkciókat biztosít a projektek tervezéséhez, erőforrás-kezeléséhez, nyomon követéséhez és kontrollingjához! Mutassa be az információs rendszerek szervezési módszereit és a BSP (Business Systems Planning) módszertan lényegét a vállalati ERP stratégia tervezésének kontextusában! Fejtse ki az ERP rendszer működtetésének alapelveit, kitérve az üzemeltetés- és szolgáltatásmenedzsment (ITIL szemlélet) legfontosabb feladataira, és ismertesse, hogyan támogatja az ERP rendszer saját, natív eszközeivel a különböző vezetési szintek döntéshozatalát!

---

### 15.1. Az ERP szerepe a projektmenedzsmentben – az SAP PS modul

Az SAP Project System (PS) modul az ERP-be integrált projektmenedzsment-eszköz. Ellentétben az önálló projektszoftverekkel (pl. MS Project), az SAP PS valós időben kapcsolódik a pénzügyi, kontrolling, anyag- és gyártásirányítási modulokhoz.

**A PS modul stratégiai értéke:**

| Funkció | Tartalom |
|---|---|
| Tervezés | WBS felépítése, hálózati tervek, mérföldkövek, határidők, felelősök rögzítése |
| Erőforrás-kezelés | Emberi és gépi kapacitások ütemezése, kapacitás-ütközések jelzése |
| Nyomonkövetés | Státuszok kezelése (tervezett → kiadott → lezárt), tényleges vs. tervezett összehasonlítás |
| Kontroll | Valós idejű költség-rálátás, budget vs. tényleges adatok, elszámolás (settlement) |
| Integráció | Automatikus könyvelés a FI-ban szállítói számla vagy anyagkivét esetén |

### 15.2. A projekt strukturálása: WBS és hálózati tervek

**WBS (Work Breakdown Structure – Munkalebontási struktúra):**  
A projekt hierarchikus modellje, amely a feladatokat kezelhető egységekre bontja. Minden WBS-elemhez rendelhető: költségkeret, felelős, határidő és mérföldkő.

```
  P/2025 – Ultralight Racing Bike fejlesztés  ← Gyökérelem (WBS 1. szint)
  ├── Engineering (Mérnöki tervezés)           ← WBS 2. szint
  │    ├── Design review
  │    └── Specifikáció véglegesítés
  ├── Prototype (Prototípus gyártás)
  ├── Testing (Tesztelés)
  ├── Small Series Production (Kis széria)
  └── Release to Mass Production
```

**Hálózati tervek (Network Activities):**  
Míg a WBS a feladatok hierarchiáját mutatja, a hálózati terv az időbeli sorrendet és logikai függőségeket ábrázolja (hasonló a Gantt-diagramhoz, de integrálva van a PS modul kapacitástervezésével).

### 15.3. A projekt életciklusa az SAP-ban

```
  TERVEZÉS              VÉGREHAJTÁS           LEZÁRÁS
  ┌────────────┐        ┌────────────┐        ┌────────────┐
  │ WBS, hálózat│       │ Státusz:   │        │ Settlement │
  │ Budget     │→→→→→→→│ REL (kiadva│→→→→→→→│ (költségek │
  │ allokálása │        │ Tényleges  │        │ átvezetése)│
  └────────────┘        │ könyvelések│        └────────────┘
                        └────────────┘
```

A lezárási fázisban a felmerült projektköltségeket **settlement**-tel (elszámolással) vezetik át a végső vevőre (belső vagy külső), biztosítva a teljes pénzügyi transzparenciát.

### 15.4. BSP – Business Systems Planning módszertan

A **BSP** (Business Systems Planning) az IBM által az 1970-es években kidolgozott módszertan az informciórendszerek vállalati stratégiával való összehangolásához. Az ERP stratégiai tervezés kontextusában ma is alkalmazott keretrendszer.

**A BSP alaplogikája:**

```
  Üzleti stratégia
        │
        ▼
  Üzleti folyamatok azonosítása
        │
        ▼
  Adatosztályok meghatározása (milyen adatra van szükség?)
        │
        ▼
  Folyamat–Adat mátrix (Process–Data Matrix)
        │
        ▼
  Informatikai architektúra tervezése (milyen rendszer kell?)
        │
        ▼
  Implementációs prioritások meghatározása
```

**A BSP kapcsolódó módszerei:**

| Módszer | Tartalom |
|---|---|
| **CSF** (Critical Success Factors) | A vállalat sikerkritériumainak azonosítása, amelyekhez az IT-t igazítani kell |
| **Folyamat–Adat mátrix** | Melyik folyamat melyik adatosztályt hozza létre vagy használja? |
| **Entitás-kapcsolat modell** | Az adatosztályok közötti összefüggések feltérképezése |

A BSP napjainkban az SAP Activate és a Solution Manager módszertanokba integrálva él tovább az ERP stratégiai tervezés eszközeként.

### 15.5. ITIL-alapú ERP üzemeltetés

Az **ITIL** (IT Infrastructure Library) az IT-szolgáltatásmenedzsment globális keretrendszere. Az ERP rendszer üzemeltetése – különösen nagyobb szervezetekben – ITIL-folyamatok mentén szerveződik.

**Kulcs ITIL-folyamatok ERP-üzemeltetés kontextusában:**

| ITIL folyamat | Mit jelent ERP esetén? |
|---|---|
| **Incident Management** | ERP leállás, modul-hiba kezelése, SLA-nak megfelelő helyreállítás |
| **Problem Management** | Ismétlődő hibák gyökérok-elemzése (pl. teljesítményprobléma a PP modulban) |
| **Change Management** | ERP frissítések, patch-ek, konfigurációváltozások engedélyezési folyamata |
| **Service Level Management** | ERP rendelkezésre állási és teljesítmény-SLA-k meghatározása és mérése |
| **Release Management** | Új ERP verziók, modulbővítések kontrollált bevezetése |

**Az ERP üzemeltetés alapelvei:**
- **Landscape (rendszertáj) kezelése:** DEV (fejlesztési) → QAS (minőségbiztosítási / teszt) → PRD (éles) rendszer hármas szintű, transzport-folyamattal irányított változtatáskezeléssel.
- **Backup és disaster recovery:** Az ERP adatbázis rendszeres mentése, helyreállítási tervek.
- **Jogosultságkezelés:** Szerepköralapú hozzáférés-vezérlés (RBAC), szegregáció elvének betartása.

### 15.6. Az ERP natív döntéstámogatása a különböző vezetési szinteken

Az SAP S/4HANA beépített (natív) eszközei különböző részletességű és célú információt nyújtanak a három klasszikus vezetési szint számára:

```
  STRATÉGIAI SZINT     │ SAP S/4HANA Fiori analitikus műszerfalak
  (Felsővezetés)       │ BSC-integrált KPI-k, profit-center elemzések
  ─────────────────────┼──────────────────────────────────────────────
  TAKTIKAI SZINT       │ CO modul: költséghelyi riportok, varianciaelemzés
  (Középvezetés)       │ PS modul: projekt-előrehaladás és cost-vs-budget
  ─────────────────────┼──────────────────────────────────────────────
  OPERATÍV SZINT       │ Fiori tranzakciós applikációk: rendelések,
  (Munkatársak)        │ készletlekérdezések, jóváhagyási munkafolyamatok
```

**SAP Embedded Analytics:** Az S/4HANA-ban nincs szükség külön adattárházba exportálni az adatokat az elemzéshez. A CDS (Core Data Services) nézetek és az SAP Analytics Cloud közvetlen kapcsolatban állnak az éles adatbázissal – az elemzés az aktuális, pillanatszintű adatokon alapul.

**Összegzés:** Az ERP rendszer a projektmenedzsmenttől az üzemeltetésen át a döntéstámogatásig egységes platformot nyújt. Az SAP PS modul a projekteket a pénzügyi és kontrolling folyamatokkal integrálja; a BSP módszertan a stratégiai tervezéshez ad keretet; az ITIL az üzemeltetést szervezi; a beágyazott analitika pedig minden szinten valós idejű döntési alapot biztosít.

---

*Forrás: GMXIV2MBLF oktatási segédanyag (2026); PMI: PMBOK Guide, 7th ed. (2021); Axelos: ITIL 4 Foundation (2019); IBM: Business Systems Planning – BSP (1984); Rockart, J.F.: „Chief Executives Define Their Own Data Needs" (HBR, 1979)*
