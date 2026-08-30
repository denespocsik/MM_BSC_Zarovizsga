## V2 – Üzleti folyamatok modellezése BPMN 2.0 szabvány szerint

**Tétel:** Üzleti folyamatok modellezése BPMN 2.0 szabvány szerint: Mutassa be a BPMN 2.0 jelölésrendszer legfontosabb elemeit és a folyamatok strukturálásának lehetőségeit! Alapvető objektumtípusok; Szervezési elemek szerepe a felelősségi körök kijelölésében; Az összekötő elemek és használati szabályaik.

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
```mermaid
flowchart LR
    S(["🟢 <b>Rendelés beérkezett</b>"]):::zoldH --> E["📋 <b>Rendelés ellenőrzése</b>"]:::kek
    E --> G{"❓ <b>Készleten van?</b>"}:::sarga
    G -- Igen --> K["🚚 <b>Kiszállítás</b>"]:::kek
    G -- Nem --> B["🛒 <b>Beszerzés</b>"]:::narancs
    K --> End(["🏁 <b>Rendelés lezárva</b>"]):::zoldH
    B --> End

    classDef kek     fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef zoldH   fill:#e8f5e9,stroke:#2e7d32,stroke-width:3px,color:#1b5e20,rx:10,ry:10;
    classDef narancs fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;
    classDef sarga   fill:#fffde7,stroke:#f9a825,stroke-width:2px,color:#f57f17,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
```

### 2.3. Szervezési elemek: medencék és sávok

**Medence (Pool):** Egy önálló résztvevőt vagy szervezetet jelöl. Pl. „Vállalat", „Ügyfél", „Beszállító". Külön medencékbe kerülnek azok a felek, amelyek egymással kommunikálnak, de belső folyamataik egymástól függetlenek.

**Sáv (Lane):** A medencén belüli felelősségi köröket jelöli. Pl. Értékesítés | Pénzügy | Raktár | Logisztika. Megmutatja, hogy melyik szervezeti egység felel az egyes tevékenységekért.

```mermaid
flowchart TD
    subgraph VALLALAT["🏢 VÁLLALAT — Pool"]
        subgraph Ert["💼 Értékesítés — Lane"]
            A["📝 <b>Rendelés rögzítése</b>"]:::kek
        end
        subgraph Rakt["📦 Raktár — Lane"]
            B["🔍 <b>Készlet ellenőrzése</b>"]:::kek
        end
        subgraph Pen["💰 Pénzügy — Lane"]
            C["🧾 <b>Számla kiállítása</b>"]:::kek
        end
    end
    A --> B --> C

    classDef kek fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;

    style VALLALAT fill:#f7f9fa,stroke:#b0bec5,stroke-width:1.5px,color:#546e7a;
    style Ert  fill:#f5f9ff,stroke:#90caf9,stroke-width:1.5px,color:#1565c0;
    style Rakt fill:#f5f9ff,stroke:#90caf9,stroke-width:1.5px,color:#1565c0;
    style Pen  fill:#f5f9ff,stroke:#90caf9,stroke-width:1.5px,color:#1565c0;

    linkStyle default stroke:#546e7a,stroke-width:2px;
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
