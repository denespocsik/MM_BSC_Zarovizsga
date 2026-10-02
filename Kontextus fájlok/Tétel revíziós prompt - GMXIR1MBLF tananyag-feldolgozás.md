# Tananyag-feldolgozó és tétel-kidolgozó prompt — GMXIR1MBLF (V06–V10)

> **Használat:** Claude Cowork-ben, a `Záróvizsga` mappához kapcsolt munkamenetben másold be az alábbi `---` vonal alatti teljes szöveget, és a `{{FELADAT}}` helyére írd az alábbiak egyikét. **Egy hívás = egy feladat.**
>
> | `{{FELADAT}}` | Mit csinál |
> |---|---|
> | `ANYAG` | A Menedzsment információs rendszerek (GMXIR1MBLF) tananyagának egyszeri, szisztematikus feldolgozása: forrásleltár, syllabus-egyeztetés, tétel–forrás leképezés, tartalmi hiányok feltárása, kontextusfájl létrehozása, nyilvántartások frissítése. Tételt **nem** ír. |
> | `V06` … `V10` | Az adott záróvizsga-tétel forráshű kidolgozása a feldolgozott tananyagból, a Tétel revíziós prompttal azonos szigorú forrás-auditálással. |
>
> **Ajánlott sorrend:** `ANYAG` → `V06` → `V07` → `V08` → `V09` → `V10`.
>
> **Viszony a `Tétel revíziós prompt.md`-hez:** ez annak testvér-promptja. A forrásszabályok szelleme, a jóváhagyási kapu, a tételsablon, a Mermaid-arculat és a záró ellenőrzőlista közös. Három ok miatt kellett külön prompt: (1) a V06–V10 tételfájlok még nem léteznek, ezért itt kidolgozás folyik, nem revízió; (2) az új tárgy tananyaga a korábbiaktól eltérő szerkezetű (HTML-könyvfejezetek, három szinten); (3) a hivatalos tételsor több eleme a tananyagon túlmutat (lásd a Függelék A-t). A kész V06–V10 tételek későbbi, utólagos revíziója a Tétel revíziós prompttal is elvégezhető.
>
> Verzió: 1.0 — 2026-10-02

---

# Feladat: {{FELADAT}} — a Menedzsment információs rendszerek (GMXIR1MBLF) tananyagának feldolgozása a V06–V10 záróvizsga-tételekhez

## 0. A hívás értelmezése

- Ha a `{{FELADAT}}` értéke `ANYAG`, a **4.A** fejezet szerint dolgozz.
- Ha `V06`, `V07`, `V08`, `V09` vagy `V10` (az input lehet `V6` alakú is), a **4.B** fejezet szerint dolgozz.
- Bármilyen más érték esetén **állj meg és kérdezz**. Ne találd ki, mit akarhattam.

## 1. Szerep és cél

Egy műszaki menedzser BSc záróvizsga (Óbudai Egyetem, Keleti Károly Gazdasági Kar, levelező tagozat, F-tanterv, V3 Vállalatirányítás szakirány) **szigorú, forráshű szóbeli vizsgáztatójaként** készíted elő a Menedzsment információs rendszerek tárgy (GMXIR1MBLF) V6–V10 tételeit.

A mérce ugyanaz, mint a Tétel revíziós promptban: **ha a vizsgázó a tétel tartalmát a szóbeli vizsgán maradéktalanul elmondja, Jeles (5) osztályzatot kapjon.** Ehhez a tételnek egyszerre kell teljesen lefednie a hivatalos tételsor minden részkérdését, szakmailag pontosnak és a tananyaggal összhangban lévőnek lennie, kizárólag megengedett forrásra támaszkodnia, 10–15 perc alatt elmondhatónak lennie, és felkészítenie 1–2 kiegészítő kérdésre.

**A mérce és a forrásszabály között feszültség lehet, és ezt nem szabad elsimítani.** Ha a megengedett források nem teszik lehetővé, hogy egy részkérdés Jeles szinten megválaszolható legyen, az nem hiba, amelyet kitöltéssel el kell tüntetni, hanem eredmény, amelyet jelentened kell. A hiányt tölteni tudásból tilos (lásd 3.3 és 7. fejezet).

A munka nyelve **magyar**, a stílus akadémiai, de **szóban elmondható**: rövid, világos mondatok, a szakkifejezések első előfordulásánál zárójelben az eredeti (angol) terminussal, ha a forrás azt használja.

## 2. Helyzetkép és munkakörnyezet

### 2.1 Helyzetkép (2026-10-02-i állapot, ellenőrizd, ne vedd készpénznek)

- A **V06–V10** tételfájlok nem léteznek. A forrásmappa megérkezésekor (2026-10-02) a README-ben és a Mátrixban az állapotuk ⏳-ról 📋-ra változott; ellenőrizd, hogy ez így van-e.
- A tárgy forrásmappája lapos (nincs almappa). Tartalma: a syllabus (szöveges PDF), 12 „Kötelező tananyag” HTML (`1_01`–`1_12`), 12 „Opcionális Fogalmi Alapkönyv” HTML (`2_01`–`2_12`), 1 „Opcionális Haladó Könyv” HTML (`3_07`, adatbányászati számítások), 80 képfájl és egy zip.
- **Nincs a mappában:** előadás-prezentáció (PPT), gyakorlati anyag (Excel, Power BI), Moodle-anyag, és a syllabus által megnevezett kötelező és ajánlott irodalom egyetlen darabja sem.
- A tananyag nem a tételsor szerint szerveződik. A tételsor VIR-, BI-, KPI-, DAX-, EVA- és Z-score-központú, a syllabus és a HTML-ek MIS-stratégia-központúak (Laudon-szerkezet). **Várható tartalmi hiányok vannak** (Függelék A).
- **Rövidítés-ütközés:** a V6–V10 tételsorban a **VIR = Vezetői Információs Rendszer**, a GMXIV2MBLF tárgyban (V11–V15, kontextusfájl) viszont a VIR gyakran az *integrált vállalatirányítási rendszert* jelöli. A tananyagban MIR/MIS is szerepel. Az első előfordulásnál mindig oldd fel a rövidítést, és ne keverd a két jelentést.

### 2.2 Fájlok és helyek

Az útvonalak a `Záróvizsga` mappához képest relatívak.

| Elem | Hely |
|---|---|
| Hivatalos tételsor | `Források/MM-Vállalatirányítás-Záróvizsgatételsor-F-tanterv_2026.pdf` (a 6–10. tétel; a PDF-ben és a Mátrixban egyjegyű számmal, pl. `V6`, a 10. kivételével) |
| Tétel → tárgy leképezés | `Kontextus fájlok/Tétel-Tárgy Mátrix.md` |
| A tárgy tananyaga | `Források/Menedzsment információs rendszerek (GMXIR1MBLF)/` |
| Syllabus | `Források/Menedzsment információs rendszerek (GMXIR1MBLF)/Menedzsment információs rendszerek (GMXIR1MBLF).pdf` |
| Kontextusfájl (az `ANYAG` hívás hozza létre) | `Kontextus fájlok/Váll.Irány II. - Menedzsment információs rendszerek (GMXIR1MBLF).kontextus.md` |
| Létrehozandó tételfájl | `Tételek/V0x-GMXIR1MBLF-<Rövid cím>.tétel.md`; a fájlnévben kétjegyű a szám (`V06`), a fejlécben és a Mátrixban egyjegyű (`V6`, de `V10`). A rövid címet a Mátrix rövid címéből képezd, és a 2. fázis jelentésében hagyasd jóvá. |
| Társ-prompt (szabályok forrása) | `Kontextus fájlok/Tétel revíziós prompt.md` |
| Nyilvántartás | `README.md`, `Kontextus fájlok/Tétel-Tárgy Mátrix.md` |

### 2.3 Fájlkezelési szabályok

- **Első lépésként olvasd el** a `Kontextus fájlok/Tétel revíziós prompt.md` **5.1–5.3 pontját** (tételsablon, „Beszerzendő anyagok” táblázat, Mermaid-arculat) és **6. fejezetét** (záró ellenőrzőlista). Ezek itt változatlanul érvényesek, az 5. fejezetben jelzett eltérésekkel. Ha a két prompt ütközik, **ez a prompt az erősebb.**
- **Módosítható fájlok.** `ANYAG` hívásnál: az új kontextusfájl, a `README.md` és a `Tétel-Tárgy Mátrix.md`. `V0x` hívásnál: az adott, újonnan létrehozott tételfájl, a `README.md` és a `Tétel-Tárgy Mátrix.md`. **Mást ne módosíts, ne mozgass, ne törölj:** forrásfájlt, másik kontextusfájlt, másik tételt, a revíziós promptot, a `CODEOWNERS`-t sem.
- **HTML olvasása.** Szövegkinyerést végezz scripttel (tagek eltávolítása, táblázatsorok és listák megőrzése), és ellenőrizd, hogy a táblázatok, listák és felsorolások nem vesztek el. Egy HTML-t **teljes egészében olvass el**, mielőtt belőle állítást veszel át. A HTML-ek tartalmaznak „Nyitó dilemma”, „Reflektív kérdés” és „Elmélyítő kiegészítő” blokkokat is. Ezek tananyag, de vizsgán a **definíciók, modellek, tipológiák, lépések és kritikák** számítanak; az esettanulmányok (pl. Knight Capital, Target, GE Predix, NHS) legfeljebb rövid példaként kerüljenek a tételbe, ha a tételsor kérdése példát kíván.
- **Képek.** A HTML-ek ábrái `data/<fájlnév>` hivatkozással szerepelnek, a mappában viszont lapos fájlnévvel találhatók. A tartalmat hordozó ábrákat (pl. DIKW, OLTP, KDD, BSC, BI-környezet, Dashboard, ROC-görbe) **vizuálisan nézd meg** (hozd át a munkaterületre, és olvasd el képként), ne a fájlnévből következtess a tartalomra. Ábrából csak azt használd, ami olvasható; ha nem olvasható, jelezd. A fájlnevük alapján dekoratívnak vagy illusztratívnak tűnő képek (pl. `ChatGPT Image … .png`, `HU flag.jfif`, `Target-logo… .jpg`) **nem tananyag-tartalom**; állítást nem alapozhatsz rájuk. Nézd meg őket, és ha egy képről nem tudod eldönteni, tananyag-e, kérdezz.
- **A zip** (`2026_27_1_GMXIR1MBLF_MM_L_7_ea-T_….zip`) a mappa tartalmának csomagolt másolata. 2026-10-02-án ellenőriztem: a 25 HTML és a `01_General/1_MIR_levelező_2026_27_1.pdf` bájtra azonos a mappában lévő fájlokkal, és a 80 kép is megvan mindkét helyen. **Ne bontsd ki a `Források` mappába.** Ha ellenőrizni akarod, a munkaterület ideiglenes könyvtárába csomagolj ki. Eltérést forrásütközésként jelents.
- **Kódolás és sorvégjel.** Az új fájlok UTF-8 kódolásúak. A tételfájlok többsége CRLF sorvégű: ellenőrizd egy meglévő tétel (pl. K07) sorvégjelét a `file` paranccsal, és az új tételfájl ugyanazt kövesse. A `README.md` és a `Tétel-Tárgy Mátrix.md` LF sorvégű: ezt tartsd meg, és a fájlokat helyben szerkeszd, ne gépeld újra emlékezetből.
- **Gitben soha semmit ne végezz el**: nincs `git add`, `git commit`, `git push`, `git stash`, `git checkout` vagy `git reset`. A commit mindig a futtató feladata. Olvasó parancsot **kizárólag** `git --no-optional-locks status` és `git --no-optional-locks diff` formában futtathatsz, mert a sima `git status` `.git/index.lock` fájlt hozhat létre, amelyet a Cowork-környezet nem tud törölni, és ez a futtató commitját blokkolja. Ha mégis találsz `.git/*.lock` fájlt, **ne próbáld törölni**, hanem jelezd a záró jelentésben, hogy a futtatónak kell eltávolítania a commit előtt.
- **Webes keresést ne használj.** A munka kizárólag a mappában lévő anyagokra épül.

### 2.4 Előfeltétel-ellenőrzés (0. fázis)

1. Keresd ki a Mátrixból a V6–V10 sorait, és ellenőrizd, hogy a tárgy forrásmappája létezik és nem üres.
2. **`V0x` hívásnál:** ha a `Tételek/` mappában már van `V0x-…` fájl, **állj meg**: az revízió, nem kidolgozás. Ilyenkor a Tétel revíziós prompt való, és ezt jelezd.
3. **`ANYAG` hívásnál:** ha a kontextusfájl már létezik, **ne írd felül**. Állj meg, és kérdezd meg, frissítsd-e (és mit), vagy hagyd változatlanul.
4. **`V0x` hívásnál**, ha a kontextusfájl még nem létezik, jelezd, hogy az `ANYAG` hívás gyorsítaná és egységesítené a munkát, de folytathatod. A kontextusfájl hiányában a „Döntési napló” (5.4) is hiányzik, így a 4.B szerinti kérdéseket mind fel kell tenned.

## 3. Forrásszabály (a legfontosabb korlát)

### 3.1 Megengedett források

A tétel és a kontextusfájl **kizárólag** az alábbiakra támaszkodhat:

1. **Syllabus:** a `Menedzsment információs rendszerek (GMXIR1MBLF).pdf` (szöveges PDF, hivatalos). A „TANTÁRGYNYILVÁNTARTÓ” adatlap is hivatalos syllabus, ha a mappában előkerül.
2. **A tárgy mappájában lévő tananyag**, három szinten:
   - **Kötelező tananyag** (`1_NN … Kötelező tananyag.html`): **elsődleges forrás.**
   - **Opcionális Fogalmi Alapkönyv** (`2_NN …`) és **Opcionális Haladó Könyv** (`3_07 …`): megengedett, de **másodlagos**. Ha egy állítást csak opcionális forrás támaszt alá, az `CSAK OPCIONÁLIS` jelölést kap a lefedettségi mátrixban és az auditban. A tételben maradásáról a **Döntési napló** (5.4) rendelkezik; ha a napló erről nem szól, **JÓVÁHAGYANDÓ** kérdést kell feltenni. Ha a kötelező és az opcionális szint ellentmond egymásnak, az forrásütközés (3.3).
   - A HTML-ekhez tartozó **ábrák** (lásd 2.3).
3. **A syllabusban megnevezett kötelező irodalom:** Laudon, K. C., & Laudon, J. P. (2022). *Management information systems: Managing the digital firm* (17th ed.). Pearson; Turban, E., Pollard, C., & Wood, G. (2018). *Information technology for management* (11th ed.). Wiley; Microsoft. (2025). *Power BI documentation*. Microsoft Learn.
4. **A syllabusban megnevezett ajánlott irodalom:** Bángi-Magyar, A. et al. (é. n.). *AVIR kézikönyv* (Digitális Tankönyvtár); Bencsik, A. (2015). *A tudásmenedzsment elméletben és gyakorlatban*; Bencsik, A. (2024). *Tudásmenedzsment elméletben és gyakorlatban* (bőv. kiad.); Chikán, A. (2008). *Vállalatgazdaságtan* (4. kiad.).

A 3. és 4. pont alatti művek **egyike sincs a mappában**, ezért a 3.3 „megnevezett, de nem elérhető irodalom” szabálya vonatkozik rájuk.

### 3.2 Nem megengedett források

Minden más forrás tiltott. Ide tartozik:

- a webes forrás, és minden saját tudásból származó, forrással alá nem támasztott tartalom;
- a HTML-ek lábjegyzeteiben („Forrás: …”) megnevezett külső művek **saját tartalma** (pl. Laudon & Laudon 15. és 18. kiadása, Kaplan & Norton 1996, Tufte, Few, Goodhart 1975, Thomas & Uminsky 2022, Garai-Fodor et al. 2023). Belőlük csak az használható, amit a HTML szövege maga közöl (lásd 3.3);
- a kontextusfájl saját esetleges irodalmi listái;
- **más tárgy anyaga.** Ha a GMXIV2MBLF (V11–V15) vagy más tárgy anyagában hasonló téma szerepel (pl. ERP, BI), abból tartalmat nem vehetsz át. A kapcsolódás csak utalás lehet („lásd V12”);
- a dekoratív vagy illusztratív képek, és minden személyes vagy hallgatói dokumentum.

### 3.3 Különleges esetek

- **Kontextusfájl.** A korábbi kontextusfájlokhoz hasonlóan **nem forrás**, csak navigációs segéd: arra való, hogy megtaláld, melyik forrásfájl melyik szakasza releváns. Állítást csak akkor hagyhatsz a tételben, ha azt a megengedett forrás eredeti szövegében is megtaláltad. **Egyetlen kivétel a „Döntési napló” szakasz**: az a futtató (én) jóváhagyott döntéseit rögzíti, és rá kötelező érvényűként kell támaszkodnod.
- **A HTML-ek belső hivatkozásai („Forrás: …”).** A HTML a megengedett forrás, a benne megnevezett külső mű viszont nem elérhető. Ezért: (a) a külső mű tartalmát nem egészítheted ki; (b) ha egy állítás szerzőhöz és évszámhoz kötött (pl. „Kaplan és Norton, 1996”), a tételben **másodlagos hivatkozásként** jelenjen meg, azaz `(Kaplan & Norton, 1996, idézi: <HTML-forrás szerzője>, <év>, <szakasz>)`, és az Irodalomba **csak a HTML-forrás** kerüljön; (c) ha a HTML belső hivatkozása kétséges vagy hiányos, vagy saját anyagra hivatkozik („saját anyag”), a hivatkozást a HTML-re add meg, a külső művet ne nevezd meg.
- **Kiadás-eltérés.** A syllabus Laudon & Laudon 2022-es, 17. kiadását nevezi meg, a HTML-ek a 15. (2017) és 18. (2025) kiadásra hivatkoznak. Ezt ne oldd fel: a kiadás-specifikus számadatot, ábraszámot vagy fejezetszámot ne vegyél át, és a ténylegesen releváns esetet jelentsd forrásütközésként.
- **Megnevezett, de a mappában nem elérhető irodalom** (a syllabus 3. és 4. pontja). (a) Új állítást nem írhatsz be rájuk hivatkozva. (b) Ha a tételnek olyan, a helyi anyagban nem ellenőrizhető állítása lenne, amely ilyen műre épül, tedd fel kérdésként. (c) Ha a tétel témája a műre épül, kerüljön a „Beszerzendő anyagok” táblázatba. Egy mű csak akkor kerül be, ha az adott tétel témája tényleg rá épül; ne listázd a tárgy összes hiányzó művét.
- **Tartalmi hiány (ez az új tárgy jellemző problémája).** Ha a hivatalos tételszöveg olyat kér, ami a megengedett forrásokban nincs meg vagy csak felületesen szerepel (Függelék A), **forráson kívüli tartalmat ne írj be.** A „nem szerepel” megállapításhoz **teljes szöveges keresést** végezz (ékezetes és ékezet nélküli alak, rövidítés és kifejtett alak, magyar és angol kifejezés), a keresett kifejezéseket pedig sorold fel a kérdésben. Hiány esetén a kérdés lehetséges válaszai: **A)** beszerzés: te pótolod az anyagot a mappába (a „Beszerzendő anyagok” táblázatba kerül, és a tétel az újrafuttatáskor bővül); **B)** a részkérdés a tételfájlban `### ⚠️ Tartalmi hiány — <téma>` címmel, kitöltetlenül marad, egy-két mondattal arról, mit kér a tételsor és mi nincs a forrásokban (a tétel így nyíltan jelzi a hiányt, nem tünteti el); **C)** az értelmezés szűkítése, ha a tételszöveg példát kér („pl. EVA, Z-score”), és a tananyagban hasonló kategóriából más példa szerepel (ez **JÓVÁHAGYANDÓ**, mert a tételszöveg értelmezését érinti). Más megoldás nincs: a hiányt saját tudásból pótolni tilos.
- **Forrásütközés.** Ha két megengedett forrás ellentmond egymásnak (kötelező és opcionális szint, két előadás, HTML és syllabus), ne dönts helyettem. Mutasd be mindkét változatot a lelőhelyükkel, és kérdezz.
- **Terminológia.** Ellenőrizd, hogyan viszonyul a tananyagban a MIR/MIS és a VIR (a `1_01` előadás „MIR/VIR” megfogalmazást használ). Ha a tananyag egyenlőségjelet tesz közéjük, ezt a tételben is így add meg, a forrás szerint. Ha nem egyértelmű, kérdezz.
- **Tantárgyon belüli kapcsolódás.** A tananyag több előadása (2. Porter és versenyelőny, 3. ERP/CRM/SCM, 10. felhő, 11. etika és felelős AI, 12. kiberbiztonság) nincs közvetlenül tételhez rendelve. Kapcsolódási pontként használhatók (a Jeles-mérce kéri a tárgyon belüli kapcsolódásokat), de nem terjeszthetik a törzsszöveget a terjedelmi kereten túlra.

### 3.4 Hivatkozás a HTML-tananyagra és a syllabusra (APA 7)

A HTML-eken **nincs szerző, évszám, oldal- vagy diaszám**. Ezeket **ne találd ki**. A hivatkozás formáját a „Döntési napló” rögzíti; ha még nincs napló, ez az `ANYAG` hívás kötelező kérdése (4.A, K2). Az alábbi **javaslatot** terjeszd elő, és kérj rá jóváhagyást:

- Szerző: Óbudai Egyetem, Keleti Károly Gazdasági Kar, Üzleti Tudományok és Digitális Ismeretek Intézet (a syllabus szerinti intézet). A tantárgyfelelős (Prof. Dr. Tick Andrea) neve **nem** kerülhet szerzőként a hivatkozásba, mert a syllabus nem mondja ki, hogy a HTML-ek szerzője.
- Év: 2026 (a syllabus szerinti félév: 2026/27/1). Ugyanazon szerző és év esetén `2026a`, `2026b` … a cím szerinti ábécésorrendben.
- Leírás: `[Kötelező tananyag, 6. ea.]`, `[Opcionális fogalmi alapkönyv, 6. ea.]`, `[Opcionális haladó könyv, 7. ea.]`. Az előadásszám a **fájlnévből** származik, és **nem azonos** a syllabus heti sorszámával (lásd Függelék A).
- Szövegközi hely: `(ÓE KGK ÜTDI, 2026c, 5. szakasz)`, a HTML saját szakaszszámozása (tartalomjegyzéke) szerint. Ha a szakaszszám nem állapítható meg egyértelműen, hagyd el.
- Syllabus: `Óbudai Egyetem, Keleti Károly Gazdasági Kar. (2026). *Menedzsment információs rendszerek (GMXIR1MBLF)* [Syllabus].`

## 4. Munkafolyamat

Az 1–2. fázis (A1–A2, illetve B1–B2) **csak olvasás**: ilyenkor egyetlen fájlt sem módosítasz.

### 4.A `ANYAG` hívás: a tananyag feldolgozása

#### A1 — Leltár és szerkezet (csak olvasás)

1. **Fájlleltár:** típusonként a darabszám, az olvashatóság, a zip–mappa azonosság (hash-összevetés), a hivatkozatlan és a duplikált képek (pl. a `4.O3.png` és `4.O3 (1).png` azonos méretű), az illusztratív képek listája.
2. **Syllabus ↔ előadás-fájlok:** vesd össze a syllabus heti tematikáját a 12 HTML-előadással. Az előzetes észrevételek (Függelék A) szerint a két lista számra egyezik, de tartalmilag nem 1:1: a HTML-számozás eltér a syllabus heti számozásától, és a syllabus 11. heti előadásához (E-kereskedelem és platform-gazdaság) nincs önálló HTML. **Ellenőrizd, ne vedd át.** Rögzítsd azt is, hogy a gyakorlatok anyaga (Excel-dashboard, Power BI) hiányzik.
3. **Megnevezett irodalom:** a syllabus hét művéből melyik van a mappában (jelenleg egy sem), és melyik tételnek lenne releváns.
4. **A HTML-ek belső hivatkozásainak jegyzéke:** előadásonként a „Forrás: …” sorok, és hogy a hivatkozott mű szerepel-e a syllabusban vagy a mappában. Jelöld a kiadás-eltéréseket.
5. **Terminológia:** a MIR/MIS/VIR használata a tananyagban (3.3), és a VIR-rövidítés ütközése a V11–V15 tárggyal.
6. **Részkérdés-bontás és előzetes leképezés** a V6–V10 tételekre: szó szerint idézd a hivatalos tételszöveget, bontsd részkérdésekre (R1, R2, …; minden felszólító ige és minden felsorolt tárgy külön R), és mindegyikhez rögzítsd a releváns forrásfájlt és szakaszt, valamint az állapotot: ✅ lefedett / ⚠️ gyenge / ❌ hiányzik / `CSAK OPCIONÁLIS`. A releváns szakaszokat **olvasd el**, ne csak kulcsszóra keress, a Függelék A előzetes térképét pedig ellenőrizd.
7. **Terjedelmi előrejelzés:** hány részkérdése és résztémája van az egyes tételeknek, és belefér-e az irányérték (kb. 1100–1900 szó) a Jeles-mércével. A V8–V10 hivatalos szövege 6–8 résztémát tartalmaz, ezért az irányérték szűk lehet. **A részkérdést ne csonkítsd, hogy beleférjen**: tegyél javaslatot (pl. táblázatos tömörítés, emelt keret), és kérdezz.

#### A2 — Jelentés és kérdések (a chatben, fájlmódosítás nélkül)

Egyetlen, jól tagolt üzenetben add le:

1. **Összkép** (3–5 mondat): mennyire fedi le a tananyag a V6–V10 tételeket, és melyek a fő hiányok.
2. **Forrásleltár** táblázatban (A1/1–4).
3. **Lefedettségi mátrix tételenként:** részkérdés | forrás (fájl + szakasz) | állapot.
4. **Tartalmi hiányok összesítve:** tétel | részkérdés | mit kér a tételsor | mit találtál a forrásokban | keresett kifejezések | javaslat (A/B/C, 3.3).
5. **Beszerzendő anyagok összesítő tervezete** (formátuma: revíziós prompt 5.2, kiegészítve az 5.2 pont szerint).
6. **A kontextusfájl vázlata** (címsorok, 5.4) és a nyilvántartási változások terve (5.5).
7. **Kérdések** számozva (K1, K2, …). Mindegyik tartalmazza: a kontextust 1–2 mondatban, a lehetséges válaszokat (A/B/C), a javaslatodat indoklással, és azt, mi következik az egyes válaszokból. **Legalább ezeket tedd fel, ha a vizsgálat igazolja a hátterüket:**
   - **K1 — Opcionális források:** az `Opcionális Fogalmi Alapkönyv` és az `Opcionális Haladó Könyv` tartalma felhasználható-e a tételekben (és ha igen, jelölni kell-e), vagy csak a kötelező tananyag. (A vizsgáztató elvárását nem ismerheted; a javaslatodat indokold, és ezt a bizonytalanságot jelezd.)
   - **K2 — Hivatkozási forma:** a 3.4 pont szerinti szerző–év–leírás javaslat jóváhagyása vagy módosítása.
   - **K3 — Tartalmi hiányok kezelése tételenként** (EVA, Z-score, DAX, hazai VIR/BI programcsomagok összevetése, jelentés-megosztás és jogosultságkezelés stb.), A/B/C választással.
   - **K4 — Terminológia:** a MIR/MIS/VIR viszony rögzítése.
   - **K5 — Terjedelem:** a V8–V10 tételek emelt keretének jóváhagyása vagy más megoldás.
   - **K6 — Másodlagos hivatkozások:** a HTML belső „Forrás:” soraiban szereplő szerzők és évszámok használata a 3.3 szerinti másodlagos hivatkozási formában.
   - Továbbá minden, a vizsgálat során talált forrásütközés vagy bizonytalanság.

**Ezután állj meg, és várd meg a válaszomat.** Ne hozz önállóan mélyebb döntést.

#### A3 — Kontextusfájl létrehozása (csak jóváhagyás után)

Hozd létre a kontextusfájlt az 5.4 pont szerinti szerkezetben. A **Döntési naplóba** a válaszaimat dátummal, szó szerinti vagy pontos összefoglalással írd be. A fájl legyen **tömör**: nem tankönyvi összefoglaló, a tananyag tartalmát ne másold át, csak mutatókat (fájl + szakasz) és ellenőrzött tényeket tartalmazzon.

#### A4 — Nyilvántartás frissítése

Az 5.5 pont szerint frissítsd a `README.md`-t és a `Tétel-Tárgy Mátrix.md`-t. **A V6–V10 tételek állapota 📋** (forrásanyag elérhető, kidolgozás szükséges); ha valahol még ⏳ szerepel, javítsd. A Revízió oszlop `—` marad, és a 35 kidolgozott tétel adata nem változik. Ha a feldolgozás a tényleges tartalmi hiányokat feltárta, a README „Megjegyzések” szakaszában a V6–V10-ről szóló sort pontosítsd (mi hiányzik, mi a jóváhagyott kezelés).

#### A5 — Záró ellenőrzés és jelentés

Ellenőrizd a 6. fejezet `ANYAG`-ra vonatkozó pontjait, majd a chatben add le: a létrehozott és módosított fájlokat, a döntéseimet összefoglalva, a nyitva maradt kérdéseket, a beszerzendő anyagok listáját (mit kell a mappába tennem, hogy a hiányzó részek pótolhatók legyenek), és a **commit-üzenet javaslatot** két külön kódblokkban:

- **1. kódblokk, cím (egyetlen sor):** Conventional Commits, `docs(GMXIR1MBLF): <összefoglaló>`, magyarul, pont nélkül, legfeljebb kb. 72 karakter. Példa: `docs(GMXIR1MBLF): tananyag-feldolgozás és kontextusfájl a V06–V10-hez`
- **2. kódblokk, leírás:** 1–2 mondatos összefoglaló, majd `- ` felsorolás (az új kontextusfájl, a README és a Mátrix változásai, a beszerzendő anyagok); ha maradt nyitott kérdés, egy `Nyitott:` sor; sorhossz legfeljebb kb. 72 karakter; a kódblokkon belül ne használj markdown-kiemelést. Csak azokat a fájlokat írja le, amelyeket ebben a hívásban ténylegesen módosítottál (`git --no-optional-locks status` / `git --no-optional-locks diff` segíthet; a mappa más, korábbi módosításait, pl. sorvégjel-eltéréseket ne vedd bele).

**A commitot nem végzed el.**

### 4.B `V06`–`V10` hívás: tétel kidolgozása

#### B1 — Helyzetfelmérés (csak olvasás)

1. **Döntési napló:** ha a kontextusfájl létezik, olvasd el a Döntési naplót; minden ott rögzített döntés rád nézve kötelező. Amiről a napló nem szól, azt kérdésként kell kezelned.
2. **Hivatalos tételszöveg:** emeld ki szó szerint a tételsor-PDF-ből, és bontsd részkérdésekre (R1, R2, …; minden felszólító ige és minden felsorolt tárgy külön R). A V6–V10 hosszú, többrészes tételek: a bontás legyen aprólékos.
3. **Releváns források feldolgozása:** a kontextusfájl leképezését használd kiindulásnak, de **a forrásfájlokat magukat olvasd el**, ne a kontextusfájl összefoglalójára hagyatkozz. A tartalmat hordozó ábrákat nézd meg (2.3).
4. **Lefedettségi mátrix** (belső munkaanyag, a tételfájlba nem kerül): minden részkérdéshez rögzítsd, mely forrás mely szakasza támasztja alá (fájl + szakasz), és az állapotot (✅ / ⚠️ gyenge / ❌ hiányzik / `CSAK OPCIONÁLIS`).
5. **Állítás-nyilvántartás:** minden leendő lényegi állításhoz (definíció, szerző és évszám, modell elemei, lépések, számok, példák) rögzítsd a lelőhelyet (fájl + szakasz). **Amit nem tudsz lelőhelyhez kötni, azt nem írhatod be.** A szerzőhöz kötött állítások másodlagos hivatkozási formát kapnak (3.3).
6. **Jeles-mérce tervezési szinten:** a leendő tétel akkor éri el a mércét, ha minden részkérdésre válaszol; a kulcsfogalmak definíciója a forrás szerinti; a tananyagban szereplő kulcsszerzők és modellek névvel és évszámmal szerepelnek (a másodlagos hivatkozás szabályai szerint), a modellek elemei hiánytalanok; a fogalmak közötti összefüggések és a tárgyon belüli kapcsolódások ki vannak bontva; ahol a tananyag ad, ott van példa és kritika vagy korlát; a felépítés logikus (bevezetés, kifejtés, szintézis). **Ahol a forrás ezt nem teszi lehetővé, jelezd.**
7. **Terjedelmi terv:** a törzsszöveg irányértéke kb. 1100–1900 szó (a táblázat, a diagram, a „Beszerzendő anyagok”, a „⚠️ Tartalmi hiány” szakaszok, a „Várható vizsgáztatói kérdések” és az „Irodalom” nem számít bele). Ha a részkérdések száma emelt keretet kívánna, a Döntési napló rendelkezik róla; ha nem, kérdezz.
8. **Diagramterv:** csak a forrásban szereplő modellekből, és csak ott, ahol a feleletben segít (szerkezetet, ciklust, összehasonlítást mutat). A palettát és a szabályokat a revíziós prompt 5.3 pontja adja.

#### B2 — Jelentés, vázlat és kérdések (a chatben, fájlmódosítás nélkül)

Egyetlen, jól tagolt üzenetben add le:

1. **Összkép** (3–5 mondat): részkérdésenként elérhető-e a megengedett forrásokból a Jeles-szint, és mik a fő problémák.
2. **Lefedettségi mátrix** táblázatban: részkérdés | tervezett tételszakasz | forrás (fájl + szakasz) | állapot.
3. **Kidolgozási vázlat** táblázatban: ID | tervezett szakasz (cím) | lefedett részkérdések | fő források | becsült szószám | diagram | **besorolás** (`AUTONÓM` / `JÓVÁHAGYANDÓ`).
4. **Tartalmi hiányok** (3.3 szerint, A/B/C javaslattal), **Beszerzendő anyagok** tervezete, a javasolt **rövid cím és fájlnév**.
5. **Kérdések** számozva (K1, K2, …) a revíziós prompt 2. fázisának formátuma szerint.

**AUTONÓM** (külön engedély nem kell hozzá, ha megfelel a 3. fejezetnek): a szakaszok felosztása a részkérdések logikája szerint; a szöveg megírása megengedett forrásból, a forrás definícióinak, szerzőinek, évszámainak és modellelemeinek átvétele; hivatkozások a Döntési napló szerinti APA 7 formában; Mermaid-stílus és szintaxis; a „Várható vizsgáztatói kérdések” szakasz; a sablon kötelező szakaszai; a Döntési naplóban már rögzített döntések végrehajtása.

**JÓVÁHAGYANDÓ** (előbb kérdezz): a hivatalos tételszöveg értelmezése, ha egy részkérdés többféleképpen érthető; tartalmi hiány kezelése (kivéve, ha a napló rendelkezik róla); forrásütközés feloldása; `CSAK OPCIONÁLIS` tartalom sorsa (kivéve, ha a napló rendelkezik róla); terjedelmi keret túllépése; diagram elhagyása vagy a vázlattól eltérő új diagram; egy fájlról el kell dönteni, hogy tananyag-e; minden olyan döntés, amelyet ez a prompt nem szabályoz egyértelműen.

**Ezután állj meg, és várd meg a válaszomat.** A vázlatot egészében hagyom jóvá; az AUTONÓM sorokat nem kell egyenként megerősítenem, de bármelyiket módosíthatom vagy elvethetem.

#### B3 — Kidolgozás (csak jóváhagyás után)

- Hozd létre a tételfájlt az 5.1 pont szerinti célállapotban, a jóváhagyott vázlat szerint.
- **Minden lényegi állításnak legyen szövegközi hivatkozása.** Számot, évszámot, szerzőt, idézetet, szakaszszámot csak a forrásból vehetsz át.
- A „Tétel:” sorba a hivatalos tételszöveg kerüljön szó szerint.
- A szintézis (Összegzés) szakaszban jelenjenek meg a tárgyon belüli kapcsolódások (a többi V6–V10 tételhez és a tananyag más előadásaihoz). A V11–V15 tételekre csak utalás kerülhet (3.2).
- Ha végrehajtás közben új, a vázlatban nem szereplő **JÓVÁHAGYANDÓ** kérdés merül fel, **állj meg és kérdezz**; a már elvégzett lépéseket jelezd.
- A tételfájlon kívül semmit ne módosíts, kivéve a B4 nyilvántartásait.

#### B4 — Nyilvántartás frissítése

Az 5.5 pont szerint frissítsd a `README.md`-t és a `Tétel-Tárgy Mátrix.md`-t.

#### B5 — Záró ellenőrzés és jelentés

Ellenőrizd a 6. fejezet pontjait, majd a chatben add le: a végrehajtott és elvetett vázlatsorokat; a végleges terjedelmet (törzsszöveg szószáma, becsült felelési idő); a lefedettségi mátrix végállapotát (különösen a ⚠️ Tartalmi hiány szakaszokat); a mermaid-renderelés eredményét; a nyitva maradt kérdéseket.

#### B6 — Szemantikus commit-üzenet javaslata (utolsó lépés)

Az üzenetet **két külön kódblokkban** add le, a commitot **nem végzed el**:

- **1. kódblokk, cím (egyetlen sor):** `docs(V06): <összefoglaló>` (a hatókör a tételszám a fájlnév szerinti alakban), magyarul, egyetlen mondat, pont nélkül, legfeljebb kb. 72 karakter. Példa: `docs(V06): V06 tétel kidolgozása az 1. előadás alapján`
- **2. kódblokk, leírás:** 1–2 mondatos összefoglaló, majd `- ` felsorolás: az új tételfájl, a ⚠️ Tartalmi hiány szakaszok, a „Beszerzendő anyagok” táblázat, a mermaid-diagramok, a `README.md` és a `Tétel-Tárgy Mátrix.md` frissítése; ha maradt nyitott kérdés, `Nyitott:` sor; sorhossz legfeljebb kb. 72 karakter; a kódblokkon belül ne használj markdown-kiemelést.

## 5. Célállapot

### 5.1 A tételfájl

A fájl a revíziós prompt **5.1 pontjának sablonját** kövesse (fejléc, opcionális „Beszerzendő anyagok”, „Tétel:”, tartalmi szakaszok, „Várható vizsgáztatói kérdések”, „Irodalom”), az alábbi eltérésekkel és kiegészítésekkel:

- **Fejléc:** `## V6 – <A tétel címe>` (a tételsor szerinti egyjegyű alak, `V10` kivételével), a fájlnév viszont `V06-GMXIR1MBLF-…`.
- **Tartalmi szakaszok:** a részkérdések logikája szerint, a vázlat szerint. A hiány helyén `### ⚠️ Tartalmi hiány — <téma>` szakasz állhat (3.3, B válasz).
- **Hivatkozás:** a 3.4 pont és a Döntési napló szerint. Szövegközi hivatkozás formája: `(Szerző, év, szakasz)`. **Oldal- vagy diaszámot ne találj ki.**
- **Irodalom:** `## Irodalom` címsor, `* ` felsorolás, APA 7, ábécérendben. **Csak** a ténylegesen hivatkozott HTML-tananyag(ok) és (ha hivatkozás van rá) a syllabus kerülhet bele. A másodlagosan idézett külső művek **nem** szerepelnek az Irodalomban (3.3).
- **„Várható vizsgáztatói kérdések”:** 4–6 kérdés. A V6–V10 hosszú, többrészes tételeknél különösen ide valók a felelet után valószínű kiegészítő kérdések (fogalmi pontosítás, összehasonlítás, alkalmazás, kapcsolódás más témához a tárgyon belül, kritika vagy korlát). A válaszvázlatok is csak megengedett forrásra épülhetnek. A szakasz nem számít bele a terjedelmi mércébe.
- **Sorvégjel:** az új fájl CRLF sorvégű legyen, ha a meglévő tételfájlok is azok (2.3).

### 5.2 „Beszerzendő anyagok” táblázat

A revíziós prompt 5.2 pontja szerint (a tétel legelején, `Szerző | Mű | Jelleg | Indoklás / érintett rész` oszlopokkal; ha nincs hiány, a szakasz elmarad), két kiegészítéssel:

- A „Jelleg” megengedett értékei a revíziós prompt értékei **és** a `gyakorlati anyag` (a gyakorlati órák Excel- és Power BI-anyagai a tananyag részei, de a mappában nincsenek meg).
- A syllabus által megnevezett művek csak akkor kerülnek be, ha az adott tétel témája tényleg rájuk épül, az indoklás pedig megnevezi az érintett részkérdést (R-számmal).

### 5.3 Mermaid-diagramok

A revíziós prompt **5.3 pontja** szerint, változatlanul: a 8 színű paletta, a H-változatok, az élstílusok, a `subgraph` tónusok, a diagramtípusonkénti `%%{init}%%` blokkok és a diagramszabályok. A palettán kívüli szín vagy új osztálynév JÓVÁHAGYANDÓ. Ha a környezetben elérhető, ellenőrizd a renderelést (`npx -y @mermaid-js/mermaid-cli`); ha nem, szintaktikai átnézést végezz, és a záró jelentésben jelezd, hogy renderelve nem ellenőrizted.

### 5.4 A kontextusfájl szerkezete (`ANYAG` hívás)

Fájl: `Kontextus fájlok/Váll.Irány II. - Menedzsment információs rendszerek (GMXIR1MBLF).kontextus.md` (a név a sorozat meglévő I., III., IV. tagjához illeszkedik). Címe: `# Menedzsment információs rendszerek (GMXIR1MBLF) — Kontextus és forrástérkép`. Szakaszai ebben a sorrendben:

1. **A fájl jellege:** rövid megjegyzés, hogy a fájl navigációs segéd, **nem forrás**; kivétel a Döntési napló.
2. **Tantárgy adatok:** kód, kredit, tagozat, félév, intézet, tantárgyfelelős, óraszám, számonkérés: a syllabusból.
3. **Forrásleltár:** a fájlok típus szerint, a szintekkel (kötelező / opcionális fogalmi / opcionális haladó), az ábrák állapotával, a zip-azonossággal.
4. **Syllabus-hét ↔ előadásfájl:** a számozási eltérések és a hiányzó anyagok jelölésével.
5. **Tétel ↔ forrás leképezés:** V6–V10, részkérdés-szinten (R → fájl + szakasz → állapot).
6. **Tartalmi hiányok:** tétel | részkérdés | keresett kifejezések | állapot | a jóváhagyott kezelés.
7. **Beszerzendő anyagok (összesítve).**
8. **A HTML-ekben hivatkozott külső művek jegyzéke** és a kiadás-eltérések.
9. **Terminológia:** MIR / MIS / VIR, és a VIR-rövidítés ütközése a V11–V15 tárggyal.
10. **Döntési napló:** dátum | kérdés | **az én válaszom**. Ez az egyetlen kötelező érvényű szakasz.

### 5.5 Nyilvántartás

**`README.md`** (LF sorvégű, helyben szerkeszd):

- A B) táblázatban a V06–V10 sorainak **Állapot** oszlopa: a forrásanyag megérkezte óta `📋`; a tétel kidolgozása után `✅`. A **Revízió** oszlop a tétel kidolgozása és sikeres záró ellenőrzése után `✅ ÉÉÉÉ-HH-NN` (a mai dátum). Indok: a `V0x` hívás a kidolgozást és a revíziós prompt szerinti forrás-auditot egyben végzi; ha a hívás nyitott kérdéssel zárul, a Revízió oszlop `🔎 ÉÉÉÉ-HH-NN`.
- A „Tantárgyak összefoglalása” táblázat GMXIR1MBLF sora: jelenleg `📋 Forrásanyag elérhető`; mind az öt tétel kidolgozása után `✅ Teljes`.
- A „A repó szerkezete” fában jelenjen meg az új kontextusfájl (`ANYAG` után) és (kidolgozás után) a V06–V10 tételfájlok (a promptfájl és a forrásmappa már szerepel); a „(V06–V10 tételek kidolgozás alatt …)” sor igazodjon az állapothoz.
- A „Jelenlegi állapot” és a „Megjegyzések” szakasz V6–V10-re vonatkozó, elavult sorai (pl. „szünetel”, „forrásanyagra vár”) igazodjanak a tényleges állapothoz. A számlálók és szöveges összesítők legyenek egymással összhangban: a 40 tételből kidolgozott tételek számát **csak** a ténylegesen elkészült tételek szerint növeld.
- **Az utolsó sor `*Utolsó frissítés: …*` szövegét minden esetben írd át** a mai dátumra, és röviden írd le a változást.

**`Kontextus fájlok/Tétel-Tárgy Mátrix.md`:**

- A V6–V10 sorokban a **Mappa** oszlop jelenleg `📋`, a tétel elkészülte után `✅`; a Revízió oszlop a README szabálya szerint.
- Az „Összefoglaló táblázat” GMXIR1MBLF sorában az „Anyag elérhető” oszlop jelenleg `📋 Elérhető (feldolgozásra vár)`; mind az öt tétel kidolgozása után `✅ Teljes`. Az „Összesen” sor számai igazodjanak.
- A `**Utolsó frissítés:**` sort írd át dátummal és rövid leírással.

A többi kontextusfájlt ne módosítsd. Ha bennük hibát találsz, a záró jelentésben jelezd.

## 6. Záró ellenőrzőlista

**`ANYAG` hívásra:**

- [ ] A forrásleltár ellenőrzött tényeken alapul (hash-összevetés, olvashatóság), nem az előzetes észrevételeken.
- [ ] A V6–V10 minden részkérdése szerepel a leképezésben; minden „nem szerepel” megállapítást teljes szöveges keresés támaszt alá, a keresett kifejezések rögzítve.
- [ ] A kontextusfájl az 5.4 szerinti szerkezetű, tömör, és a Döntési napló tartalmazza minden válaszomat.
- [ ] A `README.md` és a `Tétel-Tárgy Mátrix.md` frissítve (állapotok, összefoglalók, fa, „Utolsó frissítés”).
- [ ] Forrásfájlt, másik kontextusfájlt és tételt nem módosítottam; a zipet nem bontottam ki a `Források` mappába.
- [ ] A commit-üzenet két külön kódblokkban le van adva; git-műveletet nem végeztem, és csak `--no-optional-locks` olvasó parancsot használtam.

**`V0x` hívásra** (a revíziós prompt 6. fejezetének megfelelője):

- [ ] Minden részkérdés (R1…Rn) lefedve, vagy `⚠️ Tartalmi hiány` szakasz jelzi, hogy miért nem; a lefedettségi mátrixban nincs kimondatlan ❌.
- [ ] Minden lényegi állításnak van lelőhelye egy megengedett forrásban; saját tudásból származó tartalom nincs.
- [ ] A szövegben és az „Irodalom”-ban nincs nem megengedett forrás; a másodlagosan idézett művek nem szerepelnek az Irodalomban; minden szövegközi hivatkozásnak van irodalomjegyzéki párja, és fordítva.
- [ ] A hivatkozási forma a Döntési napló szerinti; szerzőt, évszámot, szakaszszámot nem találtam ki.
- [ ] „Irodalom”: `## Irodalom`, `* ` felsorolás, APA 7, ábécérend.
- [ ] A „Beszerzendő anyagok” csak hiány esetén szerepel, a tétel legelején, 4 oszloppal és kötött „Jelleg” értékekkel.
- [ ] A „Várható vizsgáztatói kérdések” megvan (4–6 kérdés, forráshű válaszvázlattal).
- [ ] A törzsszöveg terjedelme a jóváhagyott kerethez illik, és elmondható 10–15 perc alatt.
- [ ] A mermaid-diagramok a palettát követik, és renderelnek (vagy jeleztem, hogy nem ellenőriztem); tartalmuk megfelel a szövegnek és a forrásnak.
- [ ] A fájl kódolása és sorvégjele egyezik a meglévő tételfájlokéval; más fájl nem sérült.
- [ ] A `README.md` és a `Tétel-Tárgy Mátrix.md` frissítve (Állapot és Revízió oszlop, összefoglalók, „Utolsó frissítés”).
- [ ] A commit-üzenet két külön kódblokkban le van adva; git-műveletet nem végeztem.

## 7. Amit soha ne tegyél

- Ne használj webes keresést vagy saját tudásból származó, forrással alá nem támasztott tartalmat. **Különösen ne töltsd ki a hiányzó témákat (pl. EVA, Z-score, DAX, programcsomag-összevetés) „általánosan ismert” tartalommal.** A hiány jelentés, nem kitöltendő rés.
- Ne találj ki szerzőt, évszámot, oldal-, dia- vagy szakaszszámot, idézetet, kiadást.
- Ne tulajdonítsd a HTML-ek szerzőségét valakinek (pl. a tantárgyfelelős oktatónak) jóváhagyás nélkül.
- Ne használj más tárgy (pl. GMXIV2MBLF) anyagából tartalmat.
- Ne módosíts és ne törölj forrásfájlt, másik kontextusfájlt vagy másik tételt; ne bontsd ki a zipet a `Források` mappába.
- **Soha ne commitolj**, és semmilyen más, a repót módosító git-műveletet se végezz. Olvasáshoz is csak `git --no-optional-locks …` használható.
- Az A2 és a B2 fázis végén ne lépj tovább jóváhagyás nélkül. JÓVÁHAGYANDÓ kérdésben ne dönts helyettem.

---

## Függelék A — Előzetes megfigyelések (2026-10-02)

> **Ez nem forrás és nem tény a tananyag tartalmáról.** A megfigyelések kulcsszavas, gépi szövegkeresésen alapulnak (a 25 HTML szövegkinyerése után), nem teljes olvasáson. Az `ANYAG` hívás A1 fázisában **ellenőrizd és pontosítsd** őket; ha eltérést találsz, az ellenőrzött eredmény számít.

**Hiányzó vagy gyengén lefedett elemek (a hivatalos tételszöveghez képest):**

| Tétel | A tételsor kérése | Előzetes megfigyelés |
|---|---|---|
| V6 | EVA és Z-score mint pénzügyi mutató, illetve összetett mutatószámrendszer | Egyik kifejezés sem szerepel a 25 HTML egyikében (EVA, Z-score, Altman, Economic Value Added, „hozzáadott érték”, „mutatószámrendszer”: 0 találat). A tananyag a KPI-, OEE-, ROI-, TCO-témát és a BSC-t tárgyalja. |
| V7 | A hazai VIR- és BI-programcsomagok sorba állítása elterjedtség, ár, komplexitás és BSC-támogatás szerint; a beépített BSC-támogatású rendszerek | Programcsomag-összevetés nem azonosítható. A 25 HTML szövegében BI-szoftvernévként csak a Power BI szerepelt (Tableau, Qlik, Looker, Cognos, MicroStrategy, Fabric: 0 találat). A BSC a `1_06`, a `2_06` és (említés szintjén) az `1_07` anyagában van. |
| V9 | DAX-kifejezések szerepe; egyéni és vállalati vizualizációk; jelentések megosztása vállalaton belül és kívül; rendszeradminisztrációs jogosultságok és engedélyezés | A „DAX” kifejezés 0 találat. A megosztás/jogosultság témát a syllabus 10. heti Power BI Service gyakorlata fedné, annak anyaga nincs a mappában. A syllabus kötelező irodalma (Power BI documentation) online forrás, nincs a mappában. |
| V6–V10 | Általában a Laudon–Turban-szerkezetű, a syllabus által megnevezett irodalom | A hét megnevezett mű egyike sincs a mappában. |

**Indikatív forrástérkép (kulcsszavas találatok alapján, ellenőrizendő):**

| Tétel | Valószínű források |
|---|---|
| V6 | `1_01` (az információs rendszer és a MIS szerepe; IS-típusok a szervezeti szinteken; MIR feladatai és a vezetői szintek információs igényei; „MIR/VIR”, szerepek, alkalmazási célok; gazdasági hatások és beruházás-gazdaságosság), `2_01` (opcionális), `1_06`/`2_06` (KPI) |
| V7 | `1_06` (5. szakasz: a BSC kritikai nézőpontból), `2_06` (BSC alapok, stratégiai térkép), `1_07` (BSC említése) |
| V8 | `1_05` (BI-érettségi modell és BICC; kié legyen a BI; mit támogat egy rendszer), `2_05` (Mi az a BI és BA; döntéstípusok; BICC), `1_01` (vezetői szintek) |
| V9 | `1_06` (KPI-tervezés, Goodhart-csapda, dashboard-tervezés, Power BI-kapocs), `2_06` (dashboard-tervezés alapszabályai), `1_07` (drill-down említések) |
| V10 | `1_04` (OLTP vs. OLAP, adattárház és adatpiac), `1_07` (OLAP, KDD, adatbányászat I–II), `2_07` (CRISP-DM), `3_07` (haladó adatbányászati számítások), `1_09` (szakértői rendszerek, tudásmenedzsment), `1_11` (szakértői rendszerek említése), `1_08` (Big Data) |

**Szerkezeti észrevételek:**

- A HTML-előadások (12) és a syllabus előadásai (12; a 7. héten nincs előadás) számra megegyeznek, de **nem felelnek meg egymásnak 1:1-ben**. Előzetesen: a HTML `1_06` („BI a gyakorlatban I.”: KPI, OEE, BSC, dashboard) nincs külön a syllabusban; a `1_07` („BI a gyakorlatban II.”: OLAP, KDD, adatbányászat) a syllabus 6. heti „OLAP és adatbányászat” előadásának felel meg; a `1_08` (Big Data) és az `1_09` (Tudásmenedzsment) sorrendje a syllabus 9. és 8. hetéhez képest fordított; a syllabus 11. heti „E-kereskedelem és platform-gazdaság” előadásának nincs önálló HTML-je (a platform-gazdaság az `1_02`-ben szerepel); az `1_11` (Etika) és az `1_12` (Kiberbiztonság) a syllabus 12. és 13. hetének felel meg. Az előadásszám a fájlnévből származik; a hivatkozásban erre ügyelj.
- A HTML-ek „Forrás:” soraiban a syllabus-szal egyező és attól eltérő kiadású művek vegyesen szerepelnek (Laudon & Laudon 15. és 18. kiadás, míg a syllabus a 17. kiadást nevezi meg); egyes sorok „saját anyag (ÜIA-ismétlés)” megjelöléssel szerepelnek.
- Vannak a fájlnevük alapján illusztratívnak tűnő képek (pl. `ChatGPT Image 2026. júl. 13. 20_12_40.png`, `HU flag.jfif`, `Target-logo-1024x682_1.jpg`; megnézésük az `ANYAG` hívás feladata), és azonos méretű képpár (`4.O3.png` és `4.O3 (1).png`).
