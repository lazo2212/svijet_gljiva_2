<script setup lang="ts">
import { onMounted } from 'vue'
import { gsap } from 'gsap'
import { ScrollTrigger } from 'gsap/ScrollTrigger'

gsap.registerPlugin(ScrollTrigger)

onMounted(() => {
  const sections = document.querySelectorAll('section')

  sections.forEach((section) => {
    gsap.from(section, {
      opacity: 0,
      y: 50,
      duration: 1,
      scrollTrigger: {
        trigger: section,
        start: 'top 80%',
        end: 'top 30%',
        toggleActions: 'play none none reverse'
      }
    })
  })
})
</script>

<template>
  <header>
    <h1>Gljive</h1>
    <span>Istražite svijet ovih čudesnih organizama</span>
  </header>

  <main>
    <section>
      <h1>Dobrodošli u tajanstveni svijet gljiva</h1>
      <p>
        Zamislite svijet skriven ispod površine tla, svijet u kojem mreže finih niti, nevidljive
        golom oku, povezuju biljke, drveće i tlo u veliku, živu mrežu. To je kraljevstvo gljiva –
        jedno od najčudesnijih, najskrivenijih i još uvijek nedovoljno istraženih područja živoga
        svijeta.
      </p>

      <p>
        Iako su dugo smatrane biljkama, gljive zapravo čine posebno carstvo – carstvo Fungi. One
        nisu biljke, nisu ni životinje, ali dijele s njima mnoge osobine. Za razliku od biljaka,
        gljive ne sadrže klorofil i ne provode fotosintezu. One se hrane poput životinja – upijajući
        hranjive tvari iz svoje okoline. Ali to čine na svoj način: tiho, neprimjetno, često noću
        ili u sjeni šume, razgrađujući lišće, drvo, pa čak i stijene.
      </p>

      <p>
        Ako ste ikada zakoračili u šumu nakon kiše, sigurno ste osjetili onaj osebujni, zemljani
        miris. To su gljive na djelu. Njihov nevidljivi micelij proteže se kilometrima ispod vaših
        nogu, a tu i tamo iz tog mrežastog podzemnog tijela izroni plodište – ono što mi zovemo
        gljivom. Možda je to crvena muhara sa snježnobijelim točkama, možda zlatna lisičica ili
        krupni vrganj skriven pod lišćem.
      </p>

      <p>
        No, gljive nisu samo lijepe, ukusne ili opasne – one su temelj života u šumama. Bez njih,
        šume bi se ugušile u vlastitom otpadu. Gljive razgrađuju ono što je umrlo i vraćaju hranjive
        tvari natrag u tlo. One su ekološki reciklažni sustav planeta, bez kojeg ne bi bilo ni
        bilja, ni životinja – ni nas.
      </p>

      <p>
        U našoj priči upoznat ćete različite skupine gljiva – od mikroskopskih plijesni koje rastu
        na voću, do tartufa skrivenih ispod tla koje pronalaze dresirani psi. Naučit ćete
        razlikovati askomicete od bazidiomiceta, saznat ćete što je to mikoriza i zašto je smrčak
        toliko cijenjen među gurmanima.
      </p>

      <p>
        Ovdje se znanost susreće s čudom. Gljive nas uče o životu, povezanosti i promjeni. Njihove
        spore putuju zrakom, koloniziraju nova mjesta, i nastavljaju vjekovnu priču o
        preživljavanju, prilagodbi i suživotu.
      </p>

      <p>Pridružite nam se i zaronite dublje u svijet gljiva. Ovdje počinje potraga – gljive!</p>
    </section>

    <section>
      <h2>Vrste gljiva – bogatstvo oblika i uloga</h2>

      <p>
        Kad pomislimo na gljivu, često nam u mislima izroni klasična slika – šešir s klobukom, možda
        čak crvena sa bijelim točkicama. No, istina je mnogo bogatija. Gljive dolaze u nevjerojatnim
        oblicima, veličinama i bojama, a njihova klasifikacija otkriva svijet raznolikosti koji
        skriva mnogo više nego što se vidi na prvi pogled.
      </p>

      <h3>Askomiceti – čarobnjaci pod mikroskopom</h3>

      <p>
        Askomicete ili vrećaste gljive su možda najraznolikija skupina. Njihova plodišta su često
        mala, ali moćna. U ovu skupinu spadaju kvasci koji omogućuju da kruh naraste i vino
        fermentira, ali i tartufi – podzemne dragocjenosti koje gurmani traže diljem svijeta.
        Njihovo ime dolazi od “asca”, što znači vrećica – jer unutar mikroskopskih vrećica stvaraju
        svoje spore.
      </p>

      <h3>Bazidiomiceti – klasične šumske zvijezde</h3>
      <p>
        Bazidiomicete su one “prave” gljive koje najčešće nalazimo u šumi – vrganji, lisičarke,
        sunčanice, pa i zloglasne muhare i zelene pupavke. Njihovo ime dolazi od posebne strukture
        zvanog “bazidij” u kojoj nastaju spore. Ove gljive često oblikuju složena, vidljiva plodišta
        i najčešće ih vežemo uz šumske staze i mahovine.
      </p>

      <h3>Gljive lišajeva – simbioza u najčišćem obliku</h3>
      <p>
        Neke gljive žive u bliskom zagrljaju s algama i tvore ono što zovemo lišajevima. Iako nisu
        prava taksonomska skupina, ove simbioze su fascinantan primjer suradnje – gljiva pruža
        strukturu i zaštitu, a alga daje hranu putem fotosinteze. Skupa, mogu preživjeti i na
        najnepristupačnijim mjestima – od stijena u planinama do kora drveća u urbanim sredinama.
      </p>

      <h3>Mikroskopske gljive – svijet skriven oku</h3>
      <p>
        Ne smijemo zaboraviti ni mikroskopske gljive – plijesni i kvasce. Iako često povezane s
        propadanjem hrane, neke od njih su neprocjenjive u medicini i industriji. Penicillium, na
        primjer, dao nam je prvi antibiotik – penicilin – dok kvasci omogućuju proizvodnju kruha,
        vina i piva još od vremena starih Egipćana.
      </p>

      <p>
        Gljive su sveprisutne, iako ih često ne primjećujemo. One rastu na drveću, u zemlji, na
        hrani, pa čak i unutar živih organizama. Neke su jestive i ljekovite, druge smrtonosne. Neke
        su jednostavne, druge toliko složene da zbunjuju i iskusne mikologe.
      </p>

      <p>
        U sljedećem poglavlju priče zavirit ćemo u ulogu koju gljive imaju u ekosustavu. Jer gljive
        nisu samo individualni organizmi – one su poveznice koje omogućuju život cijelih šuma.
      </p>
    </section>

    <section>
      <h2>Tajne ispod tla – uloga gljiva u prirodi</h2>

      <p>
        Duboko ispod šumskog tla, gdje korijenje drveća plete svoje puteve, gljive vode vlastiti,
        tihi život. Ne vidiš ih, ali one rade danonoćno – bez odmora, bez buke. Njihov svijet je
        svijet mreža, razgradnje, savezništva i obnavljanja.
      </p>

      <h3>Razlagači – čistači prirode</h3>
      <p>
        Zamisli da u šumi padne stablo. Tko će ga razgraditi? Tko će mrtvo pretvoriti u novo? Tu na
        scenu stupaju gljive – moćni razlagači. One razgrađuju lišće, drvo, životinjske ostatke i
        pretvaraju ih u hranjive tvari koje se vraćaju zemlji. Bez gljiva, priroda bi se ugušila u
        vlastitom otpadu. Sve bi stajalo – ništa se ne bi vraćalo natrag u ciklus života.
      </p>

      <h3>Mikorizne gljive – tajna simbioza s biljkama</h3>
      <p>
        Ispod površine zemlje skriva se najfascinantnije partnerstvo prirode – mikoriza. To je
        simbioza između gljiva i korijenja biljaka. Gljiva pomaže biljci da upije vodu i minerale, a
        zauzvrat dobiva šećere koje biljka stvara fotosintezom. Ovo savezništvo postoji milijunima
        godina – i bez njega mnoge biljke, pa ni šume, ne bi mogle opstati.
      </p>

      <p>
        Znanstvenici to zovu “Wood Wide Web” – mreža podzemnih gljiva koja povezuje stabla,
        omogućava im da razmjenjuju hranjive tvari, pa čak i upozorenja o opasnosti. Da, stabla
        “razgovaraju”, a gljive su njihovi tihi posrednici.
      </p>

      <h3>Paraziti i patogeni – tamna strana</h3>
      <p>
        Nisu sve gljive pomagači. Neke uzimaju bez davanja – parazitske gljive napadaju biljke,
        kukce, pa čak i druge gljive. Imaju važnu ulogu jer sprječavaju prenapučenost, održavaju
        ravnotežu, ali mogu uzrokovati i bolesti – u šumi, na poljima, pa i u ljudskom tijelu. No
        čak i te, često nevoljene vrste, imaju svoje mjesto u velikom krugu života.
      </p>

      <p>
        Bez gljiva, priroda bi stala. One su skriveni motori života – razgrađuju, hrane, povezuju i
        štite. Svaki korak koji napravimo po šumskoj stazi, svaki list koji šušne pod nogom, moguć
        je zahvaljujući njihovom tihom radu.
      </p>

      <p>Sljedeći put vodi te među ljude i povijest – u Kulturni značaj gljiva.</p>
    </section>

    <section>
      <h2>Gljive kroz oči ljudi – od mita do tanjura</h2>

      <p>
        Gljive nisu samo stanovnici šuma – one su i dio naših priča, vjerovanja, obreda i tanjura
        već tisućama godina. U nekim kulturama smatrane su svetima, u drugima otrovnima i
        zlokobnima. I danas, one nas fasciniraju – tajnovite, neuhvatljive i ponekad opasne.
      </p>

      <h3>Gljive u mitovima i obredima</h3>
      <p>
        Drevni narodi vjerovali su da gljive posjeduju čudesne moći. U šamanskim kulturama Sjeverne
        i Južne Amerike koristile su se tzv. “svete gljive” – psihodelične vrste poput Psilocybe, za
        povezivanje s duhovima i bogovima. Njihovi obredi bili su puni vizija, boja i zvukova koje
        je samo svijet gljiva mogao otvoriti.
      </p>

      <p>
        U Sibiru su narodi koristili Amanitu muscariu, crvenu muhara s bijelim točkicama, u
        ritualima. Zanimljivo – neka istraživanja povezuju baš tu gljivu sa starim pričama o Djedu
        Božićnjaku. Crveno-bijela odjeća, letenje kroz zrak, darovi – sve podsjeća na vizije koje su
        ljudi imali pod njezinim utjecajem. Simbolika i praznovjerja
      </p>

      <p>
        U Europi su gljive često bile simbol nepoznatog i neobjašnjivog. Ljudi su se bojali onih
        koje niču iz ničega – doslovno preko noći – pa su ih povezivali s vilama, vješticama i
        vražjim poslovima. “Vilinski krugovi”, one savršeno kružne nakupine gljiva u travi, smatrani
        su mjestima sabata ili vilinskih plesova. Tko bi zakoračio unutra, govorkalo se, mogao bi
        zauvijek nestati u svijetu bajki.
      </p>

      <h3>Gljive u kulinarstvu</h3>
      <p>
        S druge strane, gljive su i delikatesa. Od tartufa, “crnog zlata” koje se traži uz pomoć
        svinja i pasa, do jednostavnih vrganja i lisičarki – gljive su sastavni dio kuhinja diljem
        svijeta. U Japanu se obožavaju shiitake, u Italiji porcini, a u Slavoniji vrganji na žaru s
        malo soli i maslaca znaju biti rajski obrok.
      </p>

      <p>
        Ipak, nije svaka gljiva dobrodošla na tanjur. Neke su smrtonosne već u malim količinama. Uče
        nas oprezu, znanju i poštovanju prirode.
      </p>

      <p>
        Gljive su nas hranile, liječile, zbunjivale i nadahnjivale. Dio su bajki, legendi i
        svakodnevice. One su granica između stvarnog i nestvarnog – i baš zato ih volimo.
      </p>

      <p>Sljedeći dio vodi nas dublje u ljudsku vezu s gljivama: Gljive i medicina.</p>
    </section>

    <section>
      <h2>Tihi iscjelitelji: Gljive u službi zdravlja</h2>

      <p>
        Nisu sve gljive za jelo – ali mnoge su za liječenje. Od dalekih kineskih planina do modernih
        laboratorija, gljive su stotinama godina pomagale čovjeku da preživi, ozdravi, pa čak i
        pronađe nove načine borbe protiv bolesti. One su poput starog ljekarnika iz šume –
        nenametljive, ali moćne.
      </p>

      <h3>Antibiotici iz gljiva</h3>
      <p>
        Sve je počelo kad je Alexander Fleming 1928. godine slučajno otkrio da gljivica Penicillium
        ubija bakterije oko sebe. Tako je nastao prvi antibiotik – penicilin. Taj je trenutak
        promijenio svijet. Od tada, gljive su postale neiscrpan izvor lijekova – antibiotika,
        imunosupresiva, pa čak i lijekova za snižavanje kolesterola.
      </p>

      <h3>Ljekovite gljive u tradicionalnoj medicini</h3>
      <p>
        U kineskoj medicini, gljive poput Reishi (Ganoderma lucidum), Cordyceps i Maitake poštuju se
        kao “eliksiri života”. Reishi se naziva i “gljivom besmrtnosti” jer jača imunitet i smanjuje
        stres. Cordyceps, gljiva koja raste iz tijela insekata (da, zvuči jezivo), koristi se za
        povećanje energije i izdržljivosti – čak je bila tajno oružje nekih sportaša u 90-ima.
      </p>

      <h3>Moderna istraživanja i psihoterapija</h3>
      <p>
        U posljednjih desetak godina, psihodelične gljive ponovno ulaze u medicinu – ali sada kroz
        prizmu znanosti. Aktivna tvar psilocibin, koju sadrže neke “magične gljive”, pokazuje snažne
        učinke u liječenju depresije, anksioznosti, pa čak i ovisnosti. Klinička istraživanja u
        SAD-u, Kanadi i Europi donose sve više dokaza da uz stručno vodstvo, gljive mogu pomoći
        ljudima da se pomire sa sobom, s drugima i sa svijetom.
      </p>

      <h3>Prevencija i budućnost</h3>
      <p>
        Gljive su i probiotici, i adaptogeni, i antioksidansi. Istražuju se za borbu protiv raka,
        Alzheimerove bolesti i dijabetesa. Ono što znamo sigurno – tek smo na početku razumijevanja
        njihove prave moći.
      </p>

      <p>
        U svijetu medicine, gljive su tiha revolucija. One nas podsjećaju da priroda još uvijek zna
        više nego mi – samo je treba pažljivo slušati.
      </p>

      <p>
        Sljedeći odlomak nas vodi: Kako razlikovati gljive – znanost ili sreća?, gdje ulazimo u
        avanturu prepoznavanja vrsta.
      </p>

      <p>Spremni za šumski izazov?</p>
    </section>

    <section>
      <h2>Prepoznavanje gljiva: Umijeće, instinkt i malo sreće</h2>

      <p>
        Zamislimo da hodaš šumom. Vlaga se lijepi za kožu, sunce se probija kroz krošnje, a ispred
        tebe – savršena gljiva. Krupna, čvrsta, mirisna. No je li to delicija ili opasna prevara?
      </p>

      <p>
        Razlikovati gljive nije samo pitanje znanja – to je vještina koja se razvija godinama.
        Ponekad čak i iskusni gljivari zastanu, sumnjičavo pogledaju šešir gljive i zaključe: “Neka,
        neka ostane tu.”
      </p>

      <h3>Isti oblik, druga sudbina</h3>
      <p>
        Najveća opasnost u svijetu gljiva je dvojnica – jestiva i otrovna gljiva koje izgledaju
        gotovo isto. Recimo, blagva i zelena pupavka. Jedna je kraljica stola, druga ti može
        zaustaviti jetru. A razlika? Nekad tek u boji listića ili mirisu koji osjetiš samo kad
        prerežeš dršku.
      </p>

      <h3>Čulo mirisa i dodira</h3>
      <p>
        Neke gljive imaju specifičan miris – na primjer, pečurka miriše na anis ili badem. Zelena
        pupavka je više metalna, hladna. Neke se raspadnu pod prstima, druge “krvare” kad ih
        prerežeš. Iskusni gljivari znaju: pipni, pomiriši, pažljivo gledaj.
      </p>

      <h3>Priručnici, aplikacije, ali oprezno</h3>
      <p>
        Danas postoje knjige i aplikacije za prepoznavanje gljiva, ali one ne mogu zamijeniti
        iskustvo. Fotografija može prevariti. Uvjeti rasta, doba godine, stanište – sve to mijenja
        izgled gljive. Ako nisi siguran – nemoj je brati. A pogotovo je nemoj jesti.
      </p>

      <h3>Zlatno pravilo gljivarenja</h3>
      <p>
        Ako postoji i najmanja sumnja – ostavi gljivu. Ne postoji gljiva toliko ukusna da vrijedi
        života.
      </p>

      <p>
        Prepoznavanje gljiva je kao detektivski posao – svaki detalj je važan. Nije stvar samo u
        sreći, već u pažnji, strpljenju i poštovanju prema prirodi.
      </p>

      <p>U idućem dijelu pričamo o Najsmrtonosnijim gljivama – kad šuma skriva tamnu stranu.</p>
    </section>

    <section>
      <h2>Tamna strana šume: Gljive koje ubijaju</h2>

      <p>
        U bajkama su gljive često šarene i opasne – crvene s bijelim točkicama, poput mušmule. No
        stvarni otrovi često nemaju to upozoravajuće lice. Prave ubojice skrivaju se pod maskom
        običnosti. Neke su čak lijepe. Zavaravajuće. Tihe.
      </p>

      <h3>Zelena pupavka – tihi ubojica</h3>
      <p>
        Zelena pupavka (Amanita phalloides) izgleda nevino. Zelena kapa, bijela drška, raste među
        bukvama i hrastovima. No ova gljiva je odgovorna za više od 90% smrtnih slučajeva trovanja
        gljivama u Europi.
      </p>

      <p>
        Simptomi se ne pojavljuju odmah – čak ni do 24 sata. Taman kad pomisliš da si dobro, tijelo
        počne kolabirati iznutra. Jetra prva strada. A onda i bubrezi.
      </p>

      <h3>Muhara – otrov s halucinacijom</h3>
      <p>
        Crvena muhara (Amanita muscaria) je prava zvijezda bajki. Možda ti djeluje simpatično, ali
        sadrži otrove koji uzrokuju mučninu, zbunjenost i halucinacije. U nekim kulturama se
        koristila ritualno, ali bez točne doze – vrlo je rizična.
      </p>

      <h3>Vještičina metla – mala, ali smrtonosna</h3>
      <p>
        Neke gljive ne ubijaju odmah, ali stvaraju trajnu štetu. Galerina marginata, mala i
        neugledna, sadrži iste toksine kao i zelena pupavka. Raste na trulim panjevima i često se
        miješa s jestivim vrstama.
      </p>

      <h3>Podmuklost bez okusa i mirisa</h3>
      <p>
        Najopasnije gljive često nemaju gorak okus, loš miris ili sumnjiv izgled. Upravo zato su
        toliko opasne. Ne upozore te – jednostavno djeluju kad je već prekasno.
      </p>

      <p>
        Nisu sve gljive opasne. No one koje jesu – ne daju drugu šansu. U šumi, znanje spašava
        život.
      </p>

      <p>
        Sljedeći odlomak nosi malo vedrije tonove – Gljive kroz povijest: od čarobnih napitaka do
        carskih stolova.
      </p>
    </section>

    <section>
      <h2>Putovanje kroz vrijeme s gljivama</h2>

      <p>
        Kroz tisuće godina ljudi su gljive gledali s divljenjem, strahopoštovanjem – pa čak i s
        dozom magije. Bile su lijek, otrov, hrana za careve, ali i sastojak u tajanstvenim obredima.
      </p>

      <h3>Drevne civilizacije i sveta gljiva</h3>
      <p>
        U starim kulturama, poput astečke, gljive nisu bile samo hrana – bile su sveti simboli.
        Teonanácatl – „božanska gljiva“ – koristila se u ritualima kako bi ljudi „razgovarali s
        bogovima“. Smatralo se da otvaraju vrata u duhovne svjetove.
      </p>

      <p>
        Stari Egipćani vjerovali su da su gljive „dar od boga Ozirisa“ i da ih obični smrtnici ne
        smiju jesti – bile su rezervirane za faraone.
      </p>

      <h3>Rimljani i car smrti</h3>
      <p>
        Rimljani su bili poznati po ljubavi prema gljivama, ali i po njihovoj upotrebi u… političkim
        igrama. Car Klaudije navodno je otrovan zelenom pupavkom, koju mu je podmetnula supruga
        Agripina – želeći tron za svog sina Nerona. Tako je gljiva odlučila tko će vladati Rimom.
      </p>
      <h3>Srednji vijek: strah i praznovjerje</h3>
      <p>
        U srednjem vijeku gljive su bile opasne, ali i mistične. Ljudi su ih povezivali s vješticama
        i vragom. Vjerovalo se da gljive rastu tamo gdje je vrag zakoračio, pa je i naziv "vještičji
        krug" (prsten gljiva u travi) dobio mračnu simboliku.
      </p>

      <h3>Gljive kao carski užitak</h3>
      <p>
        U Kini i Japanu, gljive poput shiitake i reishi koristile su se tisućama godina – ne samo
        zbog okusa, već i zbog svojih ljekovitih svojstava. Samo su ih carevi i plemstvo smjeli
        konzumirati.
      </p>

      <p>
        Dakle, gljive nisu samo sastojci za ručak – one su stoljećima bile dio misterija, moći i
        borbe za vlast. A i danas, kad ih stavimo u juhu ili na pizzu, nosimo djelić te povijesti sa
        sobom.
      </p>

      <p>
        U sljedećem poglavlju istražujemo šumske lijekove – prirodnu apoteku koja se skriva među
        drvećem. Kako su gljive postale naši saveznici u borbi protiv bolesti? Kako su nas naučile
        da slušamo prirodu?
      </p>
    </section>

    <section>
      <h2>Šumski lijekovi koje su zaboravili samo oni koji ne idu u šumu</h2>

      <p>
        Zamislite da umjesto da odete u ljekarnu, jednostavno zakoračite u šumu. Tamo, među
        mahovinom i lišćem, rastu gljive koje su stoljećima služile kao prirodni lijekovi. Iako
        moderna medicina često zaboravlja na njih, mnoge kulture nikada nisu prestale vjerovati u
        njihovu moć.
      </p>

      <h3>Reishi – gljiva besmrtnosti</h3>
      <p>
        U tradicionalnoj kineskoj medicini reishi (Ganoderma lucidum) nosi titulu „gljive
        besmrtnosti“. Koristila se za jačanje imuniteta, smanjenje stresa i produljenje života. Nije
        ukusna, ali je moćna – kuhala se kao čaj ili uzimala u obliku ekstrakta.
      </p>

      <h3>Chaga – crni zlato sjevera</h3>
      <p>
        Na sjeveru Europe i Sibira raste chaga – crna gljiva koja izgleda kao spaljeni komad drveta.
        No iznutra krije antioksidanse, vitamine i spojeve koji mogu pomoći kod upala, probave, pa
        čak i kod borbe protiv stanica raka.
      </p>

      <h3>Lavlja griva – hrana za mozak</h3>
      <p>
        Ova neobična, čupava gljiva ne izgleda kao ništa drugo u šumi. Zovu je lavlja griva
        (Hericium erinaceus), a poznata je po svojoj sposobnosti da potiče rast moždanih stanica.
        Istraživanja pokazuju da može pomoći kod problema s pamćenjem i neurodegenerativnih bolesti
        poput Alzheimera.
      </p>

      <h3>Cordyceps – energija iz prirode</h3>
      <p>
        Ova gljiva zapravo parazitira kukce, ali ljudi je već stoljećima koriste za povećanje
        energije, izdržljivosti i poboljšanje funkcije pluća. U modernom svijetu postala je
        popularna među sportašima i rekreativcima.
      </p>

      <p>
        Ljekovite gljive nisu čudo – one su rezultat prirodne evolucije i suživota s ljudima. Danas
        ih ponovno otkrivamo, koristeći ih u suplementima, čajevima i prahovima, ali njihova snaga
        dolazi iz istog mjesta kao i prije tisuću godina – iz šume.
      </p>

      <p>
        U sljedećem poglavlju istražujemo putovanje u druge dimenzije – kako su gljive oblikovale
        ljudsku kulturu i duhovnost kroz povijest.
      </p>

      <p>
        Pripremite se za putovanje kroz vrijeme i prostor, gdje gljive nisu samo hrana, već i vodiči
        u nepoznato.
      </p>
    </section>

    <section>
      <h2>Putovanje u druge dimenzije</h2>

      <p>
        Psilocibinske gljive, često nazvane „magične gljive“, nisu samo dio mitologije i urbanih
        legendi, već imaju bogatu povijest korištenja u mnogim kulturama diljem svijeta. Ove gljive
        sadrže psilocibin, psihoaktivnu tvar koja može izazvati duboka, introspektivna iskustva i
        promjene u percepciji.
      </p>

      <h3>Povijest u tradicijama</h3>
      <p>
        Već tisućama godina, psilocibinske gljive korištene su u ritualima i ceremonijama. U
        Meksiku, na primjer, teonanacatl (božanska gljiva) bila je korištena u vjerskim obredima,
        pomažući ljudima da stupe u kontakt s božanstvima. Šamani su vjerovali da im gljive pomažu
        da prenesu poruke iz drugih svjetova.
      </p>

      <h3>Novi val znanstvenih istraživanja</h3>
      <p>
        Iako je zbog svoje psihodeličke prirode psilocibin bio dugo zabranjen, u posljednjih
        nekoliko desetljeća svjedočimo povratku interesa za ovu gljivu, sada u kontekstu modernih
        znanstvenih istraživanja. Istraživanja su pokazala da psilocibin može imati terapeutski
        učinak kod ljudi koji pate od depresije, anksioznosti, post-traumatskog stresnog poremećaja
        (PTSP) i ovisnosti.
      </p>

      <h3>Putovanje unutra</h3>
      <p>
        Psilocibinske gljive mogu pružiti iskustva koja idu daleko izvan svakodnevnog razumijevanja
        stvarnosti. Mnogi korisnici izvještavaju o osjećajima „otvorenosti uma“, boljoj povezanosti
        s prirodom, intenzivnijem doživljaju boja i zvukova, pa čak i osjećaju prosvjetljenja. Iako
        iskustvo može biti duboko uzbudljivo i transformativno, ono također nosi i određene rizike.
        Psilocibinske gljive mogu izazvati anksioznost, zbunjenost i nelagodu, posebno u okruženju
        koje nije sigurno ili podržavajuće.
      </p>

      <h3>Legalizacija i budućnost</h3>
      <p>
        U posljednjih nekoliko godina, psilocibinske gljive su postale predmet debate u mnogim
        zemljama. Od 2020. godine, nekoliko američkih država i kanadskih provincija počelo je
        legalizirati njihovu uporabu u medicinske svrhe, dok su u nekim državama u Europi, poput
        Nizozemske, već poznate kao "legalne" za korisnike. Mnogi vjeruju da bi psilocibin mogao
        biti ključni alat u liječenju mentalnih bolesti i otvaranju novih terapeutskih mogućnosti.
      </p>

      <p>
        Psilocibinske gljive nas podsjećaju da je ljudska spoznaja i percepcija svemira daleko šira
        nego što to svakodnevno doživljavamo. Kroz njih, putovanje nije uvijek vanjsko, već duboko
        unutarnje.
      </p>
    </section>

    <section>
      <h2>Gljive kao simbol povezanosti</h2>

      <p>
        Tajanstveni svijet gljiva nije samo fascinantna biološka stvarnost, već i metafora života
        samog. Kroz njih, učimo o povezanosti svih živih bića, o neprestanom ciklusu života i smrti,
        stvaranja i uništavanja. Gljive nas podsjećaju da u svakom kutku prirode postoji nevidljiva
        mreža života, koja povezuje sve i omogućava ravnotežu. Iako ih mnogi ignoriraju ili smatraju
        nevažnima, gljive su tu, tiho i moćno održavajući ravnotežu svijeta u kojem živimo.
      </p>

      <p>
        U ovoj priči o gljivama, otkrili smo njihov nevjerojatni utjecaj na ekosustave, ali i na nas
        same. Saznali smo kako nas gljive mogu inspirirati u znanstvenim istraživanjima, medicinskim
        otkrićima i svakodnevnom životu. I možda, baš kao i gljive koje neprestano rastu i šire
        svoje mreže, tako i mi, kao ljudi, možemo pronaći načine da povežemo, učimo i rastemo,
        prepoznajući duboku povezanost svega živog.
      </p>

      <p>
        Taj svijet pod nogama, i iznad njih, čeka na nas da ga istražimo. Bez obzira na to hoće li
        nas ta potraga odvesti do ljekovitih svojstava, kulinarskih užitaka, ili do dubljeg
        razumijevanja svijesti i prirode, jedno je sigurno: svijet gljiva nas podsjeća da je
        priroda, sa svim svojim tajnama i čudima, uvijek tu, čekajući da je otkrijemo.
      </p>

      <p>
        Ovo je samo početak. Gljive, tajne koje skrivaju, i sve ono što nam još nije poznato, uvijek
        će nas pozivati na nova otkrića. A svaka spora koja odleti u zrak donosi s njom mogućnost
        novih početaka.
      </p>

      <p>
        Na kraju našeg putovanja kroz svijet gljiva, shvaćamo da su one mnogo više od jednostavnog
        organizma. One su simbol povezanosti – između ljudi i prirode, između prošlosti i
        budućnosti, između znanosti i duhovnosti.
      </p>
    </section>
  </main>
</template>

<style scoped>
header {
  background-image: url('/images/mushroom-background.jpg');
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  background-attachment: fixed;

  height: 100lvh;
  box-shadow: var(--header-box-shadow);

  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

  font-family: var(--font-family-heading);
}

header h1 {
  font-size: 8rem;
  text-shadow:
    0px 10px 5px #111,
    -2px -2px 2px #222;
  text-transform: uppercase;
}

header span {
  font-size: 3rem;
  text-shadow:
    0px 4px 3px #111,
    -1px -1px 1px #222;
}

header h1,
header span {
  transform: translateY(-100px);
  font-weight: 900;
  user-select: none;
}

section {
  padding: 2rem 0;
  margin: 2rem 0;
  text-align: justify;
}

section:first-child {
  height: 90vh;
  position: relative;
}

section:first-child img {
  position: absolute;
  right: 0;
  bottom: 0;
}

section h1 {
  font-size: 3.5rem;
  font-family: var(--font-family-heading);
  text-align: center;
  margin-bottom: 2rem;
}

section h2 {
  font-size: 2rem;
  text-align: center;
  margin-bottom: 1.5rem;
}
section h3 {
  font-size: 1.5rem;
}
section p {
  margin-bottom: 1rem;
}
</style>
