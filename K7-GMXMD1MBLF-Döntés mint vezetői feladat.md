## K7. Döntés mint vezetői feladat

**Tétel:** „Ismertesse a vezetői döntés szerepét, a döntést, mint vezetői feladatot! Mutassa be a döntési modelleket és ismertesse a döntést hátráltató tényezőket!"

### A döntés fogalma

**Kornai János** szerint a döntés „cselekvési változatok közötti szabad, tudatos választás." Három elemet tartalmaz ez a definíció: (1) legalább két alternatíva létezik, (2) a választás szabad — nem automatikus reakció, (3) tudatos — a döntéshozó átgondolja a lehetőségeket.

A döntés a menedzseri munka középpontjában áll. Tervezni, szervezni, ellenőrizni — mindegyik számos döntést foglal magában. A döntések minősége meghatározza a szervezet sikerét.

### A döntési modell hat eleme

Egy döntési helyzet hat összetevőre bontható:

| Elem | Leírás |
|---|---|
| **Döntéshozó** | Aki a választást meghozza (egyén vagy csoport) |
| **Célok** | Mit akar elérni a döntéssel |
| **Alternatívák** | A mérlegelhető lehetséges cselekvések halmaza |
| **Állapotok (természet)** | A döntéshozón kívüli körülmények, amelyek befolyásolják az eredményt |
| **Kimenet** | Az egyes alternatívák várható eredménye az egyes állapotokban |
| **Döntési kritérium** | Az a szempont, amely alapján a legjobb alternatívát kiválasztják |

### Döntési osztályok

Az információ teljessége szerint három osztályt különítünk el:

1. **Biztos körülmények között hozott döntés:** Minden kimenet ismert, a döntéshozó pontosan tudja, mi következik melyik választásból. Ritka a valóságban.

2. **Kockázatos körülmények között hozott döntés:** Az egyes kimenetekhez valószínűségek rendelhetők — nem tudjuk pontosan mi lesz, de a valószínűségeket ismerjük. Tipikus esetei: statisztikailag jól leírt piacok, biztosítási döntések.

3. **Bizonytalan körülmények között hozott döntés:** Az alternatívák kimenetelei ismertek, de valószínűségi értékek nem rendelhetők hozzájuk. Ez a vezetői döntések nagy részének jellemzője.

### Döntési kritériumok bizonytalan körülmények között

Tegyük fel, hogy egy cég három piaci stratégia (A, B, C) közül választ, és a kimenetel a gazdasági helyzettől (jó, közepes, rossz) függ. A várható nyereségek (millió Ft):

| Stratégia | Jó gazd. | Közepes | Rossz |
|---|---|---|---|
| A | 100 | 60 | 20 |
| B | 80 | 70 | 40 |
| C | 60 | 55 | 50 |

**Wald MINI-MAX (pesszimista):** Minden stratégiánál a legrosszabb kimenetet vesszük, majd azt választjuk, amelyik a legrosszabb esetben is a legtöbbet adja.
- A: min = 20, B: min = 40, C: min = 50 → **C a legjobb** (kockázatkerülő döntés)

**Wald MAX-MAX (optimista):** A legjobb kimeneteket vesszük, és a maximumot választjuk.
- A: max = 100 → **A a legjobb** (kockázatkereső döntés)

**Laplace-kritérium:** Egyenlő valószínűségeket feltételez, átlagokat számol.
- A: (100+60+20)/3 = 60; B: (80+70+40)/3 = 63,3; C: (60+55+50)/3 = 55 → **B a legjobb**

**Hurwicz-kritérium:** Pesszimizmus-optimizmus index (α) alapján súlyoz: H = α × max + (1-α) × min.
Pl. α = 0,6: A: 0,6×100 + 0,4×20 = 68; B: 0,6×80 + 0,4×40 = 64; C: 0,6×60 + 0,4×50 = 56 → **A a legjobb**

**Savage–Niehans (elmaradt haszon minimalizálása):** Minden cellánál kiszámítjuk, mennyivel volt jobb az adott állapot legjobb kimenetele az adott stratégiánál. Az így kapott „bánatmátrix" maximumait minimalizáljuk.

### Döntési eszközök kockázatos körülmények között: Bayes

**Bayes-kritérium:** Ha rendelkezünk az egyes állapotok valószínűségeivel, a várható értéket számoljuk:

> EV = Σ (kimenet × valószínűség)

Ha P(jó)=0,3; P(közepes)=0,4; P(rossz)=0,3:
- EV(A) = 100×0,3 + 60×0,4 + 20×0,3 = 30+24+6 = **60**
- EV(B) = 80×0,3 + 70×0,4 + 40×0,3 = 24+28+12 = **64** → legjobb
- EV(C) = 60×0,3 + 55×0,4 + 50×0,3 = 18+22+15 = **55**

### Döntési fa

Komplex, többlépéses döntések modellezésére használják. A fa elágazódásai döntési csomópontok (□) és véletlen csomópontok (○). A fa jobb oldalától balra haladva visszagörgetéssel (backward induction) határozható meg az optimális stratégia.

### A döntéshozatal lépései

1. A döntési helyzet felismerése és meghatározása
2. Célok, kritériumok tisztázása
3. Alternatívák feltárása
4. Az alternatívák értékelése (modellek alkalmazása)
5. A legjobb alternatíva kiválasztása
6. Megvalósítás
7. Visszacsatolás, eredmény értékelése

### Döntést hátráltató tényezők

A valóságban a döntéshozatal ritkán zajlik a modellek által feltételezett racionalitással. Számos kognitív és szervezeti akadály lép fel:

**Korlátozott racionalitás (Herbert Simon, 1956):** Az emberek nem maximálnak, hanem *kielégítenek* (*satisficing*). Nem keresik az optimális megoldást, hanem az első megfelelőt fogadják el. Az információfeldolgozási kapacitásunk véges, az idő korlátozott, a rendelkezésre álló információ hiányos.

**Csoportgondolkodás (*groupthink*, Irving Janis):** Erősen kohézív csoportokban a konszenzus igénye felülírja a kritikus elemzést. Mindenki bólint, senki nem kérdőjelez meg — az eredmény rossz döntés, amelyet mindenki „jónak látott". Ellenszer: ördög ügyvédje (*devil's advocate*) kijelölése, névtelen szavazás.

**Megerősítési torzítás (*confirmation bias*):** Az ember hajlamos csak azokat az információkat észrevenni és értékelni, amelyek megerősítik már meglévő véleményét. Disconfirmáló adatokat figyelmen kívül hagyunk vagy bagatellizálunk.

**Status quo torzítás:** Hajlunk a jelenlegi állapot fenntartására, még akkor is, ha a változtatás objektíve jobb lenne. Az ismerős biztonságos, az ismeretlen kockázatosnak tűnik.

**Rendelkezésre állási heurisztika (*availability heuristic*, Tversky–Kahneman):** Az esemény bekövetkezési valószínűségét aszerint ítéljük meg, mennyire könnyen jut eszünkbe példa. A könnyen felidézhető (pl. médiában sokat tárgyalt) eseményeket túlbecsüljük; a ritkábbakat alulbecsüljük.

**Elsüllyedt költség tévedés (*sunk cost fallacy*):** Tovább fektetünk veszteséges projektekbe, mert már annyit öltünk bele — holott a múltbeli ráfordítás döntésteoretikailag irreleváns (a jövőbeni hasznosság számít, nem a múltbeli veszteség).

A hatékony döntéshozatal ezért nemcsak módszertani tudást, hanem önreflexiót is igényel: a jó vezető felismeri saját torzításait, és szándékosan ellensúlyozza azokat.