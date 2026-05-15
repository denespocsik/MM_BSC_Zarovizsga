## K3. Tervezés

**Tétel:** „Mit jelent a cégek esetében a változó környezet, a szervezeti filozófia, a jövőkép, a küldetés, ezek milyen időtávra szólnak? Ismertesse a tervezés lépéseit és eszközeit! Ismertessen a környezet, továbbá a belső erőforrás elemzésére szolgáló módszereket!"

### A változó környezet és a stratégiai tervezés szükségessége

A vállalatok nem légüres térben működnek. A technológia felgyorsul, a fogyasztói szokások átalakulnak, a szabályozási környezet módosul, új versenytársak jelennek meg. Aki csak a napi operatív kérdésekkel foglalkozik, könnyen lejáratja magát. A stratégiai tervezés éppen arra való, hogy a szervezet ne sodródjon, hanem tudatosan alakítsa saját jövőjét.

### Vállalati célhierarchia és időtávok

A szervezeti célok és irányelvek egymásra épülő szintet alkotnak. Minél magasabb a szint, annál általánosabb és annál hosszabb az időtáv.

| Szint         | Időtáv       | Tartalom                          |
| ------------- | ------------ | --------------------------------- |
| Filozófia     | hosszú (10+) | értékek, etika, küldetés szelleme |
| Vízió         | 5–10 év      | gazdasági jövőkép, hova tartunk   |
| Misszió       | 3–5 év       | társadalmi szerep, kinek mit      |
| Célok         | 1–3 év       | konkrét, mérhető eredmények       |
| Stratégia     | 1–3 év       | hogyan érjük el a célokat         |
| Taktika       | 1 év         | részletes cselekvési tervek       |
| Operatív terv | napok–hetek  | napi feladatok                    |

**Szervezeti filozófia:** A legáltalánosabb iránymutatás — az értékek, alapelvek és etikai normák összessége. Nem változik, csak elvétve.

**Vízió (jövőkép):** Gazdasági fókuszú, „hova akarunk eljutni" kérdésre válaszol. Pl. „2030-ra piacvezető akarunk lenni a közép-európai régióban." Inspiráló, de konkrét iránymutatást ad.

**Misszió (küldetés):** Társadalmi fókuszú, „miért létezünk, kinek dolgozunk" kérdésre válaszol. Pl. „Megfizethető, fenntartható megoldásokat nyújtunk kis- és középvállalkozásoknak." A misszió kifelé is kommunikál — a vevőknek és a társadalomnak szól.

**Célok:** Konkrétak, mérhetők, határidőhöz kötöttek (SMART-elvek). A célok lefelé boncolódnak az egyéni szintű feladatokig.

### A tervezés lépései

A stratégiai tervezés nem egyszeri aktus, hanem körfolyamat:

1. **Helyzetfelmérés** — hol tartunk most? (belső és külső elemzés)
2. **Jövőkép meghatározása** — hova akarunk jutni?
3. **Alternatívák kidolgozása** — milyen utakon juthatunk oda?
4. **Választás** — melyik alternatívát valósítjuk meg?
5. **Megvalósítás** — erőforrások allokációja, felelősök kijelölése
6. **Ellenőrzés** — visszacsatolás, eltéréselemzés, korrekció

### Környezetelemzés: PESTEL

A **PESTEL-elemzés** a makrokörnyezet hat dimenzióját térképezi fel:

| Betű | Dimenzió     | Példák                                               |
| ---- | ------------ | ---------------------------------------------------- |
| P    | Politikai    | Kormánystabilitás, adópolitika, jogszabályok         |
| E    | Gazdasági    | GDP-növekedés, infláció, kamatlábak, munkanélküliség |
| S    | Társadalmi   | Demográfia, kulturális trendek, életmód              |
| T    | Technológiai | Digitalizáció, automatizáció, K+F intenzitás         |
| E    | Ökológiai    | Klímaváltozás, erőforrás-korlátok, fenntarthatóság   |
| L    | Jogi         | Munkajog, versenyjog, fogyasztóvédelem               |

### Iparági elemzés: Porter 5 erő modellje

**Michael E. Porter** (1979) szerint egy iparág vonzerejét öt erő határozza meg:

```mermaid
graph TD
    %% Csomópontok definiálása formázott szöveggel
    B("<b>Potenciális belépők</b><br/>Belépési korlátok fenyegetése")
    Sz("<b>Szállítók alkuereje</b>")
    Ve("<b>Vevők alkuereje</b>")
    H("<b>Helyettesítő termékek</b><br/>fenyegetése")
    I("<b>Iparági verseny</b><br/>meglévő versenytársak")

    %% Kapcsolatok
    B --> I
    Sz --> I
    Ve --> I
    H --> I

    %% Stílusok definiálása (classDef)
    %% Központi elem (Iparági verseny) - Lila
    classDef centerNode fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px,color:#4a148c,rx:10,ry:10;
    %% Új belépők - Kék
    classDef topNode fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    %% Szállítók - Zöld
    classDef supplierNode fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    %% Vevők - Narancs
    classDef buyerNode fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;
    %% Helyettesítők - Rózsaszín/Piros
    classDef subNode fill:#fce4ec,stroke:#c2185b,stroke-width:2px,color:#880e4f,rx:10,ry:10;

    %% Stílusok hozzárendelése
    class I centerNode;
    class B topNode;
    class Sz supplierNode;
    class Ve buyerNode;
    class H subNode;

    %% Nyilak formázása (Vastagabb, szürkéskék)
    linkStyle 0,1,2,3 stroke:#546e7a,stroke-width:2px;
```

Minél erősebbek ezek az erők, annál kisebb az iparág jövedelmezősége. Porter elemzése segít megérteni, miért nyereséges az egyik iparág és miért nem a másik.

### Belső elemzés: SWOT

A **SWOT-elemzés** a szervezet belső és külső helyzetét egyidejűleg térképezi fel:

|         | Belső                        | Külső                           |
| ------- | ---------------------------- | ------------------------------- |
| Pozitív | **Strengths** (erősségek)    | **Opportunities** (lehetőségek) |
| Negatív | **Weaknesses** (gyengeségek) | **Threats** (fenyegetések)      |

Az erősségek és gyengeségek belső tényezők (amit a szervezet kontrollál); a lehetőségek és fenyegetések a külső környezetből fakadnak. A SWOT önmagában leíró eszköz — értéke az, ha a négy mező kombinálásával stratégiai irányokat fogalmaznak meg belőle (SO, ST, WO, WT stratégiák).

### Portfolió-elemzés: BCG mátrix

A **BCG mátrix** (Boston Consulting Group) a termék/üzletágportfoliót két dimenzió mentén értékeli: piaci részesedés és piacnövekedési ütem.

```mermaid
%%{init: { 'theme': 'base', 'themeVariables': { 'quadrant1Fill': '#e1f5fe', 'quadrant2Fill': '#fff9c4', 'quadrant3Fill': '#f5f5f5', 'quadrant4Fill': '#e8f5e9', 'quadrant1TextFill': '#01579b', 'quadrant2TextFill': '#f57f17', 'quadrant3TextFill': '#616161', 'quadrant4TextFill': '#1b5e20', 'titleColor': '#263238' } } }%%
quadrantChart
    title BCG Mátrix
    x-axis "Alacsony piaci részesedés" --> "Magas piaci részesedés"
    y-axis "Lassan növő piac" --> "Gyorsan növő piac"
    quadrant-1 "Sztár (cash-semleges)"
    quadrant-2 "Kérdőjel (befektetést igényel)"
    quadrant-3 "Kutya (kivonulás?)"
    quadrant-4 "Fejőstehén (cash-termelő)"
```

- **Sztár:** nagy piaci részesedés, gyorsan növő piacon — jövő nyertesei
- **Fejőstehén:** nagy piaci részesedés, érett piacon — a cég pénzügyi motorja
- **Kérdőjel:** kis részesedés, gyorsan növő piacon — dönteni kell: befektetés vagy kilépés
- **Kutya:** kis részesedés, stagnáló piacon — általában kivonulás a cél

### Ansoff-mátrix

**Igor Ansoff** (1957) a növekedési stratégiákat termék és piac dimenzióiban rendszerezi:

|                    | Meglévő piac     | Új piac        |
| ------------------ | ---------------- | -------------- |
| **Meglévő termék** | Piacbehatolás    | Piacfejlesztés |
| **Új termék**      | Termékfejlesztés | Diverzifikáció |

A diverzifikáció a legnagyobb kockázatú stratégia (sem a termék, sem a piac nem ismert); a piacbehatolás a legkisebb kockázatú (mindkettő ismerős).

---
