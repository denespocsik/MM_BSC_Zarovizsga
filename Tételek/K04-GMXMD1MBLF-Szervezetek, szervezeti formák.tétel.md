## K4. Szervezetek, szervezeti formák

**Tétel:** „Mi a különbség a munkaszervezet és a tulajdonosi szervezet között? Ismertesse a szervezetek működését meghatározó strukturális jellemzők (munkamegosztás, hatáskör megosztás, koordináció) alapján a főbb szervezeti típusokat!"

### Munkaszervezet és tulajdonosi szervezet

A szervezeten belül két párhuzamos struktúra létezik, amelyeket nem szabad összekeverni.

**Tulajdonosi szervezet (tőkestruktúra):** A tulajdon, a tőke és az érdekeltség rendje. Ki a részvényes, ki dönt a stratégiai irányról, ki kap osztalékot. A Kft.-ben a taggyűlés, a Zrt.-ben a közgyűlés és az igazgatóság a kulcsszereplők.

**Munkaszervezet (funkcionális struktúra):** Az operatív feladatok elosztásának rendje — ki kinek a beosztottja, ki milyen feladatot lát el, hogyan koordinálódnak az egységek. Ez az, amit szervezeti ábra (*organogram*) ábrázol.

A két struktúra elvben különválik: a tulajdonos nem feltétlenül menedzser, a menedzser nem feltétlenül tulajdonos. A kis- és középvállalkozásokban azonban sok esetben összefonódnak.

### Mechanikus és organikus szervezet

**Tom Burns és G. M. Stalker** (1961) különbséget tett mechanikus és organikus szervezetek között:

| | Mechanikus | Organikus |
|---|---|---|
| Környezet | Stabil | Dinamikus, változó |
| Struktúra | Merev, hierarchikus | Rugalmas, hálózatos |
| Kommunikáció | Vertikális (felülről le) | Horizontális, informális |
| Szabályozás | Írott szabályok | Értékek, kultúra |
| Példa | Közigazgatás, gyáripar | IT-startup, kutatóintézet |

### Strukturális jellemzők

A munkaszervezet három alapvető strukturális jellemző mentén írható le:

**1. Munkamegosztás:** A feladatok részfeladatokra bontása és személyekhez/egységekhez rendelése. Minél mélyebb a specializáció, annál hatékonyabb lehet az egyes feladat elvégzése — de annál nehezebb a koordináció.

**2. Hatáskörmegosztás:** Ki dönthet, ki utasíthat kit?
- **Centralizáció:** a döntések a csúcson összpontosulnak — egységes irány, de lassú reakcióidő
- **Decentralizáció:** a döntések közel kerülnek a végrehajtóhoz — rugalmas, de koordinációt igényel

**3. Koordináció típusai:**
- *Vertikális (hierarchikus):* a felsőbb szint irányítja az alsóbbat utasításokkal és szabályokkal
- *Horizontális:* azonos szintű egységek közötti egyeztetés (bizottságok, teamek, projektcsoportok)
- *Technokratikus:* szabályok, eljárások, normák közvetítik a koordinációt (pl. ISO-standardok)
- *Személyorientált (kulturális):* közös értékek, szocializáció, bizalom tartja össze a szervezetet

### Lineáris szervezet

A legegyszerűbb forma. Minden szintnek egy felettese van; az utasítások egyértelműen fentről lefelé haladnak.

```mermaid
graph TD
    VIG("<b>Vezérigazgató</b>")
    UVA("<b>Üzemvezető A</b>")
    UVB("<b>Üzemvezető B</b>")
    MA("Munkások")
    MB("Munkások")

    VIG --> UVA
    VIG --> UVB
    UVA --> MA
    UVB --> MB

    classDef vigNode fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px,color:#4a148c;
    classDef uvNode  fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1;
    classDef mNode   fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20;

    class VIG vigNode;
    class UVA,UVB uvNode;
    class MA,MB mNode;

    linkStyle 0,1 stroke:#7b1fa2,stroke-width:2px;
    linkStyle 2,3 stroke:#1565c0,stroke-width:2px;
```

**Előnyök:** Egyértelmű felelősség, gyors döntéshozatal, átlátható.
**Hátrányok:** A vezető túlterhelt (minden hozzá fut); rugalmatlan nagyobb szervezetben.
**Mikor jó:** Kis szervezetekben, stabil, egyszerű feladatkörnyezetben.

### Funkcionális szervezet

A munkamegosztás szaktevékenységek (funkciók) szerint történik. A beosztottak több, szaktudás szerint illetékes felettestől is kaphatnak utasítást.

```mermaid
graph TD
    VIG("<b>Vezérigazgató</b>")
    HR("<b>HR</b>")
    PE("<b>Pénzügy</b>")
    MK("<b>Marketing</b>")
    TE("<b>Termelés</b>")
    LO("<b>Logisztika</b>")
    D("Dolgozók<br/>funkció szerint megosztva")

    VIG --> HR
    VIG --> PE
    VIG --> MK
    VIG --> TE
    VIG --> LO
    HR  --> D
    PE  --> D
    MK  --> D
    TE  --> D
    LO  --> D

    classDef vigNode  fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px,color:#4a148c;
    classDef funcNode fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1;
    classDef dNode    fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20;

    class VIG vigNode;
    class HR,PE,MK,TE,LO funcNode;
    class D dNode;

    linkStyle 0,1,2,3,4 stroke:#7b1fa2,stroke-width:2px;
    linkStyle 5,6,7,8,9 stroke:#1565c0,stroke-width:2px;
```

Sok szervezetben a funkcionális struktúrát **törzskarral** egészítik ki: a vezető mellé szakértő tanácsadói csoportot rendelnek (pl. jogi osztály, controlling), amely nem utasíthat, csak tanácsol.

**Előnyök:** Magas szakmai színvonal, gazdaságos specializáció.
**Hátrányok:** „Silóhatás" — az egységek egymástól elszigetelten dolgoznak; Fayol egységes utasítás elvének sérülése.

### Divizionális szervezet

Nagy, diverzifikált szervezetekben alkalmazzák. Az egységeket (*divíziókat*) tárgyi elv szerint szervezik:

- **Termék szerint:** minden divízió egy termékcsaládért felelős (pl. Unilever: élelmiszer, tisztítószer, személygondozás)
- **Vevő/piac szerint:** különböző vásárlói szegmensek (pl. B2B vs. B2C divízió)
- **Földrajzi régió szerint:** területi önállóság (pl. európai, ázsiai, amerikai divízió)

```mermaid
graph TD
    H("<b>Holding / Anyavállalat</b>")
    A("<b>A divízió</b><br/>önálló P&L, saját funkciókkal")
    B("<b>B divízió</b><br/>önálló P&L, saját funkciókkal")
    C("<b>C divízió</b><br/>önálló P&L, saját funkciókkal")

    H --> A
    H --> B
    H --> C

    classDef holdingNode fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px,color:#4a148c;
    classDef divANode    fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1;
    classDef divBNode    fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20;
    classDef divCNode    fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100;

    class H holdingNode;
    class A divANode;
    class B divBNode;
    class C divCNode;

    linkStyle 0,1,2 stroke:#7b1fa2,stroke-width:2px;
```

**Előnyök:** Rugalmasság, piachoz közeli döntéshozatal, az egységek teljesítménye jól mérhető.
**Hátrányok:** Erőforrás-duplikáció, koordináció az egységek között nehéz.

### Mátrix szervezet

A funkcionális és a projektalapú/divizionális szervezet keresztezése. Kettős alárendeltség: minden dolgozónak van egy funkcionális főnöke (pl. mérnöki osztályvezető) és egy projekt- vagy termékfelelőse.

```mermaid
graph TD
    VIG("<b>Vezérigazgató</b>")

    MKT("<b>Marketing vez.</b><br/>funkcionális fej")
    MER("<b>Mérnöki vez.</b><br/>funkcionális fej")
    PEN("<b>Pénzügyi vez.</b><br/>funkcionális fej")
    APV("<b>A projekt vez.</b><br/>koordinátor")
    BPV("<b>B projekt vez.</b><br/>koordinátor")

    MA("MKT munkatárs<br/>A projektben")
    MB("MKT munkatárs<br/>B projektben")
    MEA("Mérnök<br/>A projektben")
    MEB("Mérnök<br/>B projektben")
    PA("Pénzügyes<br/>A projektben")
    PB("Pénzügyes<br/>B projektben")

    VIG --> MKT
    VIG --> MER
    VIG --> PEN
    VIG --> APV
    VIG --> BPV

    MKT -->|"szakmai utasítás"| MA
    MKT -->|"szakmai utasítás"| MB
    MER -->|"szakmai utasítás"| MEA
    MER -->|"szakmai utasítás"| MEB
    PEN -->|"szakmai utasítás"| PA
    PEN -->|"szakmai utasítás"| PB

    APV -.->|"projektkoordináció"| MA
    APV -.->|"projektkoordináció"| MEA
    APV -.->|"projektkoordináció"| PA
    BPV -.->|"projektkoordináció"| MB
    BPV -.->|"projektkoordináció"| MEB
    BPV -.->|"projektkoordináció"| PB

    classDef vigNode  fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px,color:#4a148c;
    classDef funcNode fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1;
    classDef projNode fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100;
    classDef empNode  fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20;

    class VIG vigNode;
    class MKT,MER,PEN funcNode;
    class APV,BPV projNode;
    class MA,MB,MEA,MEB,PA,PB empNode;

    linkStyle 0,1,2,3,4 stroke:#7b1fa2,stroke-width:2px;
    linkStyle 5,6,7,8,9,10 stroke:#1565c0,stroke-width:2px;
    linkStyle 11,12,13,14,15,16 stroke:#ef6c00,stroke-width:2px,stroke-dasharray:5 5;
```

**Előnyök:** Rugalmas erőforrás-allokáció, szakmai és projektszemlélet egyszerre érvényesül.
**Hátrányok:** A kettős alárendeltség konfliktushoz vezet; az egységes utasítás elve sérül; sok koordinációs energiát emészt fel.

**Mikor jó:** Dinamikus, projektalapú iparágakban (szoftver, építőipar, tanácsadás, K+F).

### Mintzberg szervezeti konfigurációi

**Henry Mintzberg** (1979) empirikus alapon azonosította, hogy a szervezetek a valóságban öt alaptípus egyikéhez hasonlítanak, amelyeket az összetevők (csúcs, operatív mag, középvonal, technostruktúra, támogató stáb) eltérő súlya határoz meg:

| Konfiguráció | Domináns összetevő | Koordinációs mechanizmus | Tipikus példa |
|---|---|---|---|
| **Egyszerű struktúra** | Csúcsvezetés | Közvetlen felügyelet | Kisvállalat, startup |
| **Gépi bürokrácia** | Technostruktúra | Munkafolyamatok standardizálása | Tömeggyártó, bank |
| **Szakmai bürokrácia** | Operatív mag | Készségek standardizálása | Kórház, egyetem |
| **Diverzifikált forma** | Középvonal | Outputok standardizálása | Holding, konszern |
| **Adhokrácia** | Támogató stáb | Kölcsönös alkalmazkodás | K+F labor, tanácsadó cég |

A konfiguráció-elmélet üzenete: nincs univerzálisan legjobb szervezeti forma — az illeszkedés (*fit*) a környezettel és a stratégiával döntő.

---
