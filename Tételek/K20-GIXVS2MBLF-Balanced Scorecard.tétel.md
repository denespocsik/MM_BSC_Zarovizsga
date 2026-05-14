## K20 – Balanced Scorecard: fogalma, négy dimenziója, működése és alkalmazása

### A BSC fogalma és eredete

A **Balanced Scorecard (kiegyensúlyozott mutatószám-rendszer)** Kaplan és Norton nevéhez fűződik (Harvard Business Review, 1992). Alapgondolata: a vállalat működése **nem írható le csupán pénzügyi mutatókkal** – a teljesítmény csak több dimenzióból együttesen értelmezhető.

A BSC két alapvetésben tér el a hagyományos kontrolling-rendszerektől:
1. **Stratégiai célokat mér**, nem csupán pénzügyi eredményeket.
2. **Ok-okozati logikát** épít fel a négy nézőpont között.

### A BSC négy nézőpontja

```mermaid
flowchart TD
    S["🎯 KÜLDETÉS és STRATÉGIA"]

    S --> P["💰 PÉNZÜGYI nézőpont<br/><i>Hogyan látnak minket a befektetők?</i>"]
    S --> V["👥 VEVŐI / PIACI nézőpont<br/><i>Hogyan látnak minket vevőink?</i>"]
    S --> B["⚙️ BELSŐ FOLYAMATOK nézőpont<br/><i>Miben kell kiválónak lennünk?</i>"]
    S --> T["📚 TANULÁS ÉS FEJLŐDÉS nézőpont<br/><i>Hogyan tudunk fejlődni és innoválni?</i>"]

    T -->|"alapozza meg"| B
    B -->|"értéket teremt"| V
    V -->|"bevételt generál"| P
```

### A négy nézőpont részletesen

**1. Pénzügyi nézőpont** – a tulajdonosi/befektetői szemszög:

| Stratégiai cél | Példa mutatószám |
|---|---|
| Jövedelmezőség növelése | ROE, ROI, EVA |
| Árbevétel-növekedés | Éves növekedési ütem (%) |
| Költségcsökkentés | Fajlagos önköltség (Ft/db) |
| Tőkemegtérülés | ROCE, nyereségmarzs |

**2. Vevői/piaci nézőpont** – a vevői értékajánlat mérése:

| Stratégiai cél | Példa mutatószám |
|---|---|
| Vevőelégedettség | NPS (Net Promoter Score), reklamációs ráta |
| Piaci részesedés | Piaci részesedés (%) |
| Vevőmegtartás | Churn-ráta, ismételt vásárlók aránya |
| Új vevők szerzése | Új ügyfélszerzési ráta |

**3. Belső folyamatok nézőpontja** – melyek azok a folyamatok, amelyekben kiválónak kell lennünk?

| Stratégiai cél | Példa mutatószám |
|---|---|
| Termékminőség | Selejt aránya (%), reklamáció/1000 db |
| Gyártási hatékonyság | OEE (Overall Equipment Effectiveness) |
| Átfutási idő csökkentése | Lead time, ciklusidő |
| Innováció | Új termékek aránya az árbevételből |

**4. Tanulás és fejlődés nézőpontja** – az infrastruktúra, amely az előző három nézőpontot táplálja:

| Stratégiai cél | Példa mutatószám |
|---|---|
| Dolgozói elégedettség | Dolgozói elégedettségi index |
| Képzettség fejlesztése | Képzési órák/dolgozó/év |
| Fluktuáció csökkentése | Fluktuációs ráta (%) |
| IT-rendszerek minősége | Rendszerleállás (óra/hónap) |

### Az ok-okozati lánc

A BSC kulcseleme, hogy a négy nézőpont **nem független egymástól**, hanem ok-okozati összefüggésben áll:

```mermaid
flowchart TD
    T["📚 Tanulás & Fejlődés<br/>Jobb képzés, magasabb kompetencia"]
    B["⚙️ Belső folyamatok<br/>Jobb gyártási minőség, rövidebb átfutás"]
    V["👥 Vevői nézőpont<br/>Elégedettebb vevők, több megrendelés"]
    P["💰 Pénzügyi nézőpont<br/>Magasabb árbevétel, jobb ROI"]

    T -->|"képzett munkaerő javítja a folyamatokat"| B
    B -->|"jobb minőség növeli az elégedettséget"| V
    V -->|"hűséges vevők növelik a bevételt"| P
```

Ez a logika teszi a BSC-t **stratégiai irányítási rendszerré** – nem csupán mutatószám-listává.

### A BSC alkalmazásának folyamata

1. **Stratégiai célok meghatározása** (vállalatvezetés) – mi a jövőkép?
2. **Stratégiai térkép elkészítése** – ok-okozati összefüggések vizualizálása
3. **Mutatószámok, célértékek és akciók hozzárendelése** minden nézőponthoz
4. **Felelősök és ütemterv** meghatározása
5. **Rendszeres riporting és felülvizsgálat** (negyedéves, éves)
6. **Visszacsatolás a stratégiába** – a stratégia tanulási folyamat

### A BSC és a controlling kapcsolata

A BSC a stratégiai controlling egyik legfontosabb eszköze: **operacionalizálja a stratégiát** azáltal, hogy konkrét, mérhető mutatókká bontja le a hosszú távú célokat. Így a K18-ban tárgyalt stratégiai–operatív controlling kapcsolat a BSC segítségével válik kézzelfoghatóvá.

> **Irodalom:** Katona F.: CONTROLLING 9. ea.; Kaplan, R.S. – Norton, D.P.: The Balanced Scorecard (1996); Kaplan–Norton: Strategy Maps (2004); Francsovics A.: Controlling (2011); Boda Gy. – Szlávik P.: Controlling-rendszer a gyakorlatban (2005)