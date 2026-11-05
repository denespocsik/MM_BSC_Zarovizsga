# 10. előadás: 10. előadás Mi történik, ha a felhő maga omlik össze? - Kötelező tananyag

## 1. 10. fejezet: Felhő és IT-infrastruktúra — stratégiai döntés, nem IT-feladat

(forrás: 10.1.html)

### 1. 10. fejezet: Felhő és IT-infrastruktúra — stratégiai döntés, nem IT-feladat

## 2. Nyitó dilemma: a felhőszolgáltató csődje

(forrás: 10.2.html)

### 2. Nyitó dilemma: a felhőszolgáltató csődje

## Mi történik, ha a felhő maga omlik össze?

### Nyitó dilemma

🔴 Döntés előtt — Ön az informatikai igazgató

Ön egy közepes méretű bank informatikai igazgatója. A vezetőség úgy dönt, hogy a bank teljes ügyfél-adatvagyonát és core banki rendszerét egyetlen nemzetközi felhőszolgáltatóhoz költözteti — a döntést az indokolja, hogy ez rugalmasabb, skálázhatóbb és olcsóbbnak tűnik, mint a saját adatközpont fenntartása. Három évvel később a felhőszolgáltató csődöt jelent.

Mit tesz Ön ebben a helyzetben?

- A) Pánikszerűen keres egy másik szolgáltatót, és megpróbálja a lehető leggyorsabban átvinni az adatokat, bármi áron.

- B) Előveszi a három évvel korábban kidolgozott, előre megtervezett kivezetési (exit) stratégiát, és annak lépéseit követi.

- C) Vár, remélve, hogy egy másik nagyvállalat felvásárolja a csődbe ment szolgáltatót, és a szolgáltatás zavartalanul folytatódik.

Tartsa fejben a választását — a fejezet végén visszatérünk rá.

Ez nem elméleti rémtörténet. 2025. október 20-án egy tizenöt órás kiesés az Amazon Web Services (AWS) egyik régiójában 3500-nál is több vállalatot bénított meg 60-nál több országban — bankokat, tőzsdéket, légitársaságokat, kórházi rendszereket —, és ez volt már a harmadik hasonló léptékű incidens öt év alatt, ugyanabból a régióból. A kérdés tehát nem az, hogy történhet-e ilyesmi — hanem hogy egy szervezet fel van-e rá készülve.

📚 A fejezet térképe

2. oldal: honnan indultunk — az IT-infrastruktúra evolúciója a mainframe-től a hordható eszközökig → 3. oldal: SaaS/PaaS/IaaS mint döntési logika, nem definíció → 4. oldal: publikus, privát, hibrid felhő — mikor melyik és miért → 5. oldal: a felhő mítoszainak kritikai vizsgálata → 6. oldal: vendor lock-in mint stratégiai kockázat és exit-stratégia → 7. oldal: TCO a felhőben — miért nem mindig olcsóbb → 8. oldal: felhő-koncentráció és rendszerszintű törékenység → 9. oldal: szintézis, az SLA valós jelentése és hazai kitekintés.

💡 Tanulási eredmények

A fejezet elvégzése után Ön képes:

- elhelyezni a felhőalapú informatikát az IT-infrastruktúra történeti fejlődésének ívén, és kritikusan értékelni, hogy ez "haladás" vagy inga-mozgás a centralizáció és decentralizáció között

- alkalmazni a SaaS/PaaS/IaaS közötti választást mint stratégiai kontroll-átadási döntést, nem technikai definíciót

- indokolni, mikor éri meg publikus, privát vagy hibrid felhőt választani, valós vállalati bizonyítékokra alapozva

- kritikusan megkérdőjelezni a "a felhő mindig olcsóbb és egyszerűbb" közhelyet, valós vállalati adatokkal alátámasztva

- kidolgozni egy vendor lock-in kockázatot kezelő exit-stratégia alapvázát

- felismerni a felhő-koncentráció mint rendszerszintű, nem csak vállalati szintű kockázat jelentőségét

🤔 Gondolkodtató kérdés

A fenti A/B/C döntési helyzetben melyik választás előfeltétele valójában egy sokkal korábbi, a felhőbe költözés pillanatában meghozott döntésnek?

[Ábra: idővonal a 2025. október 20-i AWS-kiesésről — érintett szektorok (pénzügy, légiközlekedés, egészségügy, kiskereskedelem) és a 15 órás időtartam vizuálisan, feltüntetve, hogy ez a harmadik hasonló incidens öt év alatt.]

Forrás: AWS Outage of October 2025 — several industry analyses (WheelHouseIT, 2025; Built In, 2025; Global Relay, 2026); Demandsage internet outage statistics (2026).

## 3. Az IT-infrastruktúra evolúciója

(forrás: 10.3.html)

### 3. Az IT-infrastruktúra evolúciója

## Az inga: centralizációtól decentralizációig — és vissza

### Az IT-infrastruktúra evolúciója

Könnyű azt gondolni, hogy a felhő valami radikálisan új dolog. A valóság ennél árnyaltabb: az elmúlt hetven év informatika-története oda-vissza ingamozgás a centralizált és a decentralizált modellek között, nem egyenes vonalú "fejlődés" (Laudon & Laudon, 2018).

Korszak | Modell | Centralizáció foka | 

1950–70-es évek | Mainframe | Teljes centralizáció — egyetlen nagygép, "buta" terminálok | 

1980–90-es évek | Személyi számítógép, kliens-szerver | Decentralizáció — számítási kapacitás az asztalon | 

2000-es évek | Vállalati hálózatok, internet | Részleges újra-centralizáció — vállalati adatközpontok | 

2010-es évektől | Felhő | Újra teljes centralizáció — de most néhány globális szolgáltatónál, nem a vállalatnál | 

A felhő tehát nem "kiszabadulás" a mainframe-korszak centralizált logikájából — éppen ellenkezőleg, visszatérés hozzá, csak most a számítási kapacitás nem a vállalat saját gépterme, hanem néhány globális szereplő adatközpontja felett központosul. Ez a felismerés kulcsfontosságú a fejezet további részeihez: ha a centralizáció kockázatai (egyetlen pont kiesése az egész rendszert megbéníthatja) korábban is ismertek voltak a mainframe-korszakból, miért lepődünk meg most, hogy a felhő-koncentráció hasonló kockázatot hordoz (lásd 8. oldal)?

A mobil és hordható platform mint a legújabb állomás. Az evolúciós ív legfrissebb szakasza a mobil és hordható eszközök vállalati integrációja — és ez a fejlemény kifejezetten releváns a műszaki menedzserek számára. A globális logisztikai vállalat, a DHL, a Ricoh és az Ubimax cégekkel közösen vezetett be "vision picking" technológiát raktári műveleteiben: a dolgozók okosszemüvegen keresztül kapnak vizuális útmutatást a raktárban, ami 25%-os hatékonyságnövekedést eredményezett (Laudon & Laudon, 2018). Hasonlóan, a Southern Co. energetikai vállalat fejre és csuklóra szerelt eszközöket (okosórákat, kamerás fejpántokat) vezetett be erőműveiben és energiaelosztási infrastruktúráján, hogy a dolgozók pontosabban kövessék a dokumentált eljárásokat, és hogy a terepi és irodai személyzet közötti kommunikáció valós idejűvé váljon.

💡 Műszaki analógia

Gondoljon egy gyártósorra, ahol korábban a minőségellenőr papíralapú, majd később táblagépes ellenőrzőlistával járta végig az állomásokat. A hordható eszközök (okosszemüveg, csuklóra szerelt terminál) ennek a folyamatnak a következő állomása: a kezek szabadon maradnak, az információ pedig a munkavégzés pillanatában, kontextusban jelenik meg — nem egy külön lépésben kell érte "megállni".

A "bring your own device" (BYOD) jelenség — és a visszakozás. A 2010-es évek elejétől a munkavállalók egyre inkább saját okostelefonjukat, táblagépüket kezdték használni munkahelyi célra is — ezt nevezte el a szakirodalom a fogyasztói informatika (consumerization of IT) jelenségének (Laudon & Laudon, 2018). Az elmúlt évtizedben ez tömegesen elterjedt gyakorlattá vált: a szervezetek túlnyomó többsége ma valamilyen formában engedélyezi a személyes eszközök használatát.

Érv a BYOD mellett | Ellenérv — miért fordul a trend | 

Alacsonyabb hardverköltség — a vállalatnak nem kell eszközt vásárolnia | A rejtett üzemeltetési költség (támogatás sokféle eszköztípushoz, biztonsági incidensek kezelése) gyakran felemészti a megtakarítást | 

Nagyobb munkavállalói elégedettség és rugalmasság | A munkavállalók 71%-a érzékeny vállalati adatot tárol személyes telefonján — ez önmagában komoly biztonsági kitettség | 

Nincs betanulási görbe — a munkavállaló már ismeri saját eszközét | A vállalatok 62%-a jelenleg felülvizsgálja vagy kifejezetten elhagyja a BYOD-politikáját (Tangoe, 2025) | 

⚠️ A trend fordulóban van

Miközben a BYOD tíz évvel ezelőtt a modern, rugalmas munkahely szimbólumaként terjedt el, mára jelentős visszakozás figyelhető meg: a vállalatok több mint 60%-a felülvizsgálja vagy elhagyja a BYOD-politikát, és sok szervezet a CYOD (Choose Your Own Device) modell felé mozdul el — ahol a munkavállaló egy előre jóváhagyott, vállalat által felügyelt eszközkatalógusból választhat, megőrizve a döntési szabadság egy részét, de visszaadva az IT-osztálynak a biztonsági kontrollt. A fordulat mögött elsősorban biztonsági és jogi felelősségi aggályok állnak: egy 2026-os felmérés szerint a biztonsági vezetők (CISO-k) 78%-a kifejezetten aggódik a saját jogi felelőssége miatt egy BYOD-eszközön történő biztonsági incidens esetén.

💡 Műszaki analógia

Ez ugyanaz a mintázat, mint amikor egy gyártó üzem eleinte engedélyezi, hogy a karbantartó technikusok saját szerszámaikat hozzák be (rugalmasabb, olcsóbb a cégnek), majd rájön, hogy a nem egységesített, nem ellenőrzött szerszámok minőségbiztosítási és felelősségi kockázatot jelentenek — és visszatér az egységes, vállalati tulajdonú szerszámkészlethez, esetleg egy korlátozott választási lehetőséggel (pl. két jóváhagyott márka közül).

[Ábra: az IT-infrastruktúra evolúciójának "inga"-ábrája — centralizáció/decentralizáció tengelyen ábrázolva a mainframe → PC → vállalati hálózat → felhő → hordható eszközök ívét, hullámvonalként, nem egyenes fejlődési nyílként.]

🤔 Reflektív kérdés

Egy gyártó üzemben, ahol a mérnökök táblagépen érik el a digitális iker rendszereket (9. fejezet), mit mérlegelne: engedélyezné a saját eszköz használatát, vagy inkább vállalati, felügyelt táblagépeket adna ki? Mi dönti el a választ?

Forrás: Laudon, K. C., & Laudon, J. P. (2018). Management information systems (15th ed.). Pearson. 5. fejezet.; Tangoe (2025). Companies Are Moving Back to Corporate-Owned Devices, Should You?; SHI Resource Hub (2026). The Benefits of CYOD: Why Employee Choice Is Shifting Away from BYOD.

## 4. SaaS/PaaS/IaaS mint döntési logika

(forrás: 10.4.html)

### 4. SaaS/PaaS/IaaS mint döntési logika

## Mit adunk fel, és mit nyerünk cserébe?

### SaaS/PaaS/IaaS mint döntési logika, nem definíció

A szolgáltatási modellek (IaaS, PaaS, SaaS) technikai definícióit — ki üzemelteti a hardvert, ki telepíti az operációs rendszert — már ismerik az Üzleti Informatikai Alkalmazások tárgy anyagából. Ami ott kevésbé kap hangsúlyt, az a menedzseri döntés logikája: minden egyes szinten feljebb lépve a szervezet kontrollt ad fel, cserébe felelősséget és üzemeltetési terhet vesz le a válláról.

Szint | Amit feladunk | Amit nyerünk | 

IaaS | Fizikai hardver feletti kontroll | Nincs szerverbeszerzés, gyors skálázás | 

PaaS | Operációs rendszer, middleware feletti kontroll | Fejlesztők csak az alkalmazásra fókuszálnak | 

SaaS | Testreszabás, verziókövetés feletti kontroll | Azonnal használható, karbantartás-mentes | 

Ez pontosan ugyanaz a logika, amit a Big Data-fejezetben a build/buy/outsource döntésnél már tárgyaltunk (8. fejezet, 2. oldal): minél magasabb szintű szolgáltatást választunk, annál kevesebb a technikai terhünk, de annál kevesebb a beavatkozási lehetőségünk is, ha valami nem úgy működik, ahogyan szeretnénk.

⚠️ A döntés nem egyszeri, hanem rendszerenként újra átgondolandó

Sok szervezet hibázik abban, hogy egyetlen szolgáltatási szintet választ "vállalati szabványként" minden rendszerére. A valóságban a döntést rendszerenként érdemes meghozni: egy kritikus, egyedi versenyelőnyt jelentő rendszernél (pl. egy gyártó cég saját fejlesztésű minőségellenőrzési algoritmusa) indokolt lehet az IaaS-szintű kontroll, míg egy általános, nem megkülönböztető funkciónál (pl. e-mail, dokumentumkezelés) a SaaS a ésszerű választás.

💡 Műszaki analógia

A szolgáltatási szintek közötti választás olyan, mint amikor egy gyártó cég eldönti, hogy a szerszámgépeit saját maga tartja karban (teljes kontroll, teljes felelősség), külső szervizzel szerződik éves karbantartási csomagra (részleges kontroll), vagy gépkapacitást bérel egy másik üzemtől, amikor csúcsidőszakban van rá szükség (minimális kontroll, maximális rugalmasság).

[Ábra: a kontroll-átadás grafikonja — vízszintes tengelyen IaaS→PaaS→SaaS, függőleges tengelyen a szervezet által megtartott kontroll mértéke, csökkenő görbével ábrázolva.]

Forrás: Laudon, K. C., & Laudon, J. P. (2018). Management information systems (15th ed.). Pearson. 5. fejezet.

## 5. Publikus, privát, hibrid felhő döntési logika

(forrás: 10.5.html)

### 5. Publikus, privát, hibrid felhő döntési logika

## Melyik felhő, kinek, mikor?

### Publikus, privát, hibrid felhő — döntési logika

A telepítési modellek közötti választás — publikus, privát vagy hibrid felhő — szintén nem technikai, hanem stratégiai kérdés: attól függ, milyen kockázat-tolerancia, szabályozási környezet és terhelési mintázat jellemzi az adott rendszert.

Egy valós, számszerűsített bizonyíték a hibrid modell mellett. Az EasyJet — az Egyesült Királyság legnagyobb légitársasága — kiváló példa erre. A vállalat meglévő foglalási rendszere nem tudta kezelni az új, ügyfelek által igényelt funkciót (online ülésválasztás). Ahelyett, hogy a teljes mag-rendszert lecserélték volna, az EasyJet megtartotta a kritikus foglalási rendszert saját üzemeltetésben, és csak az új funkciót helyezte a Microsoft Azure nyilvános felhőjébe — ez a hibrid felhő stratégia tankönyvi példája (Laudon & Laudon, 2018). Az eredmény önmagáért beszél: miközben a légiipari átlag a bevétel 2%-át költi IT-re, az EasyJet ezt 0,5%-on tartja, és a vezetés kifejezetten az alacsony árak és a jó ügyfélélmény kombinációját nevezi meg versenyelőnyként.

Modell | Mikor indokolt | 

Privát felhő | Szigorú szabályozás, érzékeny adat, egyedi megfelelőségi igény (pl. banki core rendszer) | 

Publikus felhő | Változó terhelés, nem érzékeny adat, gyors skálázási igény | 

Hibrid felhő | A kritikus mag védett marad, a kiegészítő funkciók kihasználják a publikus felhő rugalmasságát — mint az EasyJet-eset | 

🤔 Kritikai kérdés

Az EasyJet-esetben az egyik vezetői érv az volt, hogy ha az új szolgáltatás nem vált volna be, a felhőalapú komponenst könnyű lett volna egyszerűen kikapcsolni — sokkal könnyebben, mint egy beépített, mag-rendszerbeli funkciót eltávolítani. Milyen más döntéseknél lehet hasznos ez a "könnyű visszavonhatóság" mint szempont?

[Ábra: az EasyJet hibrid architektúrája — a mag-foglalási rendszer helyben, az ülésválasztási modul az Azure felhőben, nyíllal jelezve az integrációt.]

Forrás: Laudon, K. C., & Laudon, J. P. (2018). Management information systems (15th ed.). Pearson. 5. fejezet (EasyJet-esettanulmány).

## 6. A felhő mítoszainak kritikai vizsgálata

(forrás: 10.6.html)

### 6. A felhő mítoszainak kritikai vizsgálata

## A felhő nem mindig olcsóbb, és nem mindig egyszerűbb

### A felhő mítoszainak kritikai vizsgálata

A felhő körüli diskurzus túlnyomó része — beleértve az ÜIA-anyagot is — a felhő előnyeit hangsúlyozza: rugalmasság, skálázhatóság, alacsony belépési költség. Ez a fejezet szándékosan ellenpéldát állít ez elé, mert a kritikus gondolkodáshoz mindkét oldal ismerete szükséges.

A 37signals esete. A 37signals (a Basecamp projektmenedzsment-eszköz és a HEY e-mail szolgáltatás fejlesztője) 2022-ben évi 3,2 millió dollárt költött AWS és Google Cloud szolgáltatásokra — annak ellenére, hogy terhelése kiszámítható, stabil volt, nem hirtelen ingadozó. A vállalat vezetője, David Heinemeier Hansson, így fogalmazott: "Máshol sem keverjük össze a bérlést a tulajdonlással — nem bérelnénk 30 évre egy házat háromszor annyiért, mint amennyibe a törlesztés kerülne."

2022 októberében a cég bejelentette a kilépést a felhőből. Hat hónap alatt, 600 000 dolláros egyszeri hardverbefektetéssel, ugyanazzal a tíz fős üzemeltetői csapattal (egyetlen új alkalmazott felvétele nélkül) sikeresen áttelepítették rendszereiket saját, kollokációs adatközpontokban elhelyezett szerverekre. Az eredmény: a hardverbefektetés hat hónap alatt megtérült, az adatbázis-lekérdezések 3-5-ször gyorsabbá váltak, és a projekció szerint 5 év alatt 10 millió dollár feletti megtakarítást ér el a vállalat. Nem elszigetelt eset: a Dropbox 2016-os hasonló lépése 75 millió dollár megtakarítást hozott 2 év alatt.

⚠️ Mikor igaz a mítosz, és mikor nem?

Fontos leszögezni: ez nem azt jelenti, hogy a felhő rossz döntés — az esettanulmányok szerzői is hangsúlyozzák: a felhő kiválóan teljesít induló vállalkozásoknál és erősen ingadozó terhelésnél (pl. a HEY szolgáltatás indulásakor 3 hét alatt 300 000 felhasználó érkezett a tervezett 30 000 helyett — ezt csak felhő-alapú rugalmassággal lehetett kezelni). A mítosz ott dől meg, ahol a terhelés stabil és kiszámítható — ott a "bérlés" tartósan drágább, mint a "tulajdonlás".

💡 Műszaki analógia

Ez ugyanaz a logika, mint amikor egy építőipari vállalkozás eldönti, hogy megvásárol-e egy exkavátort, vagy minden projektnél bérli: ha a gép folyamatosan, kiszámíthatóan dolgozik, a tulajdonlás hosszú távon olcsóbb; ha csak alkalmanként, változó léptékben van rá szükség, a bérlés ésszerűbb.

[Ábra: a 37signals éves felhőköltségének alakulása 2022 (3,2M USD) → 2023-2024 (fokozatosan 1,3M USD-ra csökkenő), a 600 000 dolláros egyszeri hardverbefektetés megjelölésével a megtérülési ponton.]

🤔 Reflektív kérdés

Milyen jellegű terhelési mintázat jellemzi az Ön saját szervezetét (vagy egy ismert vállalatot) — inkább a 37signals stabil, kiszámítható mintája, vagy a HEY hirtelen, kiszámíthatatlan növekedési mintája? Melyik érvel támasztaná alá a felhő melletti vagy elleni döntést?

Forrás: WheelHouseIT (2025). The AWS Outage of October 2025: Essential Lessons for Business Resilience.; Data Center Dynamics (2025). 37signals claims it saved almost $2m last year from cloud repatriation.; Basecamp (2023). Leaving the Cloud — Cloud Computing Isn't for Everyone. basecamp.com/cloud-exit

## 7. Vendor lock-in és exit-stratégia

(forrás: 10.7.html)

### 7. Vendor lock-in és exit-stratégia

## Mit kellett volna a banknak előre megterveznie?

### Vendor lock-in mint stratégiai kockázat és exit-stratégia

Térjünk vissza a nyitó dilemmához. A csődbe ment felhőszolgáltatóval szembesülő bank problémája nem a csőd bekövetkezése volt — hiszen szolgáltatók csődje, felvásárlása vagy szolgáltatás-megszüntetése mindig lehetséges kockázat. A valódi probléma az volt, hogy a bank ezt a kockázatot nem tervezte be előre.

A vendor lock-in azt jelenti, hogy egy szervezet olyan mértékben függővé válik egy szolgáltatótól, hogy a váltás rendkívül költséges vagy technikailag nehéz lenne. Ez a függőség nemcsak csőd esetén jelent kockázatot — áremelés, szolgáltatásminőség-romlás vagy stratégiai irányváltás (pl. a szolgáltató kivon egy funkciót) esetén is ugyanolyan súlyos lehet.

Az exit-stratégia alapelemei

- Adatkinyerhetőség előzetes tesztelése: nem elég feltételezni, hogy az adatok exportálhatók — rendszeresen tesztelni kell a tényleges exportálási és visszaállítási folyamatot

- Nyílt szabványok előnyben részesítése: a szolgáltató-specifikus, zárt formátumok elkerülése csökkenti a technikai lock-in mértékét

- Migrációs terv és időbecslés előre elkészítve: nem a válsághelyzetben kell először végiggondolni, hogyan nézne ki egy váltás

- Kritikus adatok redundáns, saját mentése: a legfontosabb adatokat a szolgáltatótól függetlenül is tárolni

Hazai kontextus — a szabályozó is ezt várja el. A Magyar Nemzeti Bank 2/2025. (I.13.) számú ajánlása kifejezetten előírja a hazai pénzügyi intézmények számára, hogy felhőszolgáltatás bevezetésekor kötelezően dolgozzanak ki kivezetési stratégiát és akciótervet — beleértve a migrációs tervet, a visszaállítási forgatókönyveket, valamint annak biztosítását, hogy a szolgáltatónál tárolt adatok (éles, tartalék és archív környezetben egyaránt) igazoltan törölhetők legyenek kilépéskor. Ez pontosan azt jelzi, hogy a szabályozó valós, komolyan veendő kockázatnak tekinti azt a helyzetet, amit a nyitó dilemmánk felvázolt — nem elméleti aggodalomról van szó.

🔑 Visszakötés a nyitó dilemmához

Ha a bank a felhőbe költözés pillanatában — nem három évvel később, a csőd bejelentésekor — kidolgozza az exit-stratégiát, a "B" válasz (előre megtervezett terv követése) reális opció lett volna. A nyitó dilemma A és C válasza egyaránt azt mutatja, hogy a szervezet utólag improvizál egy olyan helyzetben, amit elő lehetett volna készíteni.

[Ábra: exit-stratégia döntési folyamatábra — adatkinyerhetőség tesztelése → nyílt szabványok ellenőrzése → migrációs terv elkészítése → redundáns mentés — mind a felhőbe költözés előtt elvégzendő lépésként jelölve, nem utólagosként.]

Forrás: Magyar Nemzeti Bank (2025). 2/2025. (I.13.) számú ajánlás a felhőalapú szolgáltatások igénybevételéről. mnb.hu

## 8. TCO a felhőben

(forrás: 10.8.html)

### 8. TCO a felhőben

## A számla, ami sosem áll meg növekedni

### TCO a felhőben: miért nem mindig olcsóbb

A 8. fejezetben már tárgyaltuk a teljes birtoklási költség (TCO) általános "jéghegy" logikáját — a licencköltség mögött rejlő adatmérnöki munkaidő, integráció, lehetőségköltség. A felhő esetében ez a jéghegy más, felhő-specifikus elemekkel egészül ki, amelyeket érdemes külön kiemelni.

Rejtett költségelem | Miért marad gyakran észrevétlen | 

Adatkiviteli (egress) díjak | A szolgáltatók jellemzően ingyenessé teszik az adatok bevitelét, de díjazzák a kivitelét — ez önmagában lock-in-t erősítő árazási logika | 

Komplexitási költség | A felhő-specifikus jogosultságkezelési és architektúra-szabályrendszerek megtanulása és karbantartása önmagában jelentős, gyakran alul-becsült szakértői idő | 

Skálázódó díjak stabil terhelésnél | A szolgáltatói árazás nem feltétlenül csökken az idővel, még ha a tényleges használat változatlan is marad | 

"Bőség paradoxona" | Az alacsony egyedi költségű szolgáltatások miatt a szervezetek hajlamosak többre előfizetni, mint amire ténylegesen szükségük van — a felhő "digitális polcára minden felfér" | 

⚠️ A kritikus kérdés: mikor fordul meg a mérleg?

A felhő ott a legköltséghatékonyabb, ahol a terhelés erősen ingadozó vagy kiszámíthatatlan (lásd 5. oldal). Minél stabilabb és kiszámíthatóbb egy rendszer terhelése, annál inkább fordul a mérleg a saját üzemeltetés felé — pontosan az ellenkezője annak, amit a köznyelvi "a felhő mindig olcsóbb" narratíva sugall. Az 5. oldalon bemutatott eset pontosan ezt a négy költségelemet nevezte meg utólagos indoklásként, amikor a kilépés mellett döntött.

💡 Műszaki analógia

Ez ugyanaz a logika, mint egy gyártó cég döntése arról, hogy alkalmi különleges szerszámigényét külső bérmunkával oldja-e meg, vagy folyamatosan visszatérő, kiszámítható igényeit inkább saját géppark-bővítéssel. A bérmunka rugalmas, de darabonként drágább; a saját eszköz drágább a beszerzéskor, de olcsóbb hosszú távon, ha a kihasználtság stabil.

[Ábra: két görbe összevetése — a felhő-költség lineárisan/enyhén növekvő görbéje stabil terhelésnél vs. a saját infrastruktúra egyszeri beruházás utáni lapos költséggörbéje, a metszéspont megjelölésével.]

🤔 Gondolkodtató kérdés

Ha egy vállalat vezetése kizárólag a bevezetéskori (első évi) felhőköltséget hasonlítja össze a saját infrastruktúra bevezetési költségével, milyen torzított döntést hozhat?

Forrás: Data Center Dynamics (2025). 37signals claims it saved almost $2m last year from cloud repatriation.; Tick, A. Cloud alapok és Cloud ERP [előadásanyag, ÜIA]. Óbudai Egyetem — a "bőség paradoxona" fogalmának felidézése.

## 9. Felhő-koncentráció és rendszerszintű törékenység

(forrás: 10.9.html)

### 9. Felhő-koncentráció és rendszerszintű törékenység

## Amikor egyetlen régió kiesése megbénítja a fél internetet

### Felhő-koncentráció és rendszerszintű törékenység

Az eddigi oldalak a vállalati szintű kockázatokra fókuszáltak — mit veszíthet egyetlen szervezet. Ez az oldal egy szinttel feljebb lép: mi történik, ha a kockázat nem egyetlen vállalatot, hanem egész iparágakat, sőt a globális digitális infrastruktúrát érinti egyszerre.

Az eset. 2025. október 20-án egy technikai hiba az Amazon Web Services (AWS) egyik amerikai régiójában (Virginia, "US-EAST-1") DNS-feloldási hibát okozott, amely tizenöt órán át tartó, lépcsőzetes összeomláshoz vezetett. A kiesés 3500-nál is több vállalatot érintett 60-nál több országban — köztük bankokat, tőzsdéket, légitársaságokat (pl. Delta Air Lines), kiskereskedelmi láncokat és kórházi rendszereket, amelyek nem tudtak hozzáférni betegadatokhoz. A gazdasági kár becslése több mint 1 milliárd dollár, egyes elemzők szerint jóval magasabb.

⚠️ Ez nem egyszeri baleset volt

A 2025. októberi kiesés volt a harmadik nagyobb incidens öt év alatt, amely ugyanabból az US-EAST-1 régióból eredt. A jelenség oka strukturális: három nagy szolgáltató (AWS, Microsoft Azure, Google Cloud) a globális felhő-infrastruktúra piacának mintegy 60-63%-át birtokolja — ez azt jelenti, hogy a digitális gazdaság jelentős része néhány, egymással versengő, de egyenként is kritikus, egyetlen-pontú-hibaforrást (single point of failure) jelentő szereplőtől függ.

Miért fontos ez a vállalati döntéshozóknak — nem csak az IT-szakembereknek? A multi-cloud stratégia (több szolgáltató párhuzamos használata), amit az ÜIA-anyag a vendor lock-in elleni védekezésként mutat be, nem old meg mindent: ha egy vállalat kritikus rendszere ugyanabban a régióban fut, mint amelyik kiesik, a "több szolgáltató" stratégia sem segít, ha a régión belüli redundancia hiányzik. A valódi kérdés nem csupán az, hogy melyik szolgáltatót válasszuk, hanem hogy hány földrajzi régióra és hány szolgáltatóra terítjük szét a kritikus működést — és ez jelentős, gyakran alábecsült többletköltséggel jár.

💡 Műszaki analógia

Ez ugyanaz a logika, mint amikor egy gyártó vállalat eldönti, hogy egyetlen beszállítótól szerzi-e be egy kritikus alkatrészét (olcsóbb, de sérülékeny egyetlen beszállító-kiesés esetén), vagy több beszállítóval, több gyártási telephellyel dolgozik (drágább, de ellenállóbb). A felhő-koncentráció kockázata pontosan ez — csak digitális infrastruktúra szintjén.

[Ábra: térkép vagy hálózati diagram, amely szemlélteti, hogy a globális felhő-infrastruktúra hány százaléka koncentrálódik három szolgáltatónál (AWS/Azure/Google Cloud ~60-63%), és hogyan terjedt a 2025. október 20-i kiesés hatása több szektorra egyszerre.]

🤔 Kritikai kérdés

Ha a felhő-koncentráció rendszerszintű kockázat, kinek a felelőssége ezt kezelni — az egyes vállalatoké, a szabályozóké, vagy magának a néhány domináns szolgáltatónak? Érvel mindhárom mellett és ellen.

Forrás: WheelHouseIT (2025). The AWS Outage of October 2025: Essential Lessons for Business Resilience.; Demandsage (2026). 54 Internet Outage Statistics.; Built In (2025). What Caused the Massive AWS Outage in 2025?

## 10. Szintézis, az SLA valós jelentése és hazai kitekintés

(forrás: 10.10.html)

### 10. Szintézis, az SLA valós jelentése és hazai kitekintés

## Amit egyetlen döntési helyzet megtanított

### Szintézis: mit jelent a felhő mint stratégiai kockázat?

Térjünk vissza a fejezet elején feltett döntési helyzethez: a bank informatikai igazgatójaként Ön a felhőszolgáltató csődjével szembesül.

A fejezet nyolc oldala egyetlen üzenetet közvetít sokféle nézőpontból: a felhő nem "belépés egy biztonságos, gondtalan szolgáltatásba", hanem egy stratégiai függőségi viszony, amelyet ugyanolyan tudatossággal kell megtervezni, mint bármely más kritikus beszállítói kapcsolatot. Az IT-infrastruktúra evolúciójának inga-mozgása (2. oldal) megmutatta, hogy a centralizáció kockázatai nem újak. A szolgáltatási és telepítési modellek döntési logikája (3–4. oldal) megmutatta, hogy minden szint kontroll-átadással jár. A 37signals-eset (5. oldal) megkérdőjelezte az "mindig olcsóbb" mítoszt, a felhő-specifikus TCO-elemzés (7. oldal) pedig megmutatta ennek pontos mechanizmusát.

⚠️ Két kockázat, amit nem szabad összemosni

A 6. és a 8. oldal két, egymástól elkülönítendő kockázattípust tárgyalt: a vendor lock-in (6. oldal) egy vállalati szintű, szolgáltató-specifikus ragadósság — nehéz és költséges lenne váltani —, míg a felhő-koncentráció (8. oldal) egy rendszerszintű, iparági törékenység — ha az egész iparág néhány szolgáltatóra épül, egyetlen kiesés mindenkit érint egyszerre, függetlenül attól, hogy az adott vállalat mennyire volt "ragadós" kapcsolatban a szolgáltatóval. Az első ellen az exit-stratégia védekezik; a második ellen a multi-region/multi-cloud redundancia — de egyik sem oldja meg a másikat.

Az SLA mint a döntés utolsó rétege. Miután egy szervezet átgondolta a szolgáltatási modellt, a telepítési modellt, a TCO-t és mindkét kockázattípust, végül szembe kell néznie azzal is, mit garantál ténylegesen a szolgáltatási szintű megállapodás (SLA). A szolgáltatók jellemzően korlátozzák saját felelősségüket, és a nem tervezett leállás miatti kompenzáció többnyire csak jövőbeli szolgáltatás igénybevételére felhasználható szolgáltatási kreditek formájában érhető el — nem a ténylegesen elszenvedett üzleti veszteséget fedező kártérítés. Vagyis ha egy 15 órás kiesés (8. oldal) milliárd dolláros kárt okoz az érintett vállalatoknak összesen, a szolgáltató SLA-kompenzációja ennek töredékét sem fedezi — a tényleges üzleti kockázatot mindvégig a szolgáltatást igénybe vevő szervezet viseli, nem a szolgáltató. Ez az oka annak, hogy az exit-stratégia (6. oldal) és a redundancia-tervezés (8. oldal) nem "extra elővigyázatosság", hanem az egyetlen tényleges védekezés — az SLA önmagában nem az.

🔑 Hazai kitekintés

Ez a felismerés Magyarországon már szabályozói szintre emelkedett: a Magyar Nemzeti Bank 2/2025-ös ajánlása (6. oldal) kötelező érvénnyel írja elő a kivezetési stratégia kidolgozását a hazai pénzügyi intézmények számára — vagyis a szabályozó sem bízik abban, hogy egy SLA önmagában elegendő védelmet nyújt. Ezzel párhuzamosan valós, dokumentált hazai implementáció is létezik: az MBH Bank 2023-ban élesített egy felhőalapú, konténerizált (OpenShift) platformot, amely a három jogelőd bank ügyfeleinek egységes kiszolgálását teszi lehetővé — jól mutatva, hogy a hazai bankszektor aktívan halad a felhő-alapú architektúrák felé, méghozzá a szabályozó által előírt kockázatkezelési keretek mellett.

Záró reflektív kérdés: Ha Ön most, a fejezet végén, újra megkapná a nyitó döntési helyzetet — milyen egyetlen kérdést tenne fel a vezetőségnek, mielőtt a bank a felhőbe költözés mellett dönt, nem utána?

A következő fejezetben (11.) az Etika, algoritmusok és felelős AI témájára térünk át.

Forrás: Magyar Nemzeti Bank (2025). 2/2025. (I.13.) számú ajánlás.; MBH Bank Nyrt. (2024). 2024. április 29-i éves rendes közgyűlésének dokumentumai.

## 11. Elmélyítő Kiegészítő

(forrás: 10.11.html)

### 11. Elmélyítő Kiegészítő
Harmon, R., Vytelingum, P., & Babaie-Harmon, J. (2021). Cloud concentration risk: A framework agent based model for systemic risk analysis. Journal of Financial Compliance, 4(4).
Program on International Financial Systems. (2023). Cloud adoption in the financial sector and concentration risk. PIFS. https://www.fsb.org/uploads/PIFS.pdf

Magyar Nemzeti Bank. (2025). 2/2025. (I.13.) számú ajánlás a felhőalapú szolgáltatások igénybevételéről. mnb.hu

Opara-Martins, J., Sahandi, R., & Tian, F. (2016). Critical analysis of vendor lock-in and its impact on cloud computing migration: A business perspective. Journal of Cloud Computing, 5(1), 4. https://doi.org/10.1186/s13677-016-0054-z

"CVL: A Cloud Vendor Lock-In Prediction Framework." (2024). Mathematics, 12(3), 387. https://doi.org/10.3390/math12030387

## 1. 10. fejezet: Felhő és IT-infrastruktúra — Opcionális Könyv (fogalmi felidézés)

(forrás: 10.12.html)

### 1. 10. fejezet: Felhő és IT-infrastruktúra — Opcionális Könyv (fogalmi felidézés)

## 2. SaaS/PaaS/IaaS/iPaaS fogalmi meghatározása

(forrás: 10.13.html)

### 2. SaaS/PaaS/IaaS/iPaaS fogalmi meghatározása

## Amit a felhő-szolgáltatási modellek technikailag jelentenek

### SaaS/PaaS/IaaS/iPaaS — fogalmi felidézés

A Kötelező Könyv 3. oldala a szolgáltatási modellek közötti döntési logikára fókuszált. Az alábbiakban a technikai fogalmi meghatározások következnek, felidézésül.

Modell | Mit biztosít a szolgáltató | Tipikus felhasználó | 

IaaS (Infrastructure as a Service) | Szerverek, tárolókapacitás, hálózati erőforrások, virtualizáció | IT-szakemberek, fejlesztők | 

PaaS (Platform as a Service) | Az IaaS elemei + operációs rendszer, fejlesztői eszközök, adatbázis-kezelő rendszer | Alkalmazásfejlesztők | 

SaaS (Software as a Service) | Kész, azonnal használható alkalmazás — a szolgáltató kezel mindent | Végfelhasználók, üzleti területek | 

iPaaS (Integration Platform as a Service) | Különböző rendszerek (ERP, CRM, BI) közötti felhőalapú integráció | IT-integrátorok, rendszergazdák | 

Ha ezeket a fogalmakat részletesebben, konkrét vállalati példákkal (SAP S/4HANA Cloud, Microsoft Azure App Service, MuleSoft stb.) szeretné felidézni, nézze át az Üzleti Informatikai Alkalmazások tárgy "Felhőalapú és mobil üzleti alkalmazások, szoftverpiaci modellek" előadását.

Forrás: Laudon, K. C., & Laudon, J. P. (2018). Management information systems (15th ed.). Pearson. 5. fejezet.

## 3. Telepítési modellek fogalmi meghatározása

(forrás: 10.14.html)

### 3. Telepítési modellek fogalmi meghatározása

## Publikus, privát, hibrid, multi-cloud — a technikai definíciók

### Telepítési modellek fogalmi felidézése

Modell | Definíció | 

Publikus felhő | Külső szolgáltató üzemelteti, megosztott infrastruktúrán, interneten keresztül bérelve | 

Privát felhő | Kizárólag egy szervezet számára fenntartott infrastruktúra, saját vagy bérelt dedikált környezetben | 

Hibrid felhő | A publikus és privát felhő kombinációja — érzékeny adat védett környezetben, kevésbé kritikus folyamat publikus felhőben | 

Multi-cloud | Több különböző felhőszolgáltató párhuzamos használata, funkciónként eltérő szolgáltatóval | 

Ha ezeket a modelleket részletesebben, a Shared Responsibility Model teljes bontásával (IaaS/PaaS/SaaS szerinti felelősségi körök) szeretné felidézni, nézze át az Üzleti Informatikai Alkalmazások tárgy "Felhőalapú és mobil üzleti alkalmazások, szoftverpiaci modellek" előadását.

Forrás: Laudon, K. C., & Laudon, J. P. (2018). Management information systems (15th ed.). Pearson. 5. fejezet.

## 4. Az SLA felépítése

(forrás: 10.15.html)

### 4. Az SLA felépítése

## Mi van valójában egy szolgáltatási szintű megállapodásban?

### Az SLA felépítése és tipikus elemei

Egy tipikus felhő-SLA (Service Level Agreement) a következő elemekből épül fel:

Elem | Mit szabályoz | 

Rendelkezésre állási garancia | Jellemzően "99,9%+" formában megadva — évi kb. 8,7 óra megengedett kiesésnek felel meg | 

Válaszidő-vállalás | Hiba bejelentésétől a reagálásig eltelt idő, súlyossági szint szerint differenciálva | 

Kompenzációs záradék | Mit kap az ügyfél, ha a szolgáltató nem teljesíti a vállalt szintet — lásd a Kötelező Könyv 9. oldalának kritikai megjegyzését erről | 

Kizárások | Tervezett karbantartás, vis maior, harmadik fél hibája — ezekre jellemzően nem terjed ki a garancia | 

Forrás: Laudon, K. C., & Laudon, J. P. (2018). Management information systems (15th ed.). Pearson. 5. fejezet.

## 5. Az IT-infrastruktúra evolúciójának technikai állomásai

(forrás: 10.16.html)

### 5. Az IT-infrastruktúra evolúciójának technikai állomásai

## Mainframe-től a felhőig — a technikai részletek

### Az IT-infrastruktúra evolúciójának technikai állomásai

A Kötelező Könyv 2. oldala az evolúció inga-mozgás jellegére fókuszált. Az alábbi táblázat a technikai állomásokat sorolja fel részletesebben.

Korszak | Jellemző technológia | 

1950-es évek | Elektroncsöves számítógépek | 

1960–70-es évek | Tranzisztoros és mainframe-korszak | 

1980-as évek | Személyi számítógép (PC) forradalom | 

1990-es évek | Kliens-szerver architektúra, vállalati hálózatok | 

2000-es évek | Internetalapú vállalati számítástechnika | 

2010-es évektől | Felhőalapú számítástechnika, mobil és hordható eszközök | 

Forrás: Laudon, K. C., & Laudon, J. P. (2018). Management information systems (15th ed.). Pearson. 5. fejezet.
