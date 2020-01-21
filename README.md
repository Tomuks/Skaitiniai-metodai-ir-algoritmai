# Skaitiniai-metodai-ir-algoritmai
skaitiniai metodai ir algoritmai


SMA.02 – TIESISNĖS LYGČIŲ SISTEMOS. GAUSO ALGORITMAS.
Paaiškinti Gauso algoritmą tiesinių lygčių sistemai spręsti, atkreipiant dėmesį į :
Elementarieji pertvarkymai:
sistemos lygčių sukeitimas vietomis
sistemos lygties padauginimas iš nelygaus nuliui skaičiaus
vienos sistemos lygties pridėjimas prie kurios nors kitos sistemos lygties.
Atliekant pertvarkymus tikslas yra gauti trikampę matricą, jei gauname tada žinome kad bus tik vienas sprendinys. Gavus trapecinę matrica – begalo daug sprendinių.

Paaiškinkite, kokia yra grafinė interpretacija atvejų, kai dviejų tiesinių lygčių sistema: a) turi vienintelį sprendinį, - funkcijos susikerta vienoje vietoje b) neturi sprendinių – funkcijos nesusikerta, c) turi be galo daug sprendinių - funkcijos, d) silpnai apibrėžta- tenkina kitos sprendinių poros, kurios yra gan toli nuo tikrojo sprendinio.
Kokie yra Gauso algoritmo vykdymo etapai? TIESIOGINIS ŽINGSNIS – „sutvarkyti matricą“ iki trikampės matricos; ATVIRKŠTINIS ŽINGSNIS – nuosekliai, pradedant n-tąja lygtimi, apskaičiuojami nežinomieji xn, xn-1, ..., x1. 
Kas yra išplėstoji lygčių sistemos matrica? Lygčių atsakymas ??
Kas yra vedantysis elementas? VEDANTYSIS ELEMENTAS – kuris turi savo stulpelyje absoliutinį didžiausią koeficientą;
Ką daryti, jeigu vedantysis elementas lygus nuliui? Ką pagal šią reikšmę galima pasakyti apie lygčių sistemos sprendinį? SINGULIARI MATRICA – kai vedantysis elementas yra 0 (determinantas yra 0). Tai reiškia arba kad sprendinių nėra, arba yra sprendinių be galo daug. Paprasčiausias variantas – sustabdyti programą ir išvesti klaidos pranešimą. Tačiau tiesioginį Gauso algoritmo etapą galime vykdyti toliau (nes k-tojo stulpelio apatiniai elementai jau yra nuliniai). Nekeisdami k stulpelio, pereiname prie k+1 stulpelio ir parenkame vedantį elementą (k+1, k+1) pozicijoje. Taip pat prieš pradėdami Gauso algoritmo atvirkštinį etapą turime patikrinti, ar koeficientas ann yra lygus nuliui (jei lygus, tai lygčių sistema turi be galo daug sprendinių arba yra nesuderinta).
Kaip vykdyti tiesioginį Gauso algoritmo žingsnį, kai nepavyksta parinkti nelygaus nuliui vedančiojo elemento? Vykdoma toliau.
Kaip vykdomas atvirkštinis Gauso algoritmo žingsnis, kai sutinkamas lygus nuliui įstrižainės elementas? Tas sprendinys yra nulis
Kaip, vykdant atvirkštinį Gauso algoritmo žingsnį, atpažinti atvejus "be galo daug sprendinių" ir "sprendinių nėra"? kai “be galo daug sprendinių” - Paimamas bet koks skaičiu arba tiesiog p raidė. “sprendinių nėra” – stabdomas algoritmas.
Kaip skaičiuojama atveju "be galo daug sprendinių" ?
Kaip patikrinti lygčių sistemos sprendinio tikslumą? Suskaičiuojamos x reikšmės su gauso metodu, x matricą dauginame iš koeficientų matrices ir atimam lygčių atsakymus.po to dauginta iš e^-0.005.
Kas yra sprendinio Euklido norma? Visų sprendinių kvadratų sumos šaknis.
Kiek apytiksliai aritmetinių operacijų reikia atlikti, taikant Gauso algoritmą? N pakelta kūbu, padalinta iš 3. ( n nežinomųjų skaičius)
Kas yra retoji matrica, kokius žinote jų saugojimo būdus? RETOJI MATRICA -  matrica kurios daug koeficientų yra nulinių.SAUGOJIMO BŪDAI –  bendrasis pavidalas – nenulinių reikšmių ir jų indeksų saugojimas.






Kiek apytiksliai aritmetinių operacijų reikia atlikti, taikant Gauso algoritmą trijų įstrižainių matricai? 8 kart n (n – nežinomųjų skaičius)
Kaip Gauso algoritmas taikomas lygčių sistemos su daugeliu dešiniosios pusės vektorių sprendimui?
Apibūdinkite Gauso-Žordano algoritmą. Vykdomi irgi pertvarkymai, tik tvarkoma iki kad liktų tik įstrižainėje vienetai.
Kaip Gauso algoritmas gali būti pritaikytas atvirkštinei matricai ir matricos determinantui apskaičiuoti?

SMA.03 – TIESISNĖS LYGČIŲ SISTEMOS. ATSPINDŽIO IR SKAIDOS ALGORITMAI.



Kas yra atspindžio matrica? Tai vektoriaus atspindys plokštumos atžvilgiu. Atspindžio (arba QR) algoritmo idėja: kaip ir Gauso metode, pirmiausia lygčių sistema perskaičiuojama į trikampį pavidalą, o po to, taikant Gauso metodo atvirkštinį etapą, apskaičiuojami xn, xn-1, ..., x1. Pagrindinis QR metodo skirtumas nuo Gauso metodo yra tas, kad perskaičiuojant sistemą į trikampį pavidalą vietoje elementarių pertvarkių yra naudojamos atspindžio matricos.

Kaip rasti atspindinčios plokštumos normalės vektorių, kai žinomas vektorius ir jo atspindys? 

Kokią sąlygą turi tenkinti  vektorius, kad jį būtų galima laikyti atspindžio vektoriumi duotajam vektoriui?

Ką reiškia matricos ortogonalumas? Įrodykite, kad atspindžio matrica visuomet ortogonalioji.
SIMETRIŠKA MATRICA – matrica, sutampanti su savo pačios transponuota matrica.
Įrodymas:

ORTOGONALIOJI MATRICA – kai transponuota matrica yra lygi jos inversijai. QT=Q-1
Įrodymas:

Paaiškinkite, kodėl išplėstąją lygčių sistemos koeficientų matricą padauginus iš atspindžio matricos kairėje pusėje, jos sprendinys nepasikeičia.nes po kiekvieno atspindžio, stulpelių normos nepakinta.
Paaiškinkite, kaip sprendžiama lygčių sistema, taikant atspindžio metodą.
Kiekvienas stulpelis laikomas vektoriumi, kuriam gali būti pritaikytas ATSPINDŽIO PAKEITIMAS. Taikant formulę A'=QA=Qa1:n,1,a1:n,2,a1:n,n=[Qa1:n,1,Qa1:n,2Qa1:n,n], vienas ir tas pats atspindžio pakeitimas pritaikomas kiekvienam stulpeliui. Matrica [A‘] gaunama, tiesiškai kombinuojant matricos [A] eilutes (t.y. sprendžiamos sistemos lygtys). Tai reiškia, kad matricomis [A‘] ir [A] aprašomų lygčių sistemų sprendiniai yra tokie patys.

Ar galima taikyti atspindžio algoritmą, kai lygčių sistemos koeficientų matrica yra singuliari? Taip, tiesiog praleidžiamas tas stulpelis
Kodėl taikant atspindžio algoritmą, pertvarkytos koeficientų matricos stulpelių normos nepakinta?
Kas yra QR skaida?
Atspindžio algoritmas išsklaido lygčių sistemos matricą į ortogonalųjį ir trikampį daugiklius. QR skaida = ortogonalioji matrica * trikampė matrica; [A] = [Q][R];

Ką galima pasakyti apie QR skaidos daugiklio Q ortogonalumą ir simetriškumą?

Kaip QR skaida pritaikoma lygčių sistemai spręsti? Kuo toks būdas geresnis už tiesiogiai pritaikytą atspindžio metodą?

Privalumai: kartą apskaičiavę skaidos daugiklius, juos galime naudoti pakartotinai, esant vis kitokiam laisvųjų narių vektoriui. Trikampėje matricoje stulpelių normos lieka tokios pačios, kaip ir išeities matricoje. Trūkumai: daugikliai užima daugiau atminties, nei pradinė matrica.
Kas yra LU skaida ir kaip ji pritaikoma lygčių sistemai spręsti? Kokią sąlygą turi tenkinti koeficientų matrica, kad jai būtų galima pritaikyti LU skaidą?

Panaudojama:
Tiesinių lygčių sistemų sprendimui; Matricos invertavimui; Matricos determinanto skaičiavimui;
Paaiškinkite, kaip gaunami LU skaidos daugikliai L ir U. Kodėl, vykdant skaidą, reikia papildomai sugeneruoti perstatymų matricą P? 

Kas yra Choleckio skaida, kuo ji skiriasi nuo LU skaidos? Kokią sąlygą turi tenkinti koeficientų matrica, kad jai būtų galima pritaikyti Choleckio skaidą?
Kai lygčių sistemos matrica A yra simentrinė ir teigiamai apibrėžta, taikomas kitas, dvigubai spartesnis, skaidos metodas, vadinamas CHOLECKIO METODU. Simetrinė matrica kai, determinantas didesnis už nulį.

Kokie LU skaidos privalumai ir trūkumai, lyginant su QR skaida:
Privalumas – daugikliai L ir U užima pradinės matricos A vietą, o QR skaidoje – užima daugiau atminties nei pradinė matrica; Trūkumas – taikoma tik kvadratinei matricai (QR galima taikyti m x n matricai);

SMA_04. Tiesinių lygčių sistemos. Iteraciniai algoritmai, tikslumas;
Koks yra esminis tiesioginių ir iteracinių tiesinėms algebrinių lygčių sistemoms taikomų metodų skirtumas? Tiesioginiai – sprendinys gaunamas algebriškai pertvarkant lygčių sistemą. Iteracinis – koeficientų matrica išlieka nepakitusi. Sprendinį apskaičiuojame nuosekliaisiais priartėjimais.
Kaip reikia pertvarkyti lygčių sistemos koeficientų matricą, prieš pradedant taikyti paprastųjų iteracijų algoritmą? Jei įstrižainėje yra 0 reikšmė, reikia sukeisti vietomis lygtis arba kintamuosisu, metodas greičiau konverguoja, kai įstrižainėje yra absoliutiniu dydžiu didesni koeficientai.

Kokį vaidmenį atlieka koeficientai "alpha" paprastųjų iteracijų algoritme? Ką jie įtakoja? Laisvai pasirenkamas skaičius, nuo kurio galėtų priklausyti konvergavimo greitis.

Kas yra sprendimo proceso konvergavimas arba divergavimas? Kokia jų sąsaja su koeficientų "alpha" reikšmėmis?
Pagal kokias sąlygas stabdomas sprendimo paprastųjų iteracijų metodu procesas?

Paaiškinkite, kuo Gauso-Zeidelio algoritmas skiriasi nuo paprastųjų iteracijų algoritmo.





SMA_09. Skaitinis integralų apskaičiavimas. Niutono ir Koteso formulės;
Apibūdinkite apibrėžtinio integralo (AI) skaitinio apskaičiavimo bendrąją formulę.
Duotos funkcijos f(x) apibrėžtinis integralas interval [a,b] – tai suminė reikšmė su ženklu imamo ploto, kurį apriboja funkcijos kreivė, Ox ašis ir vertikalios atkartos, išvestos taškuose x=a ir x=b nuo Ox ašies iki funkcijos kreivės. Apibrėžiant matematiškai, funkcijos f(x) apibrėžtinis integralas intervale [a,b] yra „apatinės“ ir „viršutinės“ integralinių sumų riba:

Apibrėžtinis integralas skaitiškai apskaičiuojamas, pakeičiant jį baigtinio funkcijos reikšmių skaičiaus su svoriniais koeficientų suma:

Paaiškinkite, kaip taikomas Hemingo metodas AI apskaičiavimui. Kaip gaunama lygčių sistemos koeficientų matrica ir dešniųjų pusių vektorius? Kokie dydžiai gaunami, išsprendus šią lygčių sistemą?




Kaip parenkami interpoliavimo mazgai, taikant  Niutono ir Koteso formules? Koks ryšys tarp Lagranžo interpoliavimo funkcijų ir AI skaitinio apskaičiavimo koeficientų?

Skaitinio integravimo formulės koeficientai gali būti apskaičiuoti, taikant simbilinio integravimo veiksmus: 

Didinant interpoliavimo mazgų skaičių, gaunami aukštos eilės Lagrandžo daugianariai. Jie labia banduoti, todėl didinant taškų skaičių integravimo tikslumas nedidėja.
Paaiškinkite AI apskaičiavimą pagal Niutono ir Koteso formules, taikant integravimo intervalo skaidymą dalimis.
Patogu skaidyti interval [a,b] dalimis ir taikyti interpoliavimą daugianariu kiekvienoje dalyje, esant nedideliam mazgų skaičiui.


Kas yra  AI skaitinio apskaičiavimo formulės eilė? Kaip ji nustatoma? Kokios tikslumo eilės yra trapecijų ir Simpsono formulės.
TIKSLUMO EILĖ -  formulės, kuri tiksliai apskaičiuoja k laipsnio integral, tikslumo eilė yra k; formulės sudarytos taip, kad n taškų panaudojanti formulės tikslumo eilė yra bent jau n-1 .



Paaiškinkite Ričardsono ekstrapoliacijos formulę. Kam ji taikoma, nuo ko priklauso jos koeficientai?


Skirta rezultatų tikslumo eilės padidinimui.
Paaiškinkite Rombergo metodą. Kuo jis paremtas ir kam taikomas?


SMA_10. Skaitinis integralų apskaičiavimas. Gauso formulės. Skaitinis išvestinių apskaičiavimas
Koks svarbiausias skirtumas tarp Gauso ir Niutono-Koteso formulių šeimų, skirtų apibrėžtinio integralo (AI) apskaičiavimui? Niurono-Koteso fromulės išvedamos, kai tolygiai interval išdėstytų interpoliavimo mazgų padėtys iš anksto žinomos; interpoliavimo mazgus būtų galima parinkt ir kituose interval taškuose, siekinat, kad formulės tikslumo eilė būtų kuo aukštesnė.
 Naudodamiesi literatūra, paaiškinkite Gauso formulių išvedimą Hemingo būdu.







Kaip reikia naudotis lentele pateiktais Gauso-Ležandro formulių koeficientais AI apskaičiavimui?

Kam naudojamos Gauso-Ermito bei Gauso-Legero formulės? Gauso ir Ležandro formulės dažniausiai vartojamos, kai reikia integral apskaičiuoti vieną formule visame interval ( t.y. neskaidant intervalo); sudėtingos funkcijos integral galima būtų apskaičiuoti, skaidant ją intervalais ir kiekviename jų taikyti Gauso ir Ležandro formules. Gauso-Ermito ir Gauso Legero – netiesioginiam integralui apskaičiuot.

Kaip dvilypis integralas (DI) apskaičiuojamas stačiakampėje srityje, taikant Gauso-Ležandro metodą? Kaip gaunami integravimo taškai ir atitinkami svoriniai daugikliai? Duotos funkcijos f(x,y) dvilypis integralas argumentų srityje S – tai suminė reikšmė su ženklu imamo tūrio, kurį apriboja funkcijos paviršius.

Kas yra baricentrinės koordinatės ir kaip jos taikomos DI integralui trikampėje srityje apskaičiuoti (paaiškinkite naudodamiesi literatūra)? Kai sritis ne stačiakampė, Gauso-Ležandro integravimo taškai išreiškiami per baricentrines coordinates. Taikant baricentrines coordinates, bet kurio trikampiui priklausančio taško koordinatės išreiškiamos viršūnių koordinačių svertinės sumos pavidale. Taško baricentrinės koordinatės yra viršūnių koordinačių daugikliai taško koordinačių išraiškoje; baricentrinių koordinačių suma visuomet = 1;

Koks bendrasis principas naudojamas skaitiškai apskaičiuojant funkcijos išvestinę? Funkcijos f(x) i6vestin4 yra funkcija, kurios reikšmė kiekviename taške x yra kampo, kurį taške x sudaro funkcija f(x) su Ox ašimi, tangentas. 

Kas yra pirmyneigė, centrinė ir atgalinė skaitinio diferencijavimo formulės, kam jos naudojamos?




1) Kas yra interpoliavimui taikomos bazinės funkcijos: 

Jomis gali būti bet kokios tiesiškai nepriklausomos funkcijos, kurių skaičius lygus interpoliavimo mazgų skaičiui.

2) Kokiu koeficientu skiriasi mastelio funkcijų koeficientai dviejuose gretimose detalizavimo lygiuose

sqrt(2)

3) Kokios eilės daugianariai naudojami, interpoliuojant Ermito splainais

3-ios

4) Apskaičiuojant aproksimuojančią kreivę, kurios bazinių funkcijų skaičius yra m, kai duotų

 taškų  skaičius n, reikia išspręsti lygčių sistemą pavidalo 
GTGc=GTy     ,
Kokie yra matricų (vektorių) išmatavimai:

G(nxm), c(mx1),y(nx1).

5) 101 taškų seka duotą signalą aproksimuojame Furje būdu. Harmonikų skaičius parinktas taip, kad 
aproksimavimas sutaptų su interpoliavimu. Kiek yra aproksimavimo koeficientų prie cos funkcijų?

51

6) Paveiksle pavaizduotas interpoliavimo bazinės funkcijos. Kuris apibūdinimas teisingas? https://imgur.com/4VdCR4U

Ermito funkcijos U, kiekvieno daugianario eilė 9.

7) Gauso_Ležandro metodu apskaičiuokite dvilypio integralo reikšmę, 
naudodami vieno taško integravimo formulę pagal kiekvieną kintamąjį   https://imgur.com/wrRzXmL

8) Eulerio metodu sprendžiame paprastosios diferencialinės lygties pradinių reikšmių uždavinį 
Integravimo žingsnis 0.1

Raskite sprendinio reikšmę kai x = 0.3      https://imgur.com/Hp3Bye6

0.5338

9) Tarkime, skaitinio integravimo formulės eilė yra n. Kuris teiginys teisingas:

Tokia formulė tiksliai apskaičiuoja funkcijų 1,x,x^2..,x^n integralus

10) Kas yra "amplitudės slenkstis", atliekant diskrečiąją Furje aproksimaciją?

Tai reikšmė, kurios nesiekiančios aproksimuojančių harmonikų amplitudės yra atmetamos,
atkuriant signalą

11) Kas yra interpoliavimas splainais

Kai kiekviename interpoliavimo taške susijungia du skirtingi daugianariai, nustatyti gretimose intervaluose

12) Paveiksle pavaizduotos interpoliavimo bazinės funkcijos. Kuris apibūdinimas teisingas https://imgur.com/MezdFeM

Lagranžo funkcijos, kiekvieno daugianario eilė 3

13) Kiek kartų vieno integravimo žingsinio metu reikia apskaičuoti PDL funkcijos reikšmę, taikant 
Eulerio metodą?

1

14) Gauso_Ležandro metodu apskaičiuokite dvilypio integralo reikšmę, naudodami vieno taško
integravimo formulę pagal kiekvieną kintamąjį https://imgur.com/Vp5aswv

8

15) Skaitiniam išvestinės apskaičiavimui taikome 3 taškų formules.
Diferencijavimo intervale turime 100 taškų
Pagal kurią formulę skaičiuojame išvestinės reikšmę pirmame intervalo taške

[-3, 4, -1]/(2*dx)

16) IV eilės Rungės-Kutosmetodu sprendžiame paprastosios diferencialinės lygties pradinių reikšmių uždavinį

https://imgur.com/j30WZ6n

0.4985

17) Kaip sprendžiant Lagranžo integravimo uždavinį, apskaičiuojami koeficientai prie bazinių funkcijų

Jie yra lygūs interpoliavimo mazgų ordinatėms

18) Kuri iš šių formulių apibrėžia Furje aproksimavimo bazines funkcijas: https://imgur.com/WkEREA6

formulė (a)

19) Gauso_Ležandro metodu apskaičiuokite dvilypio integralo reikšmę, naudodami vieno taško
integravimo formulę pagal kiekvieną kintamąjį  https://imgur.com/JF3QdJQ

9.3333

20) Kas yra piramidinis algoritmas: 

Tai greitas algoritmas bangelių aproksimacijos koeficientams apskaičiuoti

21) Kokia yra antrojo iš kairės Čiobyševo interpoliavimo taško abscisė intervale [-2;3], kai interpoliuojama per 4 taškus

-0.46

22) Paveiksle pavaizduotos interpoliavimo bazinės funkcijos. Kuris apibūdinimas teisingas

https://imgur.com/0ZP7K75

Ermito funkcijos V, kiekvieno daugianario eilė 5

-----------------------------------------------------

Kaip skaičiuoti?

https://imgur.com/9IzLMX3

https://imgur.com/F1ynvAF

https://imgur.com/Uk2cSJq

https://imgur.com/3kwv5y7
