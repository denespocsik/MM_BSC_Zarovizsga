## V19 – Az üzleti kölcsönhatások hálózat alapú megközelítése

**Tétel:** Üzleti kölcsönhatások hálózatalapú megközelítése: Az üzleti kölcsönhatások hálózat alapú megközelítése. Ismertesse a struktúra-alapú és a folyamat-alapú megközelítés kritikáját! Mutassa be a piac hálózatalapú értelmezését!

---

### 19.1. A két klasszikus megközelítés

Az üzleti kapcsolatok és a piac elemzésére két domináns elméleti hagyomány alakult ki, amelyeket Håkansson és az IMP csoport szisztematikusan kritizált:

```mermaid
flowchart TD
    SA["<b>1. STRUKTÚRA-ALAPÚ megközelítés</b><br/>neoklasszikus közgazdaságtan, Porter<br/>A piac statikus adott — a verseny a struktúrában"]:::kek
    FA["<b>2. FOLYAMAT-ALAPÚ megközelítés</b><br/>szervezetelméletek, folyamatmenedzsment<br/>A vállalat belső folyamataiban van az érték"]:::zold
    IMP(["<b>IMP KRITIKA: mindkettő hiányos</b><br/>→ Hálózatalapú megközelítés szükséges"]):::lilaH

    SA --> IMP
    FA --> IMP

    classDef kek   fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef zold  fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef lilaH fill:#f3e5f5,stroke:#7b1fa2,stroke-width:3px,color:#4a148c,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
```

---

### 19.2. A struktúra-alapú megközelítés és kritikája

#### A megközelítés lényege

A struktúra-alapú (structural) megközelítés – amelyet leginkább a neoklasszikus mikroökonómia és Michael Porter versenyerő-modellje képvisel – az üzleti kapcsolatokat piaci struktúrák kontextusában értelmezi:

- A piac egyensúlyi állapot felé tart.
- A szereplők racionális, önérdekkövető döntéshozók.
- A kapcsolatok távolságtartók, tranzakció-orientáltak.
- A versenyhelyzet az iparági struktúra (5 erő) által meghatározott.

```mermaid
flowchart TD
    NB["<b>Új belépők</b><br/>fenyegetése"]:::kek --> V["<b>VÁLLALAT</b>"]:::lilaH
    SZ["<b>Szállítók</b><br/>alkuereje"]:::zold --> V
    VEV["<b>Vevők</b><br/>alkuereje"]:::narancs --> V
    HEL["<b>Helyettesítők</b><br/>fenyegetése"]:::rozsa --> V
    MEG["<b>Meglévő versenyzők</b><br/>rivalizálása"]:::turkiz --> V

    classDef kek     fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef zold    fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef narancs fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;
    classDef rozsa   fill:#fce4ec,stroke:#c2185b,stroke-width:2px,color:#880e4f,rx:10,ry:10;
    classDef lilaH   fill:#f3e5f5,stroke:#7b1fa2,stroke-width:3px,color:#4a148c,rx:10,ry:10;
    classDef turkiz  fill:#e0f2f1,stroke:#00695c,stroke-width:2px,color:#004d40,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
```

#### Az IMP kritika

- **Statikus kép:** A struktúraelemzés pillanatfelvételt ad, de nem magyarázza, hogyan változnak a kapcsolatok időben.
- **Egyirányú tranzakcionalitás:** A vevő–szállító kapcsolatot anonim, egyszeri tranzakcióként kezeli, holott a valóságban tartós, kölcsönösen alakuló kapcsolatokról van szó.
- **Tudás figyelmen kívül hagyása:** A kapcsolat-specifikus tudás, adaptáció és közösen épített kompetenciák nem jelennek meg.
- **Hálózati kontextus hiánya:** Egyetlen vállalat–piac párt vizsgál, nem a vállalat egész kapcsolathálóját.

| Aspektus | Struktúra-alapú | IMP kritika |
|---|---|---|
| Kapcsolat természete | Távolságtartó, anonim | Tartós, személyes, adaptált |
| Idődimenzió | Statikus | Dinamikus, múlttal és jövővel |
| Tudás szerepe | Figyelmen kívül | Kulcserőforrás |
| Piac képe | Aggregált struktúra | Egyedi kapcsolatok hálója |

---

### 19.3. A folyamat-alapú megközelítés és kritikája

#### A megközelítés lényege

A folyamat-alapú (process-based) megközelítés a szervezet belső folyamatait helyezi a középpontba. Az értékteremtés a vállalat belső értéklánca mentén zajlik (Porter értéklánc-modellje), a menedzsment feladata az optimális belső folyamatok kialakítása.

```mermaid
flowchart LR
    subgraph ELS["Elsődleges tevékenységek"]
        BL["<b>Belogisztika</b>"]:::kek --> TER["<b>Termelés</b>"]:::kek --> KL["<b>Kilogisztika</b>"]:::kek --> MK["<b>Marketing</b>"]:::kek --> SZ["<b>Szerviz</b>"]:::kek
    end
    subgraph TAM["Támogató tevékenységek"]
        INF["<b>Infrastruktúra</b>"]:::szurke ~~~ HR["<b>HR</b>"]:::szurke ~~~ TECH["<b>Technológia</b>"]:::szurke ~~~ BES["<b>Beszerzés</b>"]:::szurke
    end

    classDef kek    fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef szurke fill:#eceff1,stroke:#546e7a,stroke-width:2px,color:#263238,rx:10,ry:10;

    style ELS fill:#f5f9ff,stroke:#90caf9,stroke-width:1.5px,color:#1565c0;
    style TAM fill:#f7f9fa,stroke:#b0bec5,stroke-width:1.5px,color:#546e7a;

    linkStyle default stroke:#546e7a,stroke-width:2px;
```

#### Az IMP kritika

- **Bezárt szemlélet:** Az értékteremtést kizárólag a vállalaton belül helyezi el – holott az érték egyre inkább a **vállalatok közötti interakciókban** keletkezik.
- **Elváló be- és kimenet:** A belső folyamat-optimalizáció nem veszi figyelembe, hogy a bemenetek (pl. alapanyag, tudás) a kapcsolatok minőségétől függnek.
- **Nem tükrözi a valóságot:** A modern ellátási láncokban, platformgazdaságokban és innovációs ökoszisztémákban a értékteremtés hálózati folyamat, nem belső.

| Aspektus | Folyamat-alapú | IMP kritika |
|---|---|---|
| Értékteremtés helye | Vállalaton belül | Kapcsolatokban, hálózatban |
| Vállalat határai | Élesek, adottak | Elmosódottak, kapcsolatfüggők |
| Szállítók/vevők szerepe | Input/output | Aktív társalkotók |
| Koordináció | Belső hierarchia | Hálózati kölcsönös alkalmazkodás |

---

### 19.4. A hálózatalapú megközelítés – a piac mint hálózat

Az IMP csoport az üzleti piacokat (B2B markets) nem homogén, anonim versenytérként, hanem **egyedi kapcsolatok hálózataként** értelmezi.

```mermaid
graph LR
    SZ1["<b>Szállító 1</b>"]:::zold --- SZ2["<b>Szállító 2</b>"]:::zold
    SZ1 --- V1["<b>Vállalat 1</b>"]:::kek
    SZ2 --- V1
    SZ2 --- V2["<b>Vállalat 2</b>"]:::kek
    V1 --- V2
    V2 --- V3["<b>Vállalat 3</b>"]:::kek
    V1 --- K1["<b>Vevő 1</b>"]:::narancs
    V2 --- K1
    V2 --- K2["<b>Vevő 2</b>"]:::narancs
    V3 --- K2

    NOTE(["Minden kapcsolat egyedi, tartós,<br/>és befolyásolja a többi kapcsolatot"]):::szurke
    K2 ~~~ NOTE

    classDef kek     fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef zold    fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef narancs fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;
    classDef szurke  fill:#eceff1,stroke:#546e7a,stroke-width:2px,color:#263238,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
```

**A piac mint hálózat legfontosabb következményei:**

1. **Nincs tökéletes verseny** – a piacon valójában egyedi kapcsolatok léteznek, nem homogén tranzakciók. Egy szállítói pozíció nem lecserélhető egyszerűen egy másikra.

2. **Az ár csak az egyik koordináló mechanizmus** – a bizalom, a kölcsönös adaptáció és a kapcsolat-specifikus tudás legalább annyira fontos.

3. **A piaci pozíció = hálózati pozíció** – nem az iparági struktúrában elfoglalt hely, hanem a konkrét kapcsolatok minősége és száma határozza meg a piaci erőt.

4. **Az innováció hálózati folyamat** – az IMP empirikus kutatásai (Håkansson, 1987, 1989) azt mutatták, hogy az ipari innovációk döntő hányada vevő–szállító kapcsolatokban keletkezik, nem zárt laboratóriumokban.

---

### 19.5. Az IMP interakció-modell

A hálózatalapú megközelítés operatív magja az IMP interakció-modell, amely a vevő–szállító kapcsolatot négy dimenzióban írja le:

| Dimenzió | Tartalom |
|---|---|
| Interakciós epizódok | Konkrét ügyletek, tárgyalások, problémamegoldások (termék, pénz, info, szociális csere) |
| Kapcsolat légköre | Hatalom/függőség; konfliktus/kooperáció; bizalom; közelség/távolság |
| Szervezetek és egyének | Az interakció egyszerre szervezeti és személyes szinten zajlik |
| Környezet | Iparági struktúra; dinamizmus; internacionalizáció; szociális rendszer |

```mermaid
flowchart LR
    SZ["<b>SZÁLLÍTÓ</b><br/>szervezet + egyén"]:::zold
    INTER["<b>INTERAKCIÓS FOLYAMAT</b><br/>epizódok · légkör"]:::lilaH
    VEV["<b>VEVŐ</b><br/>szervezet + egyén"]:::narancs
    KON["<b>HÁLÓZATI KONTEXTUS</b><br/>más kapcsolatok hatása"]:::kek

    SZ <--> INTER <--> VEV
    KON --> INTER

    classDef kek     fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef zold    fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef narancs fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;
    classDef lilaH   fill:#f3e5f5,stroke:#7b1fa2,stroke-width:3px,color:#4a148c,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
    linkStyle 2 stroke:#1565c0,stroke-width:2px,stroke-dasharray: 5 5;
```

---

**Összegzés:** A struktúra-alapú megközelítés statikus piaci képe és a folyamat-alapú megközelítés vállalaton belülre zárt értékteremtési logikája egyaránt hiányos, mert figyelmen kívül hagyja az üzleti kapcsolatok tartós, dinamikus és hálózatba ágyazott természetét. Az IMP csoport hálózatalapú megközelítése a piacot egyedi kapcsolatok rendszereként értelmezi, ahol az értékteremtés, az innováció és a koordináció a vállalatok közötti kölcsönhatásokon alapul. A piac mint hálózat szemlélet következménye, hogy a vállalat piaci pozícióját nem az iparági struktúra, hanem a konkrét kapcsolatok minősége és hálózati elhelyezkedése határozza meg.

---

*Forrás: Håkansson, H. (2010): Határtalan hálózatok. Alinea Kiadó; Dr. Szilágyi Győző Attila, GMXVU2MBLF előadásanyag (2025/26); Håkansson, H. – Snehota, I. (1995): Developing Relationships in Business Networks; Porter, M.E. (1980): Competitive Strategy (mint kritika alapja)*
