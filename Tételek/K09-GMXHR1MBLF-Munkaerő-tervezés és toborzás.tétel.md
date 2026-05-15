## K9 — Munkaerő-tervezés és toborzás

### Munkaerő-tervezés

A munkaerő-tervezés (HR planning / workforce planning) előrevetíti, hogy a szervezetnek milyen emberekre lesz szüksége, mikor és milyen számban, hogy stratégiai céljait elérje. Milkovich és Glueck (1995) szerint a folyamat két lépésből áll: a kereslet előrejelzéséből (hány és milyen kompetenciájú munkavállalóra van szükség) és a kínálat elemzéséből (kik állnak rendelkezésre belülről és kívülről).

```mermaid
flowchart TD
    A(["🏢 Szervezeti célok"]):::start --> B["📈 Munkaerő-kereslet\nelőrejelzése"]:::process
    B --> C["🏠 Belső kínálat\nelemzése"]:::process
    B --> D["🌍 Külső munkaerőpiac\nelemzése"]:::process
    C --> E{"⚖️ Munkaerőhiány\nvs. felesleg?"}:::decision
    D --> E
    E -->|"🔴 Hiány"| F["📣 Toborzási terv"]:::shortage
    E -->|"🟡 Felesleg"| G["📉 Leépítési /\nátcsoportosítási terv"]:::surplus
    F --> H(["📄 Munkakörelemzés\nleírás + specifikáció"]):::end_node
    G --> H

    classDef start    fill:#dbeafe,stroke:#2563eb,color:#1e3a5f,font-weight:bold
    classDef process  fill:#f0f9ff,stroke:#0ea5e9,color:#0c4a6e
    classDef decision fill:#fef9c3,stroke:#ca8a04,color:#713f12,font-weight:bold
    classDef shortage fill:#fee2e2,stroke:#dc2626,color:#7f1d1d
    classDef surplus  fill:#fef3c7,stroke:#d97706,color:#78350f
    classDef end_node fill:#dcfce7,stroke:#16a34a,color:#14532d,font-weight:bold
```

A tervezés alapja a **munkakörelemzés (job analysis)**: minden munkakör feladatainak, felelősségeinek, szükséges kompetenciáinak és munkafeltételeinek szisztematikus feltárása. Eredménye a **munkaköri leírás** (job description) és a **munkaköri specifikáció** (job specification), amely meghatározza az alkalmazottal szemben támasztott követelményeket.

### Toborzás

A toborzás (recruitment) a potenciális jelöltek megtalálásának és bevonásának folyamata. Borgulya és munkatársai (2006) belső és külső csatornát különböztetnek meg. A belső toborzás — előléptetés, rotáció, belső álláshirdetés — olcsóbb és gyorsabb, és a jelölt már ismeri a szervezetet, de az újfajta tudást és külső perspektívát nem hozza be. A külső toborzás épp fordítva: álláshirdetések, fejvadász-cégek (executive search), campus recruitment vagy szakmai hálózatok révén friss tudást és más szervezetekből hozott tapasztalatot nyerünk, de a beilleszkedési idő és a költség is magasabb, a beválás kockázata nagyobb.

| Szempontok | Belső toborzás | Külső toborzás |
|------------|---------------|----------------|
| Költség | Alacsony | Magasabb |
| Gyorsaság | Gyors | Lassabb |
| Kockázat | Alacsonyabb | Magasabb |
| Innováció | Kevesebb | Több |
| Motivációs hatás | Ösztönzi a karriert | Belső feszültség |

Az Armstrong–Taylor szerzőpáros (2016) hangsúlyozza, hogy a toborzás hatékonysága a munkáltatói márka (employer brand) erősségétől is függ: azok a szervezetek, amelyek vonzó munkahelynek számítanak, kisebb erőforrással is jobb jelölteket vonzanak.

---
