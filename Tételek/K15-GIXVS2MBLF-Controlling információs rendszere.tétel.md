## K15 – A controlling információs rendszere és a vezetői információmenedzsment

**Tétel:** Controlling információs rendszere: A controlling információs rendszere és a vezetői információmenedzsment. A controlling információs rendszer felépítése. Tervezési és beszámolási rendszer szerepe. Mutatószámok szerepe a controllingban. A controlling mint információmenedzsment rendszer.

---

### A controlling információs rendszer felépítése

A controlling egy **zárt szabályozási körként** működő információs rendszer. Három alrendszer kapcsolódik össze benne:

```mermaid
flowchart TD
    IR["🏛️ <b>IRÁNYÍTÁS</b>"]:::lilaH
    T["📋 <b>Célmeghatározás / Tervezési rendszerek</b><br/>(Éves terv, stratégiai terv, projekttervek)"]:::kek
    V["⚙️ <b>Végrehajtás / Megvalósítás</b><br/>(Tényadatok gyűjtése a vezetői számvitelből)"]:::zold
    E["📈 <b>Elemzés és Beszámolás</b><br/>(Eltéréselemzés, riportok, intézkedési javaslatok)"]:::narancs

    IR --> T
    IR --> V
    IR --> E
    E -->|visszacsatolás| IR

    classDef kek     fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef zold    fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef narancs fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;
    classDef lilaH   fill:#f3e5f5,stroke:#7b1fa2,stroke-width:3px,color:#4a148c,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
    linkStyle 3 stroke:#c2185b,stroke-width:2px,stroke-dasharray: 5 5;
```

A controller feladata: **nem maga tervez**, hanem összefoglalja, konszolidálja és értelmezi a terveket, majd a tényadatokkal szembesíti azokat.

### Vezetői számvitel vs. pénzügyi számvitel

A controlling információs alapja a **vezetői számvitel (management accounting)**, amely lényegesen eltér a kötelező pénzügyi számviteltől (Drury, 2018; Kaplan & Atkinson, 2003):

| Szempont | Pénzügyi számvitel | Vezetői számvitel |
|---|---|---|
| Célközönség | Külső (tulajdonos, állam, hitelező) | Belső (vezetés) |
| Szabályozottság | Számviteli törvény, IFRS | Szabadon kialakítható |
| Időorientáció | Múlt (lezárt időszak) | Múlt + jelen + jövő (terv) |
| Tárgya | A vállalat egésze | Szegmensek, költséghelyek, termékek |
| Fókusz | Pontosság (auditálható) | Relevancia és gyorsaság |
| Periodicitás | Éves/negyedéves, kötött | Igény szerinti (havi, heti, ad hoc) |

### A VIM három funkciója

A **Vezetői Információs Rendszer (VIM / VIR)** három feladatot lát el:

1. **Adatgyűjtés és -tárolás** – az alapbizonylatokból és az operatív rendszerekből.
2. **Adattömörítés és szervezeti egységekhez rendelés** – aggregálás költséghelyekre és felelősségi egységekre.
3. **Döntés-előkészítő számítások** – terv–tény összehasonlítás, eltéréselemzés, előrejelzés.

A modern VIM technológiai megvalósítása az ERP-rendszer controlling modulja (pl. SAP CO).

### Tervezési rendszer

Az operatív tervezés menete (Katona F., 7. ea.):

```mermaid
flowchart TD
    A["🛒 <b>Értékesítési terv</b><br/><i>szűk keresztmetszet — innen indul a tervezés</i>"]:::kekH
    B["🏭 <b>Termelési terv</b><br/>(kapacitástervezés)"]:::kek
    C["🔩 <b>Anyag- és munkabér-terv</b><br/>(közvetlen ktg.)"]:::turkiz
    D["🏢 <b>Általános költségterv</b><br/>(közvetett ktg., overhead)"]:::narancs
    E["📊 <b>Eredményterv</b><br/>(fedezetszámítás alapján)"]:::zold
    F["💰 <b>Pénzügyi terv / Likviditási terv</b>"]:::lila

    A --> B --> C --> D --> E --> F

    classDef kek     fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef kekH    fill:#e3f2fd,stroke:#1565c0,stroke-width:3px,color:#0d47a1,rx:10,ry:10;
    classDef zold    fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef narancs fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;
    classDef lila    fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px,color:#4a148c,rx:10,ry:10;
    classDef turkiz  fill:#e0f2f1,stroke:#00695c,stroke-width:2px,color:#004d40,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
```

A tervezés **szűk keresztmetszettől indul**: az esetek nagy részében a piac (értékesíthetőség) a korlát, ezért az értékesítési terv az egész tervezési ciklus alapja.

**Tervezési megközelítések.** A klasszikus bázisalapú tervezés mellett elterjedt a **nulla bázisú tervezés (ZBB)**, amelynél minden költséget nulláról kell újra igazolni (Pyhrr, 1970); a **gördülő előrejelzés (rolling forecast)**, amely a horizontot folyamatosan görgeti; és a **Beyond Budgeting** (Hope & Fraser, 2003), amely a fix éves költségvetés helyett adaptív, relatív célokat javasol. Mindhárom megközelítés az éves tervezési ciklus merevségére reagál – más-más kompromisszummal a pontosság és a rugalmasság között.

### Beszámolási rendszer

A controlling-riport alapjellemzői:
- **Rendszeresség** – havi, negyedéves, éves zárás
- **Eltérésfókusz** – nem az abszolút számok, hanem a terv–tény különbség és annak oka fontos
- **Akcióorientáltság** – a riport ne csak leírjon, hanem döntési javaslatot is tartalmazzon

### Mutatószámok szerepe

A controlling leggyakoribb mutatószámai két csoportba sorolhatók:

**Pénzügyi mutatók:**

| Mutató | Képlet | Tartalom |
|---|---|---|
| ROI (befektetés-arányos megtérülés) | Nyereség / Befektetett tőke | Tőkehatékonyság |
| ROS (értékesítés-arányos ny.) | Nyereség / Árbevétel | Profitmarzs |
| Tőkeáttétel | Árbevétel / Befektetett tőke | Eszközforgás |
| Likviditás (I. fokozat) | Likvid eszközök / Rövid lej. köt. | Fizetőképesség |

A **Du Pont-rendszer** ezeket hierarchikusan kapcsolja össze: az ROI = ROS × Tőkeáttétel összefüggéssel dekomponálható az eredményre ható tényezők hatása.

**Nem pénzügyi mutatók** (a BSC előzményei):
- Vevőelégedettségi index, reklamációs ráta
- Átfutási idő, készletforgás
- Munkatársi elégedettség, fluktuáció

### A controller mint információmenedzser

A controller legfontosabb tulajdonsága: **az eltéréseket felfedi, értelmezi és megbeszéli** a felelős vezetőkkel. Nem ítél – a terv-tény eltérés nem terhelő bizonyíték, hanem döntési kiindulópont.

> **Irodalom:** Drury, C. (2018). *Management and cost accounting* (10th ed.). Cengage Learning. — Hope, J., & Fraser, R. (2003). *Beyond budgeting*. Harvard Business School Press. — Kaplan, R. S., & Atkinson, A. A. (2003). *Vezetői üzleti gazdaságtan*. Panem. — Pyhrr, P. A. (1970). Zero-base budgeting. *Harvard Business Review, 48*(6), 111–121. — Francsovics, A. (é. n.). *Controlling* [elektronikus tankönyv]. — Katona F.: CONTROLLING 1., 2., 7., 8. ea.

---
