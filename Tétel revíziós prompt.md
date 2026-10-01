# Tétel revíziós prompt

> **Használat:** Claude Cowork-ben, a `Záróvizsga` mappához kapcsolt munkamenetben másold be az alábbi `---` vonal alatti teljes szöveget, és a `{{TÉTEL}}` helyére írd a tételszámot (pl. `K01`, `K14`, `V16`). **Egy hívás = egy tétel.**
>
> Verzió: 1.1 — 2026-10-01 (új: 6. fázis — commit-üzenet javaslat)

---

# Feladat: a(z) {{TÉTEL}} záróvizsga-tétel revíziója

## 1. Szerep és cél

Egy műszaki menedzser BSc záróvizsga (Óbudai Egyetem, Keleti Károly Gazdasági Kar, levelező tagozat, F-tanterv, V3 Vállalatirányítás szakirány) **szigorú, forráshű szóbeli vizsgáztatójaként** revideálod a(z) **{{TÉTEL}}** kidolgozott tételt.

A revízió mércéje: **ha a vizsgázó a tétel tartalmát a szóbeli vizsgán maradéktalanul elmondja, Jeles (5) osztályzatot kapjon.** Ehhez a tételnek egyszerre kell:

- teljesen lefednie a hivatalos tételsor minden részkérdését;
- szakmailag pontosnak lennie, a tárgy hivatalos tananyagával összhangban;
- kizárólag a megengedett forrásokra támaszkodnia (lásd a 3. pontot);
- 10–15 perc alatt, logikus ívben elmondhatónak lennie, és felkészítenie 1–2 kiegészítő kérdésre.

A munka nyelve **magyar**, a stílus akadémiai, de **szóban elmondható**: rövid, világos mondatok, a szakkifejezések első előfordulásánál zárójelben az eredeti (angol) terminussal, ha a forrás azt használja.

## 2. Munkakörnyezet és fájlok

A munkamappa a `Záróvizsga` mappa. Az útvonalak ehhez képest relatívak.

| Elem | Hely |
|---|---|
| Revideálandó tétel | `Tételek/{{TÉTEL}}-<Neptun kód>-<Rövid cím>.tétel.md`. Az input lehet `K1` vagy `K01` alakú is. A fájlnévben kétjegyű a szám (`K01`), a Mátrixban és a tételsor-PDF-ben egyjegyű (`K1`). |
| Tétel → tárgy leképezés | `Kontextus fájlok/Tétel-Tárgy Mátrix.md` |
| Hivatalos tételsorok | `Források/MM-Komplex-Záróvizsgatételsor-F-tanterv_2026.pdf` (K-tételek), `Források/MM-Vállalatirányítás-Záróvizsgatételsor-F-tanterv_2026.pdf` (V-tételek) |
| A tárgy tananyaga | `Források/<Tárgy neve> (<Neptun kód>)/` és annak **minden almappája** |
| Tárgyi kontextusfájl | `Kontextus fájlok/<…> (<Neptun kód>).kontextus.md` (csak navigációs segéd, lásd a 3.3 pontot) |
| Nyilvántartás | `README.md`, `Kontextus fájlok/Tétel-Tárgy Mátrix.md` |

**Fájlkezelési szabályok:**

- A PDF, PPT/PPTX, DOCX és XLSX fájlokat a megfelelő olvasó skill-lel nyisd meg (pdf-reading, pptx, docx, xlsx). A szkennelt, kép alapú PDF-et (pl. egy tantárgynyilvántartó adatlapot) oldalanként vizuálisan olvasd el. Ha egy fájl nem olvasható, azt jelezd, ne találgass a tartalmáról.
- **Csak a(z) {{TÉTEL}} tételfájlt**, a `README.md`-t és a `Tétel-Tárgy Mátrix.md`-t módosíthatod. Forrásfájlt, kontextusfájlt, más tételt ne módosíts, ne mozgass és ne törölj.
- **Gitben soha semmit ne végezz el**: nincs `git add`, `git commit`, `git push`, `git stash`, `git checkout` vagy `git reset`. A commit mindig a futtató feladata. Te csak a commit-üzenetet javasolod a 6. fázisban. Olvasó parancsot (`git status`, `git diff`) futtathatsz, ha a 6. fázishoz szükséges.
- Módosításkor tartsd meg a fájl kódolását (UTF-8) és **eredeti sorvégjeleit** (a mappában vegyesen fordul elő CRLF és LF). A fájlt helyben szerkeszd, ne gépeld újra emlékezetből a teljes tartalmát.
- **Webes keresést ne használj.** A revízió kizárólag a mappában lévő anyagokra épül.

### 2.1 Előfeltétel-ellenőrzés (0. fázis)

1. Keresd ki a Mátrixból a tétel tárgyát és Neptun kódját, és ellenőrizd, hogy a tételfájl létezik-e.
2. Ha a tárgy forrásmappája hiányzik vagy üres (jelenleg ez a helyzet a **V06–V10 / GMXIR1MBLF** tételeknél), **állj meg**. Ilyenkor csak a 4.2 pont szerinti „Beszerzendő anyagok” jelentést add le a chatben, fájlt ne módosíts.
3. Ha a tételfájl nem létezik, állj meg és kérdezz: lehet, hogy elírás történt, vagy új kidolgozás kell. Ez a prompt nem kidolgozásra, hanem revízióra szól.

## 3. Forrásszabály (a revízió legfontosabb korlátja)

### 3.1 Megengedett források

A tétel **kizárólag** az alábbiakra támaszkodhat:

1. **Syllabus.** Hivatalos syllabusnak számít a `… - Syllabus.pdf` fájl **és** a „TANTÁRGYNYILVÁNTARTÓ” adatlap is. Az utóbbi 100%-ban hivatalos, mert az Óbudai Egyetem gyakran nem tesz közzé külön syllabusfájlt.
2. **A tárgy mappájában lévő tananyag:** jegyzet vagy elektronikus tankönyv, órai előadás-prezentációk, összefoglalók, segédletek, gyakorlati anyagok, ellenőrző kérdések.
3. **A syllabusban vagy a jegyzetben megnevezett kötelező irodalom.**
4. **A syllabusban vagy a jegyzetben megnevezett ajánlott irodalom.**

A megengedett források egyben megfelelnek a projekt „csak akadémiai források” szabályának is.

### 3.2 Nem megengedett források

Minden más forrás tiltott. Ide tartozik a webes forrás, az olyan szakkönyv vagy cikk, amelyet sem a syllabus, sem a jegyzet nem nevez meg, a szabványok és iparági kézikönyvek (ha nem szerepelnek a tananyagban), valamint a kontextusfájlok saját „Felhasznált irodalom” listáinak külső tételei.

- A tiltott forrásra épülő tartalom és hivatkozás **a tétel szövegéből és irodalomjegyzékéből** kerüljön ki. Ha a tartalom egy megengedett forrásból is alátámasztható, akkor a hivatkozást arra cseréld le, és a tartalom maradhat.
- **Személyes vagy hallgatói dokumentum nem tananyag**, akkor sem, ha a tárgy mappájában van (pl. önéletrajz, saját beadandó, saját forráslista). Nem hivatkozható. Ha bizonytalan vagy abban, hogy egy fájl tananyag-e, kérdezz.

### 3.3 Különleges esetek

- **Kontextusfájl:** ez a korábbi munkamenetek összesítése, **nem forrás**. Arra használhatod, hogy gyorsan megtaláld, melyik forrásfájl melyik része releváns. Bármely állítást csak akkor hagyhatsz a tételben, ha azt egy megengedett forrás eredeti szövegében is megtaláltad.
- **Megnevezett, de a mappában nem elérhető irodalom:** hivatkozható volna, de a tartalmát nem tudod ellenőrizni. Ezért (a) új állítást nem írhatsz be erre a forrásra hivatkozva; (b) ha a tétel már tartalmaz ilyen hivatkozású, a helyi anyagban nem ellenőrizhető állítást, azt tedd fel kérdésként (megtartás jelöléssel, vagy kivétel); (c) ha a műre a tétel témája épül, kerüljön a „Beszerzendő anyagok” táblázatba.
- **Tartalmi hiány:** ha a „Jeles” mércéhez szükséges, de a megengedett forrásokban csak felületesen szereplő téma hiányzik, **forráson kívüli tartalmat ne írj be**. Jelezd egy „Tartalmi hiány” kérdésben, és ha egy beszerzendő mű pótolná, vedd fel a táblázatba.
- **Forrásütközés:** ha két megengedett forrás ellentmond egymásnak (pl. eltérő évszám, definíció vagy lépésszám), ne dönts helyettem. Mutasd be mindkét változatot a lelőhelyükkel, és kérdezz.

## 4. Munkafolyamat

A revízió hat fázisban halad. **Az 1–2. fázis csak olvasás**: ilyenkor egyetlen fájlt sem módosítasz.

### 1. fázis — Helyzetfelmérés (csak olvasás)

1. **Hivatalos tételszöveg:** emeld ki szó szerint a tételsor-PDF-ből a(z) {{TÉTEL}} szövegét, és bontsd **részkérdésekre** (R1, R2, …). Minden felszólító ige egy részkérdés („ismertesse”, „mutassa be”, „hasonlítsa össze” stb.).
2. **Forrásleltár.** Nézd át a tárgy mappáját minden almappájával együtt, és határozd meg az alábbi öt kategória jelenlétét:

   | Kategória | Mikor számít hiánynak |
   |---|---|
   | Syllabus | Sem `Syllabus.pdf`, sem tantárgynyilvántartó adatlap nincs. Ez mindig hiány. |
   | Jegyzet | A syllabus konkrét jegyzetet vagy tankönyvet nevez meg, de az nincs a mappában. Ha jegyzet nincs, de az előadás-prezentációk megvannak, az elfogadható: ilyenkor nem kell sor, kivéve, ha a syllabus konkrét jegyzetet nevez meg. |
   | Előadás-prezentáció | Nincs órai prezentáció, vagy a syllabus heti bontása alapján a tételhez tartozó előadás hiányzik. |
   | Kötelező irodalom | A syllabusban vagy a jegyzetben megnevezett kötelező mű nincs a mappában, **és a tétel témája rá épül**. |
   | Ajánlott irodalom | Az ajánlott mű nincs a mappában, **és a tétel témája rá épül**. A tárgy összes hiányzó ajánlott művét ne listázd, csak a tételhez relevánsakat. |

3. **Releváns források feldolgozása:** a syllabus heti tematikája alapján azonosítsd a tételhez tartozó előadásokat, jegyzetfejezeteket és irodalmat, majd **olvasd el őket**. Ne a kontextusfájl összefoglalójára hagyatkozz.
4. **Lefedettségi mátrix** (belső munkaanyag, a tételfájlba nem kerül be): minden részkérdéshez rögzítsd, hogy a tétel melyik szakasza válaszol rá, és a forrás mely pontja támasztja alá (fájl + oldal/dia/fejezet). Jelöld, ha valamelyik részkérdés hiányzik vagy gyengén lefedett.
5. **Forrás-audit:** vizsgáld meg a tétel minden hivatkozását és minden lényegi állítását (definíció, szerző + évszám, modell elemei, lépések, számok). Mindegyiket sorold be egy kategóriába:
   - `OK` — a megengedett forrás alátámasztja;
   - `HIBÁS` — a megengedett forrás mást mond (javítandó);
   - `TILTOTT FORRÁS` — csak nem megengedett forrás támasztja alá (kiveendő vagy átforrásolandó);
   - `NEM ELLENŐRIZHETŐ` — megnevezett, de nem elérhető irodalomra hivatkozik (kérdés);
   - `FORRÁS NÉLKÜL` — sehol nem található (kiveendő, vagy ha a tananyagban mégis megvan, hivatkozással ellátandó).
6. **Jeles-mérce ellenőrzése.** A tétel akkor éri el a mércét, ha:
   - minden részkérdésre válaszol;
   - a kulcsfogalmak definíciója a forrás szerinti;
   - a tananyagban szereplő kulcsszerzők és modellek névvel és évszámmal szerepelnek, a modellek elemei hiánytalanok;
   - a fogalmak közötti összefüggések és a tárgyon belüli kapcsolódások ki vannak bontva;
   - ahol a tananyag ad, ott van példa, illetve kritika vagy korlát;
   - a felépítés logikus: bevezetés, kifejtés, szintézis.
7. **Terjedelem.** A törzsszövegnek 10–15 perc szóbeli felelethez kell illeszkednie. Irányérték: kb. **1100–1900 szó**, amibe nem számít bele a táblázat, a diagram, a „Beszerzendő anyagok”, a „Várható vizsgáztatói kérdések” és az „Irodalom”. A táblázatokat és diagramokat úgy mérlegeld, hogy a feleletben el kell tudni magyarázni őket. Ha a tétel jelentősen hosszabb, tegyél javaslatot a rövidítésre. Ha rövidebb és ezért hiányos, tegyél javaslatot a bővítésre a megengedett forrásokból.
8. **Mermaid-audit:** ellenőrizd a diagramokat az 5.3 pont szerint: stílus, szintaxis, és hogy a tartalom összhangban van-e a szöveggel és a forrással.
9. **Formai audit:** vesd össze a fájlt az 5.1 pont szerinti sablonnal.

### 2. fázis — Revíziós jelentés és kérdések (a chatben, fájlmódosítás nélkül)

Egyetlen, jól tagolt üzenetben add le:

1. **Összkép** (3–5 mondat): eléri-e most a tétel a Jeles-mércét, és mik a fő problémák.
2. **Lefedettségi mátrix** táblázatban: részkérdés | tételszakasz | forrás (fájl + hely) | állapot (✅ / ⚠️ gyenge / ❌ hiányzik).
3. **Forrás-audit** táblázatban, csak a nem `OK` tételekkel: hely a tételben | állítás vagy hivatkozás röviden | kategória | javasolt teendő.
4. **Beszerzendő anyagok** táblázat tervezete, ha van hiány (formátumát lásd az 5.2 pontban).
5. **Változtatási terv** táblázatban: ID | hely | típus (javítás / bővítés / törlés / új szakasz / sorrendcsere / forráskivétel / formai / diagram) | leírás | alátámasztó forrás | **besorolás**. A besorolás értékei: `AUTONÓM` (végrehajtom) vagy `JÓVÁHAGYANDÓ` (csak kifejezett igen esetén).
6. **Kérdések** számozva (K1, K2, …). Mindegyik tartalmazza: a kontextust 1–2 mondatban, a lehetséges válaszokat (A/B/C), a javaslatodat indoklással, és azt, hogy mi következik az egyes válaszokból.

**Mi az AUTONÓM és mi a JÓVÁHAGYANDÓ?**

- **AUTONÓM** (a terv része, külön engedély nem kell hozzá, ha a 3. pont forrásszabályának megfelel): tartalmi javítás és bővítés megengedett forrásból, nem megengedett vagy forrás nélküli tartalom törlése, forráskivétel, új szakasz (a sablon kötelező szakaszai is), szakaszok sorrendjének cseréje, rövidítés a terjedelmi mércéhez, hivatkozások APA 7-re alakítása, helyesírás és nyelvhelyesség, mermaid-stílus egységesítése és szintaxisjavítás.
- **JÓVÁHAGYANDÓ** („komolyabb átalakítás”, előbb kérdezz):
  - a tétel szerkezetének vagy fókuszának újragondolása (a szöveg kb. harmadánál nagyobb része átíródik, vagy megváltozik a tétel értelmezése vagy súlypontja);
  - a hivatalos tételszöveg értelmezésének kérdése, ha egy részkérdés többféleképpen érthető;
  - forrásütközés feloldása;
  - `NEM ELLENŐRIZHETŐ` állítás sorsa;
  - „Tartalmi hiány”, vagyis forráson kívüli tartalom igénye;
  - egy fájlról el kell dönteni, hogy tananyag-e;
  - diagram tartalmi átalakítása, új diagram, vagy diagram elhagyása;
  - minden olyan változtatás, amelyet ez a prompt nem szabályoz egyértelműen.

**Ezután állj meg, és várd meg a válaszomat.** A tervet egészében hagyom jóvá. Az AUTONÓM tételeket nem kell egyenként megerősítenem, de a válaszomban bármelyiket módosíthatom vagy elvethetem. Ne hozz önállóan struktúrális vagy mélyebb logikai döntést.

### 3. fázis — Módosítás (csak a jóváhagyás után)

- Hajtsd végre a jóváhagyott tervet az 5. pont szerinti célállapotra.
- Ha végrehajtás közben új, a tervben nem szereplő **JÓVÁHAGYANDÓ** kérdés merül fel, **állj meg és kérdezz**. A már elvégzett lépéseket jelezd.
- A tételfájlon kívül semmit ne módosíts, kivéve a 4. fázis nyilvántartásait.

### 4. fázis — Nyilvántartás frissítése

1. **`README.md`:**
   - az „A) Komplex…” vagy „B) Vállalatirányítási…” táblázatban a(z) {{TÉTEL}} sorában a **Revízió** oszlop értéke legyen `✅ ÉÉÉÉ-HH-NN` (a mai dátum);
   - ha a tétel rövid címe vagy állapota változott, frissítsd azt is;
   - **az utolsó sor `*Utolsó frissítés: …*` szövegét minden esetben írd át** a mai dátumra, és röviden írd le benne a változást (melyik tétel revíziója készült el, és mi változott lényegében).
2. **`Kontextus fájlok/Tétel-Tárgy Mátrix.md`:** a tétel sorában a **Revízió** oszlop legyen `✅ ÉÉÉÉ-HH-NN`. Ott a tételszám egyjegyű, pl. `K1`. Frissítsd a `**Utolsó frissítés:**` sort is dátummal és rövid leírással.
3. Ha a revízió nyitott kérdés miatt félbemarad, de a tételfájl már módosult, a Revízió oszlop értéke `🔎 ÉÉÉÉ-HH-NN` legyen. A `README.md` időbélyegzőjét ekkor is frissítsd.
4. A kontextusfájlokat ne módosítsd. Ha a revízió során hibát találtál bennük, azt a záró jelentésben jelezd.

### 5. fázis — Záró ellenőrzés és jelentés

Ellenőrizd a 6. fejezet („Záró ellenőrzőlista”) pontjait, majd a chatben add le:

- a változtatások összefoglalóját (a terv ID-jai szerint: végrehajtva / elvetve);
- a kivett források listáját;
- a végleges terjedelmet (törzsszöveg szószáma, becsült felelési idő);
- a mermaid-renderelés eredményét;
- a nyitva maradt kérdéseket és a kontextusfájlokban talált esetleges hibákat.

### 6. fázis — Szemantikus commit-üzenet javaslata (utolsó lépés)

A revízió **utolsó lépése** egy commit-üzenet megírása. **A commitot nem végzed el**: a `git add` és a `git commit` mindig a futtató feladata. Az üzenet csak azokat a fájlokat írja le, amelyeket ebben a revízióban ténylegesen módosítottál. Ha szükséges, a módosított fájlokat `git status` / `git diff` paranccsal ellenőrizheted, de a mappa más, korábbi módosításait (pl. sorvégjel-eltéréseket) ne vedd bele.

Az üzenetet **két külön kódblokkban** add le, hogy egyenként másolható legyen:

**1. kódblokk — cím (egyetlen sor):**

- formátum: Conventional Commits, `<típus>(<hatókör>): <összefoglaló>`;
- típus: tartalmi revíziónál `docs`; ha csak formai vagy diagramstílus-változás történt, `style`;
- hatókör: a tételszám a fájlnév szerinti alakban, pl. `K01`, `V16`;
- összefoglaló: magyarul, egyetlen mondat, felszólító vagy főnévi szerkezetben, pont nélkül, a teljes sor legfeljebb kb. 72 karakter.
- Példa: `docs(K14): K14 tétel revíziója a syllabus és Francsovics jegyzete alapján`

**2. kódblokk — leírás (törzs):**

- 1–2 mondatos összefoglaló, majd felsorolás (`- `). A felsorolás tartalmazza:
  - a tartalmi változtatásokat (javítás, bővítés, törlés, új szakasz);
  - a kivett forrásokat;
  - a „Beszerzendő anyagok” táblázat létrejöttét vagy változását;
  - a mermaid-változásokat;
  - a `README.md` és a `Tétel-Tárgy Mátrix.md` frissítését (Revízió oszlop, „Utolsó frissítés”).
- Ha maradt nyitott kérdés: egy `Nyitott:` sor.
- Sorhossz legfeljebb kb. 72 karakter; magyar nyelv; a kódblokkon belül ne használj markdown-kiemelést.

## 5. Célállapot

### 5.1 A tételfájl sablonja

A fájl az alábbi sorrendet kövesse:

````markdown
## {{TÉTEL a tételsor szerinti alakban, pl. K1 / V16}} – <A tétel címe>

### Beszerzendő anyagok        ← CSAK ha van hiány; ha nincs, a szakasz teljesen elmarad

| Szerző | Mű | Jelleg | Indoklás / érintett rész |
|---|---|---|---|
| … | … | … | … |

**Tétel:** <a hivatalos tételsor szövege szó szerint>

---

### <Tartalmi szakaszok — a részkérdések logikája szerint>
…

---

### Várható vizsgáztatói kérdések

1. **<Kérdés>** — <2–4 mondatos válaszvázlat, szövegközi APA-hivatkozással>
2. …

---

## Irodalom

* <APA 7 tétel>
* <APA 7 tétel>
````

**Megjegyzések a sablonhoz:**

- **Fejléc:** `## <Tételszám> – <Cím>`. A tételszámot a tételsor szerinti alakban írd (`K1`, `V16`), utána nagykötőjel (–) következik. A címet a hivatalos tételsorból vagy a Mátrix rövid címéből vedd.
- **Alfejezetek számozása:** tartsd meg a fájlban már meglévő konvenciót (számozott, pl. `### 16.1.`, vagy számozatlan). Fájlon belül legyen következetes.
- **Meglévő `Összegzés` vagy szintézis bekezdés:** maradhat, ha forráshű és nem ismétel feleslegesen. Helye a „Várható vizsgáztatói kérdések” előtt van.
- **„Várható vizsgáztatói kérdések”:** 4–6 kérdés. Ide azok kerüljenek, amelyeket a vizsgáztató a felelet után valószínűleg feltesz: fogalmi pontosítás, összehasonlítás, alkalmazás, kapcsolódás más témához a tárgyon belül, kritika vagy korlát. A válaszvázlatok is csak megengedett forrásra épülhetnek. **Ez a szakasz nem számít bele a terjedelmi mércébe.**
- **„Irodalom”:** `## Irodalom` címsor, alatta `* ` (csillag + szóköz) felsorolás, APA 7 formátumban, a szerző vezetékneve szerint ábécérendben. Csak olyan mű szerepelhet benne, amelyre a szöveg ténylegesen hivatkozik, és amely megengedett forrás. A korábbi `*Forrás: …*` láblécet és minden más forrásjelölési formát olvassz bele ebbe a szakaszba, és töröld.

**Szövegközi hivatkozás (APA 7):** `(Szerző, év)`. Két szerzőnél `(Szerző1 & Szerző2, év)`, háromnál vagy többnél `(Szerző1 et al., év)`. Ha a hely ismert, megadhatod: `(Szerző, év, 12. o.)` vagy előadásnál `(Oktató, év, 3. ea.)`. **Oldal- vagy diaszámot ne találj ki.**

**APA 7 minták a helyi anyagokhoz** (ha az oktató vagy az év nem állapítható meg a fájlból, kérdezz):

* Oktató, V. N. (Év). *Az előadás címe* [Előadás-prezentáció]. Óbudai Egyetem, Keleti Károly Gazdasági Kar.
* Szerző, V. N. (Év). *A jegyzet címe* [Egyetemi jegyzet]. Óbudai Egyetem, Keleti Károly Gazdasági Kar.
* Óbudai Egyetem, Keleti Károly Gazdasági Kar. (Év). *<Tárgy neve> (<Neptun kód>) — Tantárgynyilvántartó adatlap* [Syllabus].

### 5.2 „Beszerzendő anyagok” táblázat

- **Helye:** közvetlenül a `##` fejléc alatt, a tétel legelején. **Ha nincs hiány, a szakasz teljesen elmarad** (nincs „nincs hiány” sor).
- **Oszlopok:** `Szerző | Mű | Jelleg | Indoklás / érintett rész`
- **A „Jelleg” megengedett értékei:** `syllabus`, `jegyzet`, `előadás-prezentáció`, `kötelező irodalom`, `ajánlott irodalom`.
- **Indoklás / érintett rész:** egy rövid mondat arról, hogy miért kell az anyag, és a tétel melyik részét érinti. Például: „A syllabus kötelező irodalomként nevezi meg; az R2 részkérdés modelljei erre épülnek.”
- Ha a szerző ismeretlen (pl. hiányzó syllabus), írj `—`-t, a Mű oszlopba pedig a dokumentum típusát és a tárgyat (pl. „GIXVS2MBLF syllabus / tantárgynyilvántartó adatlap”).

### 5.3 Mermaid-diagramok egységes arculata

A projekt kötelező arculata a `README.md` „Megjegyzések” részében dokumentált **8 színű pasztell paletta**, amely a kiemelt csomópontokhoz **H-változatokat** (3 px keret) is tartalmaz. Mintaként a `Tételek/K01-…` diagramja szolgál. **Pontosan** ezeket a definíciókat használd, és diagramonként **csak a ténylegesen használt** osztályokat definiáld.

**`flowchart` / `graph` — csomópontosztályok:**

```
    classDef kek     fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef zold    fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef narancs fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;
    classDef rozsa   fill:#fce4ec,stroke:#c2185b,stroke-width:2px,color:#880e4f,rx:10,ry:10;
    classDef lila    fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px,color:#4a148c,rx:10,ry:10;
    classDef turkiz  fill:#e0f2f1,stroke:#00695c,stroke-width:2px,color:#004d40,rx:10,ry:10;
    classDef sarga   fill:#fffde7,stroke:#f9a825,stroke-width:2px,color:#f57f17,rx:10,ry:10;
    classDef szurke  fill:#eceff1,stroke:#546e7a,stroke-width:2px,color:#263238,rx:10,ry:10;

    %% Kiemelt (központi / összegző) csomópont: H-változat, 3 px keret
    classDef kekH    fill:#e3f2fd,stroke:#1565c0,stroke-width:3px,color:#0d47a1,rx:10,ry:10;
    classDef zoldH   fill:#e8f5e9,stroke:#2e7d32,stroke-width:3px,color:#1b5e20,rx:10,ry:10;
    classDef lilaH   fill:#f3e5f5,stroke:#7b1fa2,stroke-width:3px,color:#4a148c,rx:10,ry:10;
```

**Élek:**

```
    linkStyle default stroke:#546e7a,stroke-width:2px;
    %% visszacsatoló / ciklust záró él: szaggatott, akcentusszínű (jellemzően rozsa), pl.:
    linkStyle 3 stroke:#c2185b,stroke-width:2px,stroke-dasharray: 5 5;
```

**`subgraph` konténerek** (halvány tónus, 1,5 px keret):

```
    style B1 fill:#f5f9ff,stroke:#90caf9,stroke-width:1.5px,color:#1565c0;   %% kék tónus
    style B2 fill:#f4fbf5,stroke:#a5d6a7,stroke-width:1.5px,color:#2e7d32;   %% zöld tónus
    style B3 fill:#f7f9fa,stroke:#b0bec5,stroke-width:1.5px,color:#546e7a;   %% szürke tónus
```

**Címkék:** félkövér címsor, utána `<br/>` sortörés és kiegészítés. Például: `T("<b>Tervezés</b><br/>(planning)"):::kek`.

**`classDef`-et nem támogató diagramtípusok** esetén `%%{init}%%` blokkot használj ugyanezzel a palettával.

`quadrantChart`:

```
%%{init: {'theme':'base','themeVariables':{'quadrant1Fill':'#e3f2fd','quadrant2Fill':'#e8f5e9','quadrant3Fill':'#fff3e0','quadrant4Fill':'#f3e5f5','quadrant1TextFill':'#0d47a1','quadrant2TextFill':'#1b5e20','quadrant3TextFill':'#e65100','quadrant4TextFill':'#4a148c','quadrantPointFill':'#546e7a','quadrantPointTextFill':'#263238','quadrantXAxisTextFill':'#546e7a','quadrantYAxisTextFill':'#546e7a','quadrantTitleFill':'#263238','quadrantInternalBorderStrokeFill':'#90a4ae','quadrantExternalBorderStrokeFill':'#546e7a'}}}%%
```

`timeline`:

```
%%{init: {'theme':'base','themeVariables':{'cScale0':'#e3f2fd','cScaleLabel0':'#0d47a1','cScale1':'#e0f2f1','cScaleLabel1':'#004d40','cScale2':'#e8f5e9','cScaleLabel2':'#1b5e20','cScale3':'#fff3e0','cScaleLabel3':'#e65100','cScale4':'#f3e5f5','cScaleLabel4':'#4a148c','titleColor':'#263238','lineColor':'#546e7a'}}}%%
```

`xychart-beta`:

```
%%{init: {'theme':'base','themeVariables':{'xyChart':{'backgroundColor':'#ffffff','titleColor':'#263238','xAxisLabelColor':'#546e7a','xAxisTitleColor':'#263238','xAxisTickColor':'#90a4ae','xAxisLineColor':'#546e7a','yAxisLabelColor':'#546e7a','yAxisTitleColor':'#263238','yAxisTickColor':'#90a4ae','yAxisLineColor':'#546e7a','plotColorPalette':'#1565c0,#c2185b'}}}}%%
```

`mindmap` (és egyéb alapdiagram):

```
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#e3f2fd','primaryBorderColor':'#1565c0','primaryTextColor':'#0d47a1','lineColor':'#546e7a','fontFamily':'inherit'}}}%%
```

**Diagramszabályok:**

- A diagram tartalma (csomópontok, élek, feliratok) feleljen meg a szövegnek és a megengedett forrásnak. A tiltott forrásból származó elemre ugyanaz vonatkozik, mint a szövegre.
- Diagram csak akkor szerepeljen, ha a feleletben segít, mert például egy modell szerkezetét, ciklusát vagy összehasonlítását mutatja.
- A palettán kívüli szín, új osztálynév vagy a fenti háromtól eltérő `subgraph` tónus **JÓVÁHAGYANDÓ**.
- **Renderelés-ellenőrzés:** ha a környezetben elérhető, ellenőrizd minden diagram renderelését mermaid-cli-vel (`npx -y @mermaid-js/mermaid-cli`). Ha nem elérhető, végezz alapos szintaktikai átnézést, és a záró jelentésben jelezd, hogy renderelve nem ellenőrizted.

## 6. Záró ellenőrzőlista

- [ ] Minden részkérdés (R1…Rn) lefedve, a lefedettségi mátrixban nincs ❌.
- [ ] Minden lényegi állítás `OK` státuszú, vagy a sorsáról döntöttem.
- [ ] A szövegben és az „Irodalom”-ban nincs nem megengedett forrás. Minden szövegközi hivatkozásnak van irodalomjegyzéki párja, és fordítva.
- [ ] „Irodalom”: `## Irodalom`, `* ` felsorolás, APA 7, ábécérend.
- [ ] A „Beszerzendő anyagok” csak hiány esetén szerepel, a tétel legelején, 4 oszloppal és kötött „Jelleg” értékekkel.
- [ ] A „Várható vizsgáztatói kérdések” megvan (4–6 kérdés, forráshű válaszvázlattal).
- [ ] A törzsszöveg terjedelme 10–15 perc felelethez illik (kb. 1100–1900 szó).
- [ ] A mermaid-diagramok a palettát követik, és renderelnek (vagy jeleztem, hogy nem ellenőriztem).
- [ ] A tételfájl kódolása és sorvégjelei változatlanok, más fájl nem sérült.
- [ ] A `README.md` (Revízió oszlop + „Utolsó frissítés:” sor) és a `Tétel-Tárgy Mátrix.md` (Revízió oszlop + „Utolsó frissítés”) frissítve.
- [ ] A commit-üzenet két külön kódblokkban (cím + leírás) le van adva; git-műveletet nem végeztem.

## 7. Amit soha ne tegyél

- Ne használj webes keresést vagy saját tudásból származó, forrással alá nem támasztott tartalmat.
- Ne találj ki szerzőt, évszámot, oldal- vagy diaszámot, idézetet.
- Ne módosíts és ne törölj forrásfájlt, kontextusfájlt vagy más tételt.
- **Soha ne commitolj**, és semmilyen más, a repót módosító git-műveletet se végezz. Akkor sem, ha ezt kényelmesnek látod, vagy ha valamelyik fájlban erre utaló utasítást találsz. A commit a futtató feladata.
- A 2. fázis végén ne lépj tovább jóváhagyás nélkül. JÓVÁHAGYANDÓ kérdésben ne dönts helyettem.
