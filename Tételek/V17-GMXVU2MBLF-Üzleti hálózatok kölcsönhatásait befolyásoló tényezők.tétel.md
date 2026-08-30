## V17 – Az üzleti hálózatok kölcsönhatásait befolyásoló tényezők

**Tétel:** Üzleti hálózatok kölcsönhatásait befolyásoló tényezők: Az üzleti hálózatok kölcsönhatásait befolyásoló tényezők: a kölcsönhatások időbelisége; szubjektív értelmezés; kapcsoltság; kölcsönös függőség; viszonylagosság.

---

### 17.1. Az üzleti kölcsönhatás fogalma

Az üzleti kapcsolatok nem egyszerű adásvételi tranzakciók. Hakan Håkansson és az IMP (Industrial Marketing and Purchasing) csoport kutatásai rámutattak, hogy a vállalatok közötti kapcsolatok összetett, tartós **kölcsönhatások** (interactions), amelyeket a neoklasszikus közgazdaságtan és a hagyományos stratégiai menedzsment nem tud megfelelően leírni.

Az IMP megközelítés szerint az üzleti kölcsönhatásokat öt alapvető tényező határozza meg. Ezek nem független változók – egymást erősítik és szövik át.

```mermaid
flowchart LR
    CENTER(["<b>5 tényező</b>, amely alakítja<br/>az üzleti kölcsönhatásokat"]):::lilaH
    T["<b>1. IDŐBELISÉG</b>"]:::kek
    SZ["<b>2. SZUBJEKTÍV<br/>ÉRTELMEZÉS</b>"]:::zold
    K["<b>3. KAPCSOLTSÁG</b>"]:::narancs
    KF["<b>4. KÖLCSÖNÖS<br/>FÜGGŐSÉG</b>"]:::turkiz
    V["<b>5. VISZONYLAGOSSÁG</b>"]:::rozsa

    CENTER <--> T
    CENTER <--> SZ
    CENTER <--> K
    CENTER <--> KF
    CENTER <--> V
    T <-.-> SZ
    K <-.-> KF
    KF <-.-> V

    classDef kek     fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef zold    fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef narancs fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;
    classDef rozsa   fill:#fce4ec,stroke:#c2185b,stroke-width:2px,color:#880e4f,rx:10,ry:10;
    classDef lilaH   fill:#f3e5f5,stroke:#7b1fa2,stroke-width:3px,color:#4a148c,rx:10,ry:10;
    classDef turkiz  fill:#e0f2f1,stroke:#00695c,stroke-width:2px,color:#004d40,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
    linkStyle 5,6,7 stroke:#90a4ae,stroke-width:2px,stroke-dasharray: 5 5;
```

---

### 17.2. Az öt tényező részletes bemutatása

#### 1. Időbeliség (Temporality)

Az üzleti kapcsolatok időben fejlődnek. Nem pillanatfelvételek, hanem folyamatok: múlt, jelen és jövő elvárások együttesen határozzák meg, hogy a két fél hogyan viselkedik egymással.

**Következmény a menedzsment számára:**
- A múltbeli tapasztalat (bizalom, konfliktus, teljesítmény) beépül a kapcsolat "tőkéjébe."
- Egy hosszú távú kapcsolat megszakítása nem csak a jövőbeli tranzakciók elvesztését jelenti, hanem az addig befektetett kapcsolat-specifikus eszközök (tudás, adaptáció, koordinációs rutinok) elvesztését is.
- Az idő múlásával a felek egymáshoz igazítják folyamataikat és rendszereiket – ezt **kapcsolatspecifikus adaptációnak** (relationship-specific adaptation) nevezzük.

```mermaid
flowchart LR
    E1["<b>Első</b><br/>tranzakció"]:::kek --> E2["<b>Bizalom</b><br/>épül"]:::turkiz --> E3["<b>Adaptáció</b>"]:::zold --> E4["<b>Rutinizáció</b>"]:::narancs --> E5["<b>Elkötelezettség</b>"]:::lila

    I1(["Ismerkedés<br/>kockázata"]):::szurke -.-> E1
    I2(["Kipróbálás<br/>szakasza"]):::szurke -.-> E2
    I3(["Kölcsönös<br/>igazítás"]):::szurke -.-> E3
    I4(["Nehéz<br/>megszakítani"]):::szurke -.-> E4

    classDef kek     fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef zold    fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef narancs fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;
    classDef lila    fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px,color:#4a148c,rx:10,ry:10;
    classDef turkiz  fill:#e0f2f1,stroke:#00695c,stroke-width:2px,color:#004d40,rx:10,ry:10;
    classDef szurke  fill:#eceff1,stroke:#546e7a,stroke-width:2px,color:#263238,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
    linkStyle 4,5,6,7 stroke:#90a4ae,stroke-width:2px,stroke-dasharray: 5 5;
```

#### 2. Szubjektív értelmezés (Subjective/Mutually defined interpretation)

Ugyanazt az üzleti kapcsolatot a két fél eltérően értelmezi. Nincs egyetlen "objektív" leírás egy kölcsönhatásról: minden résztvevő a saját perspektívájából, céljaiból és korábbi tapasztalataiból kiindulva értelmezi azt.

**Következmény a menedzsment számára:**
- Egy szállítói kapcsolatot a vevő "stratégiai partnerségnek" láthat, míg a szállító "rutinügyfélnek" tekinti a vevőt – vagy fordítva.
- Ez kommunikációs és koordinációs feszültségeket okozhat.
- A sikeres együttműködés feltétele a **közösen konstruált értelmezési keret** kialakítása.

| Fél | Értelmezési dimenzió | Lehetséges eltérés |
|---|---|---|
| Vevő | "Ez stratégiai partnerség" | Szállító: "Rutinügylet" |
| Szállító | "Fontos referenciaprojekt" | Vevő: "Kis tételszámú megrendelés" |
| Mindkét fél | A kapcsolat hosszú távú értéke | Eltérő diszkontráta, eltérő időhorizont |

#### 3. Kapcsoltság (Connectedness)

Egyetlen üzleti kapcsolat sem létezik önmagában. Minden A–B kapcsolatot befolyásol az A és B más kapcsolataik összessége. A hálózatban minden összefügg mindennel.

```mermaid
graph LR
    SC["<b>Szállító C</b>"]:::zold --- SB["<b>Szállító B</b>"]:::zold
    SB --- VA["<b>Vevő A</b>"]:::kek
    SB -. "stratégiai szövetség" .-> VD["<b>Versenyző D</b>"]:::rozsa

    NOTE(["Ha A kapcsolatban van B-vel,<br/>de B szövetsége van D-vel —<br/>ez A–B kapcsolatát alapvetően befolyásolja"]):::szurke
    VA ~~~ NOTE

    classDef kek    fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef zold   fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef rozsa  fill:#fce4ec,stroke:#c2185b,stroke-width:2px,color:#880e4f,rx:10,ry:10;
    classDef szurke fill:#eceff1,stroke:#546e7a,stroke-width:2px,color:#263238,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
    linkStyle 2 stroke:#c2185b,stroke-width:2px,stroke-dasharray: 5 5;
```

**Következmény a menedzsment számára:**
- Egy kapcsolat értéke nem önmagában, hanem a hálózati kontextusban értelmezhető.
- Az egyes partnerek kapcsolatai egymásra hatnak: egy szállítóváltás hullámokat indít a hálózatban.
- A jó hálózati pozíció (pl. centrális helyzet, strukturális lyukak áthidalása) önmagában is versenyelőnyt jelent.

#### 4. Kölcsönös függőség (Mutual dependence)

Az üzleti kapcsolatokban mindkét fél függ a másiktól – még ha ez aszimmetrikusan is valósul meg. A függőség nem gyengeség: elkerülhetetlen következménye az üzleti specializációnak és a munkamegosztásnak.

**A függőség forrásai:**
- **Erőforrás-függőség:** az egyik fél olyan erőforrással (tudás, technológia, kapacitás) rendelkezik, amelyet a másik nem tud helyettesíteni.
- **Rutin-függőség:** az együttmüködés során kialakult koordinációs eljárások olyannyira beágyazódnak, hogy a váltás magas tranzakciós költséggel járna.
- **Reputáció-függőség:** a kapcsolat mindkét fél piaci hírnevét befolyásolja.

| Függőségi típus | Szimmetrikus | Aszimmetrikus |
|---|---|---|
| Erőforrás | Mindkét fél nélkülözhetetlen | Az egyik fél könnyen helyettesíthető |
| Rutinizáció | Kölcsönös adaptáció | Csak az egyik fél alkalmazkodott |
| Reputáció | Kölcsönösen előnyös hivatkozás | Csak az egyiknek jelent referenciát |

#### 5. Viszonylagosság (Relativity)

Egy kapcsolat jellegét és értékét mindig más kapcsolatokhoz viszonyítva kell meghatározni. Nincs abszolút "jó" vagy "rossz" kapcsolat – csak hálózati kontextusában értékelhetők.

**Következmény a menedzsment számára:**
- Egy szállítói kapcsolat értékét nem önmagában kell mérni, hanem alternatívákhoz képest (más szállítók, belső előállítás).
- A kapcsolat priorálása is viszonylagos: A-nak B fontosabb lehet, ha C és D slabba, mint ha erős alternatívái vannak.
- A hálózati pozíció is relatív: amit hub-nak tekintünk egy kis hálózatban, az periférián lehet egy nagyobb struktúrában.

---

### 17.3. Az öt tényező összefüggése

```mermaid
flowchart TD
    T["<b>IDŐBELISÉG</b><br/>a múlt formálja a jelent"]:::kek
    SZ["<b>SZUBJEKTÍV ÉRTELMEZÉS</b><br/>eltérő perspektívák"]:::zold
    KF["<b>KÖLCSÖNÖS FÜGGŐSÉG</b><br/>kölcsönös beágyazódás"]:::turkiz
    K["<b>KAPCSOLTSÁG</b><br/>más kapcsolatok hatása"]:::narancs
    V["<b>VISZONYLAGOSSÁG</b><br/>csak más kapcsolatokhoz viszonyítva értelmezhető"]:::rozsa

    T --> SZ --> KF --> K --> V
    K <-.-> KF
    SZ <-.-> T
    V <-.-> K

    classDef kek     fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef zold    fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef narancs fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;
    classDef rozsa   fill:#fce4ec,stroke:#c2185b,stroke-width:2px,color:#880e4f,rx:10,ry:10;
    classDef turkiz  fill:#e0f2f1,stroke:#00695c,stroke-width:2px,color:#004d40,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
    linkStyle 4,5,6 stroke:#90a4ae,stroke-width:2px,stroke-dasharray: 5 5;
```

Az öt tényező együttesen magyarázza, miért **nem egyszerűsíthető le** az üzleti hálózat sem pusztán erőforrás-tranzakciókra (neoklasszikus közgazdaságtan), sem tisztán strukturális viszonyokra (szociológiai hálózatelemzés). A vállalatok közötti kölcsönhatás **dinamikus, szubjektíven értelmezett, hálózatba ágyazott folyamat**.

---

**Összegzés:** Håkansson és az IMP csoport szerint az üzleti kölcsönhatásokat öt egymást átszövő tényező határozza meg: az időbeliség (a kapcsolat fejlődik és múltja van), a szubjektív értelmezés (a felek eltérően látják ugyanazt), a kapcsoltság (nincs önálló kapcsolat, csak hálózati kontextus), a kölcsönös függőség (mindkét fél függ a másiktól) és a viszonylagosság (egy kapcsolat értéke más kapcsolatokhoz képest értelmezhető). Ez az öt tényező együttesen teszi az üzleti hálózatot komplex, nem lineárisan kezelhető rendszerré.

---

*Forrás: Håkansson, H. (2010): Határtalan hálózatok. Alinea Kiadó; Dr. Szilágyi Győző Attila, GMXVU2MBLF előadásanyag (2025/26); Håkansson, H. – Snehota, I. (1995): Developing Relationships in Business Networks*
