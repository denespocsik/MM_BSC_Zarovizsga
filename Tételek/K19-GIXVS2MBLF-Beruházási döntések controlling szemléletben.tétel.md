## K19 – Beruházási és befektetési döntések controlling szemléletben

### A beruházási controlling logikája

A beruházási controlling **nem ér véget a vásárlási döntéssel**. Három szakaszt fed le:

```mermaid
flowchart LR
    A["📐 Tervezési szakasz<br/><i>döntési előkészítés</i><br/>Gazdaságossági számítások"]
    B["🔨 Megvalósítási szakasz<br/><i>projekt-controlling</i><br/>Költség- és időkontroll"]
    C["📊 Használati szakasz<br/><i>utókalkuláció</i><br/>Terv–tény összehasonlítás"]

    A -->|"döntés: megvalósítás"| B -->|"üzembe helyezés"| C
    C -->|"tapasztalatok → jövőbeli döntések"| A
```

### Gazdaságossági számítások módszerei

```mermaid
flowchart TD
    BK["💼 Beruházás-kalkuláció"]

    BK --> S["🕐 Statikus módszerek<br/><i>időtényezőt figyelmen kívül hagyják</i>"]
    BK --> D["⏳ Dinamikus módszerek<br/><i>pénz időértékét figyelembe veszik</i>"]

    S --> S1["Költség-összehasonlító számítás"]
    S --> S2["Nyereség-összehasonlító számítás"]
    S --> S3["Jövedelmezőségi számítás (ROI)"]
    S --> S4["Statikus megtérülési idő (PBPS)"]

    D --> D1["Nettó jelenérték (NPV)"]
    D --> D2["Belső megtérülési ráta (IRR)"]
    D --> D3["Jövedelmezőségi index (PI)"]
    D --> D4["Diszkontált megtérülési idő (PBPD)"]
```

### Statikus módszerek

**Megtérülési idő (PBPS)** – hány év alatt térül meg a befektetés a várható éves nyereségből/cash-flow-ból:

```
PBPS = Beruházási összeg / Éves nettó jövedelem
```

Egyszerű, de nem veszi figyelembe a pénz időértékét és az eszköz teljes élettartamát.

### Dinamikus módszerek – a pénz időértéke

Az időtényező figyelembevételéhez a jövőbeli pénzáramokat **diszkontálni** kell (jelenértékre hozni):

```
PV = CF_t / (1 + r)^t

ahol: CF_t = t-edik évben várható cash-flow
      r = elvárt hozam (diszkontráta)
```

**Nettó jelenérték (NPV):**

```
NPV = Σ [CF_t / (1+r)^t] – I₀

ahol I₀ = kezdeti beruházási összeg

Döntési szabály: NPV > 0 → gazdaságos a beruházás
```

**Belső megtérülési ráta (IRR):** az a diszkontráta, amelynél NPV = 0. Ha IRR > elvárt hozam → érdemes megvalósítani.

**Jövedelmezőségi index (PI):**

```
PI = GPV / I₀ = Σ[PV(CF_t)] / I₀

PI > 1 → gazdaságos
```

### Számítási példa

| Év | Cash-flow (MFt) | PV (14%-on) | Kumulált NPV |
|---|---|---|---|
| 0 | –500 | –500 | –500,00 |
| 1 | 90 | 78,95 | –421,05 |
| 2 | 250 | 192,37 | –228,68 |
| 3 | 300 | 202,49 | –26,19 |
| 4 | 200 | 118,42 | **+92,22** |

NPV = **+92,22 MFt** → a beruházás gazdaságos (pozitív jelenértékű többlethozam).  
PI = 592,22 / 500 = **1,18** → minden befektetett forint 1,18 Ft jelenértéket termel.  
Diszkontált megtérülési idő: PBPD ≈ 3,22 év.

### Cash-flow szerepe

A controlling **cash-flow-t használ**, nem könyvviteli nyereséget, mert:
- A cash-flow nem torzítható amortizációs politikával.
- A likviditást tükrözi, nem csak az eredményt.
- Beruházásoknál a pénzkiáramlás/befolyás tényleges időpontja számít.

> **Irodalom:** Katona F.: CONTROLLING 6. ea.; gyak_Beruházás-contr.pdf; Francsovics A.: Controlling, 4. fejezet; Brealey–Myers–Allen: Principles of Corporate Finance

---