## V18 – Hálózati működés

**Tétel:** Hálózati működés és szempontjai: Hálózati működés. Mutassa be a vállalati működés hálózatelvű megközelítését! A hálózati működés szempontjai.

---

### 18.1. A hálózatelvű megközelítés szükségessége

A hagyományos vállalatelmélet a szervezetet zárt rendszerként kezeli: a vállalat maga tervez, dönt, termel és értékesít. Ez a szemlélet kielégítő volt, amíg a vállalatok valóban viszonylag önállóan működtek. A 20. század végére azonban a munkamegosztás, a kiszervezés (outsourcing) és az ellátási láncok komplexitása oda jutott, hogy **egyetlen vállalat sem értelmezhető a kapcsolataitól függetlenül.**

A hálózatelvű megközelítés – Håkansson és az IMP csoport nyomán – nem a vállalat belső folyamataira, hanem a vállalat **hálózati pozíciójára** és **kapcsolataira** fókuszál.

```mermaid
flowchart LR
    subgraph HAG["Hagyományos szemlélet"]
        H_I["<b>Input</b>"]:::szurke --> H_F["<b>Folyamat</b>"]:::szurke --> H_O["<b>Output</b>"]:::szurke
        H_NOTE(["Vállalat — zárt rendszer"]):::szurke
    end
    subgraph HAL["Hálózatelvű szemlélet"]
        SZ["<b>Szállítók</b>"]:::zold --- HV["<b>VÁLLALAT</b>"]:::kekH --- VEV["<b>Vevők</b>"]:::narancs
        HV --- P["<b>Partnerek</b><br/>(kutatóintézetek,<br/>versenyzők,<br/>szabályozók...)"]:::lila
    end
    HAG --> HAL

    classDef kekH    fill:#e3f2fd,stroke:#1565c0,stroke-width:3px,color:#0d47a1,rx:10,ry:10;
    classDef zold    fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef narancs fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;
    classDef lila    fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px,color:#4a148c,rx:10,ry:10;
    classDef szurke  fill:#eceff1,stroke:#546e7a,stroke-width:2px,color:#263238,rx:10,ry:10;

    style HAG fill:#f7f9fa,stroke:#b0bec5,stroke-width:1.5px,color:#546e7a;
    style HAL fill:#f5f9ff,stroke:#90caf9,stroke-width:1.5px,color:#1565c0;

    linkStyle default stroke:#546e7a,stroke-width:2px;
```

---

### 18.2. A hálózati működés három szempontja

Håkansson elmélete szerint a hálózatban való működés három szempontból különbözik alapvetően az önálló vállalati működéstől:

#### 1. szempont: Irányíthatóság (Control)

**Hagyományos nézet:** A vezető irányítja a vállalatot, a vállalat irányítja folyamatait.

**Hálózati realitás:** A hálózatban nincs egyetlen szereplő sem, aki az egész rendszert uralna. Minden szereplő befolyásolja a többieket, de senki sem irányítja teljesen a hálózatot. Minél nagyobb és sürűbb a hálózat, annál kisebb az egyes szereplők kontrollja az egész felett.

**Következmény:** A menedzser feladata nem a kontroll maximalizálása, hanem a **hálózati pozíció tudatos alakítása** és a befolyás körének értelmes menedzsmentje.

```mermaid
graph TD
    A["<b>A</b>"]:::kek --- B["<b>B</b>"]:::kek --- C["<b>C</b>"]:::kek
    A --- D["<b>D</b>"]:::kek
    B --- E["<b>E</b>"]:::kekH
    C --- F["<b>F</b>"]:::kek
    D --- E
    E --- F

    NOTE(["Senki sem látja a teljes képet.<br/>Mindenki csak a saját lokális<br/>hálózatát ismeri és befolyásolja."]):::szurke
    E ~~~ NOTE

    classDef kek    fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef kekH   fill:#e3f2fd,stroke:#1565c0,stroke-width:3px,color:#0d47a1,rx:10,ry:10;
    classDef szurke fill:#eceff1,stroke:#546e7a,stroke-width:2px,color:#263238,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
```

#### 2. szempont: Tudás (Knowledge)

**Hagyományos nézet:** A szervezet tud mindent, ami a döntésekhez kell; a tudásmenedzsment a belső folyamat.

**Hálózati realitás:** A hálózatban elosztottan tárolt tudás messze meghaladja bármelyik szereplő egyéni tudását. Az innováció, a problémamegoldás és a kompetenciafejlesztés egyre inkább **kapcsolatokon keresztül** történik – nem belső fejlesztéssel, hanem partnerekkel együtt.

Mark Granovetter (1973) **gyenge kötések elmélete** ehhez szorosan kapcsolódik: az erős kötések (szoros, sürű baráti körök) bezárnak, a gyenge kötések (laza ismeretségek) hídként kötnek össze különböző tudásbázisokat.

| Kapcsolat típusa | Jellemzők | Tudás-transzfer szempontjából |
|---|---|---|
| Erős kötés | Sürű, sok közös kontakt, sok interakció | Redundáns tudás; visszaigazolás, de kevés újdonság |
| Gyenge kötés | Ritka, kevés közös kontakt | Híd különböző információs világok közt; innováció forrása |

**Következmény:** A vállalat kapcsolatai **tudásforrások** – nem csak erőforrás-csere eszközei. A tudás-hálózat menedzselése stratégiai feladat.

#### 3. szempont: Változás (Change)

**Hagyományos nézet:** A változás tervezett, vezérelt folyamat (BPR, szervezetfejlesztés).

**Hálózati realitás:** A hálózatban a változás folyamatos és részben spontán. Bármely szereplő változása hullámokat indít a hálózatban, amelyek nem mindig kiszámíthatók. A hálózat dinamikus egyensúlyi állapotban van, nem statikus struktúra.

```mermaid
flowchart TD
    E1["<b>Vállalat új technológiát vezet be</b>"]:::kek
    E2["<b>Szállítójának adaptálnia kell a csomagolást</b>"]:::zold
    E3["<b>A szállító altermékgyártója is módosít</b>"]:::turkiz
    E4["<b>Versenyző reagál — benchmark</b>"]:::narancs
    E5["<b>Iparági sztenderd változik</b>"]:::lila

    E1 --> E2 --> E3 --> E4 --> E5
    E5 -.->|"visszahat"| E1

    classDef kek     fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef zold    fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef narancs fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;
    classDef lila    fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px,color:#4a148c,rx:10,ry:10;
    classDef turkiz  fill:#e0f2f1,stroke:#00695c,stroke-width:2px,color:#004d40,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
    linkStyle 4 stroke:#c2185b,stroke-width:2px,stroke-dasharray: 5 5;
```

**Következmény:** A hálózatban való változáskezelés nem top-down tervezés, hanem **folyamatos alkalmazkodás** és a hálózati visszacsatolások figyelemmel kísérése.

---

### 18.3. Az ARA modell – tevékenységek, erőforrások, szereplők

Håkansson és az IMP csoport az ARA modellel (Activities–Resources–Actors) írja le az üzleti hálózat három alapvető dimenzióját:

```mermaid
flowchart TD
    SZ["<b>SZEREPLŐK — Actors</b><br/>● Vállalatok, divíziók, személyek<br/>● Erőforrások felett rendelkeznek"]:::kek
    T["<b>TEVÉKENYSÉGEK — Activities</b><br/>● Termelés, fejlesztés, logisztika<br/>● Összekapcsolódó tevékenység-láncok"]:::zold
    E["<b>ERŐFORRÁSOK — Resources</b><br/>● Technológia, tudás, kapcsolatok<br/>● Értéküket a hálózati felhasználás határozza meg"]:::narancs

    SZ <-->|"végzi"| T
    T <-->|"alakítja / felhasználja"| E
    E <-->|"irányítja"| SZ

    classDef kek     fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef zold    fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef narancs fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
```

A három elem egymással szorosan összekapcsolt: a szereplők tevékenységeket végeznek erőforrásokkal, a tevékenységek erőforrásokat alakítanak, az erőforrások a szereplők kontrollja alatt állnak – de nem egyetlen szereplőén, hanem a kapcsolatok hálójában megoszlva.

---

### 18.4. Erős és gyenge kapcsolatok szerepe a vállalati hálózatban

Granovetter elméletét az IMP keretrendszerben alkalmazva:

| Dimenzió | Erős kapcsolat | Gyenge kapcsolat |
|---|---|---|
| Interakció gyakorisága | Magas | Alacsony |
| Bizalom szintje | Magas | Közepes/alacsony |
| Adaptáció mértéke | Magas (kapcsolatspecifikus) | Alacsony |
| Tudás-redundancia | Magas (ugyanaz az info mindkét félnél) | Alacsony (új tudás forrása) |
| Hálózati szerep | Klaszter-kohézió | Hálózati híd (bridging) |
| Stratégiai érték | Stabilitás, megbízhatóság | Innováció, diverzifikáció |

Az optimális hálózati stratégia **vegyes portfólió**: erős kapcsolatok a kulcstevékenységekhez és megbízható ellátáshoz, gyenge kapcsolatok az innovációhoz és piaci szondázáshoz.

---

**Összegzés:** A hálózatelvű megközelítés szerint a vállalat nem zárt rendszer, hanem egy komplex hálózat csomópontja. A hálózati működés három szempontja – irányíthatóság (senki sem uralja teljesen a hálózatot), tudás (elosztott és kapcsolatokon keresztül áramlik) és változás (folyamatos, kaszkád-szerű, nem teljesen tervezett) – alapvetően megváltoztatja a menedzsment feladatát: nem vezérlés, hanem pozicionálás, kapcsolatmenedzsment és alkalmazkodás. Az ARA modell tevékenységek, erőforrások és szereplők hármasában írja le ezt a hálózatot.

---

*Forrás: Håkansson, H. (2010): Határtalan hálózatok. Alinea Kiadó; Granovetter, M. (1973): The Strength of Weak Ties; Dr. Szilágyi Győző Attila, GMXVU2MBLF előadásanyag (2025/26); Barabási Albert-László (2022): Behálózva*
