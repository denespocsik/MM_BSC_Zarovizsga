## K19 – Beruházási és befektetési döntések controlling szemléletben

### Beszerzendő anyagok

| Szerző | Mű | Jelleg | Indoklás / érintett rész |
|---|---|---|---|
| — | GIXVS2MBLF syllabus / tantárgynyilvántartó adatlap | syllabus | A tárgy mappájában nincs; a heti tematika és az irodalomjegyzék csak az 1. előadás 2. diájából rekonstruálható. |
| Francsovics A. | *Controlling – elmélet és módszertan* (Budapest, 2010) | kötelező irodalom | Az 1. előadás kötelező irodalomként nevezi meg; a beruházás-gazdaságossági rész (R3–R6) a helyi 2011-es e-jegyzet 4. fejezetére épül, a nyomtatott kötet bővebb lehet. |
| Francsovics A. | *Controlling integrált elmélete és gyakorlata* (Budapest, 2013) | kötelező irodalom | Az 1. előadás második kötelező műve; a mappában nincs, tartalma nem ellenőrizhető. |

**Tétel:** Beruházási és befektetési döntések controlling szemléletben. Gazdaságossági számítások szerepe a controllingban. Statikus beruházásértékelési módszerek. Dinamikus beruházásértékelési módszerek. Nettó jelenérték (NPV) koncepció. Cash-flow szerepe a beruházási döntésekben.

---

### A beruházási döntés és a beruházási controlling

A beruházási döntések a vállalat jövőbeni sorsát meghatározó **stratégiai döntések**: a vállalat a beruházás időpontjában arról dönt, hogy a jelenlegi és jövőbeni erőforrások felhasználásával milyen termékkel vagy szolgáltatással kíván a piacon megjelenni (Francsovics, 2011, 86. o.). A befektetési döntéseknél azzal kell számolni, hogy a hozamok és a ráfordítások eltérő időpontban és nagyságrendben jelentkeznek, és a tényleges hozam eltérhet a várttól. Ezért a döntés előtt három kérdésre kell választ adni: a hozamot **cash flow-ban vagy profitban** mérjük; **milyen kamatlábbal** számolunk; és **hogyan vesszük figyelembe az időtényezőt** (Francsovics, 2011, 75–76. o.).

A beruházási controlling végpontja nem az eszköz vásárlásáról szóló döntés: a controllingnak **az eszköz teljes élettartamára** ki kell terjednie. Három szakasza van: a **tervezési szakasz** a döntés megszületéséig tart, a **megvalósítási szakasz** az üzembe helyezésig, a **használati szakasz** pedig a beruházás ellenőrzése, vagyis a terv–tény összehasonlítás, amelyből a jövőbeli beruházási döntésekhez szűrhetők le tapasztalatok (Katona, 2022a, 2. dia).

```mermaid
flowchart LR
    A["<b>Tervezési szakasz</b><br/><i>döntési előkészítés</i><br/>Gazdaságossági számítások"]:::kek
    B["<b>Megvalósítási szakasz</b><br/><i>projekt-controlling</i><br/>Költség- és időkontroll"]:::narancs
    C["<b>Használati szakasz</b><br/><i>utókalkuláció</i><br/>Terv–tény összehasonlítás"]:::zold

    A -->|"döntés: megvalósítás"| B -->|"üzembe helyezés"| C
    C -->|"tapasztalatok → jövőbeli döntések"| A

    classDef kek     fill:#e3f2fd,stroke:#1565c0,stroke-width:2px,color:#0d47a1,rx:10,ry:10;
    classDef zold    fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px,color:#1b5e20,rx:10,ry:10;
    classDef narancs fill:#fff3e0,stroke:#ef6c00,stroke-width:2px,color:#e65100,rx:10,ry:10;

    linkStyle default stroke:#546e7a,stroke-width:2px;
    linkStyle 2 stroke:#c2185b,stroke-width:2px,stroke-dasharray: 5 5;
```

### A gazdaságossági számítások szerepe a controllingban

A beruházás-gazdaságossági vizsgálatnak három célja van: (1) az egyes beruházásokról **egyedileg** el lehessen dönteni, megvalósuljanak-e; (2) az összes beruházási igényt **sorrendbe** lehessen rendezni; (3) a számítás a **kontroll első pontja**, amelyhez képest a beruházás utólag értékelhető (Katona, 2022a, 3. dia). A harmadik cél köti a számítást a controlling-szabályozókörhöz: a tervezési szakasz kalkulációja a használati szakasz terv–tény összehasonlításának viszonyítási alapja.

A számítást megelőzi az igények **szűrése** hat szempont szerint: a beruházás célja (illeszkedik-e a stratégiához), az elvárt eredmény, a pénzügyi forrás és az emberi erőforrás rendelkezésre állása, az üzemeltetési igény (ellátható-e a keletkező többletfeladat) és a kockázat (nem veszélyezteti-e a mindennapi működést) (Katona, 2022a, 4. dia). A szűrőn átjutott igényeket **sorba rendezzük** az üzleti hasznosság, a stratégiai mutatószámokhoz való hozzájárulás, a megoldott problémák és a kötelező jelleg szerint (Katona, 2022a, 23. dia). A pénzügyi mutatókat **haszonérték-elemzés** egészítheti ki: a célkitűzéseket súlyozzuk, az alternatívákat pontozzuk, és a súlyozott pontszámot hasonlítjuk össze (Katona, 2022a, 24. dia).

Attól függően, hogy az időtényezőt hogyan kezeljük, **statikus** és **dinamikus** vizsgálatokat különböztetünk meg (Francsovics, 2011, 86. o.; Katona, 2022a, 5. dia).

### Statikus beruházásértékelési módszerek

A statikus vizsgálatok **egyetlen periódusra** vonatkoznak, az időtényezőt nem vagy csak korlátozottan veszik figyelembe (Francsovics, 2011, 86. o.). Feltételezik, hogy a beruházási kiadás egy éven belül végbemegy, a ráfordítások, az árbevétel és az eredmény évente közel azonosak, és a tőke az amortizációból megtérül (Katona, 2022a, 6. dia).

**Költség-összehasonlító számítás.** Az alternatívák periódusonkénti vagy teljesítményegységenkénti költségét (leírás, kalkulációs kamat, egyéb fix költség + fajlagos változó költségek) hasonlítja össze; a legalacsonyabb költségű a legkedvezőbb (Katona, 2022a, 7. dia). Korlátai: nem vizsgálja a hozamokat, nem méri a tőke jövedelmezőségét, rövid az időhorizontja, nem veszi figyelembe a régi berendezés maradványértékét, és csak alternatívák közötti választásra alkalmas. Elsősorban pótló beruházásokra való, ha a hozamok és ráfordítások nem ingadoznak (Francsovics, 2011, 87–88. o.).

**Nyereség-összehasonlító számítás.** A költség-összehasonlítás kibővítése az árbevétellel: a fajlagos eredményt hasonlítja össze (Francsovics, 2011, 88. o.; Katona, 2022a, 8. dia).

**Jövedelmezőségi számítás.** Az előzőek nem mondanak ítéletet a lekötött tőke jövedelmezőségéről; ezt pótolja a jövedelmezőségi számítás, amelynek a tananyag két változatát adja. Francsovics gépcsere-példájában a modern gép 500 eFt-tal drágább, de évi 200 eFt üzemeltetési költséget takarít meg: a többletbefektetés 500/200 = 2,5 év alatt térül meg, jövedelmezősége 200/500 = 40 % (Francsovics, 2011, 88–89. o.). Katona változata a **ROI**: a számviteli nyereséget hasonlítja a befektetett eszközökhöz, és az eszközmegtérülést veti össze a tőkeköltséggel; egyik módja, hogy az évenkénti eredmény / könyv szerinti eszközérték hányadosokat átlagolják (étterem-példa: 1 millió USD, 5 év, átlagos ROI 23,05 %) (Katona, 2022a, 9–11. dia). A ROI gyengéje, hogy **nem egyértelmű a kiszámítási mechanizmusa**: számlálója és nevezője többféleképpen értelmezhető (Katona, 2022a, 12. dia).

**Megtérülési periódus (pay-off period, PBPS).** Hány év alatt folyik vissza a befektetett tőke a vállalathoz. Francsovics példájában az „A” beruházás (1 200 eFt; 480 eFt nyereség + 120 eFt leírás = 600 eFt átlagos cash flow) 2 év, a „B” (1 500 eFt; 500 eFt/év) 3 év alatt térül meg, tehát „A” kedvezőbb. A módszer segít a kockázat kezelésében és jelzi a likviditási hatást, ezért a gyakorlatban a legelterjedtebb (Francsovics, 2011, 90. o.). Változata a **cut-off period**: előre rögzített időn belül akarjuk visszanyerni a teljes összeget; ez az egyik legdurvább kritérium (Francsovics, 2011, 90. o.). Hátránya, hogy a pénzáramokat nominális értéken veszi, és eltekint a megtérülés utáni pénzáramlástól: az előadás példájában a „B” projekt egy év alatt megtérül, de összesen csak 55 000-et hoz, míg a két év alatt megtérülő „A” 105 000-et (Katona, 2022a, 9–10. dia).

### Dinamikus módszerek – a pénz időértéke és a tőkeköltség

A dinamikus módszerek a beruházás **teljes élettartamára** vizsgálják az előnyösséget (Francsovics, 2011, 91. o.). Két azonos összegű, de különböző időpontban esedékes pénzösszeg nem egyenértékű, ezért a jövőbeni összegeket a kezdő kiadás időpontjára, **jelenértékre** kell hozni (Francsovics, 2011, 75–76. o.):

```
PV = CF_t / (1 + r)^t

ahol: CF_t = a t-edik évben várható cash flow
      r    = a tőke alternatív költsége (elvárt hozam, diszkontráta)
```

A diszkontrátát Francsovics **haszonáldozatnak** nevezi: ezt a hozamot áldozzuk fel azzal, hogy a pénzt nem kamatozó bankbetétbe fektetjük (Francsovics, 2011, 91. o.). Nagyságát a kockázathoz kell igazítani: az elvárt hozam `r = r_f + β(r_m − r_f)`, ahol `r_f` a kockázatmentes kamatláb, `(r_m − r_f)` a piaci kockázati prémium, `β` a piaci kockázat mérőszáma (Katona, 2022a, 15–16. dia; Francsovics, 2011, 79. o.). Vegyes finanszírozásnál a diszkontráta a **súlyozott átlagos tőkeköltség (WACC)**: az előadás példájában 66 % saját tőke 12 %-os elvárt hozammal (7,92 %) és 34 % idegen tőke 8 %-kal (2,72 %) együtt 10,64 % (Katona, 2022a, 17. dia). Az inflációt konzisztensen kell kezelni: `(1 + r_nominál) = (1 + r_reál)(1 + infláció)`; nominális kamatlábhoz folyó áras cash flow tartozik (Katona, 2022a, 15. dia; Francsovics, 2011, 81. o.).

**Nettó jelenérték (NPV).** A befektetés révén képződő jövedelmek diszkontált összegének és a kezdő befektetésnek a különbsége (Francsovics, 2011, 91. o.):

```
NPV = −C₀ + Σ [CF_t / (1 + r)^t]

Döntési szabály: akkor érdemes megvalósítani, ha NPV ≥ 0
```

**Belső megtérülési ráta (IRR).** Az a kamatláb, amelynél a nettó jelenérték éppen nulla; másként az az éves átlagos hozam, amelyet a pénzáramlás a befektetőknek biztosít. Azt a beruházást érdemes megvalósítani, amelynek IRR-je nagyobb az elvárt hozamnál (Francsovics, 2011, 97. o.; Katona, 2022a, 21. dia). Konvencionális pénzáramnál az IRR és az NPV **két egyenértékű döntési kritérium**: ha az elvárt hozam kisebb az IRR-nél, az NPV biztosan pozitív (Francsovics, 2011, 97. o.). Nehézsége, hogy n-ed fokú polinomról lévén szó, csak iterációval, grafikusan vagy interpolációval számítható (Francsovics, 2011, 98–99. o.).

**Jövedelmezőségi index (PI).** Az egységnyi beruházással megvalósuló jelenértéket fejezi ki (PI = PV / C₀; elfogadható, ha PI > 1). **Korlátozott forrás** esetén van jelentősége: ilyenkor nem az egyedi NPV, hanem az egységnyi befektetésre jutó nettó jelenérték alapján választunk (Katona, 2022a, 18. dia).

**Diszkontált megtérülési idő (PBPD).** Hány év alatt éri el a diszkontált pénzáramok kumulált összege a beruházási összeget (Katona, 2022a, 19. dia). Az egyszerű és a diszkontált megtérülési idő közös hibája, hogy a megtérülés utáni cash flow-kat nem nézik, így félrerangsorolhatnak; az előírt megtérülési idő önmagában is szubjektív elem (Katona, 2022a, 20. dia).

**Annuitás-módszer.** Az NPV-t az élettartamra vetített éves egyenletes összegre alakítja: `A = NPV / a`, ahol `a = [(1 + r)^t − 1] / [r(1 + r)^t]` az annuitási tényező. **Eltérő élettartamú** alternatíváknál szükséges: Francsovics példájában a 3 éves gép NPV-je 112 480 Ft, a 6 évesé 189 850 Ft, az évi annuitás viszont 45 230, illetve 43 590 Ft, vagyis az első gép az előnyösebb (Francsovics, 2011, 100. o.).

### Az NPV koncepció értelmezése

Az NPV-ből két dologra következtethetünk: megtérül-e a befektetés a kockázatot és a pénz időértékét is figyelembe véve, és **gyarapodik-e a befektető vagyona**. **NPV = 0**: a tőke megtérül és a kalkulációs kamatlábnak megfelelően kamatozik, a beruházás éppen kifizetődő; **NPV < 0**: a nettó jelenértéknek megfelelő veszteség; **NPV > 0**: a befektető visszanyeri tőkéjét és kamatát, és ezen felül többletre tesz szert (Francsovics, 2011, 91–92. o.). A pozitív NPV azt jelenti, hogy a beruházás többet ér, mint amennyibe került (Francsovics, 2011, 92. o.).

Az NPV a legszélesebb körben elfogadott mutató. Előnyei: **cash flow-t használ eredmény helyett**; a beruházás teljes hatását vizsgálja; figyelembe veszi a pénzáramok eltérő időbeli jelentkezését; mindig kiszámolható; egyszerűen kumulálható. Hátránya, hogy a tőkeköltség meghatározása inkább feltételezés, mint számítás, és erősen befolyásolja az eredményt (Katona, 2022a, 14. dia). Mechanikusan az NPV sem alkalmazható: lényegesen eltérő élettartamú befektetések NPV-je közvetlenül nem hasonlítható össze; azonos időtartamot kell képezni (ismételt beszerzéssel) vagy annuitást számítani (Francsovics, 2011, 93–94. o.).

**IRR vagy NPV?** Forráskorlát melletti rangsorolásnál a két kritérium eltérő sorrendet adhat. Francsovics példájában (2 600 000 keret, 10 % elvárt hozam) a negatív NPV-jű D-t mindkettő elveti; IRR alapján a B, C, E tervek választandók (együttes NPV 1 060 000), NPV alapján a C, B, A tervek (1 070 000). Érdemesebb tehát a 12 %-os IRR-ű, de nagyobb értékű A-t megvalósítani, mint a 15 %-os E-t: **az NPV alkalmazásával általában jobban biztosítható a tulajdonosi vagyon maximalizálása** (Francsovics, 2011, 101–102. o.). Az IRR helytelen számítás vagy használat esetén félrevezető lehet (Francsovics, 2011, 98. o.).

### Számítási példa

Az Úgyarat Kft. beruházásának pénzáramai (MFt), elvárt hozam 14 % (Katona, 2022b):

| Év | Cash flow (MFt) | PV (14 %-on) | Kumulált NPV |
|---|---|---|---|
| 0 | –500 | –500 | –500,00 |
| 1 | 90 | 78,95 | –421,05 |
| 2 | 250 | 192,37 | –228,68 |
| 3 | 300 | 202,49 | –26,19 |
| 4 | 200 | 118,42 | **+92,22** |

- **NPV** = 592,22 − 500 = **+92,22 MFt** → a beruházás előnyös.
- **PBPD** = 3 + 26,19/118,42 ≈ **3,22 év** (jelenértéken számítva).
- **PI** = 592,22 / 500 = **1,1844** → 1 Ft ráfordítás 1,18 Ft jelenértékű jövedelemmel jár.
- **PBPS** = 2 + 160/300 ≈ **2,53 év** (az időtényező nélkül: kumulált pénzáram –500, –410, –160, +140, +340).
- **IRR**: 15 %-on az NPV még +78,9 MFt, tehát IRR > 15 %; a pontos érték iterációval kereshető (Katona, 2022b).

### A kockázat kezelése a befektetési döntésekben

A kockázat annak valószínűsége, hogy a tényleges hozam eltér a várttól; a befektető kockázatelutasító, a nagyobb kockázatért magasabb hozamot követel. Az **egyedi kockázat** a céget és versenytársait érinti, diverzifikálással mérsékelhető; a **piaci kockázat** (market risk) egyszerre sújtja az egész gazdaságot (adóváltozás, monetáris szigorítás, válság), nem diverzifikálható, ezért érte többlethozam jár (Francsovics, 2011, 77–78. o.). Mérése a hozamok **szórásával** vagy a **β**-val történik, amely megmutatja, hány százalékkal változik a befektetés hozama, ha a piaci portfólió hozama 1 %-kal változik; a β-val arányos prémium épül be az elvárt hozamba (Francsovics, 2011, 78–79. o.). Ahol nincs fejlett értékpapírpiac, a kockázat csak becsülhető a cash flow-t meghatározó tényezők (forgalom, árak, bér, adók, élettartam) lehetséges sávjából; jó támpont a **fedezeti pont**, mert minél közelebb működik hozzá a cég, annál nagyobb az üzleti kockázata. A gyakorlatban a diszkontrátát is a rizikóhoz igazítják: gépcserénél kockázatmentes kamatláb + 1 %, bővítésnél + 2–3 % (Francsovics, 2011, 80. o.).

### A cash flow szerepe a beruházási döntésekben

A **cash flow** egy időszak alatt ténylegesen beáramló és kiáramló pénzfolyamok különbsége; a kiáramlás folyó kiadásokból és tőkekiadásokból áll. A **profit** számviteli megközelítésen, az elkönyvelt bevételeken és ráfordításokon alapul, a cash flow-nál a ténylegesen megtörtént pénzmozgásokkal számolunk, és a könyvelés meg az effektív pénzmozgás között jelentős időeltolódás lehet. A két koncepció két ponton tér el: a cash flow számításnál a **tőkekiadásokat figyelembe kell venni**, az **amortizációt viszont nem kell levonni**, mert nem jár pénzmozgással. A „cash flow vagy profit” kérdésre a válasz elméletben és gyakorlatban a cash flow javára tolódott el; **minden olyan cash flow-t** figyelembe kell venni, amely a projekt elfogadásából következik (Francsovics, 2011, 76. o.). Ezért tekinti Katona az NPV egyik előnyének, hogy cash flow-t használ eredmény helyett (Katona, 2022a, 14. dia).

A pénzáramok típusai: a **konvencionális** pénzáram előjele egyszer vált (befektetés, majd visszaáramlás), és lehet **annuitás jellegű** (évente azonos) vagy **vegyes**; a **nem konvencionális** pénzáram előjele többször változik, például felújítás miatti bezárásnál vagy a bánya bezárásakor felmerülő környezet-helyreállítási kiadásnál (Francsovics, 2011, 82–83. o.). Időbeli szerkezete szerint háromféle pénzáram van: a **kezdő pénzáram** (tárgyi kiadások, forgótőke-szükséglet és az **opportunity cost**, például a saját telek elmaradó bérleti díja), a **működési pénzáram** (adózott eredmény + amortizáció, korrigálva a pótlólagos tőkekiadásokkal) és a **végső pénzáram** (eszközök eladása, forgótőke felszabadítása). Az elemzést 5–10 éves időtartamra célszerű végezni, mert hosszabb távon túl nagy a bizonytalanság. Pótló beruházásnál a régi és az új befektetés pénzáramainak **különbségével** kell számolni (Francsovics, 2011, 83–85. o.).

### Összegzés

A controlling szemléletű beruházási döntés folyamat: az igények szűrése és rangsorolása, a gazdaságossági számítás mint döntési alap és kontrollpont, majd a megvalósítás és a használat terv–tény ellenőrzése. A statikus módszerek egy periódust néznek és nem kezelik az időtényezőt; a dinamikus módszerek a teljes élettartam cash flow-it diszkontálják a kockázatnak megfelelő tőkeköltséggel. Közülük az NPV az elsődleges, mert a tulajdonosi vagyon gyarapodását méri; az IRR, a PI, a megtérülési idő és az annuitás kiegészítő szempontot ad (hozamráta, forráskorlát, likviditás, eltérő élettartam). Mindennek alapja a döntésből következő, teljes körűen számba vett cash flow, nem a számviteli eredmény.

---

### Várható vizsgáztatói kérdések

1. **Mi a különbség a statikus és a dinamikus módszerek között, és mikor elegendő a statikus?** — A statikus vizsgálat egyetlen periódusra vonatkozik, az időtényezőt nem vagy korlátozottan kezeli; akkor alkalmazható, ha a kiadás egy éven belül végbemegy, a költségek és az árbevétel évente közel azonosak, és a tőke az amortizációból megtérül (Francsovics, 2011, 86. o.; Katona, 2022a, 6. dia). A dinamikus módszerek a teljes élettartam pénzáramait diszkontálják (Francsovics, 2011, 91. o.).
2. **Mit jelent, ha az NPV pontosan nulla?** — A befektetett tőke megtérül, és a kalkulációs kamatlábnak megfelelően kamatozik; a beruházás éppen kifizetődő, ezért Katona szerint NPV = 0 esetén is érdemes megvalósítani (Francsovics, 2011, 92. o.; Katona, 2022a, 14. dia).
3. **Ha az IRR és az NPV egyenértékű kritérium, miért adhatnak eltérő rangsort?** — Egyetlen projekt elfogadásánál egyenértékűek: ha az elvárt hozam kisebb az IRR-nél, az NPV pozitív. Rangsorolásnál és forráskorlátnál azonban az IRR a hozamrátát, az NPV az abszolút vagyongyarapodást méri; Francsovics példájában az IRR-rangsor 1 060 000, az NPV-rangsor 1 070 000 összértéket ad, ezért az NPV az elsődleges (Francsovics, 2011, 97., 101–102. o.).
4. **Miért cash flow-val és nem eredménnyel számolunk?** — Mert a cash flow a tényleges pénzmozgást mutatja, tartalmazza a tőkekiadást, és nem vonja le a pénzmozgással nem járó amortizációt; a könyvelés és a pénzmozgás között időeltolódás van (Francsovics, 2011, 76. o.). Katona ezt az NPV első előnyeként említi (Katona, 2022a, 14. dia).
5. **Mikor melyik dinamikus mutatót használjuk?** — Az NPV az alapkritérium; a PI korlátozott forrás esetén rangsorol, mert az egységnyi befektetésre jutó jelenértéket maximalizálja (Katona, 2022a, 18. dia); az annuitás eltérő élettartamú alternatívák összehasonlítására való (Francsovics, 2011, 100. o.); a megtérülési idő a likviditási hatást és a kockázatot jelzi, de a megtérülés utáni pénzáramokat figyelmen kívül hagyja (Katona, 2022a, 20. dia).
6. **Honnan jön a diszkontráta?** — A tőke alternatív költsége (haszonáldozat), amelyet a kockázattal kell összhangba hozni: elvárt hozam = kockázatmentes kamatláb + β × piaci kockázati prémium; vegyes finanszírozásnál a saját és idegen tőke elvárt hozamának súlyozott átlaga (WACC); inflációnál a nominális és reálkamatláb konzisztens kezelése szükséges (Francsovics, 2011, 79–81., 91. o.; Katona, 2022a, 15., 17. dia).

---

## Irodalom

* Francsovics, A. (2011). *Controlling* [Elektronikus jegyzet]. Óbudai Egyetem, Keleti Károly Gazdasági Kar.
* Katona, F. (2022a). *CONTROLLING 6. előadás: Beruházás gazdaságossági számítások* [Előadás-prezentáció]. Óbudai Egyetem, Keleti Károly Gazdasági Kar.
* Katona, F. (2022b). *Beruházás-controlling gyakorlati példa (gyak_Beruházás-contr)* [Gyakorlati feladat]. Óbudai Egyetem, Keleti Károly Gazdasági Kar.
