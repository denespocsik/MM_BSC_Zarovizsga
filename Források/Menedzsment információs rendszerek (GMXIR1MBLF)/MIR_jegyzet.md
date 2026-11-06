# Menedzsment információs rendszerek (GMXIR1MBLF) — ZH-készülési jegyzet (elméleti rész)

Forrás: a 12 előadás kötelező Moodle-tananyaga (kotelezo_01…12) és a tantárgyi adatlap. Kizárólag a tananyag tartalma; saját tudásból semmi nincs hozzátéve. A fejezethivatkozások formája: „N. ea. K. fej.” = N. előadás, K. fejezet (az eredeti Moodle-könyv N.K.html oldala).

**Tantárgyi adatlap — ZH-releváns tények (targyi_adatlap.txt):**

| Mi | Érték |
|---|---|
| Tantárgyfelelős | Prof. Dr. Tick Andrea |
| Intézet | Üzleti Tudományok és Digitális Ismeretek Intézet |
| Kredit | 4; levelező; magyar; 2026/27/1 félév |
| Óraszám | Előadás 5, labor 10 (féléves) |
| Félévzárás | Évközi jegy; írásbeli |
| Követelmények | 1 beadandó + félévzáró elméleti teszt + 1 ZH |
| ZH pontok | max. 50 pont (25 elmélet + 25 gyakorlat), részenként min. 20 % az aláírás feltétele; beadandó 25 pont |
| Jegyhatárok | 0–50 % elégtelen; 51–62 % elégséges; 63–74 % közepes; 75–86 % jó; **87–100 % jeles** |
| Segédeszköz | gyakorlati részhez 1 kézzel írt A4-es lap; fénymásolat, füzet, okostelefon TILOS; AI/GenAI TILOS |
| Pótlás | elégtelen teljesítés aláíráspótló vizsgán egyszer javítható; igazolt hiányzás egyszer pótolható; szóbeli nincs |
| Kötelező irodalom | Laudon & Laudon (2022) MIS 17th ed.; Turban, Pollard & Wood (2018) IT for Management 11th ed.; Microsoft Power BI documentation (2025) |
| Ajánlott | AVIR kézikönyv (Bángi-Magyar et al.); Bencsik (2015, 2024) Tudásmenedzsment; Chikán (2008) Vállalatgazdaságtan |
| Ütemterv (előadások) | 1. MIS valódi szerepe; 2. Versenyképesség és IT-stratégia (Porter, értéklánc, platform); 3. Integrált vállalat: ERP, CRM, SCM; 4. Mit ér az adat és ki felelős érte; 5. BI: kultúra, nem eszköz; 6. OLAP és adatbányászat; 7. –; 8. Tudásmenedzsment; 9. Big Data; 10. Felhő és IT-infrastruktúra; 11. E-kereskedelem és platform-gazdaság; 12. Etika, algoritmusok, felelős AI; 13. Kiberbiztonság, digitális transzformáció, MIS-jövő; 14. ZH |

⚠ forrásmegjegyzés: az adatlapon az oktatási hetek számozása (1–13. heti előadás, 7. hét üres) nem azonos a Moodle-könyv 12 előadásának számozásával: a Moodle 7. előadása = adatlap 8. hete (Tudásmenedzsment) stb. A jegyzet a Moodle-fájlok (kotelezo_01…12) számozását követi.

---

# 1. előadás: Az MIS valódi szerepe — miért nem elég a jó technológia?

## Egy mondatban (a központi tézis)

Az információs rendszerek sikerét vagy kudarcát döntő mértékben **nem a technológia minősége, hanem a szervezet, a menedzsment és a technológia közötti egyensúly** határozza meg; az IT önmagában nem termel értéket, csak komplementer (szervezeti, menedzsment, társadalmi) befektetésekkel párosítva (1. ea. 1., 2., 6. fej.).

## Nyitó eset és feloldása (1. ea. 1. és 8. fej.)

**Hershey Foods, 1999 ősz** — a világ egyik legnagyobb csokoládégyártója.

| Adat | Érték |
|---|---|
| Beruházás | 112 millió USD, teljesen új, integrált **SAP ERP** |
| Indítás időpontja | őszi csúcsszezon (halloween + karácsonyi szállítási időszak) |
| Teljesítetlen megrendelés | 100 millió USD értékű maradt a raktárakban, üres polcok |
| Részvényárfolyam | –8 % egyetlen nap alatt |
| Összes kár | > 150 millió USD |
| Ütemezés | 30 hónapos feladatot **18 hónapra** sűrítettek |

Nyitó kérdés: A) szoftver hibás; B) rossz időzítés; C) szervezet nem volt felkészülve; D) mindhárom egyszerre. **Helyes válasz: D) Mindhárom egyszerre — de nem véletlenszerűen.**

Feloldás a három dimenzió szemüvegén át (1. ea. 8. fej.):
- **Technológiai dimenzió:** a SAP-szoftver NEM volt hibás; az implementáció műszakilag sikeres volt.
- **Menedzsment dimenzió:** a felsővezetés ragaszkodott az eredeti határidőhöz (30 hónap → 18 hónap); a határidőnyomás miatt kihagyták a felhasználói tesztelést és a betanítást. „Klasszikus menedzsment-kudarc: a technikai mérföldkő fontosabb lett, mint az üzleti eredmény.”
- **Szervezeti dimenzió:** a raktárkezelők nem ismerték az új rendszert; a folyamatok nem voltak átdolgozva; a komplementer befektetések (képzés, folyamat-újratervezés, tesztelési idő) elmaradtak.
- **Következtetés:** klasszikus **„big bang” implementáció komplementer befektetések nélkül**; az eredmény „statisztikailag megjósolható volt”. Az ok-okozati lánc: **a menedzsment döntése (határidő-kényszer) okozta a szervezeti és technológiai kudarcot** — ez a lánc a MIS-kudarcok döntő többségében felismerhető.
- Elméleti pontok, amelyek bizonyítják: a három dimenzió modellje (2. fej.), a komplementer eszközök (6. fej.), az „IT természete” ellenállási tényező — big bang vs. inkrementális (5. fej.), a McKinsey–Oxford bukási statisztika (8. fej.: „a Hershey-eset tipikus, nem kivételes”).

## Fogalmak és definíciók (HU – EN)

- **Információs rendszer (IS)** — több mint számítógép: „A hatékony IS-használat megköveteli a szervezet, a menedzsment és az IT megértését, amelyek együtt formálják a rendszereket.” (Laudon & Laudon 2025, Ch.1 — a fejezet kulcsmondata, 1. ea. 2. fej.)
- **Jéghegy-modell** (Laudon Figure 1.5 alapján) — a csúcson a látható technológiai dimenzió; a víz alatt a szervezeti és menedzsment dimenzió; „a projektkudarcok döntő többsége a felszín alatt rejtőzik” (1. ea. 2. fej.).
- **TPS — tranzakció-feldolgozó rendszer (Transaction Processing System)** — operatív szint; strukturált, ismétlődő, szabályozható döntések; pontos, részletes, valós idejű tranzakciós adat (1. ea. 3. fej.).
- **MIS — menedzsment információs rendszer (Management Information System)** — taktikai szint; félig strukturált, rendszeres riportok; összesített, szűrt, trendalapú riportok.
- **DSS — döntéstámogató rendszer (Decision Support System)** — taktikai/stratégiai; félig strukturált, elemzésvezérelt; modellek, szcenárió-elemzések, what-if szimulációk.
- **ESS/EIS — vezetői információs rendszer (Executive Support System / Executive Information System)** — stratégiai szint; strukturálatlan döntés bizonytalanság alatt; külső és belső adatok aggregátuma, dashboard.
- **MIR / VIR** — menedzsment információs rendszer / vezetői információs rendszer (a tananyag a 4. fejezettől a magyar MIR/VIR rövidítéseket használja a MIS-re).
- **Kritikus sikertényező (KST / CSF — Critical Success Factor)** — az a néhány terület, aminek jól kell mennie ahhoz, hogy a szervezet sikeres legyen (1. ea. 4. fej.).
- **Kulcsfontosságú teljesítménymutató (KTM / KPI — Key Performance Indicator)** — az a mérőszám, amivel a kritikus sikertényezőt nyomon követjük.
- **Information overload** — az operatív TPS-adatok változtatás nélkül felfelé küldésének eredménye: döntésképtelenség; „a vezető adatot kap — nem információt” (1. ea. 3. fej.).
- **Szervezeti ellenállás** — „nem irracionális, hanem racionális reagálás a változással járó veszteségekre”; az IS-bevezetés „politikai kérdés, nem technikai” (Laudon & Laudon 2017, Ch.3; 1. ea. 5. fej.).
- **Termelékenységi paradoxon (productivity paradox)** — az IT-beruházások megduplázódtak, de a termelékenységi mutatók nem javultak arányosan; magyarázat (Brynjolfsson–Hitt, MIT, 2000): az IT csak komplementer befektetésekkel párosítva termel értéket (1. ea. 6. fej.).
- **Komplementer eszközök / befektetések (complementary assets)** — szervezeti, menedzsment és társadalmi befektetések, amelyek nélkül az IT-beruházás nem térül meg.
- **Teljesen digitális vállalat (fully digital firm)** — Laudon Ch.1: minden jelentős üzleti kapcsolat digitálisan közvetített; az alapvető üzleti folyamatok digitális hálózatokon futnak; a vállalati eszközök digitálisan kezelhetők és mérhetők valós időben (1. ea. 8. fej.).
- **Elszabadult projekt (runaway project)** — messze túllépi az eredeti keretet; a projektek 30–40 %-a (1. ea. 8. fej.).
- **TCO — teljes tulajdonlási költség (Total Cost of Ownership)** — a hardver- és szoftverbeszerzés csak kb. 20 %; a fennmaradó 80 % rejtett költség (1. ea. 7. fej.).
- **PV / NPV / IRR / ROI** — lásd Számítások.

## Modellek és keretek

### A) Az IS három dimenziója (Laudon-modell; 1. ea. 2. fej.)
1. **Szervezeti dimenzió** — hierarchia, szabályok, kultúra, üzleti folyamatok; az IS-nek illeszkednie kell hozzájuk, vagy tudatosan meg kell változtatnia őket; a szervezet szintjei (operatív, taktikai, stratégiai) különböző információt igényelnek; **a szervezeti kultúra az egyik legerősebb gát**.
2. **Menedzsment dimenzió** — döntések, erőforrás-allokáció, stratégia; „a rossz döntési kultúra a legjobb rendszert is haszontalanná teszi”; **felső vezetői elköteleződés nélkül a projekt szinte biztosan kudarc**.
3. **Technológiai dimenzió** — hardver, szoftver, adatbázisok, hálózatok, felhő; „csupán az egyik harmad — de erre fordítják a legtöbb figyelmet és költségvetést”.

Miért **feszültség**, nem egyensúly (3 ok): a technológia gyorsabban változik, mint a szervezeti kultúra; a menedzsment döntési stílusa nem mindig illeszkedik az adatvezérelt megközelítéshez; a szervezeti folyamatok évtizedes rutinokat tükröznek, amelyeket az új rendszer megkérdőjelez. Műszaki analógia: gyártósor-átszervezés — aki csak a gépet cseréli, „nem hogy nem nyer — hanem még veszít is”.

### B) IS-típusok piramisa (1. ea. 3. fej.) — alul TPS, középen MIS és DSS, felül ESS
Három hibaeset a szintek felcserélésekor:
1. **Túl sok adat felfelé** — TPS-adat változtatás nélkül a vezérigazgatónak → information overload, döntésképtelenség.
2. **Aggregált adat lefelé** — gyártósor-vezető csak havi összesítőt kap → problémák késve kerülnek felszínre, a beavatkozás késő.
3. **DSS operatív szinten** — raktáros komplex optimalizációs modellt kap egyszerű készletjelentés helyett → senki nem használja, túl bonyolult.

### C) A MIR feladatai és a vezetői szintek (1. ea. 4. fej.)
- Kik dolgoznak a MIR/VIR-rel (7 szerep): rendszerfejlesztők; rendszergazdák; kontrollingosok; vezetői informatikai tanácsadók/konzultánsok; informatikai rendszereket auditálók; informatikai projektek minőségbiztosítói; üzleti-vállalati folyamatokat újjászervező szakemberek.
- Alkalmazási célok (6): pénzügy; stratégia; marketing/értékesítés; HR; piaci verseny; gyártási adatok. Ezen felül: új termék/szolgáltatás fejlesztés és innováció (eljárás-, termék- és piaci innováció).
- **Egy jó KPI négy jellemzője (sorrendben):** aktuális érték; terv érték; eltérés érték; trend érték. A valódi kihívás: eldönteni, **melyik 5–10 KPI** kell egy vezetőnek. A VIR a kiugró eltérések (kivételek) kezelését is támogatja.
- A menedzsment **négy alapfunkciója**: tervezés, szervezés, irányítás, ellenőrzés — mindhárom vezetői szinten jelen van. Információ eredete: belső / külső; jellege: előrejelző, speciális, eseti, időszaki.

| Szint | Információ mennyisége | Jellemző fókusz |
|---|---|---|
| Alsó szintű vezetés | sok, részletes | napi működés, operatív adatok |
| Középszintű vezetés | közepes, szűrt | elemzés, összehasonlítás |
| Felső szintű vezetés | kevés, tömör | stratégia, versenyhelyzet |

Felfelé haladva: **csökken** az információ mennyisége, **nő** a mélységi hozzáférés igénye (drill-down bármikor) és az információ lényegszerűsége (KPI-fókusz). A rendszer feladata mindhárom szinten: nyomon-követés, irányítás, kommunikáció támogatása, versenyhelyzet és vevői igények figyelése.

### D) A szervezeti ellenállás négy tényezője (Laudon, Figure 3.7; 1. ea. 5. fej.)
1. **Szervezeti struktúra** — centralizált: hamarabb kritikus tömeg, de koordináltabb, erősebb ellenállás; decentralizált: lassabb, organikusabb adopció.
2. **Emberek és kultúra** — a legerősebb gát; ha az IS megkérdőjelezi a bevett feltételezéseket („a menedzsernek kell dönteni, nem az algoritmusnak”), a rendszert kikerülik.
3. **Feladatok jellege** — legnagyobb ellenállás, ha a napi rutint és az információ feletti hatalmat érinti; **back-office rendszerek kisebb ellenállással járnak, mint az operatív döntéstámogató rendszerek**.
4. **Az IT természete** — inkrementális fejlesztés kevesebb ellenállást vált ki, mint teljes rendszercsere; a „big bang” maximalizálja az egyidejű változást és az ellenállást.

⚠ forrásmegjegyzés: az ábra-felirat csak három tényezőt sorol („szervezeti struktúra, emberek, feladatok,”) — a szöveg négyet (struktúra, emberek, feladatok, IT); a ZH-ra a **négy** tényezőt kell tudni (a tananyag szövege így adja meg).

### E) A MIR sikerének három pillére (egyszerűbb, gyakorlatiasabb megközelítés; 1. ea. 5. fej.)
1. **A felhasználó vezető** (aki ténylegesen dönt a rendszer alapján); 2. **Az információ** (amit a rendszer szolgáltat); 3. **A technológia** (ami működteti). Ha nincs összhang → „hivatalosan bevezetik, de a gyakorlatban senki nem használja”.

Miért bukik el egy MIR-bevezetés (5 ok): a szervezeti változásokat nehezen követi a rendszer (lemarad a valós működés mögött); nem megfelelő projektvezetés; gyenge kommunikáció (a vezetők is elzárkóznak); csodát várnak a VIR-től (irreális elvárások); nem bíznak a VIR-ből származó információban.
Mi segít (4): a legbefolyásosabb vezetők nyílt támogatása; az üzletmenet alapos ismerete a fejlesztés előtt; fokozatos bővítés (nem big bang); a csoportmunka tudatos megszervezése.

### F) A három tipikus ellenállási minta (1. ea. 5. fej.)
1. **„A párhuzamos futtatás”** — titokban fenntartják a régit is; kétszeres költség; felismerhető: az új rendszerből exportált adatokat visszatöltik a régi Excelbe.
2. **„Az adatminőség-szabotázs”** — helytelen adatokkal töltik, hogy „bizonyítsák”, nem működik; tudatos és tudattalan; felismerhető: az adathibák szisztematikusan egy-egy részlegtől származnak.
3. **„A bypass kultúra”** — a menedzserek telefonon/emailen kerülik meg; a rendszer kiüresedik, nyomon követhetőség elvész.
**A mérnöki tévhit:** „ha a rendszer jó, az emberek majd használni fogják” — valóság: az emberek a változás ellen küzdenek, nem a rendszer ellen; megoldás nem jobb dokumentáció, hanem **változásmenedzsment**.

### G) A hat stratégiai üzleti célkitűzés (Laudon 2025, Ch.1; 1. ea. 6. fej.) — sorrendben, példával
1. **Működési kiválóság** — hatékonyság, folyamatoptimalizálás — Walmart RFID-alapú készletkezelés.
2. **Új termékek és üzleti modellek** — streaming vs. videókölcsönzők.
3. **Vevői és szállítói intimacy** — Amazon személyre szabott ajánlórendszer.
4. **Jobb döntéshozatal** — valós idejű adat, nem találgatás — légitársaságok dinamikus árazása.
5. **Versenyelőny** — nehezen másolható képességek — Apple App Store ökoszisztéma.
6. **Túlélés** — az IS „nem előny, hanem belépési feltétel” — online értékesítés nélküli kiskereskedelem.

### H) Komplementer befektetések három típusa (1. ea. 6. fej.)
| Típus | Példák |
|---|---|
| Szervezeti | új üzleti folyamatok, decentralizált döntéshozatal, erős IS-fejlesztési csapat, megfelelő üzleti modell |
| Menedzsment | felső vezetői elköteleződés, innovációt jutalmazó ösztönzők, csapatmunka-kultúra, képzési programok |
| Társadalmi | digitális infrastruktúra, szabványok, jogszabályok, technológiai ökoszisztéma |

**Megtérülési mátrix** (Laudon 2017, Ch.1):
- Magas IT + magas komplementer → **kiváló** megtérülés
- Magas IT + alacsony komplementer → **semmi vagy negatív**
- Alacsony IT + magas komplementer → **meglepően jó**
- Alacsony IT + alacsony komplementer → **gyenge, de arányos**
→ ezért érhet el egy kis cég olcsó felhős CRM-mel jobbat, mint egy nagyvállalat milliárdos SAP-implementációval.

### I) A MIR gazdasági hatásai — tíz terület (1. ea. 7. fej.)
1. menedzseri jelentések színvonalának javulása; 2. több időszerű adat; 3. stratégiai tervezés javulása; 4. megbízható adatbázis kialakítása (visszacsatolás — a jó rendszer önmagát is javítja); 5. pénzügyi irányítás javulása; 6. a vállalati szervezet jobb megértése; 7. gazdasági és piaci adatok minőségének javulása; 8. termékminőség és szolgáltatás színvonalának javulása; 9. piaci versenyanalízis minőségének javulása; 10. vezetői teamek közötti kommunikáció javulása.
**Csapda:** „ebből a tíz pontból egyik sem közvetlenül pénzügyi mutató — mégis mindegyik végső soron pénzügyi hatással jár” → a megtérülést nem elég egyetlen mutatóval mérni.

Üzleti előnyök (5): pénzügyi információk integrálása; megrendelői információk integrálása; gyártási folyamatok egységesítése és felgyorsítása; raktárkészlet csökkentése; HR információk egységesítése.
Szervezeti hatások funkció szerint: Beszerzés (alacsonyabb árak, integrált beszerzési osztályok, csökkent létszám); Raktár/logisztika (csökkenő készlet, alacsonyabb szállítási költség, magasabb raktározási bevétel, csökkent létszám); Termelés (rövidebb ciklusidő, nagyobb termelékenység, kapacitáskihasználás, kevesebb selejt, pontos szállítási idő, csökkent létszám); Értékesítés (megnövelt árbevétel, integrált értékesítési osztályok, csökkent létszám); Pénzügy (gyorsabb számlázás, gyorsabb kimutatások, nagyobb átláthatóság, csökkent létszám). — Minden funkciónál ott a „csökkent létszám”.

### J) TCO rejtett költségei (7 tétel; Laudon 2018, Ch.5 Table 5.4; 1. ea. 7. fej.)
telepítés; képzés; támogatás (support, help desk); karbantartás; infrastruktúra; üzemkiesés (downtime); hely és energia.

## Számok, dátumok, nevek, amiket a tananyag kiemel

| Mi | Érték | Hol |
|---|---|---|
| Hershey SAP ERP beruházás | 112 M USD, 1999 ősz | 1. fej. |
| Teljesítetlen rendelés | 100 M USD | 1. fej. |
| Részvényesés | 8 % egy nap alatt | 1. fej. |
| Összes kár | > 150 M USD | 1. fej. |
| Projekt összenyomása | 30 hónap → 18 hónap | 8. fej. |
| IT-projektek bukási aránya | 30–40 % | 1. fej. (és 8. fej. runaway) |
| Western Union memo | 1876 („telefon… nincs értéke”) | 2. fej. |
| Sir William Preece, Brit Postahivatal | 1876 („bővében vagyunk a futároknak”) | 2. fej. |
| Charles H. Duell, US Szabadalmi Hivatal | 1899 („minden feltaláltatott”) | 2. fej. |
| Thomas Watson, IBM | 1943 („négy-öt számítógép”) | 2. fej. |
| Popular Mechanics | 1949 („nem több 1,5 tonnánál”) | 2. fej. |
| Ken Olsen, DEC | 1977 („számítógép az otthonba”) | 2. fej. |
| Bill Gates, Microsoft | 1981 („640 Kb elég”) | 2. fej. |
| Jó KPI jellemzői | 4 (aktuális, terv, eltérés, trend) | 4. fej. |
| Vezetőnek szükséges KPI-k száma | 5–10 | 4. fej. |
| Menedzsment alapfunkciói | 4 (tervezés, szervezés, irányítás, ellenőrzés) | 4. fej. |
| Ellenállási tényezők (Laudon Fig. 3.7) | 4 | 5. fej. |
| Ellenállási minták | 3 | 5. fej. |
| Stratégiai üzleti célkitűzések | 6 | 6. fej. |
| Brynjolfsson–Hitt | MIT, 2000; JEP 14(4), 23–48 | 6. fej. |
| Brynjolfsson productivity paradox cikk | 1993, Communications of the ACM 36(12), 66–77 | 8–9. fej. |
| MIR gazdasági hatásai | 10 terület | 7. fej. |
| TCO: hardver+szoftver aránya | kb. 20 % (80 % rejtett) | 7. fej. |
| Számítógép TCO | akár **3×** a vételár | 7. fej. |
| Outsourcing rejtett költség | +15–57 % a szerződéses összeghez képest | 7. fej. |
| McKinsey–Oxford: költségtúllépés | átlag 66 % | 8. fej. |
| McKinsey–Oxford: határidő-túllépés | átlag 33 % | 8. fej. |
| McKinsey–Oxford: cég fennmaradását veszélyeztető | 17 % | 8. fej. |
| Runaway projektek | 30–40 % | 8. fej. |
| McKinsey „Unlocking success in digital transformations” | 2018, 1793 vállalat | 9. fej. |
| Laudon-forrás kiadások | 2025 (18th ed., Traver), 2017/2018 (15th ed.) | több fej. |

## Számítások (1. ea. 7. fej.)

A tananyag négy beruházás-gazdaságossági mutatót definiál (képletet nem ad, csak szöveges definíciót — ezért a képletek a tananyag definícióiból következnek; a számpélda **saját számokkal** készült):

| Módszer | Tananyag-definíció |
|---|---|
| **PV** — jelenérték (present value) | a jövőbeli pénzáramlások mai értéke |
| **NPV** — nettó jelenérték (net present value) | a beruházás jelenértéke mínusz a beruházás költsége; **pozitív NPV esetén éri meg** |
| **IRR** — belső megtérülési ráta (internal rate of return) | az a kamatláb, amely mellett a beruházás **NPV-je pontosan nulla** |
| **ROI** — megtérülési mutató (return on investment) | a beruházásból származó nyereség aránya a beruházás költségéhez képest |

Képletek (a definíciókból): PV = Σ CFt / (1+r)^t; NPV = PV − I₀; IRR: NPV(IRR) = 0; ROI = (nyereség − költség) / költség.

**Mintapélda (saját számok, a tananyag nem ad számot):** VIR-beruházás I₀ = 100 M Ft; éves nettó haszon 40 M Ft 3 évig; diszkontráta r = 10 %.
- PV = 40/1,1 + 40/1,1² + 40/1,1³ = 36,36 + 33,06 + 30,05 = **99,47 M Ft**
- NPV = 99,47 − 100 = **−0,53 M Ft** → negatív, a beruházás 10 %-os elvárt hozam mellett **nem éri meg** (épp alatta).
- IRR: az a ráta, ahol NPV = 0; itt kb. **9,7 %** (próbálgatással: r = 9 %-nál PV ≈ 101,25 → NPV +1,25; r = 10 %-nál −0,53 → IRR ≈ 9,7 %). Értelmezés: ha az elvárt hozam < 9,7 %, megéri.
- ROI (egyszerű, nem diszkontált) = (3·40 − 100)/100 = 20/100 = **20 %** a 3 évre.
- **„Mi változik, ha…”**: ha a TCO-logika szerint a 100 M Ft csak a vételár és a valódi költség ennek 3-szorosa (300 M Ft), akkor NPV = 99,47 − 300 = −200,5 M Ft, ROI = (120−300)/300 = −60 % → a rejtett költségek figyelmen kívül hagyása egy „megtérülő” beruházást súlyosan veszteségessé tesz. Ha a haszon 45 M Ft/év: PV = 111,9; NPV = +11,9 → megéri.

**TCO-példa (a tananyag arányaival, saját összeggel):** ha a hardver+szoftver vételár 20 M Ft, és ez a TCO kb. 20 %-a → TCO ≈ 100 M Ft, a rejtett 80 % = 80 M Ft. Outsourcing: 100 M Ft-os szerződés valódi költsége 115–157 M Ft (+15–57 %).

## Összekeverhető párok / „mi NEM igaz” csapdák

1. **Hershey: a szoftver hibás volt?** NEM — a SAP műszakilag sikeres volt; a helyes válasz D (mindhárom), de a kiváltó ok a **menedzsment döntése** (határidő-kényszer).
2. **MIS vs. DSS:** MIS = rendszeres, összesített riportok (taktikai); DSS = modellek, what-if, szcenárió (taktikai/stratégiai). **ESS/EIS** = stratégiai, dashboard, külső+belső adat. **TPS** = operatív, valós idejű tranzakció.
3. **Ellenállás = irracionális emberi gyengeség?** NEM — racionális reakció a veszteségekre; politikai, nem technikai kérdés.
4. **Jobb dokumentáció oldja meg az ellenállást?** NEM — változásmenedzsment.
5. **Back-office vs. operatív döntéstámogató rendszer:** a back-office KISEBB ellenállással jár.
6. **Centralizált vs. decentralizált:** centralizált = gyorsabb kritikus tömeg, de erősebb, koordináltabb ellenállás; decentralizált = lassabb, organikusabb.
7. **Big bang vs. inkrementális:** big bang maximalizálja az ellenállást; a tananyag a fokozatos bővítést ajánlja.
8. **A technológiai dimenzió a legfontosabb?** NEM — „csupán az egyik harmad”, de erre megy a legtöbb figyelem/költség.
9. **Magas IT + alacsony komplementer** → semmi/negatív; **alacsony IT + magas komplementer** → meglepően jó (nem fordítva!).
10. **A MIR 10 gazdasági hatása közvetlen pénzügyi mutató?** NEM — egyik sem az, de mind pénzügyi hatású.
11. **TCO:** a vételár NEM a költség nagy része — csak ~20 %; számítógép TCO akár 3× vételár.
12. **NPV vs. IRR:** NPV = pénzösszeg (PV − költség; pozitív → megéri); IRR = kamatláb, ahol NPV = 0.
13. **CSF vs. KPI:** CSF = terület, aminek jól kell mennie; KPI = mérőszám, amivel a CSF-et követjük.
14. **Felfelé a hierarchián az információ mennyisége nő?** NEM — csökken; a mélységi hozzáférés igénye és a lényegszerűség nő.
15. **A három pillér vs. a három dimenzió:** dimenziók = szervezet, menedzsment, technológia (Laudon); pillérek = felhasználó vezető, információ, technológia (egyszerűbb megközelítés).
16. **McKinsey–Oxford számok:** 66 % költség, 33 % határidő, 17 % cégveszélyeztető, 30–40 % runaway — ne keverd a sorrendet.
17. **Túlélés célkitűzés:** az IS „belépési feltétel”, nem előny — ez a 6., nem az 5. (versenyelőny).

## Kapcsolat más előadásokkal

- A „technológia nem elég” tézis és a komplementer eszközök → 2. ea. (IT csak szükséges feltétel, Porter), 5. ea. (BI kultúra, nem eszköz), 3. ea. (ERP-bevezetési kudarcok), 12. ea. (digitális transzformáció).
- TPS/MIS/DSS/ESS piramis → 3. ea. (ERP mint integrált TPS), 5–7. ea. (BI/OLAP mint DSS/ESS-eszköz).
- KPI/CSF → 6. ea. (KPI-tervezés, Goodhart, OEE), 5. ea. (dashboard a felső vezetőnek), gyakorlat (Power BI).
- TCO → 8. ea. (Big Data TCO), 10. ea. (felhő TCO), 12. ea. (TCO 3–5 éves távlatban).
- Szervezeti ellenállás, változásmenedzsment → 9. ea. (tudásmegosztás, kultúra), 12. ea. (digitális transzformáció, Ipar 4.0 kihívások).
- NPV/IRR/ROI → 12. ea. 4. fej. (IT-beruházás értékelése, FAIR, Gordon–Loeb); 10. ea. felhő-gazdaságosság.
- McKinsey 2018 „Unlocking success” → a 9. fej. szerint „releváns a 12. fejezethez is”.

## Fogalomtár-jelöltek

- **Jéghegy-modell** – iceberg model – a technológia a látható csúcs, a szervezeti és menedzsment tényezők a felszín alatt döntik el a sikert.
- **IS három dimenziója** – three dimensions of IS – szervezet, menedzsment, technológia egyidejű vizsgálata.
- **Tranzakció-feldolgozó rendszer** – TPS – operatív, valós idejű, részletes tranzakciós adat.
- **Menedzsment információs rendszer** – MIS – taktikai szint, összesített, rendszeres riportok.
- **Döntéstámogató rendszer** – DSS – modellek, what-if, szcenárió-elemzés.
- **Vezetői információs rendszer** – ESS/EIS – stratégiai, dashboard, külső+belső adat.
- **Kritikus sikertényező** – CSF – a kevés terület, aminek jól kell mennie.
- **Kulcsfontosságú teljesítménymutató** – KPI – a CSF-et mérő mutató (aktuális, terv, eltérés, trend).
- **Információs túlterhelés** – information overload – túl sok nyers adat a vezetőnek → döntésképtelenség.
- **Szervezeti ellenállás** – organizational resistance – racionális reakció a változás veszteségeire; 4 tényező.
- **Big bang bevezetés** – big bang implementation – egyidejű teljes csere, maximális ellenállás.
- **Bypass kultúra** – bypass culture – a rendszer megkerülése telefon/email útján.
- **Komplementer eszközök** – complementary assets – szervezeti, menedzsment, társadalmi befektetések az IT mellé.
- **Termelékenységi paradoxon** – productivity paradox – IT-beruházás nő, termelékenység nem arányosan (Brynjolfsson).
- **Teljesen digitális vállalat** – fully digital firm – minden kapcsolat és folyamat digitális, eszközök valós időben mérhetők.
- **Teljes tulajdonlási költség** – TCO – vételár ~20 %, rejtett ~80 %.
- **Nettó jelenérték** – NPV – PV mínusz beruházási költség; pozitív → megéri.
- **Belső megtérülési ráta** – IRR – kamatláb, ahol NPV = 0.
- **Megtérülési mutató** – ROI – nyereség / költség.
- **Elszabadult projekt** – runaway project – messze túllépi az eredeti keretet (30–40 %).

---

# 2. előadás: Hogyan teremt versenyelőnyt az IT — és mikor nem?

## Egy mondatban (a központi tézis)

Az IT **önmagában nem teremt versenyelőnyt — csak a stratégiai alkalmazása révén**; ehhez három egymást kiegészítő keret kell: Porter öt erő modellje, az IT-alapú értéklánc, és az IT-specifikus versenymodellek (hálózati közgazdaságtan, platform-gazdaság); a legjövedelmezőbb vállalatok közös jellemzője az **IT-alignment** (2. ea. 2. és 8. fej.).

## Nyitó eset és feloldása (2. ea. 2. és 8. fej.)

**A Kodak-paradoxon.**

| Adat | Érték |
|---|---|
| Első digitális fényképezőgép | 1975, Steve Sasson (Kodak mérnöke) |
| Prototípus | 3,6 kg; 0,01 megapixel; kazettára mentett |
| Felsővezetés reakciója | elzárta a projektet: „Miért mutatnánk be olyan terméket, amely tönkreteszi a filmes üzletünket?” |
| Csődvédelem | 2012 |
| Ugyanabban az évben | a 13 fős Instagram 1 milliárd USD-ért kelt el a Facebooknak |

Kérdés: A) nem fektetett eleget K+F-be; B) felismerte a digitális fényképezést, de nem változtatta meg az üzleti modelljét; C) nem volt elég tőkéje; D) a versenytársak gyorsabb hardverfejlesztéssel megelőzték. **Helyes válasz: B.**

Feloldás (8. fej.): a Kodak IT-stratégiája a **filmgyártás optimalizálására** irányult, miközben az üzleti valóság megváltozott → **klasszikus alignment-kudarc**: az IT a régi stratégiát szolgálta. „A Kodak nem technológiai, hanem **stratégiai rugalmasság-hiányban** szenvedett.” Ez az **innovator's dilemma** (Christensen, 2003): a piacvezetők saját fennálló üzletüket védik, miközben a diszruptív technológia alulról erodálja a piacukat; a Kodak „nem volt hajlandó kannibalizálni saját üzletét”. A 3. fej. szerint a Kodak azért nem látta meg a diszrupciót, „mert a Porter-logikán belül gondolkodott” (3. korlát).

Elméleti pontok, amelyek bizonyítják: IT-alignment (Luftman) számai (8. fej.), Porter-modell 3. korlátja — diszruptív innováció (3. fej.), alignment-kudarc tipikus mintái (8. fej.), a technológiai vs. stratégiai innováció megkülönböztetése (2. fej.).

## Fogalmak és definíciók (HU – EN)

- **Porter öt erő modellje (five forces)** — Michael Porter (1980, 1985): öt erő határozza meg a vállalat stratégiai mozgásterét — és az IT mindegyiket befolyásolja (3. fej.).
- **Négy generikus IT-alapú versenystratégia** — low-cost leadership; termékdifferenciálás; piacirés-fókusz (focus); vevői/szállítói intimacy (4. fej., Laudon 2017 Table 3.4).
- **Mass customization** — tömeges személyre szabás, az IT teszi lehetővé; a termékdifferenciálás és a vevői intimacy kombinációja (Nike By You: a vevő tervezi a cipőt, 3–4 héten belül legyártják; Zwack Unicum személyre szabott üvegek QR-kóddal) (4. fej.).
- **Értéklánc-modell (value chain)** — Porter 1985; a vállalat értéket hozzáadó tevékenységek sorozata; elsődleges + támogató tevékenységek; az első kérdés nem „milyen rendszert vegyünk”, hanem **„hol fáj a legjobban”** — hol a legnagyobb hatékonysági veszteség (5. fej.).
- **Értékháló (value web)** — a szállítók és vevők értékláncai összekapcsolódnak; az IT teszi hatékonnyá (Toyota Kanban: valós idejű adatmegosztás a szállítókkal → ökoszisztéma-szintű versenyképesség) (5. fej.).
- **Hálózati közgazdaságtan (network economics)** — Laudon Ch.3, Ch.5; az IT a Porter-féle lineáris logikától eltérő versenylogikát tesz lehetővé (6. fej.).
- **Metcalfe törvénye** — Robert Metcalfe, az Ethernet feltalálója, 1970 (a tananyag így adja meg): „Egy hálózat értéke exponenciálisan nő a hálózati tagok számával.” (6. fej.)
- **Kritikus tömeg (critical mass)** — aki először eléri, „szinte legyőzhetetlenné válik”, mert a hálózat értéke mindenki más számára csökken, aki kilép (Facebook, Windows, LinkedIn példák) (6. fej.).
- **Váltási költség (switching cost)** — az IT-rendszerek tudatosan tervezhetők a váltás költségének növelésére (ERP: adatok, integrációk, betanított munkaerő) — „tudatos IT-stratégia” (6. fej.).
- **Lock-in** — a kritikus tömeggel és váltási költséggel elért bezárás (6. fej. alcím: „a kritikus tömeg és a lock-in”).
- **Pipeline vs. platform** — Van Alstyne, Parker & Choudary (2016): pipeline = a vállalat hozza létre és értékesíti az értéket; platform = a felhasználók egymás között teremtik (7. fej.).
- **Üzleti ökoszisztéma (business ecosystem)** — Laudon Ch.3, p.136: az IT lehetővé teszi, hogy több iparág vállalkozásai együtt teremtsenek értéket, amelyet egyikük sem tudna egyedül (7. fej.).
- **IT-alignment** — az IT- és az üzleti stratégia összehangolása (Luftman, 2003) (8. fej.).
- **Innovator's dilemma** — Christensen (2003): a piacvezetők a fennálló üzletüket védik, a diszruptív technológia alulról erodál (3. és 8. fej.).
- **Diszruptív technológia** — Christensen: olcsóbb, egyszerűbb termékek, kezdetben rosszabbak, de gyorsan fejlődnek (3. fej.).
- **Szinergia** — ha az egyik üzleti egység outputja a másik inputja, vagy az egységek összevont piaci erőt és tudást hoznak létre → csökken a költség, nő a profit (Laudon 2017, Ch.3, p.134) (9. fej.).
- **Core competency (alapvető képesség)** — tevékenység, amelyben a vállalat világszínvonalú vezető; évtizedes tapasztalaton és elkötelezett munkatársakon alapul (p.135); az IT nem teremti, de **megsokszorozhatja** a tudásmegosztással (9. fej.).
- **Virtual company model (virtuális vállalat)** — hálózatok segítségével kapcsolódik más cégekhez anélkül, hogy szervezetileg összeolvadna; akkor, ha a képességet olcsóbb kívülről beszerezni, vagy gyorsan kell piacra lépni saját erőforrás nélkül (p.136) (9. fej.).
- **Strategic transitions (stratégiai átmenetek)** — a stratégiai IS-bevezetés szervezeti átmenetet igényel: ugrás egy **sociotechnical** szintről egy másikra; „jellemzően nehezek és fájdalmasak” (Laudon 2017, p.140) (10. fej.).
- **A fenntarthatóság paradoxona** — „ami ma versenyelőny, holnap a túlélés minimumfeltétele” (p.138) (10. fej.).

## Modellek és keretek

### A) Porter öt erő és az IT (2. ea. 3. fej.) — a tananyag sorrendje
1. **Hagyományos versenytársak** — IT gyorsítja az innovációs ciklust, de a versenytársak másolnak; Amazon Prime lojalitásprogram vevői váltási költséget épített.
2. **Új belépők fenyegetése** — az Internet csökkentette a belépési korlátokat (nincs fizikai bolt), de növelte másutt (adatközpontok, AI-infrastruktúra).
3. **Helyettesítő termékek** — a digitalizáció felgyorsítja; Netflix 2007: DVD postán → 2010: streaming — saját modelljét kannibalizálta.
4. **Vevők alkuereje** — az Internet átláthatóvá tette az árakat; IT-lojalitásprogramok (Tesco Clubcard, OTP Simple) csökkentik a váltási hajlandóságot.
5. **Szállítók alkuereje** — e-procurement növeli a vállalat alkuerejét; a Walmart automatikus készletfeltöltése „szinte teljesen elvette a szállítói alkuerőt”.

**A Porter-modell három korlátja 2026-ban** (1980-ban született — internet, platform-gazdaság és AI előtt):
1. **Lineáris értékteremtést feltételez** — a platform-gazdaságban az érték a felhasználók interakcióiból keletkezik (Uber: nem fuvaroz, kapcsolatot teremt).
2. **A hálózati hatások nem szerepelnek benne** — Porter: hatékonyság + differenciálás; hálózati hatás: az ökoszisztéma mérete, exponenciálisan erősödik (Facebook: „ott van mindenki más is”).
3. **A diszruptív innováció nem illeszkedik** — stabil iparágakat feltételez (Christensen 2003); a Kodak ezért nem látta meg.

### B) A négy IT-alapú versenystratégia (2. ea. 4. fej., Laudon 2017 Table 3.4)
| Stratégia | IT-kontextusban | Nemzetközi példa | Magyar példa | Kockázat |
|---|---|---|---|---|
| Low-cost leadership | legalacsonyabb operatív költség IT-vel | Walmart valós idejű készletkezelés | Penny/Lidl automatizált logisztika, önkiszolgáló kassza | könnyen másolható, árversenybe visz |
| Termékdifferenciálás | egyedi termék / vevői élmény | Apple iPod + iTunes | OTP Simple (egyedi UX) | drága fenntartani, a vevői igény változik |
| Piacirés-fókusz | szűk szegmens magas értékkel | Harrah's kaszinó személyre szabott CRM | MiniCRM (magyar KKV-k) | kis piac — növekedési korlát |
| Vevői/szállítói intimacy | magas váltási költség, lojalitás | Amazon ajánlórendszer, Toyota szállítói integráció | Tesco Clubcard Magyarország | adatvédelmi kockázat, túlzott függőség |

Menedzseri logika: nem minden stratégia működik minden iparágban; egy KKV nem versenyezhet a Walmart árképzésével, de résben teremthet értéket. **Fenntarthatóság:** a legtöbb IT-előny nem tartós — SABRE, Citibank ATM, FedEx csomagkövetés → „alapszolgáltatássá vált”; ha mindenki másolja, a rendszer már nem versenyelőny, hanem **belépési feltétel**.

### C) Értéklánc (2. ea. 5. fej., Laudon 2017 Fig. 3.9)
**Elsődleges tevékenységek (5, sorrendben):**
| Tevékenység | IT-eszköz | Példa |
|---|---|---|
| Beérkező logisztika | RFID raktárkezelés, automatikus készletfigyelés | Walmart automatikus rendelés |
| Termelés | CAD/CAM, MES, digitális ikrek | BMW gyártósor-szimuláció |
| Kimenő logisztika | GPS-útvonaltervezés, automatikus szállítmányütemezés | FedEx csomagkövetés |
| Értékesítés/marketing | CRM, ajánlórendszerek, dinamikus árazás | Amazon ajánlások |
| Szerviz | önkiszolgáló portálok, prediktív karbantartás IoT | Rolls-Royce hajtómű távfelügyelet |

**Támogató tevékenységek (4):** Infrastruktúra (ERP az egész vállalatra — pénzügy, kontrolling, tervezés); HR (digitális toborzás, kompetenciaadatbázis, e-learning); Technológia (R&D szimuláció, digitális ikrek, nyílt innovációs platformok); Beszerzés (e-procurement, szállítói portálok, automatikus ajánlatkérés).

**Menedzseri figyelmeztetés:** a legnagyobb veszteség legtöbbször **nem a termelésben, hanem az információáramlásban** keletkezik (késő számla-jóváhagyás, lassú döntés, silószerű adatok); az IT legértékesebb alkalmazásai az információs szűk keresztmetszetek feloldása.

### D) Metcalfe törvénye és hálózati hatások (2. ea. 6. fej.) — lásd Számítások
Üzleti példák: Microsoft Windows (több felhasználó → több szoftver → több felhasználó); LinkedIn; VISA/Mastercard (kereskedők és kártyabirtokosok kölcsönös növekedése); OTP Simple (több elfogadó kereskedő → értékesebb a felhasználóknak → vonzóbb a kereskedőknek). Menedzseri következtetés: ha hálózati hatások érvényesülnek, a hatékonysági logika nem elég; a kérdés: **hogyan érjük el a kritikus tömeget minél gyorsabban** — ezért adnak ingyen szolgáltatást a tech-cégek kezdetben.

### E) Pipeline vs. Platform (2. ea. 7. fej., Van Alstyne et al. 2016)
| Szempont | Pipeline | Platform |
|---|---|---|
| Értékteremtés | a vállalat hozza létre és értékesíti | a felhasználók egymás között |
| Versenyelőny forrása | termelési hatékonyság, Porter-stratégiák | hálózati hatások, ökoszisztéma mérete |
| Porter érvényessége | teljes mértékben | részben — más logika dominál |
| Belépési korlát | tőke, technológia, know-how | hálózati méret — az első belépő előnye óriási |

Ökoszisztéma példák: Windows — **40 000+** szoftvercég; Apple App Store — az Apple a tranzakciók **30 %-át** kapja; Telenor Közösségi Piactér (KKV-k platformja).
Porter **erős**, ha: lineáris piac; fizikai termék; termelési hatékonyságon alapuló verseny; stabil, jól definiált iparág. Porter **korlátozott**, ha: hálózatalapú piac; interakcióból keletkező érték; domináns hálózati hatás; platform-szereplők.
**Három út, ha platform-szereplő jelenik meg:** csatlakozni a platformhoz (niche-szereplőként); saját platformot építeni (ha van erőforrás és ügyfélbázis); a platform által nem kiszolgált szegmensben versenyezni.

### F) IT-alignment (2. ea. 8. fej., Luftman 2003)
- **50 %** magasabb profit azoknál, akik sikeresen összehangolják IT- és üzleti stratégiájukat.
- **25 %** — csak ennyi vállalatnál sikerül a valódi összehangolás.
- **75 %** — a cégek háromnegyedénél az IT „saját életet él”.
**A stratégiai elemzés három kérdése** (Laudon 2017, p.139): 1. Melyek az iparág domináns versenyerői, és hogyan változtatta meg ezeket az IT? 2. Hol van az értékláncban a legnagyobb fájdalom, és az IT hogyan enyhítheti? 3. Összehangoltuk-e az IT-stratégiát az üzleti célokkal?
**Alignment-kudarc tipikus mintái (3):** „Az IT az IT-osztály dolga”; „Majd a technológia megoldja”; „Csináljuk, amit eddig”.

### G) Szinergia, core competency, virtuális vállalat (2. ea. 9. fej.)
- Szinergia-példa: **JPMorgan Chase** jelzáloghitel-cég felvásárlása — az IT összekapcsolta a két ügyfélbázist → keresztértékesítés (hitelkártya, befektetés, biztosítás) új ügyfelek nélkül; „nem marketing-siker, hanem IT-architektúra-döntés eredménye”.
- Core competency példa: **P&G InnovationNet** — belső intranet, K+F, mérnöki, marketing, jogi, IT csapatokat köti össze világszerte; szakértői könyvtár; „nem a tudást tárolja, hanem a tudásmegosztást teszi lehetővé”. Eredmény: termékfejlesztési ciklus **30 %-kal rövidült**, külső ötletekből születő termékek aránya **megduplázódott** (open innovation). A core competency-tudás az emberek fejében van → KMS (7. fejezetre utal).
- Virtuális vállalat példa: **Li & Fung** (Hongkong) — LVMH, Levi Strauss, Reebok, GUESS gyártásszervezése; **40 ország 15 000+ szállítója**; nincs saját gyára, szövete, gépe; extranet a megrendelésekhez, valós idejű követés. Menedzseri következtetés: a cég azt tartja meg, amiben világszínvonalú; a többit hálózaton szerzi be.

| Szempont | Vertikális integráció | Virtual company |
|---|---|---|
| Tőkeigény | magas (saját gyár) | alacsony (IT-infrastruktúra) |
| Rugalmasság | alacsony (fix kapacitás) | magas (igény szerint skálázható) |
| Core competency | mindent belül kell tudni | csak a legjobbat kell belül tudni |
| IT szerepe | belső folyamatok optimalizálása | hálózati koordináció és átláthatóság |

### H) Internet hatása a Porter-erőkre (2. ea. 10. fej., Porter 2001; Laudon 2017 Table 3.5, p.128)
Porter (2001) következtetése: az Internet sok esetben **csökkenti a profitmarzsot** (átláthatóság ↑, belépési korlát ↓) → a digitalizáció nem automatikusan versenyelőny.
| Porter-erő | Internet hatása | Menedzseri következmény |
|---|---|---|
| Helyettesítő termékek | új helyettesítők (online enciklopédia, streaming, e-ticket) | helyettesítés iparágak között is |
| Vevők alkuereje | globális ár- és termékátláthatóság | árdifferenciálás nehéz → lojalitás, váltási költség |
| Szállítók alkuereje | e-procurement növeli a vevő alkuerejét, de a szállítók is elérik a végfelhasználót | közvetítők szerepe csökken — aki közvetlen kapcsolatot épít, nyer |
| Új belépők | csökkenti a belépési korlátokat (nincs fizikai bolt) | adatvagyon és AI-infrastruktúra új belépési korlát |
| Hagyományos versenytársak | bővíti a földrajzi piacot, több versenyző, árverseny | operatív hatékonyság alapelvárás, nem versenyelőny |

### I) AI hatása a Porter-erőkre — **más, mint az Internet** (2. ea. 10. fej., Laudon & Traver 2025 Ch.3)
- Általános: az AI javítja a meglévő üzleti modelleket és új modelleket tesz lehetővé.
- 🔴 **Növeli a fenyegetést:** helyettesítők (ChatGPT mint Google-helyettes, AI-diagnosztika mint orvos-helyettes, AI-jogi asszisztens mint ügyvéd-helyettes); új belépők (kis cégek is professzionális tartalmat/kódot/tervet — a méret előnye csökken); hagyományos versenytársak (gyorsabb innovációs ciklus, de gyors másolás).
- 🟢 **Csökkenti a fenyegetést:** vevők alkuereje (személyre szabott ajánlás → lojalitás, váltási költség — **szemben az Internettel, amely növelte a vevők alkuerejét**); adatvagyon mint korlát (NVIDIA GPU, AWS, Google Cloud → magas belépési korlát, tőkeerős szereplők előnye nő; **új szállítói függőség**).
- **AI és alignment:** az AI-befektetés ugyanolyan alignment-kérdés; aki folyamat- és adatinfrastruktúra-változtatás nélkül vezet be AI-t, ugyanúgy kudarcot vall, mint a korábbi BI- vagy ERP-projektek.

### J) Strategic transitions és a fenntarthatóság paradoxona (2. ea. 10. fej.)
Miért nehezek (3): a stratégiai rendszerek egyszerre változtatják a termékeket, szolgáltatásokat és folyamatokat (új viselkedési minták); technológia + szervezet + menedzsment precíz koordinációja kell; a versenytársak visszavágnak és másolnak.
| Rendszer | Eredetileg | Ma |
|---|---|---|
| American Airlines SABRE | stratégiai versenyelőny | iparági alapszolgáltatás |
| Citibank ATM-hálózat | stratégiai versenyelőny | belépési feltétel |
| FedEx csomagkövetés | stratégiai versenyelőny | minimumelvárás |
| Banki mobilalkalmazás | 2010: versenyelőny | 2025: belépési feltétel |

**Stratégiai rendszerelemzés — két kérdés minden IT-befektetés előtt** (ch03PPT Slide 43): 1. Az iparág struktúrája: melyik Porter-erő a legerősebb, hogyan változtatta meg az Internet és az AI? 2. A vállalat értékláncai: hol teremt az IT valódi értéket, és hol csak a versenytársak után fut?

**A fejezet öt kulcsgondolata** (10. fej.): Porter erős keret, de kiegészítésre szorul; értéklánc → „hol fáj”; szinergiák és core competencies; Internet és AI nem ugyanúgy hat, nem automatikus előny, gyakran kiegyenlít; strategic transitions — ma előny, holnap belépési feltétel. (A 8. fej. „három kulcsgondolata” a Porter/értéklánc/alignment hármas.)

## Számok, dátumok, nevek, amiket a tananyag kiemel

| Mi | Érték | Hol |
|---|---|---|
| Kodak első digitális gép | 1975, Steve Sasson; 3,6 kg; 0,01 MP | 2. fej. |
| Kodak csődvédelem | 2012 | 2. fej. |
| Instagram | 13 fő, 1 Mrd USD, Facebook, 2012 | 2. fej. |
| Porter öt erő | 1980, 1985 (Porter); HBR 2008, 86(1) | 3. fej. |
| Porter-modell születése | 1980 | 3. fej. |
| Netflix DVD → streaming | 2007 → 2010 | 3. fej. |
| Christensen, Innovator's dilemma | 2003 | 3., 8. fej. |
| Nike By You gyártás | 3–4 hét | 4. fej. |
| Metcalfe | Robert Metcalfe, Ethernet, 1970 (a tananyag így adja meg) | 6. fej. |
| Kapcsolatok száma | 2 tag → 1; 5 → 10; 100 → 4950 | 6. fej. |
| Laudon Metcalfe-oldal | Ch.5, p.202; Ch.3, p.135 | 6. fej. |
| Van Alstyne, Parker, Choudary | 2016, HBR 94(4), 54–62 | 7. fej. |
| Windows ökoszisztéma | 40 000+ szoftvercég | 7. fej. |
| Apple App Store jutalék | 30 % | 7. fej. |
| Luftman alignment | 2003; 50 % / 25 % / 75 % | 8. fej. |
| Stratégiai elemzés három kérdése | Laudon 2017, p.139 | 8. fej. |
| P&G InnovationNet | fejlesztési ciklus –30 %; külső ötletek aránya 2× | 9. fej. |
| Li & Fung | 40 ország, 15 000+ szállító; LVMH, Levi Strauss, Reebok, GUESS | 9. fej. |
| Porter „Strategy and the Internet” | 2001, HBR 79(3), 62–78 | 10. fej. |
| Internet-hatás táblázat | Laudon 2017 Table 3.5, p.128 | 10. fej. |
| Strategic transitions | Laudon 2017, p.140 | 10. fej. |
| Fenntarthatóság paradoxona | p.138 | 10. fej. |
| Banki mobilapp | 2010 előny → 2025 belépési feltétel | 10. fej. |
| Elmélyítő: Christensen, Raynor, McDonald | 2015, HBR „What is disruptive innovation?” | 11. fej. |

## Számítások — Metcalfe törvénye (2. ea. 6. fej.)

A tananyag számpéldái: 2 tag → 1 kapcsolat; 5 tag → 10; 100 tag → 4950. Ezek a **lehetséges páronkénti kapcsolatok** száma:

**Képlet:** kapcsolatok száma = n·(n−1)/2 (a tananyag a példákat adja, a képletet nem írja ki, de a számok ebből következnek).

Végigszámolva a tananyag számaival:
- n = 2: 2·1/2 = **1** ✓
- n = 5: 5·4/2 = **10** ✓
- n = 100: 100·99/2 = **4950** ✓

**Értelmezés:** a tagok 50-szeresére növelése (2 → 100) a kapcsolatok számát 4950-szeresére növeli — a növekedés nemlineáris; a tananyag szóhasználatában „exponenciálisan nő” (a tananyag így adja meg; a képlet valójában n²-es nagyságrendű). Ez a kritikus tömeg és a lock-in alapja: aki kilép, mindenki más számára csökkenti a hálózat értékét.

**„Mi változik, ha…” variánsok (saját számok):**
- n = 10: 10·9/2 = 45; n = 20: 20·19/2 = 190 → a tagok duplázása a kapcsolatok ~4,2-szeresét adja.
- n = 1000: 1000·999/2 = 499 500.
- Ha egy hálózatból 100-ról 90-re csökken a taglétszám (10 % kilép): 90·89/2 = 4005 → a kapcsolatok 19 %-a tűnik el — a hálózat értéke a tagszámnál gyorsabban csökken (ezért „szinte legyőzhetetlen” a kritikus tömeget elért szereplő).

## Összekeverhető párok / „mi NEM igaz” csapdák

1. **Kodak: nem volt K+F / tőke / lassú hardver?** NEM — B: felismerte a digitális technológiát, de nem változtatta meg az üzleti modelljét (alignment-kudarc, innovator's dilemma).
2. **Porter öt ereje vs. a négy stratégia:** az öt erő = elemzés (fenyegetések); a négy stratégia = válasz („mit tegyen a menedzser”). Ne keverd a „három korlátot” az „öt erővel”.
3. **Az öt erő sorrendje a tananyagban:** versenytársak → új belépők → helyettesítők → vevők → szállítók.
4. **Internet vs. AI a vevők alkuerejére:** az Internet **növelte** (átláthatóság), az AI **csökkenti** (személyre szabás, lojalitás).
5. **Internet és a belépési korlát:** csökkentette (nincs bolt), DE adatközpont/AI-infrastruktúra/adatvagyon **új, magas** belépési korlát.
6. **Az Internet automatikusan versenyelőny?** NEM — Porter (2001): gyakran csökkenti a profitmarzsot; kiegyenlíti a versenyt.
7. **Pipeline vs. platform:** a platform nem „gyárt” — az Uber kapcsolatot teremt; a Porter-modell platformnál csak részben érvényes.
8. **Core competency-t az IT teremt?** NEM — nem helyettesíti, hanem megsokszorozhatja (tudásmegosztás).
9. **Virtuális vállalat = fúzió?** NEM — hálózati kapcsolódás szervezeti összeolvadás nélkül; Li & Fungnak nincs saját gyára.
10. **Luftman számok:** 50 % magasabb profit (alignált cégek); 25 % sikerül; 75 % az IT „saját életet él” — ne cseréld fel.
11. **Mass customization** = differenciálás + vevői intimacy kombinációja (nem low-cost).
12. **Low-cost leadership kockázata:** könnyen másolható, árverseny; **intimacy kockázata:** adatvédelem, túlzott függőség; **fókusz:** kis piac; **differenciálás:** drága fenntartani.
13. **Metcalfe 1970 vs. Porter 1980 vs. Porter értéklánc 1985 vs. Christensen 2003 vs. Van Alstyne 2016 vs. Luftman 2003 vs. Porter 2001 (Internet).**
14. **Versenyelőny tartós?** NEM — SABRE, Citibank ATM, FedEx → alapszolgáltatás; „ami ma előny, holnap belépési feltétel”.
15. **Az értéklánc legnagyobb vesztesége a termelésben?** NEM — az információáramlásban.
16. **A JPMorgan-példa marketing-siker?** NEM — IT-architektúra-döntés (szinergia).
17. **Elsődleges vs. támogató tevékenységek:** elsődleges 5 (beérkező logisztika, termelés, kimenő logisztika, értékesítés/marketing, szerviz); támogató 4 (infrastruktúra, HR, technológia, beszerzés) — a beszerzés támogató, nem elsődleges.

## Kapcsolat más előadásokkal

- „Technológia nem elég” → 1. ea. (komplementer eszközök; a Kodak „stratégiai”, nem technológiai kudarc = alignment, mint Hershey menedzsment-kudarca).
- Strategic transitions = sociotechnical ugrás → 1. ea. szervezeti ellenállás, változásmenedzsment.
- ERP mint értéklánc-infrastruktúra, váltási költség ERP-nél → 3. ea.
- CRM / ajánlórendszer / dinamikus árazás (értékesítés) → 3. ea. CRM, 7. ea. ajánlórendszer (item-based CF).
- Core competency és KMS (P&G InnovationNet) → 9. ea. tudásmenedzsment (a tananyag „7. fejezetként” hivatkozik rá előre — a Moodle-számozásban 9.).
- Platform-gazdaság, hálózati hatás, kritikus tömeg → 3. ea. 8. fej. (B2B piacterek); külön e-kereskedelem/platform előadás a Moodle-ban nincs (⚠ lásd Forrásmegjegyzések).
- AI mint helyettesítő és belépési korlát, adatvagyon → 8. ea. Big Data, 11. ea. etika/AI.
- Felhő/AI-infrastruktúra szállítói függőség → 10. ea. felhő (vendor lock-in, felhő-koncentráció).

## Fogalomtár-jelöltek

- **Porter öt erő modellje** – five forces – versenytársak, új belépők, helyettesítők, vevők, szállítók alkuereje; az IT mindet befolyásolja.
- **Költségvezető stratégia** – low-cost leadership – IT-vel a legalacsonyabb operatív költség.
- **Termékdifferenciálás** – product differentiation – IT-vel egyedi termék vagy vevői élmény.
- **Piacirés-fókusz** – focus / niche – szűk szegmens magas értékkel.
- **Vevői/szállítói intimitás** – customer/supplier intimacy – magas váltási költség és lojalitás IT-vel.
- **Tömeges személyre szabás** – mass customization – differenciálás + intimacy kombinációja (Nike By You).
- **Értéklánc** – value chain – elsődleges és támogató értékteremtő tevékenységek sorozata (Porter 1985).
- **Értékháló** – value web – szállítói és vevői értékláncok IT-vel összekapcsolva.
- **Hálózati közgazdaságtan** – network economics – a hálózat értéke a tagszámmal nemlineárisan nő.
- **Metcalfe törvénye** – Metcalfe's law – a hálózat értéke „exponenciálisan” nő a tagok számával; n(n−1)/2 kapcsolat.
- **Kritikus tömeg** – critical mass – az azt elérő első belépő szinte legyőzhetetlen.
- **Váltási költség** – switching cost – tudatosan tervezett, a rendszerváltás ellen ható költség.
- **Platform** – platform – a felhasználók egymás között teremtik az értéket; vs. pipeline.
- **Üzleti ökoszisztéma** – business ecosystem – több iparág vállalkozásai együtt teremtenek értéket.
- **IT-alignment** – IT–business alignment – IT- és üzleti stratégia összehangolása (Luftman: +50 % profit).
- **Innovátor dilemmája** – innovator's dilemma – a piacvezető a saját üzletét védi, a diszrupció alulról erodál.
- **Szinergia** – synergy – egységek output/input összekapcsolása, összevont erő → költség ↓, profit ↑.
- **Alapvető képesség** – core competency – világszínvonalú tevékenység, amit az IT megsokszoroz.
- **Virtuális vállalat** – virtual company – hálózaton kapcsolódik partnerekhez összeolvadás nélkül (Li & Fung).
- **Stratégiai átmenet** – strategic transition – sociotechnical szintváltás a stratégiai IS bevezetésekor.
- **Fenntarthatóság paradoxona** – sustainability paradox – a mai versenyelőny holnapi belépési feltétel.

---

# 3. előadás: Az integrált vállalat: ERP, CRM, SCM

## Egy mondatban (a központi tézis)

Az ERP–CRM–SCM vonulat a MIR hetvenéves fejlődésének egy konkrét ága, amely a vállalaton belüli és vállalatok közötti **erőforrás-integrációra** fókuszál („ki lát mit, és mikor?”); a szigetrendszerek helyett egységes adat és folyamat kell — de az ERP-bevezetés **nem technikai projekt, hanem mélyreható szervezeti változás**, amelynél a sietség és a túlzott testreszabás ugyanazt a törékenységet okozza (3. ea. 3., 4., 10. fej.).

## Nyitó eset és feloldása (3. ea. 1. és 10. fej.)

**Target Canada, 2013.**

| Adat | Érték |
|---|---|
| Terjeszkedés | 133 áruház Kanadában, 2 éven belül; a cég első lépése az USA határain túl |
| Rendszer | vadonatúj, nulláról épített **SAP ERP**; kb. **75 000 termék** adatai (készlet, beszerzés, elosztás, árazás) |
| Rendelkezésre álló idő | **18 hónap**; iparági szakértők **3–4 évet** javasolnak |
| Hibás termékadat | egyes becslések szerint akár **70 %** (rossz mértékegység, hiányzó adat, elírás) — kézzel, sietve vitték fel |
| Következmény | POS és automatikus utánrendelés megbízhatatlan → üres polcok, raktárban álló készlet |
| Bezárás | **2015. január 15.**: mind a 133 áruház; veszteség kb. **7 milliárd USD**; **17 600** alkalmazott vesztette el az állását |

**Mi ment rosszul:** gyakorlatilag irányított **„big bang”** (direct cutover) 133 áruházban egyszerre, 18 hónap alatt. **A tanulság:** „a bukás oka nem a SAP szoftver minősége volt (ugyanezt világszerte sikeresen használják) — hanem az, hogy a vezetőség **technikai projektként kezelte** azt, ami valójában egy mélyreható szervezeti változás volt, és a sebesség érdekében **feláldozta az adatminőséget és a felkészülési időt**.”

Elméleti pontok, amelyek bizonyítják: a négy konverziós stratégia kockázatai (10. fej. — direct cutover: „nincs visszaút”); Crocs fázisos ellenpélda (10. fej.); az ERP-statisztikák (4. fej.: „a Hershey-eset tipikus”); a 4. fej. szála: „minél több az egyedi testreszabás, annál törékenyebb” — Targetnél „nem a testreszabás, hanem a sietség okozta ugyanazt a fajta törékenységet”. Források: Panorama Consulting, Canadian Business („The Last Days of Target Canada”), Henrico Dolfing Case Study 7.

## Fogalmak és definíciók (HU – EN)

- **MIR** — nem egyetlen technológia, hanem „közel hetven éves fejlődési folyamat eredménye” (2. fej.).
- **Szigetrendszer** — minden rendszernek saját adatstruktúrája, saját „igazsága”; ha az értékesítési és a pénzügyi rendszer nem ugyanazt az ügyféladatot látja, a vezető „két különböző valóság között kénytelen dönteni”, és az egyeztetés ideje emészti fel a versenyelőnyt (3. fej.).
- **MRP → MRP II → ERP → Internal ERP/SCM → ERP II** — lásd Modellek.
- **ERP (Enterprise Resource Planning)** ígérete: egységes adatbázis, egységes folyamatok, valós idejű átláthatóság az egész vállalatra (4. fej.).
- **CRM (Customer Relationship Management)** — egységes, **360 fokos kép** minden ügyfélről, függetlenül attól, hogy értékesítéssel, marketinggel vagy ügyfélszolgálattal lépett kapcsolatba (5. fej.).
- **Operational CRM** — napi ügyfélkapcsolati folyamatok: értékesítés-automatizálás (**SFA — Sales Force Automation**), marketingkampányok, ügyfélszolgálati esetek.
- **Analytical CRM** — ügyféladatok elemzése: kik a legértékesebb ügyfelek, kik hagyják el, mi a vásárlási mintázat.
- **Churn rate (lemorzsolódási ráta)** — milyen arányban veszítjük el az ügyfeleket; „az egyik legfontosabb korai figyelmeztető jelzés”.
- **CLTV (Customer Lifetime Value)** — mennyit ér egy ügyfél a teljes kapcsolat során, nem csak az aktuális vásárlás.
- **PRM (Partner Relationship Management)**, **ERM (Employee Relationship Management)** — a CRM-logika kiterjesztése partnerekre és alkalmazottakra.
- **Social CRM** — közösségimédia-adatok beépítése (hangulatelemzés, gyorsabb reagálás).
- **Touchpoint (érintkezési pont)** — értékesítés, marketing, ügyfélszolgálat — a műszaki analógiában „külön érzékelő” (5. fej.).
- **SCM (Supply Chain Management)** — lényege **nem a fizikai áru, hanem az információ mozgatása**: minél pontosabb információ minél gyorsabban minden szereplőhöz (6. fej.).
- **Bullwhip-effektus (ostorcsapás-hatás)** — apró keresletnövekedés a lánc mentén felerősödik (kiskereskedő kicsit többet rendel → nagykereskedő „biztonsági” többletet → gyártó még többet „hátha”) → elképesztő túlkészletezés (6. fej.). Műszaki analógia: késleltetett visszacsatolás (feedback delay) → túllövés, túlkorrigálás, oszcilláció; minél hosszabb a lánc, annál nagyobb a kilengés.
- **Push (build-to-stock)** — a termelés előrejelzésre épül: „gyártsuk le, aztán eladjuk”.
- **Pull (build-to-order, demand-driven)** — a tényleges vevői rendelés indítja a láncot: „Make what we sell, not sell what we make.” (Walmart folyamatos utánpótlása.)
- **Supply chain planning** — mit, mennyit, hol gyártsunk/tároljunk — előrejelzés-alapú; **supply chain execution** — a fizikai áramlás nyomon követése raktárból raktárba.
- **Enterprise Application Architecture** — Laudon 2.6 ábra: ERP (befelé), SCM (kifelé, beszállítók), CRM (kifelé, vevők), KMS (vállalati tudás) — a négy rendszer nem versenyez, hanem kiegészíti egymást; hub-topológia, az ERP a központi csomópont (7. fej.).
- **Intranet / extranet** — belső céges háló csak alkalmazottaknak / kiterjesztett hozzáférés partnereknek — olcsóbb alternatíva kisebb büdzsére (7. fej.).
- **Private industrial network** — egy nagy cég saját, zárt hálózata a beszállítóihoz (VW Group Supply — a Volkswagen globális beszerzésének **90 %-a**) (8. fej.).
- **Net marketplace** — sok vevő és sok eladó közös, hosszabb távú, gyakran **iparág-tulajdonú** piactere (Exostar).
- **Exchange** — **független harmadik fél** piactere, azonnali „spot” vásárlásra (Go2Paper).
- **Build / Buy / Cloud / Best-of-breed** — lásd Modellek (9. fej.).
- **Greenfield (zöldmezős)** — teljesen új rendszer a nulláról; **brownfield (barnamezős)** — technikai frissítés alapvető üzleti transzformáció nélkül (9. fej.).
- **Konverziós stratégiák** — parallel, direct cutover („big bang”), pilot study, phased approach (10. fej.).
- **Legacy rendszer** — elavult örökölt rendszer (Crocs: 24 megszüntetve) (10. fej.).

## Modellek és keretek

### A) A MIR négy nagy korszaka (Turban et al. 2002; 3. ea. 2. fej.)
| Korszak | Időszak | Cél |
|---|---|---|
| 1. Az adatfeldolgozás korszaka | '60-as évek | működési hatékonyság növelése |
| 2. A vezetői információk korszaka | '70-es évek | a vezetői munka hatékonyságának növelése |
| 3. A stratégiai információs rendszerek korszaka | '80-as–'90-es évek | üzleti előnyök szerzése |
| 4. Intelligens on-line megoldások korszaka | 2000-es évektől | a tudásalapú társadalom megteremtése |

**A MIR alrendszereinek kronológiája:** 1980-as évek: EIS, DSS; 1990-es évek: Data Warehousing (DW), Business Intelligence (BI); 2000-es évek: Dashboards and scorecards, Performance management; **2010+ …?** (szándékosan nyitva hagyva; a 9. fej. válasza: a felhőalapú, gyorsan bevezethető, kevés testreszabású megoldások — NetSuite, Salesforce — „a MIR-fejlődés jelenlegi, még nevesítetlen korszaka”).
**Funkcionális fejlődés:** e-Commerce → m-Commerce → c-Commerce (irodai eszközből mindenütt jelenlévő eszköz). **Üzemeltetési fejlődés:** on-premise → on-demand / SaaS. Új felhasználó: a modern munkavállaló (mozgásban, csapatban, projekt alapon, közösségi hálózatok).

### B) Az ERP-ág fejlődése (Turban et al. 2002; 3. ea. 3. fej.) — „ki lát mit, és mikor?”
| Év | Alap | + Hozzáadva | → Eredmény |
|---|---|---|---|
| 1960 | Beszerzés + Raktározás | Gyártástervezés | → **MRP** |
| 1970 | MRP | Pénzügy | → **MRP II** |
| 1980 | MRP II | Minden belső forrás kezelése | → **ERP** |
| 1990 | ERP | Vevők és szállítók integrálása | → **Internal ERP/SCM** |
| 2000 | Internal ERP/SCM | Üzleti intelligencia | → **ERP II** |

- Az **1990-es sor** az, ahonnan a CRM (vevők) és SCM (szállítók) ered — „nem külön történetek, hanem ugyanennek az ágnak a folytatásai”.
- A **2000-es sor** (BI → ERP II) előrevetíti az Enterprise Application Architecture logikáját (7. fej.).
- Műszaki analógia: külön PLC-k minden gépen → központi **SCADA** egy felületen; a gépek nem lettek jobbak, de a rendszerszintű átláthatóság minőségi ugrás.

### C) ERP: ígéret vs. valóság — kemény számok (Panorama Consulting 2025 ERP Report + Gartner; 3. ea. 4. fej.)
- Gartner: az ERP-projektek **70 %-a nem éri el** a kitűzött célokat
- átlagos költségtúllépés **189 %**, feldolgozóiparban **215 %**
- csak **30 %** fejeződik be időben és költségvetésen belül
- **50 %** elbukik már az első nekifutásra
- **41 %** a várt hasznoknak még a felét sem éri el
- átlagos bevezetési költség 2025-ben: **450 000 USD**

**Három figyelmeztető eset** (Laudon Ch.9, Enterprise Application Challenges):
1. **Kmart** — az i2 Technologies SCM-szoftvere nem illett a **promóció-vezérelt** üzleti modellhez (éles keresleti kilengések).
2. **Overstock.com** — házon belüli rendszer → Oracle enterprise rendszer csere: a megrendelés-követés **egy teljes hétre leállt**, mert a visszatérítési folyamatot nem szinkronizálták a követelés-nyilvántartással.
3. **Kennametal** (2 Mrd USD-os szerszámgyártó) — **13 éven át, 6400 egyedi testreszabással** tartott fenn egy ERP-t → lecserélték **„plain-vanilla”**, testreszabás nélküli SAP-ra, és a saját folyamataikat igazították a szoftverhez.
Tanulság: **minél több az egyedi testreszabás, annál törékenyebb és drágább a rendszer.**

### D) CRM két alaptípusa + AI for CRM (3. ea. 5. fej., Laudon Ch.9 9.3)
Operational vs. Analytical (lásd Fogalmak). Miért stratégiai: az új termékből fakadó előny gyorsan másolható, az ügyfélkapcsolat tartósabb — „nem az nyer, aki a legtöbb terméket adja el, hanem aki »birtokolja« az ügyfelet”. **AI for CRM:** gépi tanulás és generatív AI — automatikus churn-felismerés, ajánlat-illesztés; „nem váltja le az operatív/analitikai CRM logikáját — felgyorsítja és élesebbé teszi”; az ember a kivételekre és stratégiai döntésekre koncentrál.

### E) SCM, bullwhip, push/pull + AI for SCM (3. ea. 6. fej., Laudon Ch.9 9.2)
- **P&G Pampers példa:** a bolti vásárlás stabil volt, de az árakciók miatt a nagykereskedői rendelések kiugrottak → a lánc mentén felhalmozott készlet nem létező keresletet szolgált ki. Megoldás: pontosabb keresleti előrejelzés + megosztott, valós idejű adatok a lánc minden szereplője között.
- **AI for SCM:** pontosabb keresleti előrejelzés, működési összefüggések feltárása, raktározás/szállítás hatékonysága, több partnert átfogó hálózatokon; minél pontosabb az előrejelzés, annál kevesebb „biztonsági ráhagyás” → ugyanazt a problémát oldja, mint a valós idejű adatmegosztás, „csak egy fokkal kifinomultabb szinten”.

### F) Enterprise Application Architecture (Laudon Ch.2, 2.6 ábra; 3. ea. 7. fej.)
ERP — befelé integrál (gyártás, pénzügy, HR); SCM — kifelé, beszállítók; CRM — kifelé, vevők; KMS — a vállalati tudást fogja össze. Hub-topológia: az ERP a központi csomópont, nem mesh. Ez az ERP II (2000-es sor) vizuális kibontása. Alternatíva kisebb büdzsére: intranet + extranet.

### G) B2B piacterek (Laudon Ch.10, 10.4; 3. ea. 8. fej.)
Három típus: **private industrial network** (VW Group Supply, 90 %), **net marketplace**, **exchange**.
| | Net marketplace — **Exostar** | Exchange — **Go2Paper** |
|---|---|---|
| Kapcsolat jellege | hosszú távú, szerződéses, együttműködő | rövid távú, azonnali („spot”) |
| Tulajdonos | maga az iparág (BAE Systems, Boeing, Lockheed Martin, Raytheon, Rolls-Royce közösen) | független közvetítő cég |
| Mire jó | tervezés, fejlesztés, gyártásütemezés megosztása **100 000+ beszállítóval** a védelmi/repülőgépipari láncban | pillanatnyi szükséglet gyors kielégítése, ár-összehasonlítás |
| Kockázat | erős függés, lassabb rugalmasság | árverseny lenyomja az árakat, nincs hosszú távú garancia |
Bullwhip-kapcsolat: a net marketplace hosszú távú megosztott tervezési adatokkal csökkenti a bizonytalanságot; az exchange a pillanatnyi hiány pótlására való. Analógia: net marketplace = szabványos iparági csatlakozó (USB-port); exchange = nyílt piactér egyszeri tranzakcióra.

### H) Build / Buy / Cloud / Best-of-breed (Laudon Ch.9; 3. ea. 9. fej.)
| Opció | Lényeg | Mikor éri meg |
|---|---|---|
| Build (saját fejlesztés) | egyedi rendszer a nulláról | csak nagyon specifikus, versenyelőnyt adó folyamatoknál |
| Buy (kész szoftver, on-premise) | bevált csomag testreszabással | stabil, kiforrott folyamatoknál, ahol a testreszabás vállalható |
| Cloud | előfizetéses, gyorsan bevezethető, kevés testreszabás | KKV-knak, gyors növekedésnél — a sebesség fontosabb, mint a teljes testreszabhatóság |
| Best-of-breed | területenként a legjobb egyedi megoldás, összekötve | ha egyetlen „all-in-one” egyik területen sem elég erős |
Cloud-példák: **Oracle NetSuite** — piacvezető cloud ERP a KKV-szegmensben; **Salesforce** — cloud CRM piacvezető, **100 000+ ügyfél**.
**Magyar példa:** **MOL Csoport** (Svébis András, csoportszintű CIO, 2024-es SAP S/4HANA-konferencia): greenfield nem opció (túl komplex, sok egyedi fejlesztés, 3–4 év, közben felvásárlások) → **brownfield** (technikai frissítés üzleti transzformáció nélkül). **Kometa 99**: **greenfield** — a rendszer „szét volt fejlesztve”, töredezett → a szigetrendszer-probléma hazai változata. Forrás: ITBUSINESS.hu, 2024.

### I) A négy klasszikus bevezetési (konverziós) stratégia (Laudon Ch.13; 3. ea. 10. fej.)
| Stratégia | Leírás | Kockázat |
|---|---|---|
| **Parallel** | régi és új rendszer egyszerre fut egy ideig | biztonságos, de drága és erőforrás-igényes |
| **Direct cutover („big bang”)** | egy kijelölt napon a régit teljesen lecseréli az új | kockázatos — nincs visszaút hiba esetén |
| **Pilot study** | egy részlegen/egységen tesztelik, majd kiterjesztik | fokozatos tanulás, kisebb kockázat |
| **Phased approach** | funkciónként vagy egységenként, lépcsőzetesen | lassabb, de kontrollált |
**Crocs ellenpélda (SAP, fázisos globális rollout):** Ausztráliából indítva, régiónként; cél: a problémák egy régióra korlátozódjanak. Eredmény: **17 hónap**, **24 elavult legacy rendszer** megszüntetése.

## Számok, dátumok, nevek, amiket a tananyag kiemel

| Mi | Érték | Hol |
|---|---|---|
| Target Canada | 2013; 133 áruház; 75 000 termék; 18 hónap vs. 3–4 év | 1., 10. fej. |
| Target hibás termékadat | akár 70 % | 10. fej. |
| Target bezárás | 2015. 01. 15.; ~7 Mrd USD; 17 600 fő | 10. fej. |
| MIR fejlődés hossza | közel 70 év | 2. fej. |
| MIR négy korszaka | '60, '70, '80–'90, 2000+ | 2. fej. |
| Alrendszerek | 1980 EIS/DSS; 1990 DW/BI; 2000 dashboards/scorecards/PM; 2010+ ? | 2. fej. |
| Turban, McLean, Wetherbe | 2002, 3rd ed., Wiley | 2–3. fej. |
| ERP-ág évek | 1960 MRP; 1970 MRP II; 1980 ERP; 1990 Internal ERP/SCM; 2000 ERP II | 3. fej. |
| Gartner: ERP célt nem ér el | 70 % | 4. fej. |
| Költségtúllépés | 189 % (feldolgozóipar 215 %) | 4. fej. |
| Időben és büdzsén belül | 30 % | 4. fej. |
| Első nekifutásra bukik | 50 % | 4. fej. |
| Várt haszon felét sem | 41 % | 4. fej. |
| Átlagos bevezetési költség 2025 | 450 000 USD | 4. fej. |
| Kennametal | 2 Mrd USD; 13 év; 6400 testreszabás; plain-vanilla SAP | 4. fej. |
| Overstock.com | 1 hét leállás; Oracle | 4. fej. |
| Kmart | i2 Technologies SCM; promóció-vezérelt modell | 4. fej. |
| CRM | 360 fokos kép | 5. fej. |
| P&G Pampers | bullwhip-példa; árakciók | 6. fej. |
| Walmart | folyamatos utánpótlás = pull példa | 6. fej. |
| Laudon architektúra-ábra | 2.6 | 7. fej. |
| VW Group Supply | globális beszerzés 90 %-a | 8. fej. |
| Exostar alapítók | BAE Systems, Boeing, Lockheed Martin, Raytheon, Rolls-Royce; 100 000+ beszállító | 8. fej. |
| Go2Paper | exchange, független közvetítő | 8. fej. |
| Salesforce | 100 000+ ügyfél | 9. fej. |
| MOL CIO | Svébis András, 2024, S/4HANA; brownfield | 9. fej. |
| Kometa 99 | greenfield | 9. fej. |
| Crocs | 17 hónap; 24 legacy rendszer; Ausztráliából | 10. fej. |
| Lee, Padmanabhan, Whang | 1997, Management Science 43(4) — a „bullwhip effect” elnevezés bevezetése | 11. fej. |
| Finney & Corbett | 2007, 45 tanulmány, ERP CSF | 11. fej. |

## Számítások

Az előadás nem tartalmaz képletet. Illusztratív példa a bullwhip-effektus mechanizmusára (**saját számok**, a tananyag csak a mechanizmust írja le — kiskereskedő kicsit többet, nagykereskedő biztonsági többletet, gyártó „hátha” még többet):
- Bolti kereslet: 100 → 110 egység (+10 %).
- Kiskereskedő rendel 110 + 10 % biztonsági = 121; nagykereskedő 121 + 10 % = 133; gyártó 133 + 10 % = 146.
- A +10 %-os valós keresletnövekedés a gyártónál **+46 %**-os termelésként jelenik meg → ha a kereslet visszaáll 100-ra, 46 egység felesleges készlet halmozódik a láncban (ez a P&G Pampers-eset logikája).
- **„Mi változik, ha…”**: ha valós idejű adatmegosztással minden szereplő a bolti 110-et látja, és nincs ráhagyás, a gyártó 110-et termel — a torzítás nulla; minél több szint (hosszabb lánc), annál nagyobb a kilengés (késleltetett visszacsatolás).

## Összekeverhető párok / „mi NEM igaz” csapdák

1. **Target Canada: a SAP volt rossz?** NEM — ugyanazt a rendszert világszerte sikeresen használják; a vezetőség technikai projektként kezelte a szervezeti változást; adatminőség + felkészülési idő feláldozva.
2. **Target vs. Hershey (1. ea.):** mindkettő SAP, mindkettő big bang határidőnyomással; Hershey: 30→18 hónap, 112 M USD, 1999; Target: 18 hónap vs. 3–4 év, 7 Mrd USD, 2013/2015.
3. **MRP II = MRP + pénzügy** (1970); **ERP = MRP II + minden belső forrás** (1980); **ERP II = Internal ERP/SCM + BI** (2000). Az 1990-es lépés = vevők és szállítók integrálása.
4. **CRM = vevői oldal; SCM = szállítói oldal** — mindkettő az 1990-es sor folytatása.
5. **Operational vs. Analytical CRM:** operational = SFA, kampány, ügyfélszolgálat; analytical = elemzés (legértékesebb ügyfelek, churn, mintázat).
6. **Churn vs. CLTV:** churn = lemorzsolódási arány (korai figyelmeztető); CLTV = ügyfél teljes élettartam-értéke.
7. **SCM = áru mozgatása?** NEM — információ mozgatása.
8. **Push vs. pull:** push = build-to-stock, előrejelzés; pull = build-to-order, vevői rendelés indítja („Make what we sell…”). Walmart = pull.
9. **Supply chain planning vs. execution:** planning = mit/mennyit/hol (előrejelzés); execution = fizikai áramlás követése.
10. **Net marketplace vs. exchange:** net marketplace = hosszú távú, iparág-tulajdonú (Exostar); exchange = spot, független harmadik fél (Go2Paper). **Private industrial network** = egy cég saját zárt hálózata (VW).
11. **Kennametal tanulsága:** NEM a több testreszabás, hanem a plain-vanilla + saját folyamatok igazítása a szoftverhez.
12. **MOL = brownfield; Kometa 99 = greenfield** — ne cseréld fel.
13. **Parallel = biztonságos, de drága; big bang = nincs visszaút; pilot = egy egységen; phased = funkciónként/egységenként lépcsőzetesen.** Crocs = phased (régiónként), nem pilot.
14. **ERP II ≠ ERP** — ERP II a BI-val bővített, minden irányba nyitott architektúra.
15. **Build mikor?** Csak nagyon specifikus, versenyelőnyt adó folyamatoknál — nem alapértelmezés. **Cloud** = KKV, gyors növekedés.
16. **A MIR korszakainak célja:** '60 működési hatékonyság; '70 vezetői munka hatékonysága; '80–'90 üzleti előny; 2000+ tudásalapú társadalom.
17. **AI for CRM/SCM leváltja a korábbi logikát?** NEM — felgyorsítja/élesebbé teszi.

## Kapcsolat más előadásokkal

- Hershey (1. ea.) ↔ Target Canada: ugyanaz a big bang + határidő-kényszer minta; a 1. ea. „IT természete” ellenállási tényező (inkrementális vs. teljes csere).
- Szigetrendszer, egységes adat/„egy igazság” → 4. ea. adatminőség, adatgazda; 5. ea. BI single source of truth.
- ERP II + BI; alrendszerek kronológiája (DW, BI, dashboard) → 5. ea. BI, 7. ea. OLAP, 4. ea. adattárház.
- KMS az architektúrában → 9. ea. tudásmenedzsment.
- AI for CRM/SCM, keresleti előrejelzés → 8. ea. Big Data, 11. ea. AI.
- Cloud ERP/CRM, SaaS, on-premise → on-demand → 10. ea. felhő (IaaS/PaaS/SaaS).
- B2B piacterek (net marketplace, exchange, private industrial network), e/m/c-commerce → 2. ea. 7. fej. (platform-gazdaság); külön e-kereskedelem előadás a Moodle-ban nincs.
- Váltási költség ERP-nél (2. ea.) ↔ Kennametal 6400 testreszabás.

## Fogalomtár-jelöltek

- **Szigetrendszer** – silo / island system – külön adatstruktúrájú, saját „igazságú” rendszerek, amelyek egyeztetése felemészti a versenyelőnyt.
- **Anyagszükséglet-tervezés** – MRP – beszerzés + raktározás + gyártástervezés (1960).
- **Gyártási erőforrás-tervezés** – MRP II – MRP + pénzügy (1970).
- **Vállalati erőforrás-tervezés** – ERP – minden belső forrás kezelése egységes adatbázisban (1980).
- **ERP II** – ERP II – Internal ERP/SCM + üzleti intelligencia, minden irányba nyitott architektúra (2000).
- **Ügyfélkapcsolat-kezelés** – CRM – 360 fokos egységes ügyfélkép; operational és analytical.
- **Értékesítés-automatizálás** – SFA – az operational CRM része.
- **Lemorzsolódási ráta** – churn rate – elvesztett ügyfelek aránya.
- **Ügyfél-élettartamérték** – CLTV – az ügyfél értéke a teljes kapcsolat során.
- **Ellátásilánc-menedzsment** – SCM – információ mozgatása a lánc szereplői között.
- **Ostorcsapás-hatás** – bullwhip effect – kis keresletváltozás felerősödik a lánc mentén.
- **Toló / húzó modell** – push (build-to-stock) / pull (build-to-order) – előrejelzés- vs. rendelésvezérelt termelés.
- **Vállalati alkalmazás-architektúra** – enterprise application architecture – ERP hub + SCM + CRM + KMS.
- **Zárt ipari hálózat** – private industrial network – egy nagyvállalat saját beszállítói hálózata.
- **Hálózati piactér** – net marketplace – sok vevő–sok eladó, hosszú távú, iparág-tulajdonú.
- **Tőzsde-jellegű piactér** – exchange – független, spot vásárlás.
- **Legjobb-a-maga-nemében** – best-of-breed – területenként a legjobb megoldás összekötve.
- **Zöldmezős / barnamezős** – greenfield / brownfield – új rendszer a nulláról / technikai frissítés.
- **Közvetlen átállás** – direct cutover (big bang) – egy napon teljes csere, nincs visszaút.
- **Párhuzamos / pilot / fázisos bevezetés** – parallel / pilot / phased – a másik három konverziós stratégia.

---

# 4. előadás: Mit ér az adat és ki felelős érte?

## Egy mondatban (a központi tézis)

Az adatminőség **pénzügyi kockázat, nem IT-részlet**: a katasztrófák a DIKW-lánc egy észrevétlen töréspontjára — leggyakrabban az **adat → információ** átmenetre — vezethetők vissza; a megoldás a **„single source of truth”** elv (egyetlen, megbízhatóan karbantartott, mindenki által ugyanúgy látott adatforrás) és az explicit adatfelelősség (data governance, CDO), amely **menedzseri, nem technikai** feladat (4. ea. 2., 5., 7. fej.).

## Nyitó eset és feloldása (4. ea. 1., 2. és 7. fej.)

**Knight Capital Group, 2012. augusztus 1., New York** — az egyik legnagyobb amerikai tőzsdei kereskedő cég.

| Adat | Érték |
|---|---|
| Telepítés | új kereskedési algoritmus **8 szerverre** az éjszaka folyamán; piacnyitás 9:30 |
| Hiba | 7 szerverre sikeresen felkerült; a **8. szerveren** egy **2003 óta** használaton kívüli, elfeledett funkció (**„Power Peg”**) aktiválódott újra egy ott felejtett kódrészlet miatt |
| 45 perc alatt | **154 részvényben**, **397 millió darab** részvényt érintő, **4 millió tranzakció** — vásárolt drágán, eladott olcsón |
| Veszteség | **440 millió USD** |
| Részvényárfolyam | **–75 %** két nap alatt; a céget végül felvásárolták |
| Félrediagnózis | a csapat **20 percen át** tévesen egy másik szervert hitt a forrásnak, és az elavult kódot **minden szerverre visszaállította** — rontott a helyzeten |

**Mi ment rosszul (DIKW-diagnózis, 2. fej.):**
- **Adat:** a 8. szerver kód-állapota eltért a többitől — „a rendszer állapotáról szóló tény nem egyezett a valósággal”.
- **Információ:** senki nem alakította ezt látható, értelmezhető információvá — nem volt automatikus riasztás.
- **Tudás:** még riasztás esetén is fel kellett volna ismerni, hogy ez kritikus eltérés (kontextus, tapasztalat).
- **Bölcsesség:** a helyes döntés (azonnali leállítás) csak akkor születhet, ha az előző három szint működik — 45 percig nem történt meg.
- **Feloldás (7. fej.):** nem volt **„single source of truth”** — egyetlen megbízhatóan ellenőrzött hely, ahol tudható, hogy mind a nyolc szerver ugyanazt a kódot futtatja. Műszaki analógia: az elosztott rendszerek **konszenzus-problémája**.

**Ellenpélda — Siemens Amberg (Electronic Works Amberg), a „digitális gyár”:** évi **6 millió SIMATIC** termék, **1200 termékváltozat**, napi **350 átállás**; naponta kb. **50 millió** folyamatadat **egyetlen közös adatmodellben**. Eredmény: **99,99885 %** minőségi mutató (kb. **11 hibás darab / millió**). 2025–2026: AI-alapú minőségellenőrzés → elkerültek egy **500 000 eurós** röntgenalapú vizsgálóberendezés-beruházást, mert a megbízható adat helyettesítette a drága fizikai ellenőrzést. Forrás: HBS Case 518-054; Information Systems Journal, 2026.

## Fogalmak és definíciók (HU – EN)

- **DIKW-lánc** — adat → információ → tudás → bölcsesség (data → information → knowledge → wisdom); a fejezet **nem definícióként, hanem diagnosztikai eszközként** használja: „minden komoly IT-katasztrófa mögött megtalálható, hogy a lánc melyik pontján szakadt meg a megbízható átmenet” (2. fej.). Műszaki analógia: érzékelő (adat) → jelfeldolgozó (információ) → vezérlőalgoritmus felismeri a kritikus tartományt (tudás) → beavatkozás/riasztás (bölcsesség).
- **Adatredundancia (data redundancy)** — ugyanaz az adat több helyen, eltérő formában tárolva (3. fej.).
- **Adatinkonzisztencia (data inconsistency)** — ugyanannak az adatnak eltérő értékei különböző rendszerekben („M” vs. „medium”).
- **Program-adat függőség (program-data dependence)** — a programkód összefonódik az adat fizikai elrendezésével; apró szerkezetváltozás elrontja a kapcsolódó programokat.
- **Korlátozott adatmegosztás** — a részlegek nem férnek hozzá egymás adataihoz.
- **Relációs adatbázis (relational database)** — egyetlen közös, logikailag rendezett adatállomány; minden adatelemnek egyetlen azonosítható helye (**kulcsmező**), kapcsolódó adatok összekapcsolhatók másolás nélkül; technikai szinten oldja meg a négy problémát — „nem szünteti meg az adatminőségi kockázatot, de megteremti az alapfeltételét annak, hogy kezelhető legyen” (3. fej.).
- **OLTP (Online Transaction Processing)** — tranzakció rögzítése; ügyintéző; naprakész, részletes; írás/olvasás; relációs; tranzakciós idő; operatív feldolgozás (4. fej.).
- **OLAP (Online Analytical Processing)** — trendelemzés; elemző; történeti, összesített; főleg olvasás; csillag/hópehely séma; lekérdezési idő; döntéstámogatás.
- **FASMI** — **Fast Analysis of Shared Multidimensional Information** — az OLAP elvárásainak összefoglalása: gyors, megosztott, többdimenziós, elemzésre optimalizált hozzáférés (4. fej.).
- **Adattárház (data warehouse)** — a teljes vállalat összes releváns adatát egyesíti; minden részleg, minden funkcionális terület; hosszú távú, elemzésre optimalizált (5. fej.).
- **Adatpiac (data mart)** — az adattárház kisebb, célzott alegysége: csak **egyetlen üzleti terület** adatai (pl. csak értékesítés vagy csak HR); gyorsabban felépíthető és olcsóbb, cserébe szűkebb rálátás.
- **Data governance (adatirányítás)** — valakinek felelősséget kell vállalnia a vállalati adatvagyonért; „nem lehet, hogy minden részleg saját belátása szerint kezelje” (6. fej.).
- **CDO (Chief Data Officer)** — vállalati szintű adatirányítás és -hasznosítás; viszonylag új szerepkör; biztosítja, hogy (1) a megfelelő adatot gyűjtik, (2) a megfelelő technológiákkal elemzik, (3) az eredményeket ténylegesen felhasználják döntésekhez (6. fej.).
- **Single source of truth** — egyetlen, megbízhatóan karbantartott, mindenki által ugyanúgy látott adatforrás; döntési logika (7. fej.); KKV-méretben „nulla CDO-büdzséből”: a tulajdonos/irodavezető explicit felelős, egy közös adatforrás a szétszórt táblázatok helyett (8. fej.).
- **Digitális iker (digital twin)** — Bosch Hatvan „Plant Digital Twin” (2025): valós idejű kép a teljes gyártási folyamatról (8. fej.).

## Modellek és keretek

### A) DIKW mint diagnosztikai lánc (4. ea. 2. fej.)
Négy szint sorrendben: **Adat → Információ → Tudás → Bölcsesség.** Tanulság: „a bölcsesség szintjén hozott rossz döntés szinte mindig egy korábbi, észrevétlen töréspontra vezethető vissza — **leggyakrabban az adat→információ átmenetre**, ahol a nyers tény nem alakul át időben látható, cselekvésre ösztönző jelzéssé.”

### B) A hagyományos fájlkörnyezet négy problémája vs. relációs adatbázis (Laudon Ch.6; 4. ea. 3. fej.)
1. Adatredundancia; 2. Adatinkonzisztencia; 3. Program-adat függőség; 4. Korlátozott adatmegosztás. → Válasz: relációs adatbázis (kulcsmező, közös logikailag rendezett adatállomány).

### C) OLTP vs. OLAP táblázat (4. ea. 4. fej.) — 9 tulajdonság
| Tulajdonság | OLTP | OLAP |
|---|---|---|
| Felhasználó | ügyintéző | elemző |
| Használat | rendszeresen ismétlődő | alkalmi |
| Adatok | naprakész, aktuális állapot | történeti, archivált |
| Összegzés szintje | nagyon részletes | összesített |
| Elérés | írás/olvasás | főleg olvasás |
| Elért rekordszám | tízes nagyságrend | milliós nagyságrend |
| Adatbázis szerkezete | relációs | csillag vagy hópehely séma |
| Teljesítménymutató | tranzakciós idő | lekérdezési idő |
| Funkció | operatív feldolgozás | döntéstámogatás |
Műszaki analógia: OLTP = gyártósor valós idejű PLC-vezérlése; OLAP = havi termelési riport elemzése. OLAP-lekérdezés OLTP-n → lelassítja/leállítja a napi működést → ezért külön rendszer. Előretekintés: big data és AI kölcsönhatás → 8. fejezet.

### D) Adattárház/adatpiac — Société Générale eset (Laudon Ch.6 Interactive Session; 4. ea. 5. fej.)
- Société Générale: Franciaország legnagyobb, az EU **3. legnagyobb** bankja; **76 ország**, **33+ millió ügyfél**; naponta **tízmillió tranzakció**, **1500+ fájlban** tárolva a fő adatbázisok frissítése előtt.
- Probléma: „koszos” adat — rekordszámok és összegek változnak rendszerek között, duplikált fájlok, hiányzó/rossz sorrendű fájlok → downstream alkalmazások leállása.
- Régi megoldás: több száz alkalmazott manuálisan ellenőrzött. Új: „intelligens rendszer” (**Infogix** platform) — de a lényeg: a vezetésnek fel kellett térképeznie és kodifikálnia **220+ üzleti szabályt**, amit az alkalmazottak évek tapasztalatából alakítottak ki; csak ezután lehetett automatizálni.
- Tanulság: „az adattárház/adatpiac sikere nem azon múlik, milyen szoftvert vásárolnak, hanem azon, hogy a vezetés fel tudja-e térképezni és tudatosítani a saját szervezeti tudását az adatokról — **menedzseri feladat**, amit semmilyen technológia nem helyettesíthet.”

### E) Vezetői szerepkörök a CIO mellett (Laudon Ch.2, Ch.6; 4. ea. 6. fej.)
| Szerepkör | Felelősségi terület |
|---|---|
| **CIO** (Chief Information Officer) | az IT-stratégia egésze, a technológia integrálása az üzleti stratégiába |
| **CSO/CISO** (Chief Security Officer) | információbiztonsági szabályzat kikényszerítése, biztonsági fenyegetések kezelése |
| **CPO** (Chief Privacy Officer) | adatvédelmi jogszabályoknak való megfelelés |
| **CKO** (Chief Knowledge Officer) | a vállalati tudásmenedzsment-program |
| **CDO** (Chief Data Officer) | vállalati szintű adatirányítás és -hasznosítás — a lehető legtöbb érték kinyerése az adatokból |

### F) Hazai kitekintő (4. ea. 8. fej.)
- **A) Bosch Hatvan** (Robert Bosch Elektronika Kft.): 2025, „Plant Digital Twin”, elektromos járművek komponensei; Gyártástrend magazin **„Az Év Gyári Projektje”** díj (ipari digitalizációs kategória). **Bosch Maklár** (Robert Bosch Automotive Steering Kft.): AI-alapú minőségellenőrzés, több **Shainin Dorian-díj**.
- **B) KKV-kutatás** (Garai-Fodor, Varga, Csiszárik-Kocsir 2023; 2022: N=161, 2023: N=72; 1–5 skála, 1 = egyáltalán nem hátráltató):

| Hátráltató tényező | 2022 | 2023 |
|---|---|---|
| **Információhiány** | **3,36 (1. hely)** | **3,14 (1. hely)** |
| Szakképzett munkaerő hiánya | 3,27 | 2,90 |
| Pénzügyi problémák | 3,18 | 3,12 |
| Technológiai hiányosságok | 3,01 | 2,94 |
| Digitális készségek hiánya | 2,61 | 2,47 |

Idézet: „nem elegendő csupán a készség vagy a digitális infrastruktúra megléte — azt jól kell tudni használni, illetve alkalmazni is.” **ANOVA, sig = 0,915**: a vállalkozás mérete **nem** befolyásolja szignifikánsan az információhiány súlyosságát. ⚠ forrásmegjegyzés: 2023-ban a 2. helyen a számok szerint a pénzügyi problémák (3,12) állnak, nem a szakképzett munkaerő hiánya (2,90) — a táblázat sorrendje a 2022-es rangsort követi.

## Számok, dátumok, nevek, amiket a tananyag kiemel

| Mi | Érték | Hol |
|---|---|---|
| Knight Capital dátum | 2012. augusztus 1., New York; piacnyitás 9:30 | 1. fej. |
| Szerverek | 8 (7 jó, 1 hibás); „Power Peg” 2003 óta nem használt | 1. fej. |
| 45 perc kár | 154 részvény; 397 M db; 4 M tranzakció; 440 M USD | 1. fej. |
| Részvényesés | 75 % két nap alatt; felvásárolták | 1. fej. |
| Téves diagnózis ideje | 20 perc | 7. fej. |
| IBM 2016 becslés | 3,1 billió USD/év, USA GDP ~18 %-a (Thomas C. Redman/HBR) | 3. fej. |
| IBM IBV 2025 | adatvezetők 43 %-a: adatminőség a legfontosabb prioritás | 3. fej. |
| Veszteség-becslés | >25 % a szervezeteknek 5 M USD felett; 7 % 25 M USD felett | 3. fej. |
| Fájlkörnyezet problémái | 4 | 3. fej. |
| OLTP/OLAP tulajdonságok | 9 sor; FASMI | 4. fej. |
| Société Générale | EU 3. legnagyobb; 76 ország; 33+ M ügyfél; 10 M tranzakció/nap; 1500+ fájl; 220+ üzleti szabály; Infogix | 5. fej. |
| Vezetői szerepkörök | CIO, CSO/CISO, CPO, CKO, CDO (5) | 6. fej. |
| CDO három feladata | megfelelő adat gyűjtése; megfelelő technológia; eredmények felhasználása | 6. fej. |
| Siemens Amberg | 6 M SIMATIC/év; 1200 változat; 350 átállás/nap; 50 M folyamatadat/nap | 7. fej. |
| Amberg minőség | 99,99885 % (≈11 hibás/millió) | 7. fej. |
| Amberg AI-megtakarítás | 500 000 EUR röntgenberendezés elkerülve (2025–2026) | 7. fej. |
| HBS Case | 518-054 | 7. fej. |
| Bosch Hatvan | 2025, Plant Digital Twin, „Az Év Gyári Projektje” | 8. fej. |
| Bosch Maklár | AI minőségellenőrzés, Shainin Dorian-díjak | 8. fej. |
| KKV-kutatás minta | 2022: N=161; 2023: N=72 | 8. fej. |
| Információhiány | 3,36 → 3,14 (1. hely mindkét évben) | 8. fej. |
| ANOVA | sig = 0,915 (méret nem szignifikáns) | 8. fej. |
| Elmélyítő: Xiao, Ding, Zhang | 2024, 261 CDO | 9. fej. |
| Elmélyítő: IBM IBV & Oxford Economics | 2023; adatbiztonság a CDO-k 52 %-a szerint legkritikusabb | 9. fej. |
| Elmélyítő: Tick, A. | 2023, Acta Polytechnica Hungarica 20(2), 83–104; V4 + Szerbia + Bulgária KKV-k; 47 idéző | 9. fej. |
| Elmélyítő: Turban, Pollard, Wood | 2023, 12th ed., Ch.3 „Data Management, Data Warehouses, and Data Governance” | 9. fej. |

## Számítások

Az előadás nem ad képletet. A tananyag számaiból levezethető ellenőrzések:
- **Amberg minőségi mutató:** 99,99885 % → hibaarány = 100 − 99,99885 = 0,00115 % = 0,0000115 → **11,5 hibás darab / millió** (a tananyag „kb. 11”-et ír). Évi 6 millió darabnál ≈ 69 hibás darab/év.
- **IBM 2016:** 3,1 billió USD = az amerikai GDP kb. 18 %-a → GDP ≈ 3,1 / 0,18 ≈ 17,2 billió USD (ellenőrzés, saját számítás).
- **Knight Capital tempó (saját számítás a tananyag számaiból):** 4 millió tranzakció / 45 perc ≈ 88 900 tranzakció/perc; 440 M USD / 45 perc ≈ 9,8 M USD veszteség percenként — a 20 perces téves diagnózis önmagában ~195 M USD-nyi időt jelentett.
- **„Mi változik, ha…”**: ha az adat → információ átmenetnél lett volna automatikus riasztás, és azonnal leállítanak, a kár a 45 perc töredéke; a DIKW-lánc bármelyik szintjének hiánya a teljes lánc kudarcát okozza, még ha az eredeti adat helyes is.

## Összekeverhető párok / „mi NEM igaz” csapdák

1. **Knight Capital: a 8. szerver kódja hibás volt?** Pontosabban: egy régi, elfeledett funkció (Power Peg) aktiválódott — a hiba lényege, hogy nem volt single source of truth a szerverek állapotáról; a rossz korrekció (visszaállítás minden szerverre) rontott.
2. **DIKW mint definíció vs. diagnózis** — a tananyag diagnosztikai eszközként használja; a leggyakoribb töréspont: **adat → információ**.
3. **OLTP vs. OLAP:** OLTP = ügyintéző, írás/olvasás, tízes rekordszám, relációs, tranzakciós idő; OLAP = elemző, főleg olvasás, milliós rekordszám, csillag/hópehely, lekérdezési idő. **FASMI az OLAP-ra** vonatkozik, nem az OLTP-re.
4. **Adattárház vs. adatpiac:** adattárház = teljes vállalat; adatpiac = egy üzleti terület (gyorsabb, olcsóbb, szűkebb).
5. **Adatredundancia vs. inkonzisztencia:** redundancia = ugyanaz több helyen; inkonzisztencia = eltérő értékek.
6. **A relációs adatbázis megszünteti az adatminőségi kockázatot?** NEM — csak az alapfeltételét teremti meg a kezelhetőségnek.
7. **CDO vs. CKO vs. CPO vs. CSO:** CDO = adat; CKO = tudásmenedzsment; CPO = adatvédelem (privacy); CSO/CISO = biztonság. CIO = IT-stratégia egésze.
8. **Société Générale tanulsága: a szoftver (Infogix) volt a kulcs?** NEM — a 220+ üzleti szabály feltérképezése és kodifikálása, menedzseri feladat.
9. **Adattárház-kialakítás IT-projekt?** NEM — „menedzseri infrastruktúra, nem IT-projekt”.
10. **KKV-k fő akadálya: pénz / technológia / digitális készség?** NEM — **információhiány** (mindkét évben 1. hely); a digitális készségek hiánya az utolsó.
11. **A vállalkozás mérete befolyásolja az információhiányt?** NEM — ANOVA sig = 0,915.
12. **Siemens Amberg vs. Bosch Hatvan:** Amberg = Németország, SIMATIC, 99,99885 %, egy közös adatmodell; Hatvan = Plant Digital Twin, 2025, EV-komponensek, díj. Maklár = AI-minőségellenőrzés, Shainin Dorian.
13. **IBM 3,1 billió:** 2016-os becslés, USA gazdaság, GDP ~18 % — ne keverd a 2025-ös 43 %-kal (adatvezetők prioritása).
14. **Governance KKV-nál = CDO kinevezése?** NEM — egy tudatos döntés: valaki explicit felelős + egyetlen közös adatforrás.
15. **Amberg AI:** nem új gépet vettek — **elkerültek** egy 500 000 eurós beruházást.

## Kapcsolat más előadásokkal

- Szigetrendszer / „két igazság” (3. ea.) ↔ single source of truth, adatinkonzisztencia.
- TPS (1. ea.) ↔ OLTP; DSS/ESS ↔ OLAP; OLAP és adattárház részletesen → 7. ea. (OLAP, adatbányászat) és 5. ea. (BI, adattárház mint BI-infrastruktúra).
- Big data ↔ AI kölcsönhatás → 8. ea. (a tananyag kifejezetten előreutal).
- CKO és tudásmenedzsment → 9. ea.; CPO/adatvédelem → 11. ea. etika; CSO/CISO → 12. ea. kiberbiztonság.
- Digitális iker (Bosch) ↔ 2. ea. értéklánc (termelés: digitális ikrek); 12. ea. digitális transzformáció.
- „Technológia nem elég” → 1. ea. komplementer eszközök; Société Générale = a szervezeti tudás kodifikálása (9. ea. tacit → explicit).
- KKV-k információhiánya ↔ 1. ea. MIR célja (információ, nem adat).

## Fogalomtár-jelöltek

- **DIKW-lánc** – DIKW chain – adat → információ → tudás → bölcsesség; diagnosztikai eszköz a töréspont azonosítására.
- **Adatredundancia** – data redundancy – ugyanaz az adat több helyen, eltérő formában.
- **Adatinkonzisztencia** – data inconsistency – ugyanannak az adatnak eltérő értékei rendszerenként.
- **Program-adat függőség** – program-data dependence – a kód összefonódik az adat fizikai elrendezésével.
- **Relációs adatbázis** – relational database – közös, logikailag rendezett adatállomány kulcsmezőkkel.
- **Online tranzakció-feldolgozás** – OLTP – operatív, naprakész, részletes, írás/olvasás.
- **Online analitikus feldolgozás** – OLAP – elemző, történeti, összesített, főleg olvasás.
- **FASMI** – Fast Analysis of Shared Multidimensional Information – az OLAP elvárásai.
- **Csillag / hópehely séma** – star / snowflake schema – az OLAP adatbázis szerkezete.
- **Adattárház** – data warehouse – a teljes vállalat elemzésre optimalizált adatai.
- **Adatpiac** – data mart – egy üzleti terület célzott adattárháza.
- **Adatirányítás** – data governance – explicit felelősség a vállalati adatvagyonért.
- **Adatigazgató** – CDO (Chief Data Officer) – vállalati adatirányítás és -hasznosítás.
- **Tudásigazgató** – CKO – a tudásmenedzsment-program felelőse.
- **Adatvédelmi igazgató** – CPO – adatvédelmi jogszabályi megfelelés.
- **Biztonsági igazgató** – CSO/CISO – információbiztonsági szabályzat, fenyegetések.
- **Egyetlen igazságforrás** – single source of truth – egy megbízható, mindenki által azonosan látott adatforrás.
- **Digitális iker** – digital twin – valós idejű virtuális kép a gyártási folyamatról.

---

# 5. előadás: Üzleti intelligencia: kultúra, nem eszköz

## Egy mondatban (a központi tézis)

A BI-bevezetés kudarca jellemzően **nem technikai, hanem strukturális/koordinációs**: a technikailag kész rendszer mögül hiányzik a szabványokért, bizalomépítésért és felhasználói bevonásért felelős szervezeti egység (BICC), és a döntéshozó még tökéletes adatból is torzított szűrőkön át dönt — a BI tehát **kultúra és stratégia, nem eszköz** (5. ea. 2., 5., 8. fej.).

## Nyitó eset és feloldása (5. ea. 1. és 8. fej.)

**Saját dilemma (Laudon Ch.12 szellemében):** egy középvállalat ügyvezetője **50 millió Ft**-ot fektetett egy Power BI-alapú VIR-be; a rendszer működik, a dashboardok szépek, a riportok pontosak — de **hat hónappal** később a középvezetők többsége továbbra is Excelben dolgozik, és csak akkor nyitja meg a Power BI-t, ha az ügyvezető rákérdez egy számra.

Három versengő hipotézis:
| Hipotézis | Mit jelentene | Diagnózis (8. fej.) |
|---|---|---|
| **H1 — Felületi/képzési probléma** | túl bonyolult rendszer, kevés képzés | önmagában ritkán elégséges — a Power BI felhasználóbarát; ha ez lenne az ok, célzott képzés gyorsan megoldaná |
| **H2 — Bizalmi probléma** | nem bíznak az adat forrásában/pontosságában | gyakori, de **tünet, nem gyökérok** — nincs, aki garantálja a konzisztenciát (Microsoft Starlight-eset) |
| **H3 — Koordinációs probléma** | nincs felelős a BI szervezeti bevezetéséért; technikailag kész, szervezetileg nem | **a leggyakoribb, legmélyebb ok** — nincs BICC-szerű egység |

**A válasz:** jellemzően **H3 → H2 → H1**: „a vezetők »nem tudják használni« (H1), mert nem bíznak benne (H2), mert senki nem garantálja a mögötte álló adat és folyamat megbízhatóságát (H3). A megoldás **nem több képzés, hanem egy BICC-szerű koordináló funkció** létrehozása.”

Elméleti pontok, amelyek bizonyítják: BI-érettségi modell + BICC (2. fej.: „a probléma nem a szoftverrel van, hanem a hiányzó szervezeti híddal”); Microsoft Starlight/KPI Lake (4. fej.: inkonzisztens definíciók → bizalmatlanság); NHS Choose and Book (7. fej.: egymást erősítő okok).

## Fogalmak és definíciók (HU – EN)

- **BI-érettségi modell (Gartner BI and Performance Management Maturity Model)** — öt szint: Unaware → Tactical → Focused → Strategic → Pervasive (2. fej.). A modell önmagában **leíró**: megmondja, hol tartunk, de nem magyarázza, miért nem lépünk tovább.
- **BICC — BI Kompetencia Központ (Business Intelligence Competency Center)** — szervezeti egység, amely átível a siló-struktúrán; a legmagasabb (Strategic/Pervasive) szinten jelenik meg; három kompetenciaterületet fog össze: **üzleti** (vízió, finanszírozás, prioritások), **elemző** (módszertan, szabványok, adatdefiníciók), **IT** (infrastruktúra, adatminőség, ETL). Korlát: **nem helyettesíti a döntéshozót**, csak a döntéshozatali folyamatot támogatja (2. fej.).
- **EDW** — egységes vállalati adattárház (enterprise data warehouse) — a Strategic szint jellemzője.
- **Preskriptív analitika (prescriptive analytics)** — a Pervasive szinten a BI túllép a leíró és prediktív elemzésen: nemcsak megjósolja a jövőt, hanem konkrét cselekvést/döntést javasol (2. fej.; ZEAL Network példa).
- **Az adatminőség hét dimenziója (Laudon Ch.12, Table 12.3)** — pontosság, integritás, konzisztencia, teljesség, érvényesség, időszerűség, hozzáférhetőség (3. fej.).
- **Strukturált / félig strukturált / strukturálatlan döntés** — MIS rutinjelentés / DSS what-if / ESS + vezetői ítélőképesség (3. fej.).
- **IT-centrikus BI** — az IT-osztály tervezi, építi, karbantartja a jelentéseket: megbízható, konzisztens, de lassú és rugalmatlan (4. fej.).
- **Self-service BI (önkiszolgáló BI)** — a felhasználók maguk építik jelentéseiket: gyors, rugalmas, de a konzisztencia és a „ki mit lát” bonyolultabb (4. fej.).
- **Bimodális IT (Gartner)** — **Mode 1**: stabil, megbízhatóság-fókuszú, IT-vezérelt; **Mode 2**: gyors, kísérletező, üzleti oldal által vezérelt; a self-service vs. IT-centrikus vita ennek konkrét esete; ugyanez a felhő bevezetésénél (9. fejezet) (4. fej.).
- **Managed Self-Service BI (felügyelt önkiszolgáló BI)** — középút: közös adatszabványok + önkiszolgáló hozzáférés (Microsoft megoldása) (4. fej.).
- **Árnyék-IT / árnyék-alkalmazások (shadow IT)** — a self-service négy jellemzőjének hiányában inkonzisztenciához és árnyék-IT-hez vezet (4. fej.).
- **Management Filters (vezetői szűrők)** — még tökéletes adatot is torzított szűrőkön keresztül dolgoz fel a döntéshozó (Kahneman 2011; Tversky és Kahneman 1986): rosszul mérik fel a kockázatot, mintázatot látnak ott is, ahol nincs, megérzés/érzelem/keretezés alapján döntenek (5. fej.).
- **Algoritmus-averzió (algorithm aversion)** — Dietvorst, Simmons és Massey (2015): ha egyszer látják, hogy az algoritmus hibázott, nem bíznak benne újra, még ha összességében jobb is az emberi becslésnél (5. fej.).
- **Automation bias (automatizálási torzítás)** — az ellentéte: túlzott bizalom az automatizált javaslatban, kritika nélkül, még ha nyilvánvalóan hibás is (5. fej.).
- **Mintzberg tíz vezetői szerepe (1971)** — a rendszer nem minden szerepet támogat egyformán (6. fej.; a teljes táblázat az opcionális könyvben — nem kötelező).

## Modellek és keretek

### A) BI-érettségi modell — öt szint (Gartner; 5. ea. 2. fej.)
| Szint | Jellemző |
|---|---|
| 1. **Unaware** | nincs formális BI-folyamat, mindenki a kéznél lévő eszközzel (Excel) dolgozik |
| 2. **Tactical** | alkalmi elemzés, elszigetelt rendszerek és adatforrások |
| 3. **Focused** | kidolgozott elemzési módszertan egyes területeken, **adatpiacok** jelennek meg |
| 4. **Strategic** | egységes vállalati adattárház (**EDW**), prediktív technikák, a BI a tervezést is támogatja |
| 5. **Pervasive** | **BI-kompetenciaközpontok** működnek, kollaboratív, adatvezérelt kultúra |
- Statisztika: 2019-es felmérés szerint a szervezetek **87 %-a** az alsó két szinten (Unaware/Tactical) ragadt (Gartner).
- A **Focused → Strategic** átmenethez kell a BICC (strukturális, nem technikai ok). Aki bevezeti a technológiát (Focused), de nincs koordináló egység → „technikailag éretlenebbnek tűnik, mint amilyen valójában”.
- AI: Pervasive szinten preskriptív analitika; **ZEAL Network** (online lottószolgáltató): prediktív modellek ügyféladatokból, valós idejű személyre szabás, inaktívvá váló ügyfelek előrejelzése. Minél automatizáltabb a döntés, annál nagyobb a tét hibás adat/bizalom esetén → kapcsolat a 4. fej. single source of truth-tal.

### B) Az adatminőség hét dimenziója (Laudon Table 12.3; 5. ea. 3. fej.) — sorrendben
| Dimenzió | Kérdés |
|---|---|
| 1. Pontosság | Az adat a valóságot tükrözi? |
| 2. Integritás | Az adatszerkezet és a kapcsolatok konzisztensek? |
| 3. Konzisztencia | Az adatelemek egységesen vannak definiálva? |
| 4. Teljesség | Minden szükséges adat rendelkezésre áll? |
| 5. Érvényesség | Az értékek a megengedett tartományban vannak? |
| 6. Időszerűség | Az adat akkor áll rendelkezésre, amikor kell? |
| 7. Hozzáférhetőség | Az adat elérhető, érthető, használható? |
- Műszaki kötődés: vezérlőkörnél az **időszerűség** kritikus; minőségbiztosítási jelentésnél a **pontosság**; éves stratégiai riportnál a **teljesség**. CNC hőmérséklet-érzékelő: pontos, de 10 perces késéssel használhatatlan (szerszámtörés).
- **Trade-off:** a hét dimenzió nem egyszerre optimalizálható — minél időszerűbb, annál kevesebb validáció → csökken a pontosság; valós idejű gyártási dashboard a sebességet, pénzügyi zárás a pontosságot választja — tudatos döntés, nem tervezési hiba.

### C) Három döntéstípus (5. ea. 3. fej.)
- **Strukturált** — pl. napi rendelési mennyiség → **MIS, rutinjelentések**
- **Félig strukturált** — pl. „mi történne, ha 5 %-kal emelnénk az árat?” → **DSS, what-if elemzés**
- **Strukturálatlan** — pl. lépjünk-e be egy új piacra? → **ESS, vezetői ítélőképesség**

### D) Self-service BI négy jellemzője (saját anyag; 5. ea. 4. fej.)
1. együttdolgozik a felhasználókkal, nem helyettük dolgozik;
2. kulcsadatok grafikus megjelenítése, figyelmeztetés, egy kattintásos lefúrás;
3. adatokban „gazdag”: különböző forrásokból vegyített, aggregált és részletes, historikus és valós idejű adat;
4. felhatalmazott, beavatott dolgozók: a fontos dolgokra figyelhetnek, célokkal és versennyel motiválva, proaktívan.
→ Ha ezek hiányoznak: inkonzisztencia és árnyék-IT.

**Microsoft „Starlight/KPI Lake” belső BI-átalakítás:** a kultúra arra ösztönzött, hogy mindenki „birtokolja” saját adatait → inkonzisztens adatdefiníciók régiónként; az elemzők idejük **75 %-át** adatgyűjtéssel töltötték; a jelentések **78 %-a** „offline környezetben” készült; évi **~30 millió USD** költség árnyék-alkalmazásokra. Megoldás: **Managed Self-Service BI** — nem visszatérés az IT-centrikushoz, hanem középút.

**BI-felhasználók megoszlása** (Laudon Fig. 12.4 logikája): **80 %+ alkalmi felhasználó** (kész jelentések); felső vezetők (dashboard); középvezetők/elemzők („power user”, lekérdez és szeletel).

Menedzseri döntési szituáció: 200 fős gyártó részleg, IT 3 hetes várólista → mindenki önállóan épít Power BI-jelentést → fél év múlva **három különböző „hivatalos” selejt-arány** kering — a self-service kockázata: konzisztencia.

### E) Management Filters, két ellentétes torzítás (5. ea. 5. fej.)
- **Bear Stearns és Lehman Brothers, 2008:** alábecsülték a komplex jelzálogpapírok kockázatát; a kockázatkezelő modellek túl optimista feltételezésekre épültek — „a rendszerek pontosan azt az eredményt adták, amit a vezetés hallani akart”.
- **Intel (saját anyag):** strukturálatlan stratégiai döntésnél az adatfolyam minden lépése rendben: adatok keresése (OLAP, adatbányászat) → feldolgozás → tálalás (vizualizáció) — a lánc végén a **„vezetők korlátozottsága”**: a tökéletes adatfolyam is a döntéshozó befogadóképességén akad el.
- **Algoritmus-averzió ↔ automation bias:** a jó döntéstámogatás e két ellentétes kockázat között egyensúlyoz — „se ne utasítsuk el reflexből a gépi javaslatot, se ne fogadjuk el automatikusan, kritika nélkül”. Analógia: precíz mérőműszer hibás kijelzővel / aki soha többé nem bízik a műszerben, miután egyszer tévedett.

### F) Mintzberg-szerepek alkalmazási szinten (Laudon Table 12.2; 5. ea. 6. fej.)
- Az **„erőforrás-elosztó”** szerepet a BI/DSS kifejezetten jól szolgálja (adatalapú allokáció).
- A **„vállalkozó”** és a **„tárgyaló”** szerephez **semmilyen rendszer nem ad támogatást** — tisztán emberi, kapcsolati, kreatív feladatok.
- Műszaki menedzsernél gyakori: **„zavarelhárító”** (váratlan géphiba) és „erőforrás-elosztó” (kapacitás-, karbantartás-ütemezés). Kérdés: a BI a zavarelhárítás **döntési szakaszát** gyorsítja, vagy csak az információgyűjtést — „a kettő nem ugyanaz”. A „vállalkozó” szerepet BI-val helyettesíteni → eleve kudarc.
- Tanulság: „vezessünk be egy rendszert, ami mindent megold” → kérdezd: pontosan melyik vezetői szerepet támogatjuk?

### G) NHS „Choose and Book” — többtényezős elemzés (Laudon Ch.12 Interactive Session; 5. ea. 7. fej.)
- 2004, brit NHS, **200 millió font**; online kórház- és időpontválasztás háziorvosi beutaló alapján; 2014-re **356 millió font**; a tervezett **évi 51 millió font** megtakarítás soha nem valósult meg.
| Magyarázat | Bizonyíték mellette | Korlátja |
|---|---|---|
| (1) Rossz alapfeltevés | a kórházválasztás volt a középpont, de a betegek/háziorvosok gyors, helyi ellátást akartak | nem magyarázza, miért nem korrigálták a célt |
| (2) Hiányzó ösztönzők | a háziorvosoknak nem volt anyagi/szakmai érdeke használni | nem magyarázza, miért nem alakítottak ki utólag ösztönzőt |
| (3) Technikai inkompatibilitás | kórházi és háziorvosi rendszerek nem kommunikáltak megbízhatóan | orvosolható lett volna — mégsem történt meg |
- **Legvalószínűbb: mindhárom együtt, egymást erősítve**: (1) → motiválatlanság (2) → senki nem sürgette a technikai javítást (3) → tovább erősítette a bizalmatlanságot. „Egy komplex rendszerbukásnál ritkán van egyetlen »gyökérok« — a valódi kérdés az, hogyan erősítik egymást a különböző szintű problémák.”

### H) OTP Mobilbank — BI mindenkinek (5. ea. 8. fej.)
Személyes pénzügyi asszisztens: automatikus tranzakció-kategorizálás gépi tanulással (**90 %-os pontosság**), kiadásfigyelő dashboard, célalapú megtakarítás. Eredmény: közel **2 millió aktív felhasználó havonta**; a megtakarítási funkciót használók **20–30 %-kal** többet takarítanak meg. Siker kulcsa: bonyolult analitika intuitív felületbe csomagolva — „a BICC-elv gyakorlati alkalmazása lakossági kontextusban”.

## Számok, dátumok, nevek, amiket a tananyag kiemel

| Mi | Érték | Hol |
|---|---|---|
| Nyitó dilemma | 50 M Ft Power BI; 6 hónap | 1. fej. |
| BI-érettségi szintek | 5 (Unaware, Tactical, Focused, Strategic, Pervasive) | 2. fej. |
| Alsó két szinten ragadt | 87 % (2019, Gartner) | 2. fej. |
| BICC kompetenciaterületek | 3 (üzleti, elemző, IT) | 2. fej. |
| ZEAL Network | online lottó, prediktív modellek, preskriptív analitika | 2. fej. |
| Adatminőség dimenziói | 7 (Laudon Table 12.3) | 3. fej. |
| CNC-példa késés | 10 perc | 3. fej. |
| Döntéstípusok | 3 (strukturált/félig/strukturálatlan) | 3. fej. |
| Self-service jellemzők | 4 | 4. fej. |
| Microsoft Starlight | 75 % idő adatgyűjtés; 78 % offline jelentés; ~30 M USD/év árnyék-alkalmazás | 4. fej. |
| Alkalmi BI-felhasználók | 80 %+ (Laudon Fig. 12.4) | 4. fej. |
| Döntési szituáció | 200 fős részleg; 3 hetes IT-várólista; 3 selejt-arány | 4. fej. |
| Kahneman / Tversky és Kahneman | 2011 / 1986 | 5. fej. |
| Bear Stearns, Lehman Brothers | 2008 | 5. fej. |
| Dietvorst, Simmons, Massey | 2015, J. Exp. Psychology: General 144(1), 114–126 | 5., 9. fej. |
| Mintzberg | 1971; 10 szerep; Laudon Table 12.2 | 6. fej. |
| NHS Choose and Book | 2004; 200 M → 356 M font (2014); 51 M font/év elmaradt megtakarítás | 7. fej. |
| OTP Mobilbank | 90 % kategorizálási pontosság; ~2 M aktív felhasználó/hó; +20–30 % megtakarítás | 8. fej. |
| Elmélyítő | Martins et al. 2024; Alzghoul et al. 2024; Theodorakopoulos et al. 2025 (Electronics 14(19), 3930) | 9. fej. |

## Számítások

Az előadás nem ad képletet. A tananyag számaiból:
- **NHS költségtúllépés:** (356 − 200) / 200 = **78 %** túllépés; a 10 év alatt elmaradt megtakarítás 10 × 51 = 510 M font (saját számítás, a tananyag csak az évi 51 M-et adja).
- **Microsoft:** ha egy elemző idejének 75 %-a adatgyűjtés, csak 25 % elemzés → 4 elemzőből „1 elemez” (saját értelmezés).
- **„Mi változik, ha…”**: ha a Managed Self-Service bevezetése után az adatgyűjtési idő 75 %-ról 25 %-ra csökken, az elemzésre fordítható idő megháromszorozódik (25 % → 75 %) — ez a közös adatszabványok értéke.

## Összekeverhető párok / „mi NEM igaz” csapdák

1. **A dilemma megoldása több képzés (H1)?** NEM — H3 (koordináció, BICC) a gyökérok; H2 tünet; H1 felszín.
2. **Az érettségi modell megmagyarázza, miért nem lépünk tovább?** NEM — leíró; az ok strukturális (BICC hiánya).
3. **BICC hol jelenik meg?** Strategic/Pervasive szinten; **adatpiac** = Focused; **EDW** = Strategic; **BI-kompetenciaközpontok működnek** = Pervasive.
4. **BICC helyettesíti a döntéshozót?** NEM — a folyamatot támogatja.
5. **Hét dimenzió vs. négy fájlkörnyezeti probléma (4. ea.):** a hét = pontosság, integritás, konzisztencia, teljesség, érvényesség, időszerűség, hozzáférhetőség. Konzisztencia ≠ integritás (definíció egységessége vs. szerkezet/kapcsolatok).
6. **Időszerűség vs. pontosság trade-off:** gyorsabb → kevesebb validáció → kisebb pontosság; ez tudatos döntés.
7. **Self-service = kevesebb IT-kontroll?** NEM — tudatosan tervezett felhasználói élmény (4 jellemző).
8. **Microsoft megoldása = vissza az IT-centrikushoz?** NEM — Managed Self-Service (középút).
9. **Mode 1 vs. Mode 2:** Mode 1 = stabil, IT-vezérelt; Mode 2 = gyors, kísérletező, üzleti oldal.
10. **Algoritmus-averzió vs. automation bias:** averzió = elutasítás egy hiba után; automation bias = kritikátlan elfogadás. Dietvorst et al. 2015 = averzió.
11. **Bear Stearns/Lehman: rossz adat?** NEM — túl optimista modellfeltételezések; a rendszer azt adta, amit hallani akartak (management filters).
12. **Mintzberg: melyik szerepet támogatja a BI jól / egyáltalán nem?** Jól: erőforrás-elosztó. Egyáltalán nem: vállalkozó, tárgyaló.
13. **NHS: egyetlen gyökérok?** NEM — mindhárom egymást erősítve.
14. **NHS számok:** 200 → 356 M font; 51 M font/év tervezett megtakarítás; 2004 → 2014.
15. **87 % (érettség) vs. 80 %+ (alkalmi felhasználók) vs. 90 % (OTP pontosság)** — három különböző szám.
16. **Preskriptív vs. prediktív:** prediktív = megjósolja; preskriptív = cselekvést javasol (Pervasive).

## Kapcsolat más előadásokkal

- Single source of truth, adatminőség (4. ea.) ↔ a hét dimenzió, bizalmi probléma (H2), ZEAL automatizált döntés tétje.
- MIS/DSS/ESS és döntéstípusok → 1. ea. piramis; OLAP, adatbányászat (Intel-példa) → 7. ea.
- Adatpiac/EDW az érettségi modellben → 4. ea. adattárház/adatpiac.
- Bimodális IT (Mode 1/Mode 2) → 10. ea. felhő (a tananyag „9. fejezetként” utal előre — a Moodle-számozásban 10.).
- Management filters, algoritmus-averzió/automation bias → 11. ea. (etika, algoritmusok, felelős AI — emberi felügyelet).
- Árnyék-IT → 12. ea. kiberbiztonság.
- Szervezeti ellenállás, „bypass kultúra”, bizalomhiány (1. ea.) ↔ Excel-visszatérés a dilemmában (párhuzamos futtatás minta).
- KPI/dashboard (1. ea.) ↔ BI-felhasználói rétegek (dashboard a felső vezetőnek).
- Preskriptív analitika, prediktív modellek → 8. ea. Big Data, 11. ea. AI.

## Fogalomtár-jelöltek

- **BI-érettségi modell** – BI maturity model – Unaware, Tactical, Focused, Strategic, Pervasive (Gartner).
- **BI-kompetenciaközpont** – BICC – silókon átívelő egység; üzleti, elemző, IT kompetenciák; nem helyettesíti a döntéshozót.
- **Vállalati adattárház** – EDW – egységes adattárház a Strategic szinten.
- **Preskriptív analitika** – prescriptive analytics – cselekvést javasló elemzés a Pervasive szinten.
- **Adatminőség hét dimenziója** – data quality dimensions – pontosság, integritás, konzisztencia, teljesség, érvényesség, időszerűség, hozzáférhetőség.
- **Strukturált döntés** – structured decision – rutin, MIS-jelentés.
- **Félig strukturált döntés** – semi-structured decision – DSS, what-if.
- **Strukturálatlan döntés** – unstructured decision – ESS, vezetői ítélőképesség.
- **IT-centrikus BI** – IT-centric BI – az IT építi a jelentéseket; megbízható, lassú.
- **Önkiszolgáló BI** – self-service BI – a felhasználó építi; gyors, konzisztencia-kockázat.
- **Felügyelt önkiszolgáló BI** – managed self-service BI – közös szabványok + önkiszolgálás (Microsoft).
- **Bimodális IT** – bimodal IT – Mode 1 stabil/IT-vezérelt, Mode 2 gyors/üzleti (Gartner).
- **Árnyék-IT** – shadow IT – nem hivatalos, szétszórt alkalmazások és jelentések.
- **Vezetői szűrők** – management filters – kognitív torzítások az adat feldolgozásában.
- **Algoritmus-averzió** – algorithm aversion – a hibázó algoritmus tartós elutasítása.
- **Automatizálási torzítás** – automation bias – az automatizált javaslat kritikátlan elfogadása.
- **Mintzberg vezetői szerepek** – managerial roles – 10 szerep; erőforrás-elosztó jól támogatott, vállalkozó és tárgyaló nem.

---

# 6. előadás: BI a gyakorlatban I. — KPI-tervezés kritikusan (a Goodhart-csapdától az OEE-gamingig)

⚠ forrásmegjegyzés: a tantárgyi adatlap 6. heti előadáscíme „OLAP és adatbányászat: mit kérdezünk az adatoktól?”, a Moodle 6. előadás kötelező könyve viszont „BI a gyakorlatban I. — KPI-tervezés kritikusan”; az OLAP/adatbányászat a Moodle 7. előadásban van (a 6. ea. 8. fej. kitekintése is ezt mondja: „a 7. előadásban… az OLAP-tól a valódi adatbányászatig… a Target terhesség-előrejelző algoritmusáig”). A 8. fejezet („Szintézis”) a forrásban kétszer szerepel (6.8.html és 6.9.html) azonos tartalommal — egyként kezelve. A kötelező könyv ennél az előadásnál a Szintézis fejezettel ér véget.

## Egy mondatban (a központi tézis)

Nem az a kérdés, hogyan mérjünk többet, hanem hogyan mérjünk **jól**: egy jó KPI-rendszer a döntéshozó ítélőképességét **támogatja, nem helyettesíti** — bármelyik jól megtervezett mutató elromlik, ha célponttá válik (Goodhart), a technikailag pontos OEE is megjátszható, a BSC bürokratikus rituálévá silányulhat, és a dashboard sosem „semleges” (6. ea. 2., 3., 8. fej.).

## Nyitó eset és feloldása (6. ea. 2. és 8. fej.)

**Nyitó dilemma — „Amikor 22 KPI kevesebbet mond, mint 3”:** egy közepes gyártóüzem vezetése minden fontos szempontot látni akar a napi dashboardon → **22 KPI** egyetlen felületen (selejtarány, OEE, energiafogyasztás, túlóra-arány, beszállítói pontosság, vevői reklamáció, karbantartási költség…), mind zölden/pirosan villogva. **Három hónap** múlva a műszakvezetők egyre kevesebbet nézik — nem érdektelenségből, hanem mert nem tudják eldönteni, melyik szám számít most. „Amikor minden piros, semmi sem sürgős; amikor minden zöld, semmi sem árulkodik a valódi kockázatról.” → **elemzési bénultság (analysis paralysis)**.

**Feloldás (8. fej.):** a 22 KPI-s dashboard „nem azért volt rossz, mert a mutatók egyenként hibásak lettek volna — hanem mert a rendszer egésze **nem tett különbséget a fontos és a kevésbé fontos között**.” Záró tanulság: ha a vezető minden döntését kizárólag a dashboardra hivatkozva hozza, és nem meri megkérdőjelezni a mutatót, „az már nem adatvezérelt vezetés, hanem **mikromenedzsment automatizált álruhában**.”

Elméleti pontok, amelyek bizonyítják: Goodhart-törvény (3. fej.), OEE-gaming és helyi vs. rendszerszintű optimalizálás (4. fej.), BSC-kritika (5. fej.), data-ink ratio / Lie Factor (6. fej.), a 1. ea. 4. fej. „melyik 5–10 KPI” elve.

## Fogalmak és definíciók (HU – EN)

- **Elemzési bénultság (analysis paralysis)** — túl sok egyidejű mutató mellett a döntéshozó nem tudja eldönteni, mi számít (2. fej.).
- **Goodhart törvénye (Goodhart's law)** — Charles Goodhart, **1975**, eredetileg monetáris politikai kontextusban: **„amikor egy mutató célponttá válik, megszűnik jó mutatónak lenni.”** (3. fej.)
- **AHT — átlagos hívásidő (Average Handling Time)** — call center példa: egyetlen KPI-ként az AHT javul, de az ismételt hívások aránya drasztikusan nő — „a mutató javult, a valódi cél romlott” (3. fej.).
- **SMART-kritériumok, lag- és lead-mutatók** — a tananyag „már ismertként” említi, nem részletezi (3. fej.).
- **OEE — Teljes Eszközhatékonyság (Overall Equipment Effectiveness)** — a gyáripar egyik legelterjedtebb összetett mutatója: Rendelkezésre állás × Teljesítmény × Minőség (4. fej.).
- **OEE gaming** — az egyik komponens javítása a másik rovására; helyi optimalizálás rendszerszintű kárral (4. fej.).
- **Bottleneck-gép (szűk keresztmetszet)** — ha a sor egésze nem gyorsul, a rendszer átfutási ideje nem javul (4. fej.).
- **Balanced Scorecard (BSC)** — Kaplan és Norton (1996); négy perspektíva: pénzügyi, vevői, belső folyamat, tanulás-fejlődés; eredeti szándék szerint **oksági lánc**, nem mutatólista (5. fej.).
- **Stratégiai térkép (strategy map)** — a valódi oksági lánc ábrázolása, amit a gyakorlatban gyakran nem építenek meg (5. fej.).
- **Data-ink ratio** — Edward Tufte elve: minden vizuális elemnek információt kell hordoznia (6. fej.).
- **Stephen Few 13 gyakori dashboard-hibája** — túlzsúfoltság, félrevezető skálázás, felesleges 3D-effektek stb. (6. fej.).
- **Lie Factor** — a grafikonon látható vizuális változás mértékének aránya a mögötte lévő valós adatváltozáshoz képest; nem nulláról indított y-tengely: 2 %-os valós növekedés vizuálisan akár 200 %-osnak tűnhet (6. fej.).
- **AI-alapú döntéstámogatás kockázatai** (Laudon 18. kiad., Ch.12 „Risks Introduced by Using AI in Decision Making”): beépült torzítás (bias), az átláthatóság hiánya, etikai kérdések (6. fej.).
- **Key Influencers (Power BI)** — automatikusan azonosítja, mely tényezők befolyásolják leginkább egy mutatót (pl. mi korrelál az OEE ingadozásával) (7. fej.).
- **Anomaly Detection (Power BI)** — önműködően jelzi, ha egy idősor szokatlanul viselkedik (7. fej.).
- **GE Predix** — General Electric platformja: emberi felügyeletű KPI-monitorozás → AI-alapú anomáliadetektálás (7. fej.).

## Modellek és keretek

### A) Goodhart-csapda (6. ea. 3. fej.)
- Call center AHT-példa; gyártás: egyetlen KPI „gyártott darabszám/műszak” → minőség vagy gépkarbantartás rovására növelik.
- Műszaki analógia: szenzor kalibrálva, hogy mindig a kívánt tartományban mérjen — a mutató és a valóság elszakad.
- **AI-korban:** Thomas és Uminsky (2022, *Patterns*, Cell Press, 3(5)): a mai AI-rendszerek — különösen a mélytanulási modellek — „fegyverként használják” a Goodhart-törvényt: könyörtelenül egyetlen metrikára optimalizálnak → a gép „megjátssza” a mérőszámot, az eredeti cél sérül.

### B) OEE — képlet és gaming (6. ea. 4. fej.) — lásd Számítások
Három gaming-mód:
1. **Teljesítmény** javítása: a gépet a hivatalos névleges sebességnél alacsonyabb „ideális ciklusidővel” veszik nyilvántartásba.
2. A **minőségi hibákat a műszak végén** rögzítik, nem valós időben.
3. **Helyi optimalizálás rendszerszintű kárral:** egy gépcsoport OEE-jét egyedileg hajtják fel, miközben a sor egésze (bottleneck) nem gyorsul → az átfutási idő nem javul.
Analógia: autó fogyasztását csak lejtőn mérni.

### C) Balanced Scorecard kritikai nézőpontból (6. ea. 5. fej.)
- Kaplan–Norton oksági lánc: **tanulás-fejlődés → belső folyamatok → vevői elégedettség → pénzügyi eredmény**.
- A gyakorlatban a szervezetek gyakran: (1) **utólag illesztik** a mutatókat a meglévő jelentési struktúrához strategy map helyett; (2) a négy perspektívát **négy külön silóként** kezelik; (3) a rendszer **bürokratikus rituálévá** válik (negyedéves táblázat, amit senki nem használ döntésre).
- Rokon a Goodhart-csapdával: ha a mutatók kitöltése önmagáért való cél, elveszti stratégiai funkcióját. Analógia: rutinból kipipált karbantartási checklist.

### D) Dashboard-tervezés tudománya (6. ea. 6. fej.)
- Tufte data-ink ratio; Few 13 hibája; Lie Factor.
- Etikai réteg: tudatosan csonkolt y-tengely a negyedéves jelentésben — „nem hazudik technikai értelemben — de manipulál”; a dashboard-tervező hatalma mint egy szerkesztőé: „eldönti, mit látunk meg először”.
- AI-korban élesebb: az emberi tervező tudatosan dönt; az AI-alapú „automatikus kiemelés” (Power BI Key Influencers) **öntudatlanul** is torzíthat — a torzítás forrása a tanítóadat vagy az algoritmus, nehezebben azonosítható.

### E) Power BI gyakorlati kapocs — GE Predix (Laudon 15. kiad., Ch.12; 6. ea. 7. fej.)
- GE repülőgép-hajtómű flotta: bizonyos üzemeltetési környezetek (**Közel-Kelet, Kína** hőmérsékleti és porviszonyai) szisztematikusan gyorsabb kopáshoz vezettek — a felismerés **nem egy gép adatából, hanem a teljes flotta összevetéséből**.
- Power BI: Key Influencers, Anomaly Detection. Analógia: tapasztalt karbantartó, aki „beleérzi magát a gép hangjába” — az algoritmus adatokból szerzi a tapasztalatot.
- Kritika: ezek megkönnyítik a mintázatfelismerést, de **nem mentesítenek** a Goodhart/OEE-gaming kritikák alól; az automatikus kiemelés nehezebben kérdőjelezhető meg, mert „objektívnek” tűnik.

### F) Szintézis négy pontja (6. ea. 8. fej.)
1. Goodhart: bármely jó KPI elromlik, ha céllá válik — AI-ban is. 2. OEE pontossága nem garancia a manipuláció ellen — a gaming a helyi optimalizálás és a rendszerszintű cél feszültségéből fakad. 3. BSC csak akkor stratégiai, ha nem rituálé. 4. A dashboard-tervezés sosem semleges — ember vagy AI, mindig értékítélet.

## Számok, dátumok, nevek, amiket a tananyag kiemel

| Mi | Érték | Hol |
|---|---|---|
| Nyitó dilemma | 22 KPI; 3 hónap | 2. fej. |
| Goodhart | Charles Goodhart, 1975, monetáris politika | 3. fej. |
| Thomas & Uminsky | 2022, Patterns (Cell Press) 3(5) — „Reliance on metrics is a fundamental challenge for AI” | 3. fej. |
| OEE számpélda | 480 perc tervezett, 432 perc tényleges (90 %); teljesítmény 85 %; minőség 98 %; OEE 75 % | 4. fej. |
| World class OEE | ~85 %; a legtöbb üzem 40–60 % | 4. fej. |
| BSC | Kaplan & Norton 1996; 4 perspektíva | 5. fej. |
| Tufte | data-ink ratio | 6. fej. |
| Few | 13 dashboard-hiba | 6. fej. |
| Lie Factor példa | 2 % valós → akár 200 % vizuális | 6. fej. |
| AI-kockázatok | 3 (bias, átláthatóság hiánya, etika) — Laudon 18. kiad. Ch.12 | 6. fej. |
| GE Predix | Közel-Kelet, Kína; Laudon 15. kiad. Ch.12 | 7. fej. |
| Power BI funkciók | Key Influencers; Anomaly Detection | 7. fej. |

## Számítások — OEE (6. ea. 4. fej.)

**Képlet (a tananyag pontos megfogalmazása):**
- **OEE = Rendelkezésre állás × Teljesítmény × Minőség**
- Rendelkezésre állás (Availability) = tényleges üzemidő ÷ tervezett üzemidő
- Teljesítmény (Performance) = (ciklusidő × legyártott darabszám) ÷ tényleges üzemidő
- Minőség (Quality) = jó darabszám ÷ összes legyártott darabszám

**A tananyag számpéldája végigszámolva:**
- Tervezett műszak 480 perc; tényleges üzemidő 432 perc → Rendelkezésre állás = 432 / 480 = **0,90 (90 %)**
- Teljesítmény = a névleges kapacitás 85 %-a = **0,85**
- Minőség = a darabok 98 %-a megfelelő = **0,98**
- **OEE = 0,90 × 0,85 × 0,98 = 0,7497 ≈ 0,75 → 75 %**

Értelmezés: a tananyag szerint „ez világszínvonalúnak számít a gyáriparban (a »world class« OEE ~85 % körül van, a legtöbb üzem valós OEE-je 40–60 % között mozog)”. ⚠ forrásmegjegyzés: a 75 % a tananyag saját számai szerint a world class 85 % **alatt**, de a tipikus 40–60 % **felett** van — a „világszínvonalú” minősítés és a 85 %-os küszöb ellentmond egymásnak; ZH-ra: world class ≈ 85 %, tipikus 40–60 %, a példa 75 %.

**Kiegészítő levezetés (saját számok a teljesítmény-komponenshez, mert a tananyag csak a 85 %-ot adja):** ha az ideális ciklusidő 0,5 perc/db és 432 perc alatt 734 darab készül: Teljesítmény = (0,5 × 734) / 432 = 367 / 432 = 0,85 ✓. Minőség: 734 db-ból 719 jó → 719/734 = 0,98 ✓.

**„Mi változik, ha…” variánsok:**
- Ha a rendelkezésre állás 80 %-ra esik (384 perc üzem): OEE = 0,80 × 0,85 × 0,98 = **0,666 → 66,6 %** — 10 pontnyi availability-romlás ~8,3 pontnyi OEE-romlás, mert a komponensek **szorzódnak**.
- Ha mindhárom komponens 90 %: OEE = 0,9³ = **72,9 %** — három „jó” komponensből sem lesz 90 %-os OEE.
- **Gaming-példa:** ha a műszakvezető az ideális ciklusidőt 0,5 helyett 0,55 percre „állítja”: Teljesítmény = (0,55 × 734)/432 = 0,934 → OEE = 0,90 × 0,934 × 0,98 = **82,4 %** — a szám javult, a gép valós teljesítménye nem (ez az 1. gaming-mód). Ha a selejtet a műszak végén rögzítik, a valós idejű minőség 100 %-nak látszik: OEE = 0,90 × 0,85 × 1,00 = 76,5 % a műszak közben (2. gaming-mód).

**Lie Factor (6. fej.) — illusztráció saját számokkal:** valós változás 100 → 102 (+2 %); ha az y-tengely 99-től indul, az oszlop 1 egységről 3 egységre nő (+200 %) → Lie Factor = 200 % / 2 % = **100** (a tananyag definíciója: vizuális változás ÷ valós változás; a „2 % → 200 %” számpár a tananyagból).

## Összekeverhető párok / „mi NEM igaz” csapdák

1. **22 KPI: a mutatók voltak hibásak?** NEM — egyenként jók; a rendszer nem rangsorolt.
2. **Goodhart: a mutató rossz?** NEM — jó mutató is elromlik, ha **célponttá** válik. 1975, monetáris politika — nem gyártás.
3. **AHT-példa:** az AHT javul, az **ismételt hívások aránya** nő — a mutató és a cél elválik.
4. **OEE komponensek sorrendje és képlete:** Rendelkezésre állás (tényleges/tervezett üzemidő), Teljesítmény ((ciklusidő × db)/tényleges üzemidő), Minőség (jó/összes). Összeg NEM — **szorzat**.
5. **OEE 75 % = world class?** A tananyag „világszínvonalúnak” nevezi, de a world class küszöböt ~85 %-nak adja; tipikus 40–60 % (⚠ lásd fent).
6. **OEE gaming = adathamisítás?** Nem feltétlenül: alacsonyabb ideális ciklusidő nyilvántartása, selejt műszakvégi rögzítése, helyi optimalizálás — „technikailag pontos” mutató is megjátszható.
7. **BSC = mutatólista?** NEM — Kaplan–Norton: oksági lánc (tanulás → folyamat → vevő → pénzügy); a silóként kezelés a hiba.
8. **BSC négy perspektívája:** pénzügyi, vevői, belső folyamat, tanulás-fejlődés — a strategy map a lánc ábrája.
9. **Data-ink ratio = Tufte; 13 hiba = Few; Lie Factor** = vizuális változás / valós változás.
10. **Csonkolt y-tengely = hazugság?** „Nem hazudik technikai értelemben — de manipulál.”
11. **Emberi vs. AI torzítás a dashboardon:** ember tudatosan dönt; AI öntudatlanul (tanítóadat/algoritmus) — nehezebben azonosítható.
12. **Key Influencers vs. Anomaly Detection:** Key Influencers = mely tényezők befolyásolják a mutatót; Anomaly Detection = szokatlan idősor-viselkedés jelzése.
13. **GE Predix felismerése egy gép adatából?** NEM — a teljes flotta összevetéséből.
14. **Power BI AI-funkciók mentesítenek a Goodhart-kritika alól?** NEM — sőt, nehezebben megkérdőjelezhetők.
15. **Jó KPI-rendszer helyettesíti a döntéshozót?** NEM — támogatja az ítélőképességet; ellenkező esetben mikromenedzsment.

## Kapcsolat más előadásokkal

- KPI négy jellemzője, CSF, „melyik 5–10 KPI” (1. ea. 4. fej.) ↔ 22 KPI dilemma, information overload (1. ea. 3. fej.).
- Management filters, automation bias (5. ea.) ↔ „objektívnek tűnő” automatikus kiemelés; dashboard a felső vezetőnek (5. ea. Fig. 12.4).
- Adatminőség-dimenziók (5. ea.: időszerűség vs. pontosság) ↔ selejt műszakvégi rögzítése (valós idejűség).
- AI-kockázatok (bias, átláthatóság, etika) → 11. ea. etika és felelős AI; Thomas–Uminsky Goodhart az AI-ban.
- OLAP, adatbányászat, Target terhesség-előrejelzés → 7. ea. (a tananyag kitekintése).
- GE Predix (IoT, flottaadat) → 8. ea. Big Data; prediktív karbantartás (2. ea. értéklánc, szerviz).
- Power BI gyakorlat (labor) ↔ 6. ea. 7. fej.

## Fogalomtár-jelöltek

- **Elemzési bénultság** – analysis paralysis – túl sok mutató miatt nem születik döntés.
- **Goodhart törvénye** – Goodhart's law – a célponttá vált mutató megszűnik jó mutatónak lenni (1975).
- **Átlagos hívásidő** – AHT (Average Handling Time) – call center KPI, a Goodhart-példa.
- **Teljes eszközhatékonyság** – OEE – rendelkezésre állás × teljesítmény × minőség.
- **Rendelkezésre állás** – availability – tényleges / tervezett üzemidő.
- **Teljesítmény** – performance – (ciklusidő × darabszám) / tényleges üzemidő.
- **Minőség** – quality – jó darab / összes darab.
- **OEE-gaming** – OEE gaming – egy komponens javítása a másik vagy a rendszer rovására.
- **Szűk keresztmetszet** – bottleneck – a sor átfutási idejét meghatározó gép.
- **Kiegyensúlyozott mutatószámrendszer** – Balanced Scorecard – négy perspektíva oksági láncban (Kaplan–Norton 1996).
- **Stratégiai térkép** – strategy map – a BSC oksági láncának ábrája.
- **Adat-tinta arány** – data-ink ratio – Tufte: minden vizuális elem hordozzon információt.
- **Hazugsági faktor** – Lie Factor – vizuális változás / valós adatváltozás.
- **Kulcsbefolyásolók** – Key Influencers – Power BI vizuál a mutatót befolyásoló tényezőkre.
- **Anomáliadetektálás** – anomaly detection – szokatlan idősor-viselkedés automatikus jelzése.

---

# 7. előadás: BI a gyakorlatban II. — valós kutatás, OLAP és adatbányászat

⚠ forrásmegjegyzés: a tantárgyi adatlapon a 7. hét üres („–”), a 8. hét „Tudásmenedzsment”; a Moodle 7. előadás kötelező könyve az OLAP/adatbányászat (az adatlap 6. heti címe). A jegyzet a Moodle-számozást követi.

## Egy mondatban (a központi tézis)

A 6–7. előadás közös íve: **minél kifinomultabb egy mérési vagy előrejelző eszköz, annál nagyobb a felelősség, hogyan használjuk** — az OLAP megmondja, *hol* a probléma, az adatbányászat *miért*, de a KDD-folyamat 80 %-a adat-előkészítés (GIGO), a magas konfidencia a Lift nélkül félrevezető, és a prediktív modell (Target) hamis pozitívjai valódi emberi kárt okoznak: „az algoritmus vagy mutató eszköz, nem döntéshozó” (7. ea. 2., 4., 5., 7., 8. fej.).

## Nyitó eset és feloldása (7. ea. 2. és 8. fej.)

Ennek az előadásnak nincs klasszikus nyitó dilemmája; a nyitó „eset” egy **publikált kutatás**: **Tokola, Gröger, Järvenpää & Niemi (2016)**, „Designing Manufacturing Dashboards on the Basis of a Key Performance Indicator Survey”, *Procedia CIRP*, 57, 619–624. Eredmény: a legtöbb vállalati dashboard **nem a döntéshozó tényleges kérdéseiből indul ki, hanem abból, milyen adat éppen rendelkezésre áll**; a szerzők strukturált tervezési módszertant javasolnak, amely a KPI-kiválasztást a **felhasználói szerepkörhöz** (műszakvezető, üzemvezető, felső vezetés) igazítja. Ez empirikusan igazolja a 6. ea. 22 KPI-dilemmáját: „a probléma nem a mutatók száma, hanem az, hogy nem lett átgondolva, kinek, milyen döntéshez kell az adott mutató.” Ábra: egy vállalati célszám (pl. OEE) lebomlása a hierarchia szintjein különböző részletezettségű dashboardokká.

**Az előadás „esete” a végén a Target-eset (7. fej.),** amelynek feloldása az etikai határ és a hamis pozitívok kérdése — lásd Modellek F).

**Szintézis (8. fej.):** a Bosch Hatvan-i és Siemens Amberg-i példákban „a technológia (szenzorok, valós idejű dashboardok, prediktív karbantartás) önmagában nem hozott automatikusan jobb döntéseket” — a siker azon múlt, hogyan illesztették be az emberi döntéshozók a saját ítélőképességükbe. A műszaki menedzser legnagyobb kockázata ma „nem az, hogy nincs elég adata — hanem hogy túl sok, túl kifinomult, túl »objektívnek tűnő« adata van, és emiatt hajlamos lemondani a saját szakmai ítélőképességéről.”

## Fogalmak és definíciók (HU – EN)

- **OLAP alapműveletek** — slice, dice, drill-down, roll-up; a tananyag szerint „az OLAP nem technika, hanem **gondolkodásmód**” — a képesség, hogy a vezető folyamatosan új kérdéseket tegyen fel az adatnak; „nem technika, hanem nyomozás” (3. fej.).
- **Slice (szeletelés)** — egy dimenzió kimetszése az adatkockából (pl. csak „selejt”, adott hónapra).
- **Dice (kockázás)** — több dimenzió egyszerre szűrése (gyártósor + műszak + termékcsalád).
- **Drill-down (lefúrás)** — havi összesítésről napi, majd műszakos szintre.
- **Roll-up (összesítés)** — visszalépés magasabb szintre (más gyártósorokon is jelentkezik-e).
- **KDD — Knowledge Discovery in Databases** — Fayyad, Piatetsky-Shapiro és Smyth (**1996**); az adatbányászat „receptje”; öt lépés (4. fej.).
- **GIGO — „Garbage In, Garbage Out” (szemét be, szemét ki)** — hibás/hiányos adatból a legkifinomultabb algoritmus is hibás mintázatot „fedez fel” (4. fej.).
- **CRISP-DM** — a KDD „ipari szabvány-változata” (a kőbánya-esettanulmány módszertana; Chapman et al. 2000) (6. fej.). (A tananyag kötelező része ennél többet nem mond róla.)
- **Társításelemzés (Association Rule Mining)** — „mi vásárlódik/fordul elő együtt?”; Support, Confidence, Elvárt konfidencia, Lift (5. fej.).
- **Support** — az együttes előfordulás aránya az összes ügyfélhez képest.
- **Confidence (konfidencia)** — feltételes arány: ha valakinek van C-je, mekkora eséllyel van S-e.
- **Lift** — Confidence ÷ Elvárt konfidencia; **Lift < 1** → a kapcsolat nem erősebb, mint a véletlen egybeesés.
- **Osztályozás (Classification)** — ismert kimenetelű adathalmazból tanult modell, amely új, ismeretlen eseteknél előre jelzi a kimenetelt (churn) (5. fej.).
- **Döntési fa (CART)** — a maláj telekom churn-kutatás algoritmusa (Mustafa et al., 2021) (5. fej.).
- **NPS** — ügyfél-elégedettségi mutató, a churn-modell egyik kulcstényezője (NPS-pontszám trendje) (5. fej.).
- **Csalásdetektálás (Fraud Detection)** — a szokásos mintázattól való eltérést keresi: nem azt tanulja, „milyen egy csalás”, hanem „milyen a normális”, és onnan jelzi az anomáliát; rokon a Power BI Anomaly Detectionnel (6. fej.).
- **Keresletelőrejelzés** — nem egyetlen jövőbeli szám „megjóslása”, hanem történeti mintázatok alapján valószínűségi becslés (6. fej.).
- **Ajánlórendszer — tételalapú kollaboratív szűrés (item-based collaborative filtering)** — Amazon: nem „kihez hasonlítasz te”, hanem „mely termékeket vásárolják gyakran együtt mások” — a társításelemzés kereskedelmi alkalmazása (6. fej.).
- **Hitelbírálat / Scoring (Credit Scoring)** — korábbi hiteltörténet, jövedelmi és egyéb adatok → jövőbeli fizetési hajlandóság becslése (6. fej.).
- **Hamis pozitív / hamis negatív (false positive / false negative)** — a prediktív modell sosem 100 % pontos; Target: 100 megjelölt nőből 60 valóban terhes → 40 hamis pozitív = „valódi emberi kellemetlenség vagy kár” (7. fej.). (Ábra: confusion mátrix.)

## Modellek és keretek

### A) OLAP-nyomozás négy lépése — selejt-forgatókönyv (7. ea. 3. fej., Laudon Ch.6)
Kiinduló kérdés: „Miért nőtt a selejtarány a múlt hónapban?”
1. **Slice** — csak a „selejt” dimenzió, adott hónap: a selejtarány **3 %-ról 5 %-ra** nőtt.
2. **Dice** — gyártósor + műszak + termékcsalád kombinációja a kör szűkítésére.
3. **Drill-down** — havi → napi → műszakos: a növekedés túlnyomó része a **hétvégi éjszakai műszakra** koncentrálódik.
4. **Roll-up** — vissza magasabb szintre: más gyártósorokon is jelentkezik-e, vagy csak egy gépnél.
Elv: „minden OLAP-művelet egy-egy miért-kérdésre ad választ, és minden válasz egy újabb kérdést nyit meg” — szemben a statikus riporttal. **Korlát:** az OLAP megmondja, **hol** a probléma, de nem azt, **miért** pont ott → statisztikai/adatbányászati elemzés kell.

### B) KDD-folyamat öt lépése (Fayyad et al. 1996; 7. ea. 4. fej.) — sorrendben
1. **Kiválasztás (Selection)** — melyik adatforrásból, mely adatok?
2. **Előfeldolgozás (Preprocessing)** — hiányzó, hibás, duplikált adatok kezelése
3. **Transzformáció (Transformation)** — az algoritmus által feldolgozható formára hozás
4. **Adatbányászat (Data Mining)** — az algoritmus futtatása (osztályozás, csoportosítás, társításelemzés stb.)
5. **Kiértékelés/interpretáció** — üzleti értelmezés: valódi felismerés vagy statisztikai véletlen?
**Kulcstanulság:** az öt lépésből **három (1–3) az adat előkészítése**, és csak a 4. a „bányászat” — amit a köznyelv az egész folyamattal azonosít.
- Gartner (Laudon Ch.6): a nagyvállalatok adatbázisaiban a kritikus adatok **több mint 25 %-a** pontatlan vagy hiányos.
- Press (2016, Forbes): az adatelemzők idejük **kb. 80 %-át** adat-előkészítéssel töltik.
- **AI az adatmenedzsmentben** (Laudon 18. kiad.): osztályozás, katalogizálás, adatminőség-javítás, biztonság, adatintegráció és -elemzés → a KDD 1–3. lépése egyre inkább AI-támogatott — de ez **nem szünteti meg a GIGO-elvet, csak áthelyezi**: az adatminőséget javító AI-eszköz maga mennyire megbízható?

### C) Adatbányászat I. — társításelemzés és osztályozás (7. ea. 5. fej.) — lásd Számítások
- **Osztályozás — churn:** Mustafa et al. (2021, F1000Research), maláj telekomcég, valós NPS-adatok, **CART döntési fa**, **98 %-os pontosság**; kulcstényezők: **panaszkezelési idő** és az **NPS-pontszám trendje**. Gyártóknak: ugyanaz az osztályozási logika gépmeghibásodás-előrejelzésre — „melyik gép fog meghibásodni” — más címke.

### D) Adatbányászat II. — négy további alkalmazás (7. ea. 6. fej.)
1. **Csalásdetektálás** — anomália a „normálistól”.
2. **Keresletelőrejelzés** — kőbányavállalat esettanulmány: CRISP-DM-mel **öt algoritmus** összehasonlítása (döntési fa, neurális háló, random forest, naiv Bayes, logisztikus regresszió) a gyártási késések előrejelzésére → **„nincs egyetlen legjobb algoritmus”**, a modellválasztás az adatstruktúrától és az üzleti kérdéstől függ.
3. **Ajánlórendszer** — Amazon item-based collaborative filtering.
4. **Hitelbírálat/scoring** — ZEAL Network (korábban **Tipp24 AG**): prediktív modellek ügyfélszegmensek viselkedésére, beleértve, mely inaktív ügyfelek térnek vissza (Laudon Ch.12).
Az adatbányászat fő üzleti alkalmazási területei összesen (tanulási eredmények): társításelemzés, osztályozás, csalásdetektálás, keresletelőrejelzés, ajánlórendszer, hitelbírálat — **6 terület**.

### E) Target-eset (2012; 7. ea. 7. fej.)
- Egy amerikai férfi berontott egy Target áruházba, mert középiskolás lánya terhesség-témájú kuponokat kapott postán; néhány nap múlva bocsánatot kért — a lánya valóban terhes volt. Az algoritmus a vásárlási mintázatokból (**illatmentes testápoló, bizonyos vitaminkészítmények, nagyméretű táskák**) hamarabb jött rá, mint az apa.
- Két kritikus kérdés: **(1) hamis pozitív/negatív arányok** (100 → 60 valódi, 40 téves, kínos, károkozó); **(2) etikai határ — mit szabad megjósolni, még ha lehet is?** A Target jogszabályt nem sértett (nyilvánosan hozzáférhető vásárlási adatok), de kérdés a legitim üzleti érdek; a Target végül a terhességi kuponokat semleges termékek közé „keverte”.
- Előremutatás a **11. fejezetre** (etika, felelős AI): ugyanez a dilemma AI-alapú felvételi vagy hitelbírálati algoritmusoknál, nagyobb téttel.

## Számok, dátumok, nevek, amiket a tananyag kiemel

| Mi | Érték | Hol |
|---|---|---|
| Tokola, Gröger, Järvenpää, Niemi | 2016, Procedia CIRP 57, 619–624 | 2. fej. |
| Dashboard-szerepkörök | műszakvezető, üzemvezető, felső vezetés | 2. fej. |
| OLAP műveletek | 4: slice, dice, drill-down, roll-up | 3. fej. |
| Selejtarány a példában | 3 % → 5 %; hétvégi éjszakai műszak | 3. fej. |
| KDD | Fayyad, Piatetsky-Shapiro, Smyth 1996; 5 lépés; AI Magazine 17(3) | 4., 9. fej. |
| Gartner: pontatlan kritikus adat | > 25 % | 4. fej. |
| Press 2016, Forbes | elemzők idejének ~80 %-a adat-előkészítés | 4. fej. |
| Bank-példa | 10 000 ügyfél; 6000 C; 5000 S; 5000 mindkettő | 5. fej. |
| Support / Confidence / Elvárt / Lift | 50 % / 83 % / 85 % / 0,98 | 5. fej. |
| Mustafa et al. | 2021, F1000Research 10, 1274; Malajzia; CART; 98 % | 5., 9. fej. |
| Kőbánya-esettanulmány | CRISP-DM; 5 algoritmus | 6. fej. |
| ZEAL Network | korábban Tipp24 AG | 6. fej. |
| Target-eset | 2012; 100 → 60 valódi / 40 hamis pozitív | 7. fej. |
| CRISP-DM 1.0 | Chapman et al. 2000, SPSS | 9. fej. |

## Számítások — társításelemzés: Support, Confidence, Lift (7. ea. 5. fej.)

**Adatok (a tananyag bank-példája, MIS_BIG_DATA.pdf):** 10 000 ügyfél; 6000-nek folyószámla (**C**); 5000-nek megtakarítási számla (**S**); 5000-nek mindkettő.

**Képletek (a tananyag számaiból):**
- **Support(S és C)** = (mindkettővel rendelkezők) / (összes ügyfél) = 5000 / 10 000 = **50 %**
- **Confidence(C → S)** = (mindkettő) / (C-vel rendelkezők) = 5000 / 6000 = **83 %** — „ha valakinek van folyószámlája, 83 % eséllyel van megtakarítási számlája is”
- **Elvárt konfidencia** (ha a két termék független lenne) = **85 %** (a tananyag így adja meg)
- **Lift** = Confidence / Elvárt konfidencia = 0,83 / 0,85 = **0,98**

**Értelmezés (a tananyag kulcsmondata):** mivel a Lift **kisebb, mint 1**, a két termék együttes birtoklása „valójában nem erősebb kapcsolat, mint amit a véletlen egybeesés önmagában indokolna — annak ellenére, hogy a 83 %-os konfidencia önmagában lenyűgözőnek tűnik.” → **A magas konfidencia félrevezető lehet, ha nem vetjük össze az elvárt (véletlenszerű) aránnyal.**

⚠ forrásmegjegyzés: a tananyag adataiból az „elvárt konfidencia” (= S aránya az összes ügyfél között, ha független) 5000/10 000 = 50 % lenne, nem 85 %; a 85 %-os érték a példában külön adatként szerepel, és a Lift (0,98) ebből számolódik. A ZH-n a tananyag számait kell használni: Support 50 %, Confidence 83 %, Elvárt 85 %, Lift 0,98 (< 1). Ha a kérdés saját számokból kéri a liftet, az elvárt konfidencia a következmény (S) önálló aránya.

**„Mi változik, ha…” variánsok (saját számok):**
- Ha az elvárt konfidencia 60 % lenne (a S-t az ügyfelek 60 %-a birtokolja függetlenül): Lift = 0,83 / 0,60 = **1,38 > 1** → a folyószámla-birtoklás valóban növeli a megtakarítási számla valószínűségét — érdemes keresztértékesíteni.
- Ha csak 3000 ügyfélnek van mindkettő (C = 6000, S = 5000): Support = 3000/10 000 = 30 %; Confidence(C→S) = 3000/6000 = 50 %; elvárt (S aránya) = 50 % → Lift = 1,0 → pontosan független.
- Lift > 1: pozitív kapcsolat; Lift = 1: független; Lift < 1: a két termék inkább „kizárja” egymást a véletlenhez képest.

**Target hamis pozitív (7. fej.) — a tananyag számai:** 100 megjelölt, 60 valódi → precizitás 60 %, **40 hamis pozitív**. „Mi változik, ha…”: ha a modell 1 millió vásárlóra fut, és 1 %-ot jelöl meg (10 000 fő) 60 %-os találati aránnyal → 4000 nő kap téves terhességi kupont — a hamis pozitív „nem statisztikai absztrakció”.

## Összekeverhető párok / „mi NEM igaz” csapdák

1. **Tokola-kutatás: a dashboardok a döntéshozó kérdéseiből indulnak?** NEM — a rendelkezésre álló adatból; javaslat: szerepkörhöz igazított KPI-kiválasztás.
2. **Slice vs. dice:** slice = egy dimenzió; dice = több dimenzió egyszerre. **Drill-down vs. roll-up:** le részletbe / fel összesítésbe.
3. **OLAP megmondja, miért?** NEM — csak hol; a miérthez adatbányászat kell.
4. **KDD = adatbányászat?** NEM — az adatbányászat a KDD 4. lépése; 1–3. az előkészítés.
5. **KDD lépések sorrendje:** Selection → Preprocessing → Transformation → Data Mining → Interpretation.
6. **80 % vs. 25 %:** 80 % = elemzők ideje adat-előkészítésre (Press/Forbes 2016); >25 % = pontatlan kritikus adat (Gartner).
7. **AI megszünteti a GIGO-t?** NEM — áthelyezi (az AI-eszköz megbízhatósága a kérdés).
8. **Support vs. Confidence vs. Lift:** support = együttes / összes; confidence = együttes / feltétel; lift = confidence / elvárt. **Lift < 1 → nem erősebb a véletlennél**, hiába 83 % a confidence.
9. **Osztályozás vs. társításelemzés:** osztályozás = címkézett adatból tanult modell (churn, CART); társítás = együttes előfordulás.
10. **Csalásdetektálás a csalás mintáját tanulja?** NEM — a „normálist”, és az eltérést jelzi.
11. **Amazon ajánlórendszer = felhasználó-alapú?** NEM — **tételalapú** (item-based) kollaboratív szűrés = társításelemzés.
12. **Van legjobb előrejelző algoritmus?** NEM — a kőbánya-eset: adatstruktúra és üzleti kérdés dönt.
13. **Target jogszabályt sértett?** NEM — a kérdés etikai (legitim érdek, felhasználás).
14. **Target vs. Target Canada (3. ea.):** itt a terhesség-előrejelző algoritmus (2012, etika); ott az SAP-bevezetés kudarca (2013–2015).
15. **CRISP-DM vs. KDD:** CRISP-DM = a KDD ipari szabvány-változata (Chapman et al. 2000).
16. **ZEAL Network** = Tipp24 AG; megjelenik az 5. ea.-ban (preskriptív analitika) és itt (hitelbírálaton túli prediktív modell).
17. **Churn-modell pontossága 98 %** (Mustafa) — ne keverd a 90 %-kal (OTP kategorizálás, 5. ea.).

## Kapcsolat más előadásokkal

- 6. ea. Goodhart/OEE/BSC/Tufte → közös ív; Anomaly Detection ↔ csalásdetektálás; 22 KPI ↔ Tokola.
- OLAP (4. ea. OLTP/OLAP, FASMI; adattárház) ↔ OLAP-nyomozás.
- GIGO ↔ 4. ea. adatminőség (Knight Capital, DIKW adat→információ), 5. ea. hét dimenzió.
- Churn, CLTV (3. ea. CRM analytical) ↔ osztályozás churn-előrejelzésre; Amazon ajánlórendszer (1., 2. ea.).
- Preskriptív/prediktív analitika, ZEAL (5. ea.).
- Target-eset → 11. ea. etika, felelős AI (a tananyag kifejezetten előreutal); hamis pozitív/negatív.
- AI az adatmenedzsmentben, Big Data ↔ AI → 8. ea.
- Bosch Hatvan, Siemens Amberg (4. ea.) ↔ szintézis: a technológia nem hoz automatikusan jobb döntést (1. ea. komplementer eszközök).
- Kitekintés: felhő alapú BI (10. ea.), AI és etikus algoritmustervezés (11. ea.).

## Fogalomtár-jelöltek

- **Szeletelés** – slice – egy dimenzió kimetszése az adatkockából.
- **Kockázás** – dice – több dimenzió egyidejű szűrése.
- **Lefúrás** – drill-down – részletesebb szintre lépés.
- **Összesítés** – roll-up – magasabb aggregációs szintre lépés.
- **Tudásfeltárás adatbázisokból** – KDD – Fayyad et al. 1996 ötlépéses folyamata.
- **Szemét be, szemét ki** – GIGO – rossz bemenet → rossz mintázat, bármilyen jó az algoritmus.
- **CRISP-DM** – CRISP-DM – a KDD ipari szabvány-változata.
- **Társításelemzés** – association rule mining – együttes előfordulások feltárása (support, confidence, lift).
- **Támogatottság** – support – együttes előfordulás aránya az összes esetben.
- **Konfidencia** – confidence – feltételes arány (ha A, akkor B).
- **Lift** – lift – confidence / elvárt konfidencia; < 1 nem erősebb a véletlennél.
- **Osztályozás** – classification – címkézett adatból tanult modell ismeretlen esetek besorolására.
- **Döntési fa** – decision tree (CART) – kérdéssorozat alapján osztályoz (churn-példa).
- **Csalásdetektálás** – fraud detection – a normális mintázattól való eltérés jelzése.
- **Tételalapú kollaboratív szűrés** – item-based collaborative filtering – Amazon ajánlórendszer.
- **Hitelbírálat** – credit scoring – fizetési hajlandóság becslése hiteltörténetből.
- **Hamis pozitív** – false positive – tévesen pozitívnak jelölt eset (Target: 40/100).

---

# 8. előadás: Big Data — hogyan nyerjünk belőle valódi értéket?

## Egy mondatban (a központi tézis)

A Big Data **nem informatikai projekt, hanem szervezeti-stratégiai döntés**: a projektek 60–85 %-a nem a technológia, hanem a szervezeti kultúra, a hiányzó üzleti kérdés („miért?”) és a gyenge adat-governance miatt bukik el; az AI felerősíti a jó adatstratégiát — és a rosszat is (8. ea. 2., 4., 5., 10. fej.).

## Nyitó eset és feloldása (8. ea. 2., 4. és 10. fej.)

**Nyitó dilemma:** Ön középvállalati IT-vezető; a vezérigazgató: „A versenytársaink Big Data-ba fektetnek. Nekünk is lépnünk kell… mennyi idő alatt tudunk platformot választani?” Opciók: **A)** piaci Big Data-platformok felmérése, rövid lista; **B)** visszakérdez: „Milyen konkrét üzleti problémát oldana meg ez?” — csak utána technológia; **C)** külső tanácsadó cég a teljes projektre. **Helyes irány: B.** (4. fej.: „Ha az A) opciót választotta — azonnal technológiai szállítót keresni —, érdemes újragondolni: a GE pontosan ezt tette, és ez volt az egyik fő bukási ok.”)

**A tét — bukási statisztikák (2. fej.):**
| Adat | Érték |
|---|---|
| 2015-ös elemzői előrejelzés (Gartner, BI & Analytics Summit) | a Big Data-projektek **60 %-a** nem jut túl a pilot fázison — fő ok: régi gondolkodásmód és szervezeti kultúra |
| 2017-es felülvizsgálat | valós bukási arány közelebb **85 %-hoz**; „a probléma nem a technológia” — üzleti folyamatokba illesztés, vezetői ellenállás, belső politika, szakemberhiány, hiányos adat-governance |
| NewVantage Partners felmérés | a cégek **85 %-a** indított adatvezérelt kultúra-programot, de csak **37 %** számolt be sikerről |

**A gerinc-eset: GE és a Predix (4. fej.) — „egy zászlóshajó-projekt két olvasata”.**
- **Első olvasat (2016 siker-narratíva):** a GE (repülőgép-hajtóművek, mozdonyok, erőművi turbinák) szoftvercéggé akart alakulni; a **Predix** ipari IoT-alapú felhőszolgáltatás: szenzoradatok (hőmérséklet, vibráció, nyomás, fordulatszám) → meghibásodás-előrejelzés, karbantartás-optimalizálás. Cél: **2020-ra a top 10 amerikai szoftvercég**, évi több milliárd USD bevétel.
- **Második olvasat (idővonal):** 2013–2014 Predix indul saját felhő-adatközponttal → 2016 csúcs-narratíva (GE Digital) → 2018–2019 bevételi célok elmaradnak, digitális üzletág leépítése → **2024 a GE konglomerátum szétválik** (a Predix-kudarc is szerepet játszott). Befektetés: **több mint 7 milliárd USD**.
- **Három bukási ok (stratégiai és kulturális, nem technikai):** 1. **Saját infrastruktúra-építés versenyhelyzetben** (saját felhő-adatközpont Amazon/Microsoft/Google helyett — verseny a nagyobb tech-cégekkel); 2. **Univerzális platform diffúz stratégiával** (repülőgépgyártás, energia, egészségügy egy platformon — szélturbina vs. MRI); 3. **Termékközpontú, nem szolgáltatásközpontú szemlélet** (fejlesztői közösség, UX, iterációs sebesség hiánya).
- **Tanulság:** nem elég a technológiai képesség és a tőke — fókuszált, saját szakértelemre épülő stratégia és tényleges kultúraváltás kell. A 6. fej. szerint hibrid, edge-alapú architektúrával elkerülhető lett volna a saját centralizált adatközpont építése.

**Feloldás (10. fej.):** „A Big Data-projektek sikere és kudarca nem a technológián, hanem a szervezeti gondolkodáson múlik.” Az AI és az edge computing bővíti az eszköztárat, „de egyik sem old meg egy rosszul definiált üzleti problémát vagy egy adatellenes szervezeti kultúrát. Az AI felerősíti a jó adatstratégiát, és felerősíti a rosszat is.”

## Fogalmak és definíciók (HU – EN)

- **Big Data döntési logika (McAfee & Brynjolfsson, 2012, HBR 90(10), 60–68)** — a kérdés nem „van-e elég adatunk, hogy Big Data-nak nevezzük”, hanem hogy a probléma jellege igényli-e a **nagy volumenű, nagy sebességű vagy nagy változatosságú** adatok kezelését; sok cég a „Big Data” presztízse miatt épít drága infrastruktúrát „kis” adatelemzéssel megoldható problémákra (3. fej.).
- **Build / Buy / Outsource** — lásd Modellek A).
- **GIGO a Big Data-ban** — élesebb, mint a hagyományos BI-nál (volumen és változatosság miatt nehezebb a tisztítás); elemzők idejének **50–80 %-a** adattisztítás/előkészítés → **erőforrás-allokációs menedzseri döntés** (3. fej.).
- **Vendor lock-in** — a Buy opció fő kockázata (3. fej.).
- **Predix** — a GE ipari IoT-alapú felhőplatformja (4. fej.).
- **Big Data ↔ AI kölcsönös kapcsolat** — „Ki kinek a tápláléka?”: az AI-nak Big Data kell (a Big Data az AI „üzemanyaga”); a Big Data-nak AI kell (a gépi tanulás mintázatot ismer fel ott, ahol az ember zajt lát) (5. fej.).
- **Edge computing (peremhálózati számítás)** — az adatfeldolgozás egy része nem a távoli felhőszerveren, hanem közvetlenül a berendezés mellett, helyben történik (6. fej.).
- **Hibrid architektúra (edge + fog + cloud)** — edge: valós idejű szűrés/riasztás; felhő: hosszú távú komplex elemzés, modelltanítás; a sikeres prediktív karbantartási rendszerek réteges architektúrát használnak (6. fej.).
- **Small Data vs. Big Data — okság vs. korreláció** — hagyományos statisztika: kevés, pontos adat, oksági összefüggés („miért”); Big Data: kusza, hatalmas adat, korreláció („mi jár együtt mivel”) — tudatos kompromisszum (Mayer-Schönberger & Cukier, 2013) (7. fej.).
- **Adatosítás (datafication)** — egyre több, korábban nem számszerűsíthető dolog válik adattá: szavak → keresési adat; helymeghatározás → GPS-adat; emberi kapcsolatok → hálózatelemzési adat; az adat árucikk, elsődleges és másodlagos értékkel (Mayer-Schönberger & Cukier, 2013) (7. fej.).
- **Sabermetrics** — a Moneyball szisztematikus statisztikai játékosértékelése (7. fej.).
- **TCO (Ellram, 1993)** — teljes birtoklási költség; TCO-jéghegy (9. fej.).
- **ROI-számítás csapdája** — technológiai aktivitást mérő mutatók („hány terabájt naponta”) az üzleti érték helyett — rokon a Goodhart-törvénnyel (9. fej.).

## Modellek és keretek

### A) Build / Buy / Outsource döntési keret (McAfee & Brynjolfsson 2012; 8. ea. 3. fej.)
| Opció | Mikor indokolt | Fő kockázat |
|---|---|---|
| **Build** (saját fejlesztés) | az adatelemzés a versenyelőny megkülönböztető eleme | magas költség, hosszú átfutás, technológiai versenyhelyzet |
| **Buy** (kész platform) | az adatelemzés támogató funkció, nem fő tevékenység | vendor lock-in, testreszabhatóság korlátai |
| **Outsource** (kiszervezés) | gyors indulás, korlátozott belső szakértelem | függőség, adatbiztonság, a tudás nem épül be a szervezetbe |
A döntés stratégiai: az adatelemzés kritikus megkülönböztető elem vagy támogató funkció? Gyártó cég karbantartás-tervezése → kész platform/kiszervezés alacsonyabb kockázatú, gyorsabban megtérülő. (Ábra: döntési fa „hagyományos BI elég” vs. „Big Data indokolt”.) Műszaki analógia: új gyártósor — nem azért, mert lehetséges, hanem mert a volumen és a minőségi követelmény indokolja.

### B) Big Data és AI (8. ea. 5. fej.)
- Prediktív karbantartási modell egy gép néhány hónapos adatán vs. több ezer berendezés több éves adatán.
- **Mit tenne ma a generatív AI a Predix helyén?** A 2014-es koncepció (szenzoradatok, szabályalapú küszöbértékek, emberi elemzői jelentések) automatizálhatóbb: ML-modellek előre nem definiált mintázatokban is anomáliát ismernek fel; a generatív AI nyers szenzoradatból természetes nyelvű karbantartási jelentést állít össze.
- **Kritikai fenntartás:** 2018-as elemzői előrejelzés (Gartner CIO Agenda Survey): **2022-ig az AI-projektek 85 %-a** téves vagy hasznavehetetlen eredményt ad — ugyanaz a szervezeti-kulturális minta. „Az AI felerősíti a jó adatstratégia előnyeit, de nem helyettesíti azt… a hibás mintázatokat nagyobb magabiztossággal, nagyobb léptékben termeli újra.”
- **Gyors ellenőrző kérdés (a tananyagból):** rosszul kalibrált szenzorok + prediktív karbantartási AI → A) javít, B) **ront — nagyobb magabiztossággal és léptékben termeli újra a hibás mintázatokat**, C) nincs hatás. **Helyes: B.**

### C) Edge vs. felhő (8. ea. 6. fej., Achouch et al. 2022)
| Architektúra | Jellemző válaszidő | Mire alkalmas |
|---|---|---|
| **Felhő (cloud)** | ~100–500 ezredmásodperc | hosszú távú, komplex elemzés, modell-tanítás |
| **Edge (gép melletti)** | egyszámjegyű – alacsony kétjegyű ezredmásodperc | azonnali riasztás, kritikus beavatkozás |
- Turbina csapágyhibája másodperceken belül → a 100–500 ms-os felhő-riasztás elkésett.
- Nem „vagy-vagy”, hanem hibrid (edge, fog, felhő).
- Edge = **stratégiai kockázatcsökkentés**: kevesebb függés a centralizált infrastruktúrától, alacsonyabb sávszélesség-költség, működőképesség hálózati kimaradáskor. Analógia: minőségellenőrzés a gép mellett, nem a központi irodában.
- Reflektív példa: magyar KKV 15 régi CNC-géppel — edge vagy felhő?

### D) Adatosítás — három példa három világból (8. ea. 7. fej.)
1. **Moneyball** — Lewis 2003-as könyv, 2011-es film (Miller, Columbia Pictures); **Oakland Athletics**, korlátozott költségvetés; scoutok megérzése helyett **sabermetrics**; lényeg: **szervezeti ellenállás** — a tapasztalt szakemberek elutasították, mert az adat szembement a szakértői tapasztalattal.
2. **Zara** (Inditex; HBS Case 604-081, McAfee, Dessain & Sjoman 2007) — előre tervező divatlogika helyett **valós idejű adatvisszacsatolási hurok**; a boltvezetők kézi eszközökkel rögzítik, mit próbálnak fel és nem vesznek meg — „maguk is adatgyűjtővé válnak”.
3. **Tesco Clubcard** — **1995**, az Egyesült Királyság első nagy áruházlánci lojalitásprogramja; **Lord MacLaurin** (elnök): „három hónap alatt többet tudtok meg a vásárlóimról, mint én harminc év alatt” (Emerald Publishing 2004, interjú Clive Humbyval); a hűségkártya nem jutalmazási eszköz, hanem **adatgyűjtő infrastruktúra**.
**Közös tanulság:** „az adat nem attól válik értékessé, hogy sok van belőle, hanem attól, hogy egy korábban megérzés-alapú döntést szisztematikussá és megismételhetővé tesz.”

### E) Az adatvezérelt szervezet érettségi modellje — négy lépés (Davenport & Harris 2007/2017 nyomán, leegyszerűsítve; 8. ea. 8. fej.)
| Lépés | Jellemző | Kapcsolódó eset |
|---|---|---|
| 1. Szórványos kísérletezés | izolált próbálkozások, nincs vezetői mandátum | a legtöbb elbukó projekt |
| 2. Technológiai befektetés mandátum nélkül | megvan a technológia, hiányzik a „miért” | **GE/Predix** |
| 3. Adatvezérelt döntés egy területen | mérhető eredmény egy konkrét problémán | Moneyball, Zara, Tesco |
| 4. Szervezeti kultúra átalakítása | adatvezérelt döntés az alapértelmezett elvárás | BICC-érettség (5. fejezet) |
Magyar kontextus: egy hazai közepes gyártó tipikusan a **2–3. lépés között**; KKV-nak nem kell egyből a 4.-re ugrani — a 3. lépés (jól kiválasztott pilot-terület) a reális belépési pont. Analógia: minőségbiztosítási rendszer bevezetése.

### F) Big Data ROI és TCO (Ellram 1993; 8. ea. 9. fej.)
| TCO-elem | Miért marad figyelmen kívül |
|---|---|
| Adatmérnöki/adatelemzői létszám | az 50–80 %-os adattisztítási arány rejtve marad a licenc-árban |
| Integráció a meglévő rendszerekkel | a valós mérték csak bevezetés közben derül ki |
| Stratégiai lehetőségköltség | GE/Predix: a rossz irányba fektetett erőforrás máshol hiányzik |
- **Helyes logika (fordított):** először a konkrét üzleti döntés, amit a Big Data jobbá tehet → utána mennyit ér pénzben.
- **Mikor NEM éri meg:** ha nem tudják megfogalmazni, milyen rosszul meghozott döntést javítana → ROI légből kapott; ha a probléma mérete nem indokolja → a TCO szinte garantáltan meghaladja a hasznot.
- „A versenytárs már bevezette” — önmagában nem indoklás pozitív ROI-hoz.

## Számok, dátumok, nevek, amiket a tananyag kiemel

| Mi | Érték | Hol |
|---|---|---|
| Big Data pilot-bukás | 60 % (2015, Gartner) → 85 % (2017 felülvizsgálat) | 2. fej. |
| NewVantage Partners | 85 % indított kultúra-programot; 37 % siker | 2. fej. |
| McAfee & Brynjolfsson | 2012, HBR 90(10), 60–68 „Big Data: The management revolution” | 2–3. fej. |
| Adattisztítás aránya | 50–80 % az elemzők idejéből | 3., 9. fej. |
| GE Predix célja | 2020-ra top 10 amerikai szoftvercég | 4. fej. |
| Predix idővonal | 2013–14 indul; 2016 csúcs; 2018–19 leépítés; 2024 GE szétválik | 4. fej. |
| Predix befektetés | > 7 Mrd USD | 4. fej. |
| Bukási okok | 3 (saját infrastruktúra; univerzális platform; termékközpontú szemlélet) | 4. fej. |
| AI-projektek téves eredménye | 85 % 2022-ig (2018-as Gartner CIO Agenda Survey) | 5. fej. |
| Felhő válaszidő | ~100–500 ms | 6. fej. |
| Edge válaszidő | egyszámjegyű – alacsony kétjegyű ms | 6. fej. |
| Achouch et al. | 2022, Applied Sciences 12(16), 8081 | 6., 11. fej. |
| Mayer-Schönberger & Cukier | 2013 | 7. fej. |
| Moneyball | könyv 2003 (Lewis), film 2011 (Miller); Oakland Athletics | 7. fej. |
| Zara HBS case | 604-081 (McAfee, Dessain, Sjoman 2007) | 7. fej. |
| Tesco Clubcard | 1995; Lord MacLaurin; „3 hónap vs. 30 év”; Clive Humby interjú 2004 | 7. fej. |
| Érettségi modell | 4 lépés; Davenport & Harris 2007/2017 | 8. fej. |
| Magyar gyártó | 2–3. lépés között | 8. fej. |
| Ellram TCO | 1993, Int. J. Purchasing and Materials Management 29(4), 3–11 | 9. fej. |
| Elmélyítő: Fodor & Kosztyi | 2020, dBEM, Óbudai Egyetem | 11. fej. |

## Számítások — Big Data ROI és TCO (8. ea. 9. fej.)

A tananyag képletet nem ad; a ROI és TCO fogalmát az 1. ea. 7. fej. definíciói szerint használja (ROI = nyereség / beruházási költség; TCO = a vételáron túli összes költség). **Mintapélda saját számokkal, a tananyag arányaival:**

- Big Data platform licenc + hardver: **40 M Ft/év** (ez a „látható” költség).
- Rejtett TCO-elemek (9. fej. táblázata): adatmérnöki létszám — ha 2 elemző évi 24 M Ft bérrel, és idejük 50–80 %-a tisztítás, akkor **24–38 M Ft/év** „rejtett” tisztítási költség; integráció a meglévő rendszerekkel: **30 M Ft** egyszeri; stratégiai lehetőségköltség: nehezen számszerűsíthető (GE: „máshol hiányzik”).
- **TCO (1. év) ≈ 40 + 48 + 30 = 118 M Ft** (teljes elemzői bér beszámítva), amiből a licenc csak ~34 % — összhangban az 1. ea. TCO-jéghegyével (vételár ~20 %).
- **ROI:** ha az azonosított üzleti döntés (pl. prediktív karbantartással elkerült állásidő) **évi 150 M Ft** hasznot hoz: ROI = (150 − 118) / 118 = **+27 %**. Ha csak a licencet nézik: (150 − 40)/40 = 275 % — **a TCO figyelmen kívül hagyása tízszeresen túlbecsüli a megtérülést**.
- **„Mi változik, ha…”**: ha nincs azonosítható üzleti döntés (csak „terabájt/nap” aktivitás-mutató), a haszon-oldal 0 → ROI = −100 % — „a ROI-számítás eleve légből kapott”. Ha a probléma hagyományos BI-val (pl. 10 M Ft/év) megoldható, a Big Data TCO (118 M) „szinte garantáltan meghaladja a realizálható hasznot”.
- **GE/Predix nagyságrend (a tananyag számai):** > 7 Mrd USD befektetés, a bevételi célok elmaradtak → negatív megtérülés + lehetőségköltség (a konglomerátum 2024-es szétválásában is szerepet játszott).

## Összekeverhető párok / „mi NEM igaz” csapdák

1. **Nyitó dilemma: A (platformlista) a helyes?** NEM — B (üzleti probléma előbb); a GE az A-t tette.
2. **60 % vs. 85 % vs. 85 % vs. 37 %:** 60 % = 2015 pilot-bukás; 85 % = 2017 felülvizsgált bukás ÉS 2018-as AI-előrejelzés (85 % téves eredmény) ÉS NewVantage (85 % indított programot); 37 % = siker.
3. **A Big Data-bukás oka a technológia?** NEM — szervezeti kultúra, folyamatba illesztés, vezetői ellenállás, belső politika, szakemberhiány, governance.
4. **Build vs. Buy vs. Outsource:** build = versenyelőny-elem (magas költség); buy = támogató funkció (lock-in); outsource = gyors indulás (függőség, tudás nem épül be). Vö. 3. ea. build/buy/cloud/best-of-breed — itt **outsource** a harmadik, nincs best-of-breed.
5. **Predix bukási okok:** saját adatközpont (nem AWS/Azure/Google); univerzális platform; termék- nem szolgáltatásközpontú. NEM technikai hiba.
6. **GE 2024:** a konglomerátum **szétválik** — nem csődbe ment (a tananyag ezt nem állítja).
7. **AI kiszűri a rossz szenzoradatot?** NEM — B: ront, nagyobb léptékben termeli újra.
8. **Edge vs. cloud válaszidő:** edge = ms egyszámjegyű–alacsony kétjegyű; cloud = 100–500 ms. Edge = riasztás/beavatkozás; cloud = komplex elemzés, modelltanítás. Nem „vagy-vagy” — hibrid (edge, fog, cloud).
9. **Small Data = okság; Big Data = korreláció** — Big Data gyakran nem tudja, „miért”, de a megbízható korreláció elég lehet.
10. **Moneyball tanulsága = a statisztika jobb?** A tananyag kiemelt lényege: a **szervezeti ellenállás**.
11. **Tesco Clubcard = jutalmazás?** NEM — adatgyűjtő infrastruktúra; 1995, UK első nagy áruházlánci programja.
12. **Zara: a tervezők döntenek előre?** NEM — valós idejű visszacsatolás; a boltvezetők adatgyűjtők.
13. **Érettségi modell 4 lépése és példái:** 1. szórványos (elbukó projektek); 2. technológia mandátum nélkül (**GE**); 3. egy terület (**Moneyball, Zara, Tesco**); 4. kultúra (**BICC**). KKV: 3. lépés a belépő, nem a 4.
14. **ROI-mutató: „terabájt/nap”?** NEM — technológiai aktivitás, Goodhart-csapda; előbb az üzleti döntés.
15. **TCO rejtett elemei itt:** adatmérnöki létszám; integráció; lehetőségköltség — nem azonos az 1. ea. 7 tételével (telepítés, képzés…).
16. **Ellram 1993 (TCO)** vs. **McAfee–Brynjolfsson 2012 (Big Data management revolution)** vs. **Mayer-Schönberger–Cukier 2013 (adatosítás)** vs. **Davenport–Harris 2007/2017 (Competing on analytics)**.

## Kapcsolat más előadásokkal

- Komplementer eszközök, „technológia nem elég”, TCO 20/80, ROI (1. ea.) ↔ Big Data bukás, TCO-jéghegy.
- Build/buy/cloud/best-of-breed (3. ea.) ↔ build/buy/outsource.
- GIGO, KDD, 80 % adat-előkészítés (7. ea.) ↔ 50–80 % adattisztítás mint erőforrás-döntés.
- GE Predix (6. ea. 7. fej. — pozitív olvasat: flottaadat, Közel-Kelet/Kína) ↔ itt a második olvasat (kudarc). **Csapda:** a 6. ea. sikerpéldaként, a 8. ea. figyelmeztető példaként használja ugyanazt az esetet.
- BICC-érettség (5. ea.) = az adatvezérelt szervezet 4. lépése; Goodhart (6. ea.) ↔ ROI-csapda.
- Big Data ↔ AI kölcsönhatás (4. ea. előreutalás).
- Edge/fog/cloud, saját adatközpont vs. felhőszolgáltató → 10. ea. felhő; Tesco Clubcard (2. ea. lojalitás, váltási költség); Moneyball szervezeti ellenállás (1. ea.).
- Kitekintés (10. fej.): „a következő fejezetben (9.) a Tudásmenedzsment és intelligens szervezet” — a Moodle 9. előadás valóban ez.

## Fogalomtár-jelöltek

- **Big Data** – big data – nagy volumenű, sebességű, változatosságú adat; szervezeti-stratégiai döntés, nem IT-projekt.
- **Saját fejlesztés / kész platform / kiszervezés** – build / buy / outsource – a Big Data-képesség beszerzésének három útja.
- **Szállítói bezártság** – vendor lock-in – a kész platform fő kockázata.
- **Predix** – Predix – a GE ipari IoT felhőplatformja (2013–2024), > 7 Mrd USD, stratégiai kudarc.
- **Peremhálózati számítás** – edge computing – helyi, gép melletti adatfeldolgozás ms-os válaszidővel.
- **Hibrid architektúra** – edge/fog/cloud – réteges feldolgozás: edge riaszt, felhő tanít.
- **Adatosítás** – datafication – nem számszerűsíthető dolgok adattá válása (Mayer-Schönberger & Cukier 2013).
- **Okság vs. korreláció** – causation vs. correlation – small data „miért” vs. big data „mi jár együtt”.
- **Sabermetrics** – sabermetrics – Moneyball statisztikai játékosértékelése.
- **Adatvezérelt érettségi modell** – data-driven maturity – 4 lépés: kísérletezés → technológia mandátum nélkül → egy terület → kultúra.
- **Teljes birtoklási költség** – TCO (Ellram 1993) – rejtett elemek: létszám, integráció, lehetőségköltség.
- **ROI-csapda** – ROI trap – aktivitás-mutató üzleti érték helyett (Goodhart-rokon).

---

# 9. előadás: Tudásmenedzsment és intelligens szervezet

⚠ forrásmegjegyzés: az adatlapon a Tudásmenedzsment a 8. hét, a Felhő a 10. hét; a Moodle-ban a Tudásmenedzsment a 9. előadás, és a 10. fej. szerint „a következő fejezetben (10.) a Felhő és IT-infrastruktúra”. A 2. ea. 9. fej. „7. fejezetben tárgyaljuk” és a 8. ea. 10. fej. „9. fejezetre kitekintés” utalásai erre az előadásra vonatkoznak.

## Egy mondatban (a központi tézis)

A tudás **nem magától értetődően marad meg** egy szervezetben: a tacit tudás nem „leíratható”, a tárolás önmagában kevés (a megtalálhatóság a kulcs), a tudástárak kultúra és ösztönzés nélkül „temetővé” válnak, és az AI — a szabályalapú szakértői rendszerektől a RAG-alapú generatív AI-ig — egyre jobb a mintázatfelismerésben, de a **megbízhatóság és a magyarázhatóság** mindvégig központi probléma marad (9. ea. 10. fej.).

## Nyitó eset és feloldása (9. ea. 2. és 10. fej.)

**Nyitó dilemma:** Ön egy repülőgép-karbantartó vállalat üzemvezetője; idén **öt**, egyenként **25+ éves** tapasztalatú mérnök vonul nyugdíjba egyszerre.
| Adat | Érték |
|---|---|
| Repülőgép-karbantartó technikusok átlagéletkora (pandémia előtt) | **57 év** |
| ATEC (Aviation Technician Education Council) 2022 Pipeline report | a pandémia legalább **5000** új mechanikustól fosztotta meg az iparágat |
| Másik felmérés (JMC Recruitment Solutions; idézi Vitrek 2024, Saxon Aerospace 2024) | a légiközlekedési mérnökök **38 %-a** elhagyta az iparágat, **4 %** korai nyugdíjazást választott |

Opciók: **A)** megköszöni, bízik, hogy az utódok „belejönnek”; **B)** szisztematikusan dokumentáltatja a diagnosztikai tudást az utolsó hónapokban; **C)** külső tanácsadó „tudásátadási workshopot” szervez.

**Feloldás a tananyag érvelése alapján** (⚠ a tananyag nem jelöl ki egyetlen „helyes” betűt, hanem mindhárom korlátját mutatja meg): A = a probléma tudomásulvétele cselekvés nélkül; B korlátja (3. fej.): aki azt hiszi, a tacit tudás „dokumentálható”, és megkéri a kilépőt, „írja le, amit tud”, csalódni fog — a dokumentum az explicit réteget rögzíti, a tapasztalati megérzés elvész; C korlátja (3. fej.): „elég egy tudásmegosztó workshopot tartani” → alábecsüli, hogy a tudás mozgatása **időt, ismételt gyakorlást és tudatos szervezeti erőfeszítést** igényel, nem egyszeri eseményt. Ami működött volna: **évekkel korábban szakértő-kereső rendszer** (4. fej.: célzott tervezés, ki kitől mit vesz át), **digitális iker** (5. fej.: a megérzés küszöbértékként beépül a modellbe), a tudás négylépéses mozgatása közös munkával (3. fej.). Szintézis (10. fej.): „a tudás nem magától értetődően marad meg… ehhez tudatos, szisztematikus erőfeszítés kell, és ez jóval túlmutat az egyszerű dokumentáláson.”

**Hazai kitekintés (10. fej.):** Business Fest 2026 nyitó kerekasztal — a magyar gyártóipar kritikus ponthoz ért: új gyárak jönnek, de egyre kevesebb a megfelelő tudású szakember; „nem a technológia, hanem a munkaerőhiány és a kompetenciák hiánya” a legnagyobb akadály (idézi: Piac&Profit, Pénzcentrum, ProfitLine, 2026).

## Fogalmak és definíciók (HU – EN)

- **Explicit tudás (explicit knowledge)** — kifejezett, dokumentált; könnyen leírható: karbantartási kézikönyv, szabványeljárás, adatbázis-bejegyzés (3. fej.).
- **Tacit tudás (tacit knowledge)** — hallgatólagos, nem megfogalmazott; amit a tapasztalt mérnök „megérez” — nyelvi eszközökkel nehezen vagy egyáltalán nem ragadható meg (szokatlan zajminta, rezgés „furcsasága”) (Laudon & Laudon 2018, 11. fej.).
- **A tudás mozgásának négy lépése** — megosztás → explicitté tétel → kombinálás → elsajátítás (3. fej.); a tananyag szerint „egy jól ismert, klasszikus tudásmenedzsment-modell logikáját követi”, amelynek neve és négykvadránsos mátrixa az Opcionális Könyvben van (Nonaka & Takeuchi 1995 a forrásjegyzékben) — a kötelező anyag csak a négy lépést adja meg.
- **Tudásmenedzsment-értéklánc (KM value chain)** — Laudon & Laudon 2018: megszerzés, tárolás, terjesztés, alkalmazás (4. fej.).
- **Szakértő-kereső rendszer** — nem a tudást tárolja, hanem azt segít megtalálni, **ki tudja** az adott dolgot a szervezetben („keresse meg X mérnököt”); realistább cél, mint a tacit tudás teljes explicitté tétele (4. fej.).
- **Tudásmunka-rendszerek (Knowledge Work Systems, KWS)** — mérnökök, tudósok, tudásmunkások számára, új tudás létrehozására és alkalmazására; három releváns típus: **CAD, VR/AR, digitális iker** (5. fej.).
- **Digitális iker (digital twin)** — Michael Grieves, 2000-es évek eleje; egy fizikai eszköz folyamatosan szinkronizált virtuális mása, amely valós idejű szenzoradatok alapján tükrözi az aktuális állapotot (Grieves & Vickers 2017); három emberi képességet támogat: **konceptualizáció, összehasonlítás, együttműködés** (5. fej.).
- **„SharePoint-temető”** — lelkesen elindított, majd senki által nem használt/frissített dokumentumtár (6. fej.).
- **Szervezeti felejtés (organizational forgetting)** — de Holan & Phillips (2004, Management Science 50(11)): **szándékos** (tudatosan elavultnak ítélt tudás elengedése) vs. **véletlen** (nem szándékolt, kárt okozó tudásvesztés); a véletlen felejtés évi több millió dolláros veszteséget okozhat (MIT Sloan Management Review 2004) (6. fej.).
- **Szakértői rendszer (expert system)** — szabályalapú program, szűk, jól körülhatárolt szakterületen egy emberi szakértő döntési logikáját adja vissza, jellemzően **IF-THEN** szabályokkal (7. fej.). Architektúra: felhasználói felület → **következtető motor (inference engine)** → tudásbázis.
- **Fuzzy logika** — a szabályalapú rendszer finomítása: bizonytalan, „elmosódott” kategóriák kezelése (a hőmérséklet nem csak „meleg” vagy „hideg”) (7. fej.).
- **Gépi tanulás és neurális hálók** — nem előre megírt szabályok, hanem mintázatok tanulása nagy mennyiségű adatból; ez a paradigmaváltás a generatív AI technikai alapja (7. fej.).
- **Esetalapú következtetés (case-based reasoning)** — korábbi hasonló esetek adatbázisa; új problémánál a legjobban illeszkedő korábbi eset megoldását ajánlja (8. fej.).
- **Genetikus algoritmusok** — optimalizálás rendkívül sok lehetséges megoldás között, a „természetes szelekció” logikájával, generációról generációra; mérnöki megfelelője a **generatív tervezés (generative design)** (8. fej.).
- **Intelligens ágensek** — beépített vagy tanult tudásbázissal rendelkező szoftverek, amelyek egy felhasználó vagy folyamat nevében végeznek feladatokat (pl. releváns információ keresése nagy adatmennyiségben) (8. fej.).
- **Hibrid AI-rendszerek** — több technika kombinációja: pl. neurális háló felismeri a mintázatot, a szakértői rendszer adja a szabályalapú, emberi nyelven magyarázható indoklást → **magyarázhatóság** (8. fej.).
- **Hallucináció** — a nyelvi modell magabiztosan, de tévesen állít valamit, mert nincs megbízható hozzáférése ellenőrizhető forrásokhoz (9. fej.).
- **RAG — Retrieval-Augmented Generation** — a modell először visszakeresi a releváns dokumentumrészleteket a szervezet saját, ellenőrzött forrásaiból (karbantartási kézikönyv, hibajelentés), és csak ez alapján generál választ (Fan et al. 2024) (9. fej.).
- **Tudásgráf** — a dokumentumok tartalma összekapcsolt fogalmak hálózataként strukturálva (Graph RAG; Peng et al. 2024) (9. fej.).

## Modellek és keretek

### A) A tudás mozgásának négy lépése (9. ea. 3. fej.) — hajtómű-hangminta példa
| Lépés | Mi történik |
|---|---|
| 1. **Megosztás** | közös munka közben, tapasztalati úton adja át a „megérzést” — a tudás tacit marad, de már két emberben él |
| 2. **Explicitté tétel** | a mintázat mérhető, szenzoradattal alátámasztott küszöbértékké alakul |
| 3. **Kombinálás** | a szabály más explicitté tett szabályokkal teljesebb diagnosztikai eljárássá egyesül |
| 4. **Elsajátítás** | az új mérnök megtanulja, alkalmazza, saját tapasztalatává — ismét tacit tudássá — alakítja |
Kritikai pont: **nem lineáris, nem automatikus — minden lépésnél elveszhet valami.** Analógia: a rajzon lévő tűréshatár (explicit) vs. a mérnök „látta már működni” korrekciós tapasztalata.

### B) KM-értéklánc (Laudon & Laudon 2018; 9. ea. 4. fej.)
| Lépés | Jelentése |
|---|---|
| 1. **Megszerzés** | azonosítás és összegyűjtés — dokumentumokból, adatbázisokból, tapasztalt munkatársak fejéből |
| 2. **Tárolás** | rendszerezett, visszakereshető megőrzés |
| 3. **Terjesztés** | eljuttatás azokhoz, akiknek kell, amikor kell |
| 4. **Alkalmazás** | beépítés a napi döntéshozatalba és munkafolyamatokba |
A legtöbb szervezet **a tárolásra fókuszál túlzottan**, és elhanyagolja a **terjesztést** (tudja-e valaki, hogy létezik, és meg tudja-e találni?). Analógia: alkatrész-katalógus — nem az alkatrészt tárolja, csak jelzi, melyik polcon van és ki a felelőse.

### C) Knowledge Work Systems — három típus (9. ea. 5. fej.)
1. **CAD** — digitális tervezés és tesztelés fizikai prototípus előtt → rövidebb tervezési ciklus, alacsonyabb költség.
2. **VR/AR** — immerzív vizsgálat; terepen dolgozó technikusoknak valós idejű, vizuálisan rárétegzett útmutatás.
3. **Digitális iker** — „a legaktuálisabb és a KM szempontjából talán a legfontosabb”; a tacit tudás egy részét explicitté teheti **szavak nélkül**: a megérzés küszöbértékként/mintafelismerési szabályként beépül a modellbe → „nem dokumentum, hanem működő modell formájában” éli túl a nyugdíjazást. Analógia: élő, a berendezéssel együtt „öregedő” műszaki rajz.

### D) SharePoint-temető és a TCS-ellenpélda (9. ea. 6. fej.)
- Miért buknak a tudástárak: **nem technikai ok** — a tudásmunkások nem szeretik, ha „menedzselik” őket, ellenállnak a rájuk kényszerített tudásmegosztásnak; ugyanaz a minta, mint a Big Data-fejezetben: a rendszer megépül, kultúra és motiváció nélkül üresen marad.
- **Tata Consulting Services (TCS)** — India egyik legnagyobb szoftverexportőre; vállalati szintű KM-rendszer tacit és explicit tudásra, amelyet **piacra vihető szolgáltatásként is értékesített** más cégeknek (Laudon 2018). A különbség: a vezetés beépítette-e a tudásmegosztást a **napi munkafolyamatokba és az ösztönzőrendszerbe**, nem „extra” feladatként.

### E) Szakértői rendszerek — négy tudásbázis-típus (Iván, é.n.; 9. ea. 7. fej.)
| Típus | Leírás |
|---|---|
| **Esetbázisú** | korábbi hasonló esetek és megoldásaik tárolása, visszakeresése |
| **Keretbázisú** | strukturált „sablonok” objektumokról és tulajdonságaikról |
| **Objektumalapú** | objektumok és a köztük lévő kapcsolatok modellezése |
| **Szabálybázisú** | explicit IF-THEN logikai szabályok gyűjteménye |
Előny: a szakértő tudása tartósan, fáradtság nélkül elérhető — a szakértő távozása után is. **Korlátok:** nem tanulnak önmaguktól; karbantartásuk/bővítésük költséges; nem reagálnak előre nem látott helyzetekre. Analógia: relémeghajtású vezérlés (megbízható, de új helyzetben tehetetlen) vs. gépi tanulás = tapasztalt operátor (alkalmazkodik, de nem mindig világos, miért döntött).

### F) Történeti ív: szabályalapú → tanuló-alapú → hibrid → generatív (9. ea. 7–9. fej.)
Szakértői rendszerek (IF-THEN) → fuzzy logika → gépi tanulás/neurális hálók → esetalapú következtetés, genetikus algoritmusok, intelligens ágensek → **hibrid AI** (mintázat + magyarázat) → **generatív AI + RAG** (hallucináció ellen). Közös szál: **megbízhatóság és magyarázhatóság**.

### G) Generatív AI mint KM-eszköz (Laudon, Laudon & Traver 2025; 9. ea. 9. fej.)
- Ígéret: dokumentumok összefoglalása, kérdésekre válasz, karbantartási jelentés nyers adatból.
- Probléma: **hallucináció**. Válasz: **RAG** (Fan et al. 2024); egy **2025 decemberi, 63 tanulmányt** elemző szisztematikus áttekintés (Karakurt & Akbulut 2026, Applied Sciences 16(1), 368) megerősítette: jelentősen csökkenti a hallucináció kockázatát dokumentumintenzív vállalati feladatokban.
- RAG = válasz a SharePoint-temetőre: nem egyszer „betanít”, hanem folyamatosan a szervezet aktuális, szétszórt dokumentumaiból dolgozik. Fejlettebb: tudásgráfok (Peng et al. 2024, arXiv:2408.08921).
- Analógia: technikus, aki nem fejből, hanem a friss szervizkönyvből diagnosztizál — lassabb, de ellenőrizhető forráshoz köthető.
- **Lehatárolás:** ez a fejezet a technikai/szervezeti **megbízhatóságot** vizsgálja; az etikai/társadalmi vonatkozások (torzítás, felelősség, méltányosság) a 11. fejezetben.

## Számok, dátumok, nevek, amiket a tananyag kiemel

| Mi | Érték | Hol |
|---|---|---|
| Nyugdíjba vonuló mérnökök | 5 fő, 25+ év tapasztalat | 2. fej. |
| Technikusok átlagéletkora | 57 év (pandémia előtt) | 2. fej. |
| ATEC 2022 | ≥ 5000 elvesztett új mechanikus | 2. fej. |
| Elvándorlás | 38 % elhagyta; 4 % korai nyugdíj | 2. fej. |
| Tudás mozgásának lépései | 4 (megosztás, explicitté tétel, kombinálás, elsajátítás) | 3. fej. |
| Nonaka & Takeuchi | 1995, The knowledge-creating company (háttér; részletek az opcionális könyvben) | 3. fej. |
| KM-értéklánc | 4 lépés (megszerzés, tárolás, terjesztés, alkalmazás) | 4. fej. |
| KWS típusok | 3 (CAD, VR/AR, digitális iker) | 5. fej. |
| Digitális iker | Michael Grieves, 2000-es évek eleje; Grieves & Vickers 2017; 3 képesség | 5. fej. |
| de Holan & Phillips | 2004, Management Science 50(11), 1603–1613 | 6. fej. |
| TCS | Tata Consulting Services, India | 6. fej. |
| Tudásbázis-típusok | 4 (eset-, keret-, objektum-, szabálybázisú) — Iván Cs., ÓE | 7. fej. |
| Laudon & Laudon 2018 | 15th ed., 11. fejezet | 3–8. fej. |
| RAG | Fan et al. 2024; Peng et al. 2024 (Graph RAG, arXiv:2408.08921) | 9. fej. |
| Szisztematikus áttekintés | 2025 december, 63 tanulmány (Karakurt & Akbulut 2026) | 9., 11. fej. |
| Business Fest | 2026, magyar gyártóipar munkaerő- és kompetenciahiány | 10. fej. |
| Következő fejezet | 10.: Felhő és IT-infrastruktúra | 10. fej. |

## Számítások

Az előadás nem tartalmaz képletet vagy számítást. A tananyag számaiból levonható arányok (saját számítás): a 38 % + 4 % = **42 %** a légiközlekedési mérnökök közül távozott vagy korán nyugdíjba ment; öt 25+ éves mérnök = **legalább 125 „mérnökév”** tapasztalat távozik egyszerre — „mindegyikük magával víve évtizedes, sehol le nem írt tapasztalatát”. „Mi változik, ha…”: ha a 4 lépéses tudásmozgatás minden lépésénél a tudás 20 %-a elvész (a tananyag: „minden lépésnél elveszhet valami”), a 4. lépés végére 0,8⁴ ≈ **41 %** marad — ezért nem elég az egyszeri workshop.

## Összekeverhető párok / „mi NEM igaz” csapdák

1. **Tacit tudás dokumentálható („írja le, amit tud”)?** NEM — csak az explicit réteg rögzül; a tacit nyelvileg nehezen/nem ragadható meg.
2. **Tacit vs. explicit:** explicit = kézikönyv, szabványeljárás, adatbázis; tacit = megérzés, zajminta, rezgés „furcsasága”.
3. **A tudás mozgásának 4 lépése vs. a KM-értéklánc 4 lépése:** mozgás = megosztás → explicitté tétel → kombinálás → elsajátítás; értéklánc = megszerzés → tárolás → terjesztés → alkalmazás. Két különböző négyes!
4. **A szervezetek melyik értéklánc-lépést hanyagolják el?** A **terjesztést** (a tárolásra fókuszálnak túlzottan).
5. **Szakértő-kereső rendszer tárolja a tudást?** NEM — azt mutatja, **ki** tudja.
6. **Digitális iker = dokumentum?** NEM — „működő modell”; Grieves 3 képessége: konceptualizáció, összehasonlítás, együttműködés (nem „tárolás”).
7. **Tudástárak bukásának oka technikai?** NEM — a tudásmunkások ellenállása a rájuk kényszerített megosztásnak; kultúra és ösztönzők.
8. **Szándékos vs. véletlen szervezeti felejtés** (de Holan & Phillips 2004): a véletlen okoz kárt.
9. **TCS: miért sikerült?** Beépítés a napi munkafolyamatba és ösztönzőrendszerbe; a KM-rendszert szolgáltatásként is eladta.
10. **Szakértői rendszer tanul?** NEM — szabályalapú (IF-THEN), nem tanul önmagától; a gépi tanulás tanul, de kevésbé magyarázható.
11. **Esetbázisú tudásbázis vs. esetalapú következtetés (CBR):** ugyanaz a logika (korábbi esetek) — az egyik a szakértői rendszer tudásbázis-típusa (7. fej.), a másik önálló intelligens technika (8. fej.).
12. **Genetikus algoritmus = tanulás?** NEM — optimalizálás szelekcióval; mérnöki párja a generatív tervezés. **Intelligens ágens** = felhasználó nevében feladatot végző program.
13. **Hibrid AI célja:** mintázatfelismerés + **magyarázhatóság** (neurális háló + szakértői rendszer).
14. **RAG = a modell újratanítása?** NEM — visszakeresés az ellenőrzött dokumentumokból generálás előtt; a hallucináció ellen. Lassabb, de megbízhatóbb.
15. **A 9. ea. az AI etikáját tárgyalja?** NEM — a megbízhatóságot; az etika a 11. fejezet.
16. **Fuzzy logika = gépi tanulás?** NEM — a szabályalapú rendszer finomítása elmosódott kategóriákra.
17. **Nonaka–Takeuchi modell neve/mátrixa a kötelező anyagban?** NEM — csak az opcionális könyvben; a kötelező a 4 lépést és a forráshivatkozást adja.

## Kapcsolat más előadásokkal

- Core competency, P&G InnovationNet, „a tudás az emberek fejében van” (2. ea. 9. fej.) → ide utal előre.
- KMS az Enterprise Application Architecture-ben (3. ea. 7. fej.); CKO (4. ea. 6. fej.).
- Société Générale 220+ üzleti szabály kodifikálása (4. ea.) = tacit → explicit tétel; Siemens Amberg / Bosch digitális iker (4. ea.) ↔ digitális iker mint KWS.
- „Technológia nem elég” — SharePoint-temető ↔ 1. ea. komplementer eszközök, 5. ea. BI-kultúra, 8. ea. Big Data-bukás (a tananyag kifejezetten hivatkozik a Big Data-fejezetre).
- Generatív AI karbantartási jelentés nyers adatból (8. ea. 5. fej.) ↔ 9. fej.; „az AI felerősíti a jó és a rossz adatstratégiát is”.
- Magyarázhatóság, hallucináció, torzítás → 11. ea. etika/felelős AI (a tananyag előreutal).
- Szervezeti ellenállás (1. ea.), Moneyball szakértői ellenállás (8. ea.) ↔ tudásmunkások ellenállása.
- Következő: 10. ea. Felhő és IT-infrastruktúra.

## Fogalomtár-jelöltek

- **Hallgatólagos tudás** – tacit knowledge – tapasztalati, nehezen megfogalmazható tudás.
- **Kifejezett tudás** – explicit knowledge – dokumentált, leírható tudás.
- **Tudásmenedzsment-értéklánc** – KM value chain – megszerzés, tárolás, terjesztés, alkalmazás.
- **Szakértő-kereső rendszer** – expertise location system – ki tudja, nem mit tudunk.
- **Tudásmunka-rendszer** – Knowledge Work System (KWS) – CAD, VR/AR, digitális iker.
- **Digitális iker** – digital twin – szinkronizált virtuális más; Grieves; konceptualizáció, összehasonlítás, együttműködés.
- **Szervezeti felejtés** – organizational forgetting – szándékos vs. véletlen tudásvesztés (de Holan & Phillips 2004).
- **Szakértői rendszer** – expert system – IF-THEN szabályalapú, szűk szakterület; következtető motor + tudásbázis.
- **Fuzzy logika** – fuzzy logic – elmosódott kategóriák kezelése.
- **Esetalapú következtetés** – case-based reasoning – legjobban illeszkedő korábbi eset megoldása.
- **Genetikus algoritmus** – genetic algorithm – szelekciós optimalizálás; generatív tervezés.
- **Intelligens ágens** – intelligent agent – felhasználó nevében feladatot végző program.
- **Hibrid AI-rendszer** – hybrid AI – neurális háló + szakértői rendszer: riasztás + indoklás.
- **Hallucináció** – hallucination – magabiztos, téves nyelvi modell-állítás.
- **Visszakereséssel bővített generálás** – RAG – ellenőrzött forrásból visszakeresés, majd generálás.
- **Tudásgráf** – knowledge graph – fogalmak hálózataként strukturált tudás (Graph RAG).

---

# 10. előadás: Felhő és IT-infrastruktúra — stratégiai döntés, nem IT-feladat („Mi történik, ha a felhő maga omlik össze?”)

## Egy mondatban (a központi tézis)

A felhő **nem „belépés egy biztonságos, gondtalan szolgáltatásba”, hanem stratégiai függőségi viszony**, amelyet úgy kell megtervezni, mint bármely kritikus beszállítói kapcsolatot: minden szolgáltatási szint kontroll-átadás, a felhő nem mindig olcsóbb (stabil terhelésnél a „bérlés” drágább a „tulajdonlásnál”), a vendor lock-in ellen exit-stratégia, a felhő-koncentráció ellen multi-region/multi-cloud redundancia véd — az SLA önmagában nem (10. ea. 10. fej.).

## Nyitó eset és feloldása (10. ea. 2., 7. és 10. fej.)

**Nyitó dilemma:** Ön egy közepes bank informatikai igazgatója; a vezetőség a teljes ügyfél-adatvagyont és a core banki rendszert **egyetlen** nemzetközi felhőszolgáltatóhoz költözteti (rugalmasabb, skálázhatóbb, olcsóbbnak tűnik). **Három évvel később a szolgáltató csődöt jelent.** Opciók: **A)** pánikszerű váltás bármi áron; **B)** elővenni a három évvel korábban kidolgozott **exit-stratégiát**; **C)** várni, hátha felvásárolják. **Helyes: B** — de csak akkor lehetséges, ha a felhőbe költözés **pillanatában** elkészült (7. fej.: „a bank problémája nem a csőd bekövetkezése volt… hanem hogy ezt a kockázatot nem tervezte be előre”; A és C = utólagos improvizáció).

**A valós háttér — AWS-kiesés, 2025. október 20.** (2. és 9. fej.):
| Adat | Érték |
|---|---|
| Régió | AWS **US-EAST-1** (Virginia); **DNS-feloldási hiba**, lépcsőzetes összeomlás |
| Időtartam | **15 óra** |
| Érintettek | **3500+ vállalat, 60+ ország** — bankok, tőzsdék, légitársaságok (Delta Air Lines), kiskereskedelmi láncok, kórházi rendszerek (betegadat-hozzáférés) |
| Kár | **> 1 milliárd USD** (egyes elemzők szerint jóval több) |
| Ismétlődés | a **harmadik** hasonló léptékű incidens **öt év alatt**, ugyanabból a régióból |

Elméleti pontok: exit-stratégia négy eleme (7. fej.), MNB 2/2025 ajánlás (7., 10. fej.), vendor lock-in vs. felhő-koncentráció megkülönböztetése (10. fej.), SLA korlátai (10. fej.).

## Fogalmak és definíciók (HU – EN)

- **Inga-mozgás (centralizáció ↔ decentralizáció)** — az elmúlt 70 év informatika-története nem egyenes vonalú fejlődés, hanem oda-vissza ingamozgás (Laudon & Laudon 2018, 5. fej.); a felhő = **visszatérés a mainframe-kori centralizációhoz**, csak néhány globális szolgáltatónál (3. fej.).
- **Vision picking** — DHL (Ricoh, Ubimax): okosszemüveges vizuális útmutatás a raktárban → **25 %-os hatékonyságnövekedés** (3. fej.).
- **Fogyasztói informatika (consumerization of IT)** — a munkavállalók saját eszközeiket használják munkára (3. fej.).
- **BYOD (Bring Your Own Device)** — saját eszköz; **CYOD (Choose Your Own Device)** — előre jóváhagyott, vállalat által felügyelt eszközkatalógusból választás (3. fej.).
- **IaaS / PaaS / SaaS mint döntési logika** — minden szinttel feljebb a szervezet **kontrollt ad fel**, cserébe felelősséget és üzemeltetési terhet vesz le; nem technikai definíció (4. fej.).
- **Privát / publikus / hibrid felhő** — telepítési modellek; a választás stratégiai: kockázat-tolerancia, szabályozás, terhelési mintázat (5. fej.).
- **Felhő-mítosz** — „a felhő mindig olcsóbb és egyszerűbb”; a mítosz ott dől meg, ahol a terhelés **stabil és kiszámítható** (6. fej.).
- **Cloud repatriation (kilépés a felhőből)** — 37signals, Dropbox (6. fej.).
- **Vendor lock-in** — olyan mértékű függés egy szolgáltatótól, hogy a váltás rendkívül költséges vagy technikailag nehéz; kockázat nemcsak csődnél, hanem áremelés, minőségromlás, funkció-kivonás esetén is (7. fej.).
- **Exit-stratégia (kivezetési stratégia)** — négy alapelem (7. fej.); MNB 2/2025. (I.13.) ajánlás kötelezően előírja pénzügyi intézményeknek.
- **Egress díj (adatkiviteli díj)** — bevitel ingyenes, kivitel díjazott → lock-in-t erősítő árazás (8. fej.).
- **„Bőség paradoxona”** — alacsony egyedi költség miatt többre fizetnek elő, mint kell — „a felhő digitális polcára minden felfér” (Tick A., ÜIA) (8. fej.).
- **Felhő-koncentráció** — három szolgáltató (AWS, Azure, Google Cloud) a globális felhő-infrastruktúra piac **~60–63 %-át** birtokolja → **single point of failure** rendszerszinten (9. fej.).
- **Multi-cloud / multi-region** — több szolgáltató / több földrajzi régió; a multi-cloud önmagában nem segít, ha a régión belüli redundancia hiányzik (9. fej.).
- **SLA (Service Level Agreement, szolgáltatási szintű megállapodás)** — a szolgáltatók korlátozzák felelősségüket; kompenzáció jellemzően csak **szolgáltatási kredit** jövőbeli igénybevételre, nem kártérítés; „a tényleges üzleti kockázatot mindvégig az igénybe vevő viseli” (10. fej.).

## Modellek és keretek

### A) Az IT-infrastruktúra evolúciója — inga (Laudon 2018; 10. ea. 3. fej.)
| Korszak | Modell | Centralizáció foka |
|---|---|---|
| 1950–70-es évek | **Mainframe** | teljes centralizáció — egyetlen nagygép, „buta” terminálok |
| 1980–90-es évek | **Személyi számítógép, kliens-szerver** | decentralizáció — kapacitás az asztalon |
| 2000-es évek | **Vállalati hálózatok, internet** | részleges újra-centralizáció — vállalati adatközpontok |
| 2010-es évektől | **Felhő** | újra teljes centralizáció — néhány globális szolgáltatónál |
Legújabb állomás: **mobil és hordható eszközök** — DHL vision picking (+25 %); **Southern Co.** (energetika): okosórák, kamerás fejpántok erőművekben — eljárások pontosabb követése, valós idejű terep–iroda kommunikáció.

**BYOD érvek és ellenérvek (3. fej.):**
| Érv mellette | Ellenérv — miért fordul a trend |
|---|---|
| alacsonyabb hardverköltség | rejtett üzemeltetési költség (sokféle eszköz támogatása, incidensek) felemészti |
| nagyobb elégedettség, rugalmasság | a munkavállalók **71 %-a** érzékeny vállalati adatot tárol személyes telefonján |
| nincs betanulási görbe | a vállalatok **62 %-a** felülvizsgálja vagy elhagyja a BYOD-politikát (Tangoe 2025) |
Trend: **BYOD → CYOD**; 2026-os felmérés: a CISO-k **78 %-a** aggódik saját jogi felelőssége miatt BYOD-incidens esetén. Analógia: saját szerszám behozatala → vissza az egységes vállalati szerszámkészlethez.

### B) IaaS / PaaS / SaaS — kontroll-átadás (10. ea. 4. fej.)
| Szint | Amit feladunk | Amit nyerünk |
|---|---|---|
| **IaaS** | fizikai hardver feletti kontroll | nincs szerverbeszerzés, gyors skálázás |
| **PaaS** | operációs rendszer, middleware feletti kontroll | fejlesztők csak az alkalmazásra fókuszálnak |
| **SaaS** | testreszabás, verziókövetés feletti kontroll | azonnal használható, karbantartás-mentes |
Ugyanaz a logika, mint a build/buy/outsource (8. fej.). **A döntés rendszerenként újra átgondolandó** — hiba egyetlen szintet „vállalati szabványként” választani: kritikus, egyedi versenyelőnyt adó rendszer (saját minőségellenőrzési algoritmus) → IaaS-szintű kontroll; általános funkció (e-mail, dokumentumkezelés) → SaaS. Analógia: saját karbantartás / éves szervizszerződés / gépkapacitás bérlése csúcsidőben.

### C) Publikus / privát / hibrid (Laudon 2018, 5. fej.; 10. ea. 5. fej.)
| Modell | Mikor indokolt |
|---|---|
| **Privát felhő** | szigorú szabályozás, érzékeny adat, egyedi megfelelőség (banki core rendszer) |
| **Publikus felhő** | változó terhelés, nem érzékeny adat, gyors skálázás |
| **Hibrid felhő** | kritikus mag védett, kiegészítő funkciók a publikus felhőben — EasyJet |
**EasyJet-eset:** az Egyesült Királyság legnagyobb légitársasága; a foglalási rendszer nem tudta kezelni az **online ülésválasztást** → a mag-rendszer saját üzemeltetésben maradt, csak az új funkció került a **Microsoft Azure** publikus felhőbe. Eredmény: a légiipari átlag a bevétel **2 %-át** költi IT-re, az EasyJet **0,5 %-on** tartja; versenyelőny: alacsony ár + jó ügyfélélmény. Vezetői érv: a felhős komponens **könnyen visszavonható/kikapcsolható**, szemben a mag-rendszerbe épített funkcióval.

### D) A felhő mítoszai — 37signals (10. ea. 6. fej.)
- **37signals** (Basecamp, HEY e-mail): 2022-ben **évi 3,2 M USD** AWS + Google Cloud költés, **stabil, kiszámítható** terhelés mellett. **David Heinemeier Hansson:** „Máshol sem keverjük össze a bérlést a tulajdonlással — nem bérelnénk 30 évre egy házat háromszor annyiért, mint amennyibe a törlesztés kerülne.”
- **2022 október:** kilépés bejelentése; **hat hónap** alatt, **600 000 USD** egyszeri hardverbefektetéssel, ugyanazzal a **tíz fős** üzemeltetői csapattal (új alkalmazott nélkül) áttelepítés saját, **kollokációs** adatközpontokba. Eredmény: a hardver **hat hónap alatt megtérült**; adatbázis-lekérdezések **3–5× gyorsabbak**; projekció: **5 év alatt > 10 M USD** megtakarítás. Ábra: 3,2 M USD (2022) → ~1,3 M USD (2023–24).
- **Dropbox** 2016: hasonló lépés, **75 M USD** megtakarítás **2 év** alatt.
- **Mikor igaz a mítosz:** induló vállalkozások, erősen ingadozó terhelés — a **HEY** indulásakor **3 hét alatt 300 000 felhasználó** a tervezett **30 000** helyett → csak felhővel kezelhető. Analógia: exkavátor vétele vs. bérlése.

### E) Exit-stratégia alapelemei (10. ea. 7. fej.) — négy pont
1. **Adatkinyerhetőség előzetes tesztelése** — rendszeresen tesztelni az exportálási és visszaállítási folyamatot.
2. **Nyílt szabványok előnyben részesítése** — zárt, szolgáltató-specifikus formátumok kerülése.
3. **Migrációs terv és időbecslés előre** — nem válsághelyzetben először.
4. **Kritikus adatok redundáns, saját mentése** — a szolgáltatótól függetlenül.
**MNB 2/2025. (I.13.) ajánlás:** kötelező kivezetési stratégia és akcióterv felhőszolgáltatás bevezetésekor — migrációs terv, visszaállítási forgatókönyvek, az adatok (éles, tartalék, archív) **igazolt törölhetősége** kilépéskor.

### F) Felhő-specifikus TCO-elemek (10. ea. 8. fej.) — négy tétel
| Rejtett költségelem | Miért észrevétlen |
|---|---|
| **Adatkiviteli (egress) díjak** | bevitel ingyenes, kivitel díjazott — lock-in-t erősítő árazás |
| **Komplexitási költség** | felhő-specifikus jogosultságkezelés, architektúra-szabályok megtanulása, karbantartása — alulbecsült szakértői idő |
| **Skálázódó díjak stabil terhelésnél** | az árazás nem feltétlenül csökken az idővel változatlan használat mellett |
| **„Bőség paradoxona”** | többre fizetnek elő, mint kell |
Mikor fordul a mérleg: minél stabilabb a terhelés, annál inkább a saját üzemeltetés felé. Ábra: felhő-költség enyhén növekvő görbéje vs. saját infrastruktúra egyszeri beruházás utáni lapos görbéje, metszésponttal. Csapda: csak az első évi költség összehasonlítása → torzított döntés.

### G) Két kockázat, amit nem szabad összemosni (10. ea. 10. fej.)
| | Vendor lock-in (7. fej.) | Felhő-koncentráció (9. fej.) |
|---|---|---|
| Szint | vállalati, szolgáltató-specifikus „ragadósság” | rendszerszintű, iparági törékenység |
| Lényeg | nehéz és költséges váltani | egyetlen kiesés mindenkit érint egyszerre, függetlenül a „ragadósságtól” |
| Védekezés | **exit-stratégia** | **multi-region / multi-cloud redundancia** |
„Egyik sem oldja meg a másikat.” Analógia: egy beszállító (olcsó, sérülékeny) vs. több beszállító, több telephely (drágább, ellenállóbb).

### H) Hazai kitekintés (10. ea. 10. fej.)
MNB 2/2025 ajánlás — a szabályozó sem bízik abban, hogy az SLA elég; **MBH Bank 2023**: felhőalapú, konténerizált (**OpenShift**) platform a **három jogelőd bank** ügyfeleinek egységes kiszolgálására (MBH Bank Nyrt. 2024. április 29-i közgyűlési dokumentumok). Következő fejezet: **11. Etika, algoritmusok és felelős AI.**

## Számok, dátumok, nevek, amiket a tananyag kiemel

| Mi | Érték | Hol |
|---|---|---|
| AWS-kiesés | 2025. 10. 20.; US-EAST-1 (Virginia); DNS-hiba; 15 óra; 3500+ cég; 60+ ország; >1 Mrd USD; 3. incidens 5 év alatt | 2., 9. fej. |
| Infrastruktúra-korszakok | 4 (mainframe; PC/kliens-szerver; vállalati hálózat/internet; felhő) | 3. fej. |
| DHL vision picking | Ricoh, Ubimax; +25 % hatékonyság | 3. fej. |
| Southern Co. | energetika; okosórák, kamerás fejpántok | 3. fej. |
| BYOD | 71 % érzékeny adat személyes telefonon; 62 % felülvizsgál/elhagy (Tangoe 2025); CISO-k 78 % aggódik (2026) | 3. fej. |
| EasyJet | UK legnagyobb légitársaság; Azure; IT = bevétel 0,5 % vs. iparági 2 % | 5. fej. |
| 37signals | 3,2 M USD/év (2022); 600 000 USD hardver; 6 hónap; 10 fős csapat; 3–5× gyorsabb DB; >10 M USD / 5 év; DHH idézet | 6. fej. |
| HEY indulás | 300 000 felhasználó 3 hét alatt (terv: 30 000) | 6. fej. |
| Dropbox | 2016; 75 M USD / 2 év | 6. fej. |
| Exit-stratégia elemei | 4 | 7. fej. |
| MNB ajánlás | 2/2025. (I.13.) | 7., 10. fej. |
| Felhő-TCO rejtett elemek | 4 (egress, komplexitás, skálázódó díj, bőség paradoxona) | 8. fej. |
| Három nagy szolgáltató piaci részesedése | ~60–63 % (AWS, Azure, Google Cloud) | 9. fej. |
| MBH Bank | 2023; OpenShift; 3 jogelőd bank | 10. fej. |
| Elmélyítő | Harmon et al. 2021; PIFS 2023; Opara-Martins et al. 2016; CVL 2024 (Mathematics 12(3), 387) | 11. fej. |

## Számítások — felhő vs. saját üzemeltetés TCO (10. ea. 6. és 8. fej.)

A tananyag képletet nem ad, de a 37signals-eset számai végigszámolhatók:
- Felhőköltség: **3,2 M USD/év** (2022). Egyszeri hardverbefektetés: **0,6 M USD**. A tananyag szerint a hardver **6 hónap alatt megtérült** → a felhőköltség-megtakarítás legalább 0,6 M USD / 0,5 év = **≥ 1,2 M USD/év** nagyságrendű.
- Ábra: 3,2 M → ~1,3 M USD/év → éves megtakarítás ≈ **1,9 M USD** (a Data Center Dynamics 2025 forrás címe: „saved almost $2m last year”). Megtérülési idő = 0,6 / 1,9 ≈ **0,32 év ≈ 4 hónap** (a tananyag 6 hónapot mond — a hardver nem az első naptól hozott teljes megtakarítást).
- 5 éves projekció: 5 × 1,9 ≈ 9,5 M, plusz további optimalizálás → **> 10 M USD** (a tananyag száma).
- **„Mi változik, ha…”**: ha a terhelés a HEY-indulás mintáját követi (10× a tervezett forgalom 3 hét alatt), a saját 600 000 USD-os hardver nem skálázható azonnal → a felhő rugalmassága ér többet, mint a megtakarítás. Ha a felhő-TCO négy rejtett elemét (egress, komplexitás, nem csökkenő díj, bőség paradoxona) is beszámítják, a felhő tényleges éves költsége a 3,2 M-nál is magasabb → a mérleg még erősebben a saját üzemeltetés felé fordul stabil terhelésnél.
- **EasyJet arány:** ha a bevétel 1 Mrd GBP (saját feltevés), az iparági 2 % = 20 M, az EasyJet 0,5 % = 5 M GBP IT-költés → **negyedannyi**.
- **AWS-kiesés vs. SLA:** > 1 Mrd USD kár 15 óra alatt ≈ 67 M USD/óra az érintettek összességére (saját számítás); az SLA-kompenzáció szolgáltatási kredit, „ennek töredékét sem fedezi”.

## Összekeverhető párok / „mi NEM igaz” csapdák

1. **Nyitó dilemma: a probléma a csőd?** NEM — a be nem tervezett kockázat; B csak akkor opció, ha az exit-stratégia a költözéskor készült.
2. **A felhő radikálisan új?** NEM — visszatérés a mainframe-centralizációhoz, csak globális szolgáltatóknál (inga).
3. **Korszakok sorrendje:** mainframe (1950–70) → PC/kliens-szerver (1980–90) → vállalati hálózat/internet (2000) → felhő (2010+) → mobil/hordható.
4. **BYOD trend erősödik?** NEM — fordul: 62 % felülvizsgál/elhagy, CYOD felé.
5. **IaaS/PaaS/SaaS: mit adunk fel?** IaaS = hardver; PaaS = OS/middleware; SaaS = testreszabás/verziókövetés. Feljebb = kevesebb kontroll, kevesebb teher.
6. **Egy szolgáltatási szint vállalati szabványként?** NEM — rendszerenként döntendő (kritikus → IaaS; e-mail → SaaS).
7. **Privát vs. publikus vs. hibrid:** privát = szabályozott, érzékeny (banki core); publikus = változó terhelés, nem érzékeny; hibrid = EasyJet (mag helyben, ülésválasztás Azure-ban).
8. **EasyJet IT-költés:** 0,5 % vs. iparági 2 % (nem fordítva).
9. **A felhő mindig olcsóbb?** NEM — stabil, kiszámítható terhelésnél a bérlés drágább; ingadozó terhelésnél/startupnál igen (HEY).
10. **37signals számok:** 3,2 M USD/év; 600 k USD hardver; 6 hónap; 10 fő; 3–5×; >10 M/5 év. **Dropbox:** 2016, 75 M USD/2 év — ne keverd.
11. **Vendor lock-in csak csődkor?** NEM — áremelés, minőségromlás, funkció-kivonás is.
12. **Vendor lock-in vs. felhő-koncentráció:** vállalati vs. rendszerszintű; exit-stratégia vs. multi-region/multi-cloud; egyik sem oldja meg a másikat.
13. **Multi-cloud mindent megold?** NEM — ha a kritikus rendszer ugyanabban a régióban fut, régión belüli redundancia nélkül nem segít.
14. **Egress díj:** a **kivitel** díjazott, a bevitel ingyenes.
15. **SLA = kártérítés?** NEM — szolgáltatási kredit; a kockázatot az igénybe vevő viseli; az SLA nem védekezés, az exit-stratégia és a redundancia az.
16. **MNB 2/2025 kötelezően előírja** az exit-stratégiát pénzügyi intézményeknek — nem csak ajánlja „jó gyakorlatként” (a tananyag: „kötelező érvénnyel írja elő”).
17. **MBH Bank 2023 OpenShift** ≠ MNB ajánlás 2025 — két különböző hazai tétel.
18. **Felhő-TCO négy eleme** ≠ Big Data-TCO három eleme (8. ea.: létszám, integráció, lehetőségköltség) ≠ 1. ea. hét TCO-tétel.

## Kapcsolat más előadásokkal

- TCO 20/80, rejtett költségek (1. ea. 7. fej.) és Big Data TCO-jéghegy (8. ea. 9. fej.) ↔ felhő-TCO (a tananyag kifejezetten visszautal a 8. fejezetre).
- Build/buy/outsource (8. ea.) ↔ IaaS/PaaS/SaaS kontroll-átadás; build/buy/cloud (3. ea.); cloud ERP/CRM, on-premise → SaaS (3. ea. 2. fej.).
- GE Predix saját adatközpont vs. felhőszolgáltató (8. ea. 4. fej.) ↔ felhő-koncentráció, hibrid.
- Edge/fog/cloud (8. ea. 6. fej.) ↔ centralizáció kockázata.
- Bimodális IT (5. ea. 4. fej.) — a tananyag szerint a felhő bevezetésénél is ez a minta.
- Váltási költség mint tudatos IT-stratégia (2. ea. 6. fej.) ↔ egress díj, vendor lock-in; AI-infrastruktúra szállítói függőség (2. ea. 10. fej.).
- Digitális iker táblagépen (9. ea.) ↔ BYOD/CYOD döntés (a tananyag reflektív kérdése).
- CISO (4. ea.), biztonsági incidens, BYOD → 12. ea. kiberbiztonság.
- Következő: 11. ea. Etika, algoritmusok és felelős AI.

## Fogalomtár-jelöltek

- **Nagyszámítógép-korszak** – mainframe – teljes centralizáció, buta terminálok (1950–70).
- **Kliens-szerver** – client-server – decentralizáció a PC-korszakban (1980–90).
- **Inga-modell** – centralization–decentralization pendulum – a felhő visszatérés a centralizációhoz.
- **Hordható eszközök** – wearables – DHL vision picking, Southern Co.
- **Fogyasztói informatika** – consumerization of IT – saját eszközök munkahelyi használata.
- **Hozd a saját eszközöd / válaszd a saját eszközöd** – BYOD / CYOD – saját vs. jóváhagyott katalógusból választott eszköz.
- **Infrastruktúra / platform / szoftver szolgáltatásként** – IaaS / PaaS / SaaS – egyre több kontroll feladása egyre kevesebb teherért.
- **Privát / publikus / hibrid felhő** – private / public / hybrid cloud – telepítési modellek kockázat és terhelés szerint.
- **Felhő-repatriáció** – cloud repatriation – visszaköltözés saját infrastruktúrára (37signals, Dropbox).
- **Kollokáció** – colocation – saját szerverek bérelt adatközponti elhelyezése.
- **Szállítói bezártság** – vendor lock-in – költséges/nehéz váltás; nemcsak csődkor.
- **Kivezetési stratégia** – exit strategy – adatkinyerés tesztelése, nyílt szabványok, migrációs terv, redundáns mentés.
- **Adatkiviteli díj** – egress fee – a kivitel díjazása, lock-in-t erősít.
- **Bőség paradoxona** – paradox of plenty – túl-előfizetés olcsó szolgáltatásokra.
- **Felhő-koncentráció** – cloud concentration – 3 szolgáltató ~60–63 %; rendszerszintű single point of failure.
- **Több szolgáltató / több régió** – multi-cloud / multi-region – redundancia a koncentráció ellen.
- **Szolgáltatási szintű megállapodás** – SLA – korlátozott felelősség, szolgáltatási kredit, nem kártérítés.

---

# 11. előadás: Etika, algoritmusok és felelős AI — „Amikor a gép megtanulja a múlt hibáit”

## Egy mondatban (a központi tézis)

A gépi tanulásos rendszer torzítása nem rosszindulat, hanem az adathalmaz statisztikai eloszlásából **„örökölt”**, fekete dobozban rejtett hiba, amelyért **a felelősség emberi marad**; a méltányosság matematikailag nem „megoldható”, hanem tudatos kompromisszum (Kleinberg–Mullainathan–Raghavan), ezért az etikai elvek, az elszámoltathatóság és a szabályozás (EU AI Act) három védvonala együtt is csak csökkenti a kockázatot — **az emberi felügyelet és a tudatos értékválasztás nem kiváltható** (11. ea. 4., 7., 8., 11. fej.).

## Nyitó eset és feloldása (11. ea. 2. és 11. fej.)

**Amazon toborzási AI (Dastin, Reuters 2018):** egy nagy technológiai vállalat **2014-ben** automatizálni akarta a toborzást: AI, amely **száz** önéletrajzból kiválasztja az **öt** legjobbat; betanítva **az elmúlt tíz év** jelentkezési anyagain. **2015-re** kiderült: a rendszer szisztematikusan hátrébb sorolta a **„women's”** szót tartalmazó önéletrajzokat („women's chess club captain”), és előnyben részesítette a férfias kódolású igéket (**„executed”, „captured”**). A konkrét torzításokat megpróbálták javítani, de nem tudták garantálni, hogy más, rejtettebb módon nem torzít → **a projektet leállították**.

**Feloldás (4. és 11. fej.):** a rendszer a férfi-dominanciájú tech-szektor tíz évnyi önéletrajzából nem azt „tanulta”, hogy nőket kell hátrányosan kezelni, hanem azt, hogy bizonyos szavak/mintázatok (amelyek véletlenül gyakrabban fordultak elő a „sikeresnek” minősített, jellemzően férfi jelentkezőknél) magasabb pontszámmal járnak — **adattorzítás**, „örökölt”, nem szándékos; fekete doboz. A 11. fej. visszatérése: miért torzult (3–4. fej.), milyen elvekkel értékelhető (5. fej.), ki felelős (6. fej.), miért nem lehetett „kijavítani” a méltányosságot (7–8. fej.), milyen jogi kategória (9. fej.: **magas kockázat**) — és hogy létezik jobb út: **LinkedIn**.

**Pozitív ellenpélda — LinkedIn Talent Search (2018 körül; Geyik, Ambler & Kenthapadi, KDD '19):** a keresési találatok nem tükrözték arányosan a releváns, képzett jelöltek nemek szerinti eloszlását → nem titkolták el, nem állították le csendben, hanem **méltányosság-tudatos újrarangsorolási algoritmust** fejlesztettek (a végső lista arányosan tükrözi a releváns jelölti kör összetételét), és **lektorált tudományos konferencián publikálták** — átlátható, dokumentált, ellenőrizhető megoldás.

## Fogalmak és definíciók (HU – EN)

- **Szabályalapú szakértői rendszer (rule-based expert system)** — „HA… AKKOR…” szabályok; a torzítás forrása egy konkrét, valaki által megírt szabály; a szabálybázis **átlátható és visszakereshető** (3. fej.; visszautalás a 9. fejezetre).
- **Gépi tanulásos rendszer** — nem kap kész szabályokat, nagy történeti adatból statisztikai mintázatokat von ki (4. fej.).
- **Fekete doboz (black box)** — a mély tanulási (deep learning) rendszerek belső működése „nem emberi léptékben értelmezhető” — probléma az átláthatóság és elszámoltathatóság szempontjából (4. fej.). Analógia: több ezer összefonódó mérleg, nincs egyetlen, amit kicserélve megoldanád.
- **Adattorzítás** — a tanító adathalmazban bizonyos csoportok alul- vagy túlreprezentáltak; **algoritmikus torzítás** — maga a modell felépítése vagy súlyozási módja okozza (4. fej.). „A felelősség emberi marad — csak a hiba mechanizmusa más.”
- **Laudon hat klasszikus etikai elve** (Laudon 15. kiad., 4. fej.) — lásd Modellek B).
- **Felelősség (responsibility)** — annak elfogadása, hogy valaki viseli döntéseinek költségeit, kötelezettségeit és következményeit (6. fej.).
- **Elszámoltathatóság (accountability)** — rendszerek és intézmények jellemzője: mechanizmusok, amelyek lehetővé teszik megállapítani, ki tett valamit és ki felelős érte (6. fej.).
- **Jogi felelősség (liability)** — a felelősség kiterjesztése a jog területére: jogi keret, amelyben az egyének kártérítést követelhetnek elszenvedett károkért (6. fej.). Analógia: repülőgép-baleset — felelősség = aki hibázott; elszámoltathatóság = fekete doboz, karbantartási napló; jogi felelősség = kártérítés az áldozatok családjának.
- **Explainable AI (XAI)** — a magyarázhatóság technikai eszközei; a kötelező anyag csak megemlíti (ÜIA lecke, Opcionális Könyv) (6. fej.).
- **Alap-előfordulási gyakoriság (base rate)** — csoportonként eltérő alapgyakoriság; a méltányossági paradoxon feltétele (7. fej.).
- **Kalibráció** — a kockázati pontszám ugyanazt jelenti minden csoportra (7. fej.).
- **Osztályozási egyensúly** — a pozitív, ill. negatív besorolású egyének átlagos pontszáma csoportonként megegyezik (7. fej.).
- **Méltányossági paradoxon (Kleinberg, Mullainathan & Raghavan, 2016)** — eltérő base rate mellett nem létezik algoritmus, amely egyszerre kalibrált és osztályozásilag kiegyensúlyozott — kivéve, ha tökéletes az előrejelzés (7. fej.). „A méltányosság nem »megoldható« probléma — hanem tudatos kompromisszum.”
- **COMPAS** — amerikai bíróságokon használt szoftver a vádlottak visszaesési kockázatának becslésére (8. fej.).
- **EU AI Act** — 2024-ben elfogadott rendelet; a világ első átfogó, jogilag kötelező erejű AI-szabályozása; **kockázatalapú** megközelítés (9. fej.).
- **GPAI (általános célú AI-modellek)** — az AI Act V. fejezete (51–56. cikk), 2025 augusztusa óta kötelezi a fejlesztőket (OpenAI, Anthropic, Google): technikai dokumentáció, szerzői jogi megfelelési politika, nyilvános tanítóadat-összefoglaló (9. fej.).
- **AI energiaköltsége** — rövid lekérdezés kb. **0,4 Wh**, hosszú, összetett következtetés akár **33 Wh** → közel **80-szoros** különbség (Jegham et al. 2025, 30 nagy nyelvi modell benchmark) (10. fej.).

## Modellek és keretek

### A) Szabályalapú vs. gépi tanulásos torzítás (11. ea. 4. fej.)
| Szempont | Szabályalapú rendszer | Gépi tanulásos rendszer |
|---|---|---|
| A torzítás forrása | egy konkrét, valaki által megírt szabály | az adathalmaz statisztikai eloszlása |
| Visszakereshetőség | könnyű — megmutatható a hibás szabály | nehéz — több ezer súly együttes hatása |
| Szándékosság | általában tudatos (vagy hanyagság) | jellemzően nem szándékos, „örökölt” |
| Miért „fekete doboz”? | nem releváns — a logika olvasható | a belső működés nem emberi léptékben értelmezhető |
Példa a 3. fej.-ből: banki hitelbírálati szabály „25 év alattiak kockázati pontszáma +10 pont” — szabályalapúnál kideríthető, melyik sor okozza.

### B) Laudon hat etikai elve — alkalmazva a 97 %-os gépi látásos minőségellenőrzésre (11. ea. 5. fej.)
Helyzet: gépi tanulásos, gépi látáson alapuló minőségellenőrzés **97 %-os pontossággal**; a fennmaradó **3 %-ot senki nem ellenőrzi** emberi szemmel — ez a költségmegtakarítás lényege.
| Elv | Meghatározás | Alkalmazás |
|---|---|---|
| 1. **Aranyszabály** | tedd másokkal azt, amit szeretnél, hogy veled tegyenek | elfogadnád-e, hogy a te biztonságodat érintő terméket egy 3 %-os hibaarányú, felügyelet nélküli rendszer engedje át? |
| 2. **Kant kategorikus imperatívusza** | csak úgy cselekedj, hogy cselekvésed elve egyetemes törvénnyé válhasson | ha minden gyártó feladná az emberi ellenőrzést, elfogadható lenne-e társadalmi szinten? |
| 3. **Lejtő-elv (slippery slope)** | egy ártalmatlannak látszó lépés visszafordíthatatlan folyamatot indíthat | ma 3 %, holnap 5 %, ha még olcsóbb? |
| 4. **Utilitarista elv** | a legtöbb embernek a legtöbb hasznot hozó cselekvés | a megtakarítás hány munkahelyet ment meg — szemben a hibás termékek káraival? |
| 5. **Kockázatkerülési elv** | a legnagyobb kárt okozó lehetőséget kerüld, alacsony valószínűség esetén is | mi, ha a 3 %-ba biztonságkritikus alkatrész-hiba esik? |
| 6. **„Nincs ingyen ebéd” elv** | minden érték valakinek a tulajdona/munkája — felhasználásáért kompenzáció jár | a rendszer a minőségellenőrök történeti hibaadatain tanult — jár-e nekik elismerés/átképzés? |

### C) Felelősség – elszámoltathatóság – jogi felelősség + NAIH-eset (11. ea. 6. fej.)
- **Hazai eset — NAIH-85-3/2022 határozat:** egy hazai bank **közel négy éven át** AI-alapú **hangelemző rendszert** alkalmazott az ügyfélszolgálatra telefonálók hanghordozásának és érzelmi állapotának automatikus elemzésére. Bár a folyamat végén formálisan **emberi döntés** született, a NAIH szerint az adatkezelés joghatással bírhatott az érintettekre, és a bank **nem tájékoztatta megfelelően** az érintetteket az alkalmazott logikáról és következményeiről.
- Tanulság: **„végül egy ember dönt” önmagában nem old meg minden elszámoltathatósági problémát** — ha az ember nem érti/nem tudja megmagyarázni a rendszer javaslatának logikáját, az elszámoltathatóság sérül. „A rendszer magától tanulta, nem én programoztam bele” — nem elfogadható válasz.

### D) Méltányossági paradoxon és COMPAS (11. ea. 7–8. fej.)
- **ProPublica, 2016** (Angwin, Larson, Mattu, Kirchner — „Machine Bias”): azok közül, akik a következő két évben **nem** estek vissza, az **afroamerikai** vádlottak **45 %-át** tévesen sorolta magas kockázatúnak a COMPAS, a **fehér** vádlottaknál **24 %**.
- A fejlesztő válasza: az eltérés a két csoport eltérő alap-visszaesési arányából adódik — **technikailag igaza volt**: a rendszer **kalibrált** volt, csak nem volt egyben **osztályozásilag kiegyensúlyozott**. „Mindkét fél technikai szempontból igazat állított, mégis homlokegyenest ellenkező következtetésre jutott” — a Kleinberg-tétel gyakorlati megnyilvánulása.
- Üzenet (Amazon + COMPAS): „a méltányosság technikai garantálása korlátozott — az emberi felügyelet és a tudatos értékválasztás nem kiváltható.” Analógia: híd — teherbírás max., költség min., építési idő min. egyszerre nem lehet.

### E) EU AI Act kockázati kategóriák — magyar gyártó cég példáin (11. ea. 9. fej.)
| Kockázati kategória | Példa a gyártó cégnél | Következmény |
|---|---|---|
| **Minimális kockázat** | gépi látásos hibafelismerő rendszer a gyártósoron | nincs különös szabályozás |
| **Korlátozott kockázat** | ügyfélszolgálati chatbot | átláthatósági kötelezettség: jelezni kell, hogy AI-val kommunikál |
| **Magas kockázat** | automatizált toborzási/előszűrő rendszer (Amazon-eset), munkavállalói teljesítményértékelő AI | kockázatértékelés, dokumentáció, emberi felügyelet, átláthatóság kötelező |
| **Elfogadhatatlan kockázat** | munkavállalók valós idejű biometrikus viselkedés-megfigyelése a gyártócsarnokban | **tilos** |
- Szabályozási mozgás (a tananyag 2026 nyarán készült): a magas kockázatú kötelezettségek eredeti határideje **2026. augusztus 2.**, egy **2026 májusi** politikai megállapodás (Omnibus) **2027. december 2-ra** halasztja a toborzási/teljesítményértékelő rendszereknél. A **GPAI-kötelezettségeket** (V. fejezet, 51–56. cikk, 2025 augusztusa óta) **nem érinti** a halasztás.
- „Ki a »te« a táblázatban?” — a táblázat a **használó** vállalat rendszereinek besorolása; a **modellfejlesztőkre** külön, párhuzamos réteg vonatkozik.
- Reflektív: billentyűzet-aktivitás figyelése „termelékenységi” célból — melyik kategória? (a tananyag nyitva hagyja).

### F) Három védvonal — pro és kontra (11. ea. 11. fej.)
Védvonalak: **etikai elvek, elszámoltathatósági mechanizmusok, szabályozás.**
| ✅ Pro | ⚠ Kontra |
|---|---|
| az elvek döntési keretet adnak, amikor a jog még nem szabályoz | az elvek gyakran ellentmondanak egymásnak |
| az elszámoltathatóság visszakövethetővé teszi a hibát | a méltányossági paradoxon miatt az audit csak azt mutatja, melyik kritérium sérül |
| a szabályozás jogilag kikényszeríthető | a jogalkotás mindig lassabb, mint a technológia |
| együtt jelentősen csökkentik a kockázatot | együtt sem garantálják egy új, ismeretlen torzítási mintázat időbeni felismerését |
**Műszaki-menedzseri szemszög — a négy helyes kérdés:** Milyen adaton tanult a rendszer? Ki tudja megmagyarázni a döntéseit? Milyen kockázati kategóriába esik? Milyen emberi felügyeletet igényel? Következő fejezet: AI- és digitalizációs stratégia beruházás-gazdaságossági szempontból.

## Számok, dátumok, nevek, amiket a tananyag kiemel

| Mi | Érték | Hol |
|---|---|---|
| Amazon toborzási AI | 2014 indul; 2015 kiderül; 100 → 5 önéletrajz; 10 év tanítóadat; „women's”; „executed”, „captured”; leállítva | 2. fej. |
| Forrás | Dastin, J. (2018), Reuters | 2., 4. fej. |
| Hitelbírálati példa | 25 év alatt +10 pont | 3. fej. |
| Gépi látásos minőségellenőrzés | 97 % pontosság; 3 % ellenőrizetlen; lejtő: 5 % | 5. fej. |
| Etikai elvek | 6 (Laudon 15. kiad., 4. fej.) | 5. fej. |
| Három összekevert fogalom | responsibility, accountability, liability | 6. fej. |
| NAIH-határozat | NAIH-85-3/2022; hazai bank; ~4 év; hangelemzés | 6. fej. |
| Kleinberg, Mullainathan, Raghavan | 2016 (arXiv:1609.05807; ITCS 2017) | 7., 12. fej. |
| ProPublica COMPAS | 2016; Angwin, Larson, Mattu, Kirchner; 45 % vs. 24 % | 8. fej. |
| EU AI Act | 2024 elfogadva; 4 kockázati kategória | 9. fej. |
| Határidő-halasztás | 2026. 08. 02. → 2027. 12. 02. (2026 májusi megállapodás, Gibson Dunn 2026) | 9. fej. |
| GPAI | V. fejezet, 51–56. cikk; 2025 augusztusa óta; Article 53 | 9. fej. |
| AI energia | 0,4 Wh vs. 33 Wh; ~80× (Jegham et al. 2025, 30 LLM) | 10. fej. |
| LinkedIn Talent Search | 2018 körül; Geyik, Ambler, Kenthapadi, KDD '19 | 11. fej. |
| Védvonalak | 3 (etikai elvek, elszámoltathatóság, szabályozás) | 11. fej. |
| Elmélyítő | Fabris et al. 2024 (ACM TIST); WP251; Csatlós E. 2023 (Pro Futuro) | 12. fej. |

## Számítások

Képlet nincs; a tananyag számaiból:
- **AI energia:** 33 / 0,4 = **82,5** → „közel 80-szoros” különbség. „Mi változik, ha…”: 10 000 rövid lekérdezés/nap = 4 kWh; ugyanannyi összetett = 330 kWh/nap — a feladattípus megválasztása üzleti és fenntarthatósági döntés (10. fej. tanulsága).
- **COMPAS hamis pozitív arányok:** afroamerikai 45 % vs. fehér 24 % a nem visszaesők között → 1,9-szeres különbség a téves magas-kockázat besorolásban; a fejlesztő szerint a **kalibráció** teljesült (azonos pontszám = azonos tényleges visszaesési valószínűség minden csoportra), az **osztályozási egyensúly** nem — a Kleinberg-tétel szerint eltérő base rate mellett a kettő egyszerre nem teljesíthető.
- **Minőségellenőrzés 3 %:** 100 000 db/hó termelésnél 3000 db ellenőrizetlen; ha ezek 1 %-a biztonságkritikus hiba → 30 db hibás termék a piacon havonta (saját számok) — ez a kockázatkerülési elv kérdése. Ha a lejtő-elv szerint 5 %-ra nő: 5000 ellenőrizetlen → 50 hibás.
- **Amazon:** 100 önéletrajzból 5 — 5 %-os átengedési arány; tíz év férfi-dominanciájú adat → a „women's” szó negatív súlyt kapott (a tananyag nem ad számszerű torzítást).

## Összekeverhető párok / „mi NEM igaz” csapdák

1. **Az Amazon-AI-t megtanították a nők hátrányos kezelésére?** NEM — a tíz év férfi-dominanciájú adatból „örökölte”; adattorzítás, nem szándékos.
2. **Sikerült kijavítani?** NEM — nem tudták garantálni, hogy rejtettebb módon nem torzít → leállították. (LinkedIn viszont javította és publikálta.)
3. **Szabályalapú vs. ML torzítás:** szabály = konkrét sor, visszakereshető, tudatos/hanyag; ML = adateloszlás, nehéz, örökölt, fekete doboz.
4. **Adattorzítás vs. algoritmikus torzítás:** adat = alul/túlreprezentált csoportok; algoritmikus = a modell felépítése/súlyozása.
5. **A hat elv neve és sorrendje:** aranyszabály; Kant kategorikus imperatívusza; lejtő-elv; utilitarista; kockázatkerülési; „nincs ingyen ebéd”. (Laudon 15. kiad. 4. fej.) Kockázatkerülés ≠ utilitarizmus: a legnagyobb kárt kerüli alacsony valószínűségnél is vs. legtöbb haszon a legtöbbnek.
6. **Felelősség / elszámoltathatóság / jogi felelősség:** responsibility = viselem a következményeket; accountability = mechanizmus, amivel kideríthető, ki tette; liability = kártérítés joga.
7. **„A végén ember dönt” elég?** NEM — NAIH-eset: ha az ember nem érti a logikát, az elszámoltathatóság sérül; tájékoztatási kötelezettség.
8. **Kalibráció vs. osztályozási egyensúly:** kalibráció = a pontszám ugyanazt jelenti minden csoportra; egyensúly = a pozitív/negatív besoroltak átlagpontszáma csoportonként egyenlő. COMPAS: kalibrált volt, egyensúly nem.
9. **COMPAS: a ProPublica vagy a fejlesztő hazudott?** Egyik sem — mindkettő technikailag igaz (paradoxon).
10. **A méltányosság technikailag megoldható?** NEM — tudatos kompromisszum; kivétel: tökéletes előrejelzés.
11. **EU AI Act kategóriái (4):** minimális (gépi látás a soron); korlátozott (chatbot — átláthatóság); magas (toborzás, teljesítményértékelés — kockázatértékelés, dokumentáció, emberi felügyelet); elfogadhatatlan (valós idejű biometrikus megfigyelés — tilos).
12. **Az Amazon-rendszer ma melyik kategória?** Magas kockázat.
13. **Halasztás 2027. 12. 02. mindenre vonatkozik?** NEM — a toborzási/teljesítményértékelő magas kockázatú kötelezettségekre; a GPAI-kötelezettségek (2025. aug. óta) érintetlenek.
14. **Az AI Act a világ első átfogó, jogilag kötelező AI-szabályozása** — 2024.
15. **AI energiaköltség egyforma?** NEM — 0,4 Wh vs. 33 Wh, ~80×.
16. **Három védvonal garantálja a biztonságot?** NEM — együtt csökkentik a kockázatot, de nem garantálják új torzítási minta felismerését.
17. **A műszaki menedzser feladata AI-algoritmust írni?** NEM — a helyes négy kérdést feltenni.

## Kapcsolat más előadásokkal

- Szakértői rendszer, IF-THEN, fekete doboz vs. magyarázhatóság, hibrid AI, RAG (9. ea.) — a tananyag kifejezett „retrieval”-ja.
- Target terhesség-előrejelzés, hamis pozitív/negatív, „mit szabad megjósolni” (7. ea. 7. fej.) → itt a magas kockázatú/felvételi/hitelbírálati algoritmusok.
- Hitelbírálat/scoring (7. ea. 6. fej.) ↔ hitelbírálati szakértői rendszer torzítása (3. fej.).
- AI-döntéstámogatás kockázatai: bias, átláthatóság hiánya, etika (6. ea. 6. fej.); Goodhart az AI-ban (6. ea. 3. fej.); automation bias / algoritmus-averzió (5. ea.).
- CPO/adatvédelem (4. ea.) ↔ NAIH-határozat; GDPR-logika.
- AI mint helyettesítő/belépési korlát (2. ea. 10. fej.); „AI felerősíti a jó és a rossz adatstratégiát” (8–9. ea.) ↔ „nagyobb léptékben termeli újra a hibás mintázatot”.
- Felhő-döntés mint üzleti és fenntarthatósági döntés (10. ea.) ↔ AI energiaköltsége.
- Következő (12. ea.): AI- és digitalizációs stratégia, beruházás-gazdaságosság, digitális jövő.

## Fogalomtár-jelöltek

- **Adattorzítás** – data bias – alul-/túlreprezentált csoportok a tanítóadatban.
- **Algoritmikus torzítás** – algorithmic bias – a modell felépítéséből/súlyozásából eredő torzítás.
- **Fekete doboz** – black box – nem emberi léptékben értelmezhető belső működés (deep learning).
- **Felelősség** – responsibility – a döntés következményeinek viselése.
- **Elszámoltathatóság** – accountability – mechanizmus annak megállapítására, ki tett mit.
- **Jogi felelősség** – liability – kártérítés követelésének jogi kerete.
- **Magyarázható AI** – Explainable AI (XAI) – a döntések magyarázhatóságának technikai eszközei.
- **Aranyszabály** – Golden Rule – tedd másokkal, amit magadnak kívánsz.
- **Kategorikus imperatívusz** – Kant's categorical imperative – csak egyetemessé tehető elv szerint cselekedj.
- **Lejtő-elv** – slippery slope – ártalmatlan lépés visszafordíthatatlan folyamatot indíthat.
- **Utilitarista elv** – utilitarian principle – legtöbb haszon a legtöbb embernek.
- **Kockázatkerülési elv** – risk aversion principle – a legnagyobb kár kerülése alacsony valószínűségnél is.
- **„Nincs ingyen ebéd”** – no free lunch rule – minden érték valakié, kompenzáció jár.
- **Alapgyakoriság** – base rate – csoportonkénti alap-előfordulási arány.
- **Kalibráció** – calibration – a pontszám jelentése csoportfüggetlen.
- **Osztályozási egyensúly** – classification balance – pozitív/negatív besoroltak átlagpontszáma csoportonként egyenlő.
- **Méltányossági paradoxon** – fairness impossibility (Kleinberg et al. 2016) – kalibráció és egyensúly egyszerre nem teljesíthető eltérő base rate mellett.
- **COMPAS** – COMPAS – visszaesési kockázatbecslő szoftver; ProPublica 45 % vs. 24 %.
- **EU AI-rendelet** – EU AI Act (2024) – kockázatalapú, négy kategória; GPAI-kötelezettségek.
- **Általános célú AI-modell** – GPAI – a modellfejlesztőkre vonatkozó külön szabályozási réteg (51–56. cikk).

---

# 12. előadás: Kiberbiztonság, digitális transzformáció és a MIR jövője

⚠ forrásmegjegyzés: az adatlap 11. heti „E-kereskedelem és platform-gazdaság” előadásának nincs megfelelő Moodle-fejezete a 12 kötelező fájl között (a platform-gazdaság a 2. ea. 7. fej.-ben, a B2B piacterek a 3. ea. 8. fej.-ben szerepelnek); a Moodle 11. = Etika, 12. = Kiberbiztonság/digitális transzformáció (adatlap 12–13. hét).

## Egy mondatban (a központi tézis)

A kiberbiztonsági beruházás **nem „biztonsági kiadás”, hanem kockázatkezelési döntés** ugyanazzal a logikával, mint bármely IT-beruházás (TCO, ROI, NPV, IRR, FAIR, Gordon–Loeb); a digitális transzformáció sikere **kontextusfüggő** (érettség, kultúra, folyamat) — az AI csak ott gyorsít, ahol megvan az alap, másutt torzít és szélesíti a szakadékot; a műszaki menedzser feladata **a helyes kérdéseket feltenni és az igazolt állítást a közhelytől megkülönböztetni** (12. ea. 3., 4., 6., 10. fej.).

## Nyitó eset és feloldása (12. ea. 2. fej.)

**„A digitális transzformációk 70 %-a kudarcot vall” — vagy mégsem?** Szinte minden cikk, konferencia és tanácsadói jelentés idézi, a hivatkozás „szinte mindig a McKinsey-hez vezet”. **Hughes, M. (2011, Journal of Change Management)** lektorált cikke szisztematikusan végignézte a forrásokat: **nem talált mögötte empirikus tanulmányt**; a nyom egy **1993-as Hammer & Champy-könyvhöz** vezet, ahol a szerzők maguk nevezték **„tudománytalan becslésnek”**. A McKinsey 2015-ös és 2020-as cikkei egymásra és egy **Forbes-publicisztikára** hivatkoznak, nem mérési adatra. (Statisztika-nyomkövetés: reliamag.com.)
- **Mi ment rosszul:** vezetői döntést sosem igazolt statisztikára alapozni = nem felelős döntéshozatal. Analógia: alkatrész-adatlap teljesítményértéke ismeretlen tesztkörülmények között — a mérnök ellenőrzi a mérési módszertant.
- **Elméleti pont:** forráskritika mint a félév kritikai gondolkodásának része (10. fej.: „meg tudd különböztetni az igazolt állítást a közhelytől”).
- **Záró visszatérés (10. fej.):** „a félév elején (1. fejezet) egy nyitó dilemmával indultunk — idézd fel” → Hershey (1. ea.): big bang, menedzsment-kudarc, komplementer eszközök hiánya.

## Fogalmak és definíciók (HU – EN)

- **Cost of breach** — a biztonsági incidens pénzügyi, reputációs és jogi dimenziói (ÜIA-ból ismert; Maersk/NotPetya-eset — a tananyag nem ismétli) (3. fej.).
- **FAIR — Factor Analysis of Information Risk** — elismert kockázatelemzési szabvány (FAIR Institute, Standard v3.0, 2025): a kockázatot **elsődleges veszteségre** (közvetlen: helyreállítás, javítás, közvetlen bevételkiesés) és **másodlagos veszteségre** (közvetett: reputációs kár, ügyfélvesztés, versenyhátrány, bírságok) bontja; nyilvános, ügyfeleket érintő incidensnél a másodlagos gyakran meghaladja az elsődlegest (3. fej.).
- **TCO** — teljes tulajdonlási költség: nem csak vételár, hanem üzemeltetés, karbantartás, képzés (4. fej.).
- **ROI** — megtérülési ráta (4. fej.).
- **NPV** — nettó jelenérték, a pénz időértékét figyelembe véve (4. fej.).
- **IRR** — belső megtérülési ráta: az a diszkontráta, amely mellett a projekt NPV-je pontosan nulla; „különösen hasznos, ha több beruházási lehetőséget kell rangsorolni” (4. fej.).
- **Kvantifikált kockázatértékelés (FAIR)** — teljes várható éves veszteség = bekövetkezési valószínűség × (elsődleges kár + másodlagos kár) (4. fej.).
- **Gordon–Loeb modell (2002)** — az optimális védelmi beruházás (z*) sosem haladja meg a várható veszteség **1/e-ed részét (kb. 37 %)** (4. fej.).
- **FMEA (Failure Mode and Effects Analysis)** — mérnöki analógia a FAIR + Gordon–Loeb logikára, csökkenő hozadékú védelmi költséggel (4. fej.).
- **Digitális érettségi önértékelés (Kane et al. 2017, MIT SMR/Deloitte)** — 3500+ vezető felmérése; állítások 1–10-ig; átlag = szervezeti pontszám; sávok: **kezdő 1–3 / fejlődő 4–6 / érett 7–10** (5. fej.).
- **Digital Readiness Level (drl-tool.org)** — három pillér (**Leadership / Technology / Value**), nyolcfokozatú létra (5. fej.).
- **AI mint a digitalizáció „enablere”** — nem párhuzamos jelenség, hanem beágyazott elem, mint a felhő vagy az IoT; klasszikus AI/ML (predikció, osztályozás, anomália-felismerés) magas digitális érettséget feltételez (6. fej.).
- **GenAI kétrétegű képe** — alapszinten demokratizál (OECD 2025: csökkentette a belépési küszöböt a kisebb cégeknek), mélyszinten ugyanaz az érettségi követelmény: „az ágensalapú AI nem pótolja a hiányzó digitális alapokat” (6. fej.).
- **Termelékenységi paradoxon (Brynjolfsson 1993)** — az IT-beruházás nem automatikusan termel produktivitás-növekedést; ma az AI-ra és a digitalizációra is felmerül (6. fej.).
- **Moderate Innovator** — Magyarország besorolása a European Innovation Scoreboard-on (2026. július 9.); 2025: **39,6 %** „innovációs potenciállal rendelkező, de nem innováló” (7. fej.).
- **KKV-tipológia** (Vodafone Policy Paper 2020) — öt típus: **Fadeaways, Reinventors, Adaptors, Windfallers, Digital Dynamos** (7. fej.).
- **Digitarthatóság** (Saáry, Kárpáti-Daróczi & Tick 2022, 2023) — az az állapot, ahol a digitalizáció és a fenntarthatóság nem egymás rovására valósul meg; két klaszter: **„Aggódó Elkötelezettek”** (mindkettőre törekszenek) és **„Közömbös Konzervatívok”** (egyiken sem mozdulnak) (7. fej.).
- **Digitális szakadék három szintje** (Van Deursen & Helsper 2015) — első: hozzáférés; második: készségek és használat; harmadik: eredmények és előnyök (8. fej.). EU 2023: a polgárok **46 %-ának** hiányoztak az alapvető digitális készségei.
- **Ipar 4.0 döntési keret** — nyolc tipikus kihívás és megoldási irány (9. fej.).
- **10 lépéses gyakorlati keret** (10. fej.) — lásd Modellek.

## Modellek és keretek

### A) Kiberbiztonság mint beruházási döntés (12. ea. 3. fej.)
Dilemma: (A) **8 millió Ft** hálózati szegmentáció (zsarolóvírus terjedésének korlátozása gyártósorok között) vs. (B) ugyanennyi kapacitásbővítésbe. A döntéshozó B-re hajlik („látható” hozam), A hozama „csak akkor látszik, ha nem történik baj”. Analógia: híd biztonsági tartaléka — kiszámolt terhelés és valószínűség, nem „jó dolog”.

### B) FAIR kvantifikált kockázatértékelés és Gordon–Loeb (12. ea. 4. fej.) — lásd Számítások
| Védelem költsége a teljes várható veszteséghez képest | Értékelés |
|---|---|
| **≤ 37 %** | egyértelműen ésszerű befektetés |
| **37–100 %** | vitatható — egyedi mérlegelés (szabályozói elvárás, márkakockázat) |
| **> 100 %** | gazdaságilag nem indokolható |
ERP-dilemma: (A) olcsóbb, korlátozott vs. (B) drágább, skálázható — a vételár-összehasonlítás félrevezető, a **3–5 éves TCO** gyakran megfordítja a sorrendet.

### C) Digital Readiness Level — nyolc fokozat (12. ea. 5. fej.)
| Szint | Gyakorlatban |
|---|---|
| 1. Digital Outsider | papíralapú nyilvántartás |
| 2. Digital Rookie | Excel-táblák, e-mail, nincs egységes rendszer |
| 3. Digital Novice | alapszintű vállalatirányítási szoftver |
| 4. Digital Explorer | integrált rendszer egy-két területen |
| 5. Digital Adopter | több terület összekapcsolva |
| 6. Digital Leader | valós idejű adatok, folyamatautomatizálás |
| 7. Digital Expert | prediktív elemzés, AI-alapú döntéstámogatás |
| 8. Digital Champion | teljesen adatvezérelt szervezet |
Dilemma: Digital Rookie szintű KKV prediktív karbantartást akar → nem a technológia elvetése, hanem **a sorrend megváltoztatása**: előbb alapszintű digitalizáció (adatgyűjtés, folyamat-egységesítés). Rookie → Expert közvetlenül = „2. osztályos tanuló egyetemi kurzuson”; „nem telepítesz robotkart olyan sorra, ahol az alapvető minőségellenőrzés sincs szabványosítva”.

### D) AI és digitalizáció viszonya (12. ea. 6. fej.)
- Klasszikus AI: csak ott gyorsít, ahol megvan az alap (strukturált adat, adatinfrastruktúra, elemzők).
- GenAI: felhőalapú, természetes nyelvi felület, technikai szakértelem nélkül → alacsonyabb érettségű KKV is profitálhat alapszintű feladatokra; de specializált alkalmazásnál ugyanaz a korlát.
- Alacsony érettség + AI = **torzít, nem gyorsít**; magas érettség + AI = **katalizátor** — „ugyanaz az AI homlokegyenest ellentétes hatást válthat ki, attól függően, hova érkezik.”
- **Digitális szakadék erősödése:** az AI nem csökkenti, hanem erősítheti — az érettek gyorsulnak, a lemaradók lemaradnak. Ábra: **BCG 2025 „Widening AI Value Gap”** — future-built **5 %** / scalers **35 %** / laggards **60 %**; bevételnövekedés **1,7×**.
- Analógia: erősebb motor gyenge alvázban → törés; kisebb kiegészítő alkatrész a gyengébb alvázon is működik.

### E) Magyar KKV-k (12. ea. 7. fej.)
Elsődleges gátló tényező (hazai kutatás, Garai-Fodor, Varga & Csiszárik-Kocsir 2023): **nem a digitális készségek hiánya**, hanem **információhiány, szakképzett munkaerő hiánya, pénzügyi korlátok** → a beavatkozási pont: információs csatornák nyitása és finanszírozási út, nem (csak) képzés. KKV-tipológia 5 típus; digitarthatóság 2 klaszter; analógia: Pareto-optimális egyensúly két versengő paraméter között; ábra: 2×2 mátrix (digitalizáció × fenntarthatóság).

### F) Digitális szakadék (12. ea. 8. fej.)
Három szint (Van Deursen & Helsper 2015; OECD Education Working Papers No. 299, 2023) — szűkülő tölcsér. Korrelációs pont: magas digitalizációs szintű KKV-nál valószínűtlen az alacsony munkaerő-digitális-érettség — a kettő kölcsönösen erősíti/hiányolja egymást. Visszautalás a 9. fejezetre (KM és AI változtatja a munkakörök kompetencia-elvárásait); a szakadék ennek társadalmi ára: kiszorulás munkakörökből, szolgáltatásokból, állampolgári jogokból. Menedzseri felelősség: teljesen digitális ügyfélszolgálat → kiszoruló csoportok.

### G) Ipar 4.0 — nyolc kihívás és megoldási irány (12. ea. 9. fej.; Tick A. 51. dia)
1. ellenállás a változással szemben → erős vezetői kommunikáció
2. digitális készséghiány → képzési program
3. örökölt rendszerek → fokozatos átállás
4. adatbiztonsági aggály → robusztus biztonsági intézkedések
5. költségvetési korlát → prioritás-alapú befektetés
6. stratégia hiánya → ütemterv
7. kulturális ellenállás → vezetői példamutatás
8. szállítóválasztás → alapos kiértékelés, pilot projekt
Melyik technológia először (AI-prediktív elemzés / digitális iker / IoT+Big Data / blockchain-ellátási lánc)? **Kontextusfüggő**: digitális érettség, iparági kontextus, a legnagyobb azonnal kezelhető akadály. Analógia: szűk keresztmetszet — nem a legmodernebbé tehető gépet fejleszted, hanem ami korlátoz.

### H) A 10 lépéses gyakorlati keret (12. ea. 10. fej.)
(1) digitális érettség felmérése → (2) célok kitűzése → (3) digitalizációs stratégia → (4) megfelelő technológia kiválasztása → (5) munkavállalói képzés és változáskezelés → (6) adatbiztonság és megfelelés → (7) ügyfélélmény-fejlesztés → (8) monitorozás és optimalizálás → (9) partnerségek és együttműködés → (10) rendszeres felülvizsgálat és adaptáció.

### I) Kritikai záróértékelés (12. ea. 10. fej.)
| ✅ Pro | ⚠ Kontra |
|---|---|
| módszertani eszközök (TCO, ROI, IRR, kockázatszámítás, érettségi modellek) számszerűsíthető alapot adnak | egyik módszer sem garantálja a sikert — a termelékenységi paradoxon mindig fennáll |
| kritikai gondolkodás (statisztika-ellenőrzés, forráskritika) végigkísérte a félévet | a döntéshozók időnyomás alatt, hiányos információval dolgoznak |
| a technológia hatása kontextusfüggő (érettség, kultúra, folyamat) | bonyolultabb döntéshozatal, nincs egyszerű recept |
Műszaki-menedzseri szemszög: nem minden technológiát a legmélyebb szinten ismerni, hanem **helyes kérdéseket feltenni, igazolt állítást közhelytől megkülönböztetni, tudni, mikor kell szakértőt bevonni.**

## Számok, dátumok, nevek, amiket a tananyag kiemel

| Mi | Érték | Hol |
|---|---|---|
| „70 % kudarc” mítosz | Hughes 2011 (J. of Change Management); Hammer & Champy 1993 „tudománytalan becslés”; McKinsey 2015, 2020; Forbes | 2. fej. |
| Szegmentációs projekt | 8 M Ft (A) vs. kapacitásbővítés (B) | 3. fej. |
| FAIR | Standard v3.0 (2025); elsődleges/másodlagos veszteség | 3–4. fej. |
| FAIR példa 1 | belső leállás: évi 4×; 200 000 + ~50 000 Ft → 1 000 000 Ft/év | 4. fej. |
| FAIR példa 2 | nyilvános DDoS: 10 évente 1×; 15 M + ~35 M Ft → 5 000 000 Ft/év | 4. fej. |
| Gordon–Loeb | 2002, ACM TISSEC 5(4), 438–457; z* ≤ (1/e)·v·p·ℓ; 1/e ≈ 37 % | 4. fej. |
| Védelmi sávok | ≤37 % / 37–100 % / >100 % | 4. fej. |
| TCO távlat | 3–5 év | 4. fej. |
| Kane et al. | 2017, MIT SMR/Deloitte; 3500+ vezető; 1–10 skála; sávok 1–3 / 4–6 / 7–10; fiktív KKV 3,8 | 5. fej. |
| Digital Readiness Level | 3 pillér; 8 fokozat (Outsider → Champion) | 5. fej. |
| OECD | 2025, AI adoption by SMEs | 6. fej. |
| BCG 2025 | future-built 5 % / scalers 35 % / laggards 60 %; 1,7× bevételnövekedés | 6. fej. |
| Brynjolfsson | 1993 productivity paradox | 6. fej. |
| European Innovation Scoreboard | 2026. 07. 09.; Moderate Innovator; 39,6 % (2025) | 7. fej. |
| KKV-tipológia | 5 típus (Vodafone 2020) | 7. fej. |
| Digitarthatóság | Saáry, Kárpáti-Daróczi & Tick 2022, 2023; Információs Társadalom 23(1), 40–60 | 7., 11. fej. |
| Digitális szakadék | 3 szint (Van Deursen & Helsper 2015); EU 2023: 46 % | 8. fej. |
| Ipar 4.0 kihívások | 8 | 9. fej. |
| Gyakorlati keret | 10 lépés | 10. fej. |
| Elmélyítő: Kalender & Žilka | 2024, Procedia Computer Science 232, 903–912 | 11. fej. |

## Számítások (12. ea. 4. fej.) — FAIR várható veszteség és Gordon–Loeb

### 1. FAIR — teljes várható éves veszteség
**Képlet (a tananyag szerint):** Teljes várható éves veszteség = bekövetkezési valószínűség (gyakoriság) × (elsődleges kár + másodlagos kár)

**A tananyag két forgatókönyve végigszámolva:**
| Forgatókönyv | Gyakoriság | Elsődleges | Másodlagos | Számítás | Várható éves veszteség |
|---|---|---|---|---|---|
| Belső, nem nyilvános rendszerleállás | évi 4× | 200 000 Ft | ~50 000 Ft (alacsony láthatóság) | 4 × (200 000 + 50 000) = 4 × 250 000 | **1 000 000 Ft** |
| Nyilvános, ügyfeleket érintő incidens (DDoS) | 10 évente 1× = 0,1/év | 15 000 000 Ft | ~35 000 000 Ft (magas láthatóság) | 0,1 × (15 M + 35 M) = 0,1 × 50 M | **5 000 000 Ft** |

**Értelmezés:** a ritka, nyilvános incidens várható éves vesztesége **ötször** nagyobb, mint a gyakori belső leállásé, és ott a **másodlagos kár (35 M) több mint kétszerese az elsődlegesnek (15 M)** — „a puszta helyreállítási költség félrevezetően alacsonynak tűnhet”. Ha csak elsődleges kárral számolnánk: DDoS 0,1 × 15 M = 1,5 M Ft/év — a kockázat **70 %-át** alábecsülnénk.

### 2. Gordon–Loeb — optimális védelmi beruházás
**Képlet:** z* ≤ (1/e) × v × p × ℓ, ahol v = sebezhetőség (sikeres áttörés valószínűsége a jelenlegi védelem mellett, 0–1), p = a támadás bekövetkezésének valószínűsége, ℓ = a kár mértéke (FAIR elsődleges + másodlagos); **v × p × ℓ = a teljes várható veszteség**; 1/e ≈ 0,368 ≈ **37 %**.

**Mintapélda a tananyag számaival:** a DDoS-forgatókönyv várható éves vesztesége 5 000 000 Ft → z* ≤ 0,37 × 5 000 000 = **1 850 000 Ft/év** az ésszerű felső védelmi ráfordítás. A belső leállásnál: 0,37 × 1 000 000 = **370 000 Ft/év**. A két forgatókönyvre együtt (6 M Ft várható veszteség): z* ≤ **2,22 M Ft/év**.

**A 8 M Ft-os szegmentációs projekt (3. fej.) értékelése:** ha a projekt egyszeri 8 M Ft, és 5 évre vetítve 1,6 M Ft/év, az a 6 M Ft/év teljes várható veszteség **27 %-a** → „≤ 37 %: egyértelműen ésszerű befektetés”. Ha csak az elsődleges károkkal számolnánk (4×200 000 + 0,1×15 M = 2,3 M Ft/év), 1,6/2,3 = **70 %** → „vitatható” sáv — ezért nem szabad a másodlagos kárt kihagyni (a tananyag reflektív kérdésének válasza).

**Explicit v·p·ℓ példa (saját számok):** v = 0,5 (a jelenlegi védelem mellett a támadások fele sikeres), p = 0,2/év, ℓ = 50 M Ft → várható veszteség = 0,5 × 0,2 × 50 M = 5 M Ft → z* ≤ 1,85 M Ft.

**„Mi változik, ha…”:**
- Ha a sebezhetőség v a szegmentáció után 0,5-ről 0,1-re csökken: várható veszteség 5 M → 1 M Ft → a következő védelmi beruházás plafonja már csak 370 000 Ft — **csökkenő hozadék** (FMEA-analógia).
- Ha a másodlagos kárt 35 M helyett 0-nak vesszük: DDoS várható veszteség 1,5 M → a védelmi plafon 555 000 Ft — alulvédés.
- Ha a védelem költsége a várható veszteség > 100 %-a (pl. 7 M Ft/év a 6 M-ra): „gazdaságilag nem indokolható”, kivéve szabályozói/márkaérv (37–100 % sáv feletti).

### 3. TCO / ROI / NPV / IRR (12. ea. 4. fej. definíciói) — példa
ERP (A) vételár 20 M Ft, éves üzemeltetés+karbantartás+képzés 8 M; (B) 35 M Ft, évi 4 M (saját számok). 5 éves TCO: A = 20 + 5×8 = **60 M**; B = 35 + 5×4 = **55 M** → „a TCO-számítás 3–5 éves távlatban gyakran megfordítja a sorrendet”. IRR: ha két projekt közül kell választani, a magasabb IRR-ű rangsorolódik előre (a tananyag: „különösen hasznos, ha több beruházási lehetőséget kell rangsorolni”); NPV-képlet és példa az 1. ea. Számítások részében.

## Összekeverhető párok / „mi NEM igaz” csapdák

1. **„70 % kudarc” = McKinsey empirikus adat?** NEM — Hughes 2011: nincs empirikus tanulmány; Hammer & Champy 1993 „tudománytalan becslés”.
2. **Kiberbiztonság = biztonsági kiadás?** NEM — kockázatkezelési döntés, mint bármely IT-beruházás.
3. **Elsődleges vs. másodlagos veszteség (FAIR):** elsődleges = helyreállítás, javítás, közvetlen bevételkiesés; másodlagos = reputáció, ügyfélvesztés, versenyhátrány, bírság. Nyilvános incidensnél a másodlagos gyakran nagyobb.
4. **FAIR képlet:** valószínűség × (elsődleges + másodlagos) — nem csak elsődleges.
5. **Gordon–Loeb 37 %:** 1/e-ed rész a **várható veszteségnek**, nem a bevételnek/IT-büdzsének; z* felső korlát („sosem haladja meg”).
6. **Sávok:** ≤37 % ésszerű; 37–100 % vitatható; >100 % nem indokolható.
7. **IRR vs. NPV:** IRR = diszkontráta, ahol NPV = 0, rangsoroláshoz; NPV = pénzösszeg.
8. **Kane et al. sávok (1–3 / 4–6 / 7–10) vs. DRL 8 fokozat** — két különböző modell; DRL 3 pillére: Leadership/Technology/Value.
9. **DRL sorrend:** Outsider → Rookie → Novice → Explorer → Adopter → Leader → Expert → Champion. Rookie = Excel/e-mail; Novice = alapszintű VIR; Expert = prediktív/AI; Champion = teljesen adatvezérelt.
10. **Digital Rookie prediktív karbantartást akar — elvetni?** NEM — a sorrendet változtatni: előbb alapok.
11. **AI = párhuzamos jelenség a digitalizációval?** NEM — beágyazott enabler, mint felhő/IoT.
12. **GenAI megszünteti az érettségi korlátot?** Részben: alapszinten demokratizál, mélyszinten nem („az ágensalapú AI nem pótolja a hiányzó digitális alapokat”).
13. **AI csökkenti a digitális szakadékot?** NEM — erősítheti (BCG: 5/35/60 %).
14. **Magyar KKV fő akadálya a digitális készség?** NEM — információhiány, szakképzett munkaerő, pénzügy (ugyanaz, mint 4. ea. 8. fej.).
15. **KKV-tipológia 5 típusa** (Fadeaways, Reinventors, Adaptors, Windfallers, Digital Dynamos) ≠ **digitarthatóság 2 klasztere** (Aggódó Elkötelezettek, Közömbös Konzervatívok).
16. **Digitális szakadék szintjei:** 1. hozzáférés; 2. készségek/használat; 3. eredmények/előnyök — nem „eszköz, internet, mobil”.
17. **Magyarország EIS-kategória:** Moderate Innovator (2026); 39,6 % potenciállal rendelkező, de nem innováló (2025).
18. **Nyolc Ipar 4.0 kihívás párosítása:** változás-ellenállás → vezetői kommunikáció; kulturális ellenállás → vezetői példamutatás (két külön tétel!); szállítóválasztás → pilot.
19. **A módszerek garantálják a sikert?** NEM — a termelékenységi paradoxon mindig fennáll.

## Kapcsolat más előadásokkal

- Hershey nyitó dilemma (1. ea.) — a 12. ea. 10. fej. visszautal rá; komplementer eszközök, termelékenységi paradoxon (Brynjolfsson 1993, 1. ea. 6., 9. fej.) ↔ 6. fej.; McKinsey „Unlocking success” (1. ea. 9. fej. szerint „releváns a 12. fejezethez”).
- TCO/ROI/NPV/IRR (1. ea. 7. fej.; 8. ea. 9. fej.; 10. ea. 8. fej.) ↔ 4. fej. definíciók; TCO 3–5 év; ERP A/B dilemma ↔ 3. ea. build/buy.
- CSO/CISO (4. ea.), BYOD-biztonság, CISO felelősség (10. ea.) ↔ kiberbiztonság mint beruházás.
- Big Data érettségi modell (8. ea. 8. fej.), BI-érettség/BICC (5. ea.) ↔ Kane és DRL; „előbb alapok” ↔ 8. ea. „KKV a 3. lépéssel kezdjen”.
- AI felerősíti a jó és a rossz adatstratégiát (8–9. ea.) ↔ „torzít, nem gyorsít” alacsony érettségnél; GenAI (9. ea. RAG).
- KKV-kutatás: információhiány (4. ea. 8. fej.) ↔ 7. fej.; Tick A. V4 KKV Ipar 4.0 (4. ea. 9. fej. elmélyítő).
- Munkaerő-kompetencia, nyugdíjba vonuló mérnökök, Business Fest 2026 (9. ea.) ↔ digitális szakadék.
- Szervezeti ellenállás, változásmenedzsment (1. ea. 5. fej.) ↔ Ipar 4.0 kihívások 1. és 7.; fokozatos átállás ↔ 3. ea. phased.
- Etika/AI Act (11. ea.) ↔ adatbiztonság és megfelelés (10 lépés 6. pontja); digitális ügyfélszolgálat kiszoruló csoportjai.

## Fogalomtár-jelöltek

- **Incidens költsége** – cost of breach – pénzügyi, reputációs, jogi dimenziók.
- **Információs kockázat faktoranalízise** – FAIR – elsődleges + másodlagos veszteség; várható éves veszteség = valószínűség × (kár).
- **Elsődleges veszteség** – primary loss – helyreállítás, javítás, közvetlen bevételkiesés.
- **Másodlagos veszteség** – secondary loss – reputáció, ügyfélvesztés, versenyhátrány, bírság.
- **Gordon–Loeb modell** – Gordon–Loeb model (2002) – optimális védelmi beruházás ≤ 1/e (~37 %) × várható veszteség.
- **Hibamód- és hatáselemzés** – FMEA – mérnöki analógia a kockázatalapú védelmi ráfordításra.
- **Digitális érettségi önértékelés** – digital maturity self-assessment (Kane et al. 2017) – 1–10 skála, kezdő/fejlődő/érett.
- **Digitális felkészültségi szint** – Digital Readiness Level – 3 pillér, 8 fokozat (Outsider → Champion).
- **Enabler** – enabler – az AI mint a digitalizáció beágyazott eleme.
- **Termelékenységi paradoxon** – productivity paradox – IT/AI-beruházás ≠ automatikus teljesítmény (Brynjolfsson 1993).
- **AI-értékszakadék** – AI value gap (BCG 2025) – future-built 5 %, scalers 35 %, laggards 60 %.
- **Mérsékelt innovátor** – Moderate Innovator – Magyarország EIS-besorolása.
- **KKV-tipológia** – SME typology – Fadeaways, Reinventors, Adaptors, Windfallers, Digital Dynamos.
- **Digitarthatóság** – digital sustainability – digitalizáció és fenntarthatóság együtt; Aggódó Elkötelezettek vs. Közömbös Konzervatívok.
- **Digitális szakadék** – digital divide – hozzáférés, készség/használat, eredmény (3 szint).
- **Ipar 4.0** – Industry 4.0 – nyolc tipikus bevezetési kihívás és válasz.

---

# Átívelő témák (a tananyagban több előadáson keresztül visszatérő gondolatok)

## 1. „A technológia nem elég” — a kurzus gerince
| Előadás | Hol, milyen formában |
|---|---|
| 1. | Hershey: a SAP nem volt hibás, menedzsment-kudarc; IS három dimenziója; komplementer eszközök; „aki csak a szoftvert veszi meg, a probléma kétharmadát figyelmen kívül hagyja” |
| 2. | Kodak: nem technológiai, hanem stratégiai rugalmasság-hiány; IT-alignment (25 %/50 %/75 %); AI-bevezetés folyamat/adatinfrastruktúra nélkül = ERP/BI-kudarc |
| 3. | Target Canada: „technikai projektként kezelte” a szervezeti változást; ERP 70 % nem éri el a célt; Kennametal plain-vanilla |
| 4. | Knight Capital: single source of truth hiánya; Société Générale: a 220+ szabály kodifikálása menedzseri feladat, „semmilyen technológia nem helyettesítheti”; KKV: nem az eszköz hiányzik, hanem az információ |
| 5. | BI = kultúra, nem eszköz; H3 koordináció → H2 bizalom → H1 képzés; NHS egymást erősítő okok |
| 6. | A jó KPI-rendszer támogatja, nem helyettesíti az ítélőképességet; dashboard sosem semleges |
| 7. | Bosch/Amberg: a technológia nem hoz automatikusan jobb döntést; algoritmus = eszköz, nem döntéshozó |
| 8. | Big Data 60–85 % bukás szervezeti okból; GE Predix stratégiai, nem technikai kudarc; „az AI felerősíti a jó és a rossz adatstratégiát is” |
| 9. | SharePoint-temető: kultúra és ösztönzők nélkül üres; TCS beépítette a munkafolyamatba |
| 10. | Felhő = stratégiai függőségi viszony; SLA nem védekezés; exit-stratégia |
| 11. | Három védvonal együtt sem garantál; emberi felügyelet és értékválasztás nem kiváltható |
| 12. | Termelékenységi paradoxon az AI-ra is; AI alacsony érettségnél torzít; „a technológia hatása kontextusfüggő” |

## 2. Szervezeti ellenállás és változásmenedzsment
1. ea. (4 tényező, 3 minta, big bang vs. inkrementális) → 2. ea. (strategic transitions, sociotechnical ugrás) → 3. ea. (konverziós stratégiák, Crocs vs. Target) → 5. ea. (Excel-visszatérés, árnyék-IT, tudásmunkások) → 8. ea. (Moneyball szakértői ellenállás; „vezetői ellenállás, belső politika”) → 9. ea. (tudásmunkások ellenállnak a menedzselésnek) → 12. ea. (Ipar 4.0 kihívások: változás-ellenállás, kulturális ellenállás).

## 3. Big bang vs. fokozatos
1. ea. (IT természete; „fokozatos bővítés, nem big bang”) → 3. ea. (direct cutover vs. phased; Hershey és Target big bang; Crocs phased; MOL brownfield) → 8. ea. (KKV a 3. lépéssel kezdjen) → 12. ea. (Rookie ne ugorjon Expertre; örökölt rendszerek → fokozatos átállás).

## 4. Adat → információ → döntés; adatminőség; single source of truth
1. ea. (TPS-adat ≠ információ; information overload) → 3. ea. (szigetrendszer „két igazsága”) → 4. ea. (DIKW törés adat→információ; 4 fájlkörnyezeti probléma; 7 dimenzió 5. ea.-ban; SSOT) → 5. ea. (bizalmi probléma = konzisztencia hiánya; Microsoft Starlight) → 7. ea. (GIGO, KDD 1–3 lépés, 80 %) → 8. ea. (50–80 % adattisztítás; GIGO élesebb Big Data-nál) → 11. ea. (adattorzítás a tanítóadatból).

## 5. Mutatók, KPI-k, mérés csapdái
1. ea. (KPI 4 jellemzője, 5–10 KPI, kivételkezelés; 10 gazdasági hatás nem pénzügyi mutató) → 5. ea. (dashboard felső vezetőnek) → 6. ea. (22 KPI, Goodhart, OEE gaming, BSC rituálé, Lie Factor) → 7. ea. (Tokola: szerepkörhöz igazított KPI; magas confidence Lift nélkül félrevezető) → 8. ea. (ROI „terabájt/nap” Goodhart-csapda) → 12. ea. (70 % statisztika forráskritikája).

## 6. Megtérülés és rejtett költségek (TCO)
1. ea. (TCO 20/80, 3×, outsourcing +15–57 %; PV/NPV/IRR/ROI; megtérülési mátrix) → 3. ea. (ERP 189 % költségtúllépés; 450 000 USD) → 8. ea. (Big Data TCO: létszám, integráció, lehetőségköltség; ROI-csapda) → 10. ea. (felhő-TCO: egress, komplexitás, skálázódó díj, bőség paradoxona; 37signals) → 12. ea. (TCO 3–5 év; FAIR; Gordon–Loeb 37 %).

## 7. AI mint kétélű eszköz
2. ea. (AI más, mint az Internet; helyettesítő/belépő, de adatvagyon-korlát, szállítói függőség; alignment) → 3. ea. (AI for CRM/SCM gyorsít, nem vált le) → 5. ea. (preskriptív analitika, algoritmus-averzió ↔ automation bias) → 6. ea. (Goodhart az AI-ban; Key Influencers öntudatlan torzítás; 3 AI-kockázat) → 7. ea. (Target etika) → 8. ea. (Big Data ↔ AI; 85 % AI-projekt téves; rossz szenzor → B) → 9. ea. (szabályalapú → ML → hibrid → GenAI/RAG; hallucináció; magyarázhatóság) → 11. ea. (torzítás, fekete doboz, méltányossági paradoxon, AI Act, energia) → 12. ea. (AI enabler; GenAI kétrétegű; AI szélesíti a szakadékot).

## 8. Érettségi modellek (mind „hol tartunk” típusú)
5. ea. Gartner BI-érettség (5 szint, 87 % alsó kettő) → 8. ea. adatvezérelt szervezet (4 lépés) → 12. ea. Kane 1–10 (3 sáv) és Digital Readiness Level (8 fokozat). Csapda: ne keverd a szintek számát és neveit.

## 9. Centralizáció vs. decentralizáció; függőség és bezártság
1. ea. (centralizált/decentralizált szervezet ellenállása) → 2. ea. (váltási költség mint IT-stratégia; lock-in; AI-infrastruktúra függőség) → 3. ea. (ERP hub; Kennametal; best-of-breed; private network vs. exchange) → 8. ea. (edge vs. cloud; vendor lock-in a Buy-nál) → 10. ea. (inga; vendor lock-in vs. felhő-koncentráció; exit-stratégia).

## 10. Hazai kitekintők (ZH-ban kérdezhető magyar példák)
2. ea.: OTP Simple, Penny/Lidl, MiniCRM, Tesco Clubcard HU, Zwack Unicum, Telenor Közösségi Piactér · 3. ea.: MOL (brownfield, Svébis András), Kometa 99 (greenfield) · 4. ea.: Bosch Hatvan (Plant Digital Twin), Bosch Maklár; KKV-kutatás (információhiány 3,36/3,14; ANOVA 0,915) · 5. ea.: OTP Mobilbank (90 %, ~2 M, +20–30 %) · 8. ea.: magyar gyártó a 2–3. lépés között · 9. ea.: Business Fest 2026 · 10. ea.: MNB 2/2025 ajánlás, MBH Bank OpenShift 2023 · 11. ea.: NAIH-85-3/2022 hangelemzés · 12. ea.: EIS Moderate Innovator, 39,6 %; digitarthatóság (Tick és tsai).

## 11. Ismétlődő esetek különböző szerepben
- **GE Predix:** 6. ea. (siker: flottaadat, Közel-Kelet/Kína) vs. 8. ea. (kudarc: >7 Mrd USD, három ok).
- **ZEAL Network (Tipp24):** 5. ea. (preskriptív analitika) és 7. ea. (prediktív modell, hitelbírálaton túl).
- **Target:** 3. ea. Target Canada (ERP 2013–15) vs. 7. ea. Target terhesség-algoritmus (2012).
- **Walmart:** 1. ea. (RFID), 2. ea. (low-cost; szállítói alkuerő; beérkező logisztika), 3. ea. (pull).
- **Amazon:** 1. ea. (intimacy), 2. ea. (Prime, ajánlórendszer), 7. ea. (item-based CF), 11. ea. (toborzási AI).
- **Tesco Clubcard:** 2. ea. (lojalitás), 8. ea. (adatgyűjtő infrastruktúra, 1995, MacLaurin).
- **Brynjolfsson:** 1. ea. (1993 paradoxon; 2000 Hitt), 8. ea. (McAfee & Brynjolfsson 2012), 12. ea. (paradoxon az AI-ra).
- **Garai-Fodor, Varga & Csiszárik-Kocsir 2023:** 4. ea. és 12. ea.

---

# Összes számítás egy helyen (képletgyűjtemény, előadás-hivatkozással)

| # | Képlet / szabály | Előadás | Tananyag-számok |
|---|---|---|---|
| 1 | **PV** = Σ CFt/(1+r)^t — jövőbeli pénzáramok mai értéke | 1. ea. 7. fej.; 12. ea. 4. fej. | definíció, szám nincs |
| 2 | **NPV** = PV − beruházási költség; **NPV > 0 → megéri** | 1. ea. 7. fej.; 12. ea. 4. fej. | definíció |
| 3 | **IRR**: az a kamatláb/diszkontráta, ahol NPV = 0; rangsoroláshoz | 1. ea. 7. fej.; 12. ea. 4. fej. | definíció |
| 4 | **ROI** = nyereség / beruházás költsége | 1. ea. 7. fej.; 8. ea. 9. fej.; 12. ea. 4. fej. | definíció |
| 5 | **TCO**: vételár ≈ 20 %, rejtett ≈ 80 %; számítógép TCO akár 3× vételár; outsourcing rejtett +15–57 % | 1. ea. 7. fej. | 20/80; 3×; 15–57 % |
| 6 | **Megtérülési mátrix**: IT × komplementer befektetés (magas/magas kiváló; magas/alacsony semmi-negatív; alacsony/magas meglepően jó; alacsony/alacsony gyenge-arányos) | 1. ea. 6. fej. | — |
| 7 | **Metcalfe**: kapcsolatok = n(n−1)/2; 2→1, 5→10, 100→4950; a hálózat értéke „exponenciálisan” nő (a tananyag így adja meg) | 2. ea. 6. fej. | 1 / 10 / 4950 |
| 8 | **IT-alignment**: +50 % profit; 25 % sikerül; 75 % „saját életet él” | 2. ea. 8. fej. | 50/25/75 |
| 9 | **ERP statisztika**: 70 % nem éri el a célt; 189 % (215 %) költségtúllépés; 30 % időben/büdzsén belül; 50 % első nekifutásra bukik; 41 % haszon fele sem; 450 000 USD | 3. ea. 4. fej. | — |
| 10 | **Amberg minőség**: 99,99885 % ≈ 11 hibás/millió (100 − 99,99885 = 0,00115 %) | 4. ea. 7. fej. | 99,99885 % |
| 11 | **OEE** = Rendelkezésre állás × Teljesítmény × Minőség; RÁ = tényleges/tervezett üzemidő; T = (ciklusidő × db)/tényleges üzemidő; M = jó db/összes db | 6. ea. 4. fej. | 432/480 = 0,90; 0,85; 0,98 → **0,75 (75 %)**; world class ~85 %; tipikus 40–60 % |
| 12 | **Lie Factor** = vizuális változás / valós adatváltozás | 6. ea. 6. fej. | 2 % valós → 200 % vizuális |
| 13 | **Support** = együttes/összes; **Confidence(A→B)** = együttes/A; **Lift** = Confidence/Elvárt konfidencia; Lift < 1 → nem erősebb a véletlennél | 7. ea. 5. fej. | 5000/10 000 = 50 %; 5000/6000 = 83 %; elvárt 85 %; 0,83/0,85 = **0,98** |
| 14 | **Hamis pozitív (Target)**: 100 megjelölt, 60 valódi → 40 hamis pozitív | 7. ea. 7. fej. | 100/60/40 |
| 15 | **KDD arány**: 5 lépésből 3 előkészítés; elemzői idő ~80 % (Press 2016); Gartner >25 % pontatlan kritikus adat; Big Data 50–80 % tisztítás | 7. ea. 4. fej.; 8. ea. 3. fej. | 80 %; 25 %; 50–80 % |
| 16 | **Big Data bukás**: 60 % (2015) → 85 % (2017); 85 % kultúra-program / 37 % siker; AI 85 % téves (2018→2022) | 8. ea. 2., 5. fej. | — |
| 17 | **Edge vs. cloud válaszidő**: edge egyszámjegyű–alacsony kétjegyű ms; cloud 100–500 ms | 8. ea. 6. fej. | — |
| 18 | **Big Data TCO/ROI**: előbb az üzleti döntés, aztán a pénz; TCO rejtett: létszám, integráció, lehetőségköltség | 8. ea. 9. fej. | — |
| 19 | **Felhő-repatriáció (37signals)**: 3,2 M USD/év → ~1,3 M; 600 k USD hardver, 6 hónap megtérülés; 3–5× gyorsabb; >10 M USD/5 év; Dropbox 75 M USD/2 év; EasyJet IT 0,5 % vs. 2 % | 10. ea. 5–6. fej. | — |
| 20 | **Gordon–Loeb**: z* ≤ (1/e)·v·p·ℓ ≈ 0,37 × várható veszteség; sávok ≤37 % / 37–100 % / >100 % | 12. ea. 4. fej. | 1/e ≈ 37 % |
| 21 | **FAIR várható éves veszteség** = valószínűség × (elsődleges + másodlagos kár) | 12. ea. 4. fej. | 4×(200 000+50 000) = **1 000 000 Ft**; 0,1×(15 M+35 M) = **5 000 000 Ft** |
| 22 | **AI energia**: 0,4 Wh vs. 33 Wh ≈ 80× | 11. ea. 10. fej. | — |
| 23 | **COMPAS**: nem visszaesők közül tévesen magas kockázatú: afroamerikai 45 % vs. fehér 24 %; kalibrált, de nem osztályozásilag kiegyensúlyozott | 11. ea. 8. fej. | 45/24 |
| 24 | **Kane érettség**: állítások 1–10, átlag; kezdő 1–3 / fejlődő 4–6 / érett 7–10 | 12. ea. 5. fej. | — |

---

# Forrásmegjegyzések (⚠ tételek összegyűjtve)

1. **Előadás-számozás eltérése adatlap vs. Moodle:** adatlap: 6. hét OLAP, 7. hét üres, 8. Tudásmenedzsment, 9. Big Data, 10. Felhő, 11. E-kereskedelem, 12. Etika, 13. Kiberbiztonság; Moodle kötelező könyv: 6. KPI-tervezés (BI I.), 7. OLAP/adatbányászat (BI II.), 8. Big Data, 9. Tudásmenedzsment, 10. Felhő, 11. Etika, 12. Kiberbiztonság/DT. **Az adatlap „E-kereskedelem és platform-gazdaság” előadásához nincs külön Moodle-fejezet** (platform: 2. ea. 7. fej.; B2B piacterek, e/m/c-commerce: 3. ea. 2., 8. fej.). A jegyzet a Moodle-számozást követi; a tananyag belső előre-/visszautalásai („7. fejezetben tárgyaljuk” a KMS-t a 2. ea.-ban; „9. fejezet” a bimodális IT-nél az 5. ea.-ban a felhőre; „8. fejezet” Big Data a 4. ea.-ban) részben a Moodle-számozást, részben korábbi számozást követik — a 2. ea. „7. fejezet” = KM = Moodle 9.; az 5. ea. „9. fejezet” = felhő = Moodle 10.; a 4. ea. „8. fejezet” = Big Data = Moodle 8. ✓; a 8. ea. „9. fejezet” = KM ✓; a 9. ea. „10. fejezet” = felhő ✓; a 7. és 9. ea. „11. fejezet” = etika ✓; az 1. ea. „12. fejezethez is releváns” = DT ✓.
2. **1. ea. 5. fej.:** az ellenállás-ábra felirata csak három tényezőt sorol („szervezeti struktúra, emberek, feladatok,”), a szöveg négyet (+ az IT természete, Laudon Fig. 3.7). ZH-ra: **négy**.
3. **2. ea. 6. fej.:** Metcalfe törvényét a tananyag „exponenciális” növekedésként fogalmazza meg, a számpéldák (1, 10, 4950) az n(n−1)/2 (négyzetes) képletet követik; dátumként 1970-et ad. A tananyag változatát kell tudni.
4. **4. ea. 8. fej.:** a KKV-kutatás táblázatának sorrendje a 2022-es rangsort követi; 2023-ban a pénzügyi problémák (3,12) megelőzik a szakképzett munkaerő hiányát (2,90). Az információhiány mindkét évben 1.
5. **6. ea. (teljes):** a 8. „Szintézis” fejezet duplán szerepel (6.8.html és 6.9.html) azonos szöveggel — egyként kezelve. Az előadás címe az adatlapon „OLAP és adatbányászat”, a Moodle-ban „KPI-tervezés kritikusan”.
6. **6. ea. 4. fej.:** az OEE-példa 75 %-át a tananyag „világszínvonalúnak” nevezi, miközben a „world class” küszöböt ~85 %-ban adja meg (tipikus 40–60 %) — belső ellentmondás; ZH-ra mindhárom számot tudni kell (75 % példa; ~85 % world class; 40–60 % tipikus).
7. **7. ea. 5. fej.:** a bank-példában az „elvárt konfidencia = 85 %” nem következik a megadott adatokból (a megtakarítási számla aránya 5000/10 000 = 50 % lenne); a Lift = 0,83/0,85 = 0,98 a tananyag számaival számolandó. Támogatás 50 %, konfidencia 83 % az adatokból helyesen következik.
8. **7. ea.:** a nyitó eset nem dilemma, hanem a Tokola et al. (2016) kutatás; a Target-eset a 7. fej.-ben van. A hamis pozitív/negatív és a confusion mátrix csak ábra-feliratként és szövegesen jelenik meg (képlet nélkül); a CRISP-DM-et a kötelező anyag egy mondatban említi (a KDD ipari szabvány-változata) — a módszertan részletei és az osztályozás értékelési mutatói az opcionális könyvben vannak, nem kötelezők.
9. **9. ea. 2. fej.:** a nyitó A/B/C dilemmára a tananyag nem jelöl ki egyetlen helyes betűt; mindhárom opció korlátját mutatja be (A = tudomásulvétel; B = dokumentáltatás csak az explicit réteget menti; C = egyszeri workshop alábecsüli az időigényt), és a megoldást a korábban kiépített szakértő-kereső rendszer, digitális iker és a négylépéses tudásmozgatás együttesében adja.
10. **9. ea. 3. fej.:** a négylépéses tudásmozgatás modelljének nevét és négykvadránsos mátrixát a kötelező anyag szándékosan az opcionális könyvre hagyja (forrásként Nonaka & Takeuchi 1995 szerepel); a ZH-ra a kötelező anyag négy lépése (megosztás, explicitté tétel, kombinálás, elsajátítás) tanulandó.
11. **9. ea. 7. fej.:** a szakértői rendszer négy tudásbázis-típusa (eset-, keret-, objektum-, szabálybázisú) „Iván Cs. (é.n.)” ÓE előadásanyagból származik, nem Laudonból — a tananyag így adja meg.
12. **11. ea. 9. fej.:** az EU AI Act határidői a tananyag készítésekor (2026 nyara) mozgásban voltak (2026. 08. 02. → 2027. 12. 02. a toborzási/teljesítményértékelő magas kockázatú rendszereknél; GPAI 2025. aug. óta); a tananyag maga kéri az aktuális állás ellenőrzését — ZH-ra a tananyag dátumai.
13. **12. ea. 7. fej.:** a KKV-tipológia öt típusát (Fadeaways, Reinventors, Adaptors, Windfallers, Digital Dynamos) a tananyag csak felsorolja, nem definiálja; a 2×2 mátrix-ábra a 4 negyedben 5 kategóriát helyez el — a definíciók a forrásban (Vodafone Policy Paper 2020) vannak, a kötelező szöveg nem adja meg.
14. **12. ea. 4. fej.:** a TCO/ROI/NPV/IRR képleteket a tananyag sehol nem írja le explicit formában (csak szöveges definíciót ad az 1. és a 12. ea.-ban); a jegyzet képletei a definíciókból következnek, a számpéldák saját számokkal készültek. A Gordon–Loeb képlet (z* ≤ (1/e)·v·p·ℓ) és a FAIR példaszámok a tananyagból valók.
15. **8. ea. 4. fej. és 6. ea. 7. fej.:** a GE Predix két ellentétes olvasata (6. ea.: sikeres flottaelemzés; 8. ea.: stratégiai kudarc) — nem ellentmondás, hanem szándékos „két olvasat”; a ZH-n a kérdés kontextusa dönt.
16. **1. ea. 7. fej.:** a Laudon-forrás itt „2018, 15th ed.”, másutt „2017, 15th ed.” — ugyanaz a kiadás, két évszámmal hivatkozva; a 3. ea. a Laudon-fejezetekre kiadásszám nélkül hivatkozik (Ch.2, Ch.9, Ch.10, Ch.13).
17. **Tantárgyi adatlap:** kötelező irodalomként Laudon 17th ed. (2022) szerepel, a Moodle-fejezetek a 15th (2017/2018) és 18th (2025, Traver) kiadásra hivatkoznak — a ZH a Moodle-tananyag tartalmát kéri.

