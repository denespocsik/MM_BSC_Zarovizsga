## V20 – Hálózati üzleti stratégia

**Tételkérdés:** Mutassa be az üzleti stratégiaalkotás hálózati megközelítését! Hogyan értelmezi a hálózati stratégia: a szervezeti határokat és a szervezeti eredményességet.

---

### 20.1. A hagyományos stratégia korlátai hálózati környezetben

A klasszikus stratégiai menedzsment – Porter versenyerő-modellje, az erőforrás-alapú elmélet (RBV) – az egyes vállalatot mint önálló stratégiaalakítót kezeli, amely a versenyképességét belülről, saját erőforrásaiból és képességeiből fakadóan építi fel.

```
  KLASSZIKUS STRATÉGIAI LOGIKA:

  Vállalat → belső erőforrások/képességek → versenyelőny → piaci pozíció

  HÁLÓZATI STRATÉGIAI LOGIKA:

  Kapcsolathálózat → hálózati pozíció → stratégiai mozgástér → versenyelőny
```

A hálózati megközelítés szerint a stratégia nem csupán a vállalaton belülről fakad, hanem **a hálózatban elfoglalt pozícióból és a kapcsolatokból** is. A kapcsolatok nem csak erőforrások szerzésének eszközei – ők maguk is stratégiai erőforrások.

---

### 20.2. Hálózati pozíció mint stratégiai alap

Barabási Albert-László skálafüggetlen hálózat-elmélete szerint a hálózatokban a kapcsolatok nem egyenlően oszlanak el: néhány csomópont (hub) rendkívül sok kapcsolattal rendelkezik, a legtöbb csomópontnak viszont csak kevés van. Ez a **power-law (hatványfüggvény) fokszámeloszlás**.

```
  SKÁLAFÜGGETLEN HÁLÓZAT – FOKSZÁMELOSZLÁS

  p(k) ~ k^(-γ)  ahol γ általában 2–3

  Csomópontok száma
     ▲
     │  *
     │   *
     │    *
     │     **
     │       ***
     │          *****
     │               ********
     └────────────────────────→ Fokszám (k)

  Kevés HUB (sok kapcsolat)  +  Sok periférikus csomópont
```

**Preferential attachment (preferenciális kapcsolódás):** Az új szereplők nem véletlenszerűen kötődnek a hálózatba, hanem inkább a már jól kapcsolt csomópontokat keresik. „A gazdag gazdagodik" elv hálózati megfelelője.

**Stratégiai következmény:** Aki korán és hatékonyan kiépíti a kapcsolatait, hub-pozícióba kerülhet – és ez a pozíció önmagát erősítő folyamat révén fenntartható versenyelőnnyé válik.

---

### 20.3. A hálózati stratégia három szintje

```
  ┌──────────────────────────────────────────────────────┐
  │              HÁLÓZATI STRATÉGIA SZINTJEI             │
  │                                                      │
  │  1. KAPCSOLATPORTFÓLIÓ-MENEDZSMENT                  │
  │     Milyen kapcsolatokat tartsunk, bővítsünk,       │
  │     zárjunk le? Erős vs. gyenge kötések aránya.     │
  │                                                      │
  │  2. HÁLÓZATI POZICIONÁLÁS                           │
  │     Hub, híd (broker) vagy periférikus pozíció?      │
  │     Melyik klaszterben legyünk centrálisak?          │
  │                                                      │
  │  3. HÁLÓZATALAKÍTÁS (co-evolution)                  │
  │     Aktív hálózatalakítás: új kapcsolatok            │
  │     ösztönzése, szabványok, platformok,              │
  │     konzorciumok létrehozása.                        │
  └──────────────────────────────────────────────────────┘
```

#### Hub-stratégia
Célja a centrális pozíció megszerzése és megtartása. A hub magas betweenness centralitással rendelkezik: sok legrövidebb útvonal halad át rajta, ami kontrollt ad az információ- és erőforrásáramlás felett.

**Példák:** Amazon (kereskedelmi hub), Google (információs hub), SAP (üzleti szoftver-ökoszisztéma hub).

#### Híd (broker) stratégia
Célja a strukturális lyukak (structural holes – Burt, 1992) kitöltése: olyan pozíció kiépítése, ahol a vállalat két egyébként nem összekötött hálózati klasztert kapcsol össze.

```
  STRUKTURÁLIS LYUK (Burt):

  Klaszter A        Klaszter B
  ●─●─●             ●─●─●
   ╲ │ ╱             ╲ │ ╱
    \│/               \│/
     ●                 ●
      ╲               ╱
       ●─── HÍD ────●        ← A híd pozíciója: információs előny,
       (bróker)               koordinációs hatalom
```

**Következmény:** A bróker látja mindkét klasztert, de a klaszterek nem látnak egymásba – ez információs és koordinációs hatalmat jelent.

---

### 20.4. Szervezeti határok a hálózati stratégiában

A hagyományos vállalatelmélet a szervezeti határt jogi és tulajdonosi alapon húzza meg: ami a vállalathoz tartozik, az belül van; ami nem, az kívül. A hálózati megközelítés ezt alapvetően újraértelmezi.

**A szervezeti határok három értelmezése hálózati szemléletben:**

| Határkoncepció | Hagyományos | Hálózati |
|---|---|---|
| Jogi határ | A vállalat tulajdonában lévő eszközök | Formálisan megmarad, de stratégiailag kevéssé releváns |
| Kompetencia határ | Amit a vállalat tud elvégezni | Kiterjed a partnerek kompetenciáira is (kiszervezés, co-development) |
| Kapcsolati határ | Nem értelmezhető | A vállalat hálózati identitása: kit tekint partnernek, kivel nem akar kapcsolatot |

```
  SZERVEZETI HATÁROK HÁLÓZATBAN:

  ┌─────────────────────────────────────────┐
  │  VÁLLALAT JOGI HATÁRA                  │
  │  ┌──────────────────┐                  │
  │  │   Mag-kompetencia│────── Szállító A  │
  │  │   (saját)        │                  │
  │  └──────────────────┘                  │
  │  ┌──────────────────┐                  │
  │  │  Kiszervezett    │────── Partner B   │
  │  │  funkciók        │                  │
  │  └──────────────────┘                  │
  │  ┌──────────────────┐                  │
  │  │  Co-development  │────── Kutató C    │
  │  └──────────────────┘                  │
  └─────────────────────────────────────────┘

  A vállalat határa elmosódik: a stratégiailag
  releváns "egység" a teljes kapcsolathálózat.
```

**Következmény:** A kiszervezés, a stratégiai szövetség, a joint venture és a platform-ökoszisztéma mind a hálózati szemlélet produktuma: a vállalat nem próbál mindent belül csinálni, hanem tudatosan alakítja a kapcsolatait.

---

### 20.5. Szervezeti eredményesség hálózati nézőpontból

A hagyományos hatékonyság-fogalom (efficiency) belső folyamatok optimalizálásáról szól. A hálózati megközelítés az **eredményességet (effectiveness)** hálózati kontextusban definiálja:

**Eredményesség hálózatban:**
- Nem csak a saját folyamatok optimálisak, hanem a kapcsolatokon keresztül elérhető értékteremtés is maximalizált.
- A hálózati pozíció értéke: közbeesettségi centralitás, elérhetőség (más csomópontokhoz való közelség), híd-funkció.
- A kapcsolati tőke (relational capital) megőrzése: a hosszú távú kapcsolatok értékének fenntartása.

```
  SZERVEZETI EREDMÉNYESSÉG MUTATÓI HÁLÓZATBAN:

  ┌───────────────────────────────────────────────────┐
  │  HÁLÓZATI POZÍCIÓ MUTATÓI                        │
  │  ● Betweenness centralitás (hány út megy át)     │
  │  ● Closeness centralitás (átlagos távolság)       │
  │  ● Degree centralitás (közvetlen kapcsolatok)     │
  │                                                   │
  │  KAPCSOLATI PORTFÓLIÓ MINŐSÉGI MUTATÓI           │
  │  ● Kulcskapcsolatok stabilitása                   │
  │  ● Erős/gyenge kötések aránya                    │
  │  ● Hídkapcsolatok száma (más klaszterekbe)        │
  │                                                   │
  │  HÁLÓZATI ROBOSZTUSSÁG                           │
  │  ● Hány kulcspartner kiesése után omlik össze    │
  │    az értékteremtési hálózat?                    │
  └───────────────────────────────────────────────────┘
```

**Robosztusság és reziliencia:** Az előadás perkolációs elmélete alapján a skálafüggetlen hálózatok véletlenszerű meghibásodásokkal szemben robosztusak (sok kis csomópont kiesése nem szakítja szét a hálózatot), de célzott hubeltávolítással szemben sérülékenyek. A stratégiai tervezésnek figyelembe kell vennie: ha a vállalat hub-függő, akkor hub-kiesés esetén mi a B-terv?

---

**Összegzés:** A hálózati üzleti stratégia nem csupán a versenyerők és a belső folyamatok optimalizálásáról szól, hanem a hálózatban elfoglalt pozíció tudatos kialakításáról és menedzseléséről. A szervezeti határok a hálózati szemléletben elmosódottak: a stratégiailag releváns egység a vállalat és kapcsolatai együttesen. Az eredményesség mérése kiterjed a hálózati pozíció mutatóira (centralitás, híd-funkció) és a kapcsolati portfólió minőségére. A preferenciális kapcsolódás elvéből következik, hogy a korai és tudatos pozicionálás a legfontosabb stratégiai lépés egy hálózatban.

---

*Forrás: Barabási Albert-László (2022): Behálózva; Barabási Albert-László (2024): A hálózatok tudománya; Håkansson, H. (2010): Határtalan hálózatok; Burt, R.S. (1992): Structural Holes; Dr. Szilágyi Győző Attila, GMXVU2MBLF előadásanyag (2025/26)*
