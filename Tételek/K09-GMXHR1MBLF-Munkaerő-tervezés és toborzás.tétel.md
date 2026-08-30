## K9 — Munkaerő-tervezés és toborzás

**Tétel:** Munkaerő tervezés és toborzás: Ismertesse a munkaerő tervezés fogalmát és jelentőségét! Mutassa be a toborzás fő formáit és csatornáit! Ismertesse a belső és külső toborzás előnyeit és hátrányait!

---

### Munkaerő-tervezés

A munkaerő-tervezés (HR planning / workforce planning) előrevetíti, hogy a szervezetnek milyen emberekre lesz szüksége, mikor és milyen számban, hogy stratégiai céljait elérje. Milkovich és Glueck (1995) szerint a folyamat két lépésből áll: a kereslet előrejelzéséből (hány és milyen kompetenciájú munkavállalóra van szükség) és a kínálat elemzéséből (kik állnak rendelkezésre belülről és kívülről).

```mermaid
flowchart TD
    A(["🏢 <b>Szervezeti célok</b>"]):::kekH --> B["📈 <b>Munkaerő-kereslet</b><br/>előrejelzése"]:::kek
    B --> C["🏠 <b>Belső kínálat</b><br/>elemzése"]:::kek
    B --> D["🌍 <b>Külső munkaerőpiac</b><br/>elemzése"]:::kek
    C --> E{"⚖️ <b>Munkaerőhiány</b><br/>vs. felesleg?"}:::sarga
    D --> E
    E -->|"🔴 Hiány"| F["📣 <b>Toborzási terv</b>"]:::rozsa
    E -->|"🟡 Felesleg"| G["📉 <b>Leépítési /</b><br/>átcsoportosítási terv"]:::narancs
    F --> H(["📄 <b>Munkakörelemzés</b><br/>leírás + specifikáció"]):::zoldH
    G --> H

    classDef kek     fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef kekH    fill:#e3f2fd,stroke:#1565c0,stroke-width:3px,color:#0d47a1,rx:10,ry:10;
    classDef zoldH   fill:#e8f5e9,stroke:#2e7d32,stroke-width:3px,color:#1b5e20,rx:10,ry:10;
    classDef narancs fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;
    classDef rozsa   fill:#fce4ec,stroke:#c2185b,stroke-width:2px,color:#880e4f,rx:10,ry:10;
    classDef sarga   fill:#fffde7,stroke:#f9a825,stroke-width:2px,color:#f57f17,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
    linkStyle 5 stroke:#c2185b,stroke-width:2px;
    linkStyle 6 stroke:#ef6c00,stroke-width:2px;
```

A tervezés alapja a **munkakörelemzés (job analysis)**: minden munkakör feladatainak, felelősségeinek, szükséges kompetenciáinak és munkafeltételeinek szisztematikus feltárása. Két fő kimenete a **munkaköri leírás** (*job description* — mit kell csinálni) és a **munkaköri specifikáció** (*job specification* — milyen ember kell hozzá), amely meghatározza az alkalmazottal szemben támasztott kompetencia-, képesítési és tapasztalati követelményeket (Milkovich & Glueck, 1995).

A **munkakör-értékelés** (*job evaluation*) a munkakörök relatív szervezeti súlyának és értékének megállapítása — ez adja az igazságos bérrendszer alapját. Elkülönül a munkakörelemzéstől: míg az utóbbi leírja a munkakört, az értékelés annak szervezeti fontosságát rangsorolja.

### Toborzás

A toborzás (recruitment) a potenciális jelöltek megtalálásának és bevonásának folyamata. Borgulya és munkatársai (2006) belső és külső csatornát különböztetnek meg. A belső toborzás — előléptetés, rotáció, belső álláshirdetés — olcsóbb és gyorsabb, és a jelölt már ismeri a szervezetet, de az újfajta tudást és külső perspektívát nem hozza be. A külső toborzás épp fordítva: álláshirdetések, fejvadász-cégek (executive search), campus recruitment vagy szakmai hálózatok révén friss tudást és más szervezetekből hozott tapasztalatot nyerünk, de a beilleszkedési idő és a költség is magasabb, a beválás kockázata nagyobb.

| Szempontok | Belső toborzás | Külső toborzás |
|------------|---------------|----------------|
| Költség | Alacsony | Magasabb |
| Gyorsaság | Gyors | Lassabb |
| Kockázat | Alacsonyabb | Magasabb |
| Innováció | Kevesebb | Több |
| Motivációs hatás | Ösztönzi a karriert | Belső feszültség |

Dessler (2020) keretrendszere szerint a toborzási csatorna megválasztása a munkakör jellegétől, a munkaerőpiaci helyzettől és a rendelkezésre álló időtől függ.

**Munkáltatói márka (employer branding).** Armstrong és Taylor (2014) hangsúlyozza, hogy a toborzás hatékonysága a munkáltatói márka erősségétől függ: a szervezet mint munkahely vonzerejét a tudatosan épített *munkavállalói értékajánlat* (*EVP — employee value proposition*) alapozza meg. Azok a szervezetek, amelyek vonzó munkahelynek számítanak, kisebb erőforrással is jobb jelölteket vonzanak.

---

## Irodalom

- Armstrong, M. & Taylor, S. (2014). *Armstrong's handbook of human resource management practice* (13th ed.). Kogan Page.
- Borgulya I-né et al. (2006). *Emberi erőforrás menedzsment kézikönyv.* CompLex Kiadó, Budapest.
- Dessler, G. (2020). *Human resource management* (16th ed.). Pearson.
- Milkovich, G. T. & Glueck, F. W. (1995). *Personnel/Human Resource Management: A Diagnostic Approach.* Business Publications Inc., Texas.
