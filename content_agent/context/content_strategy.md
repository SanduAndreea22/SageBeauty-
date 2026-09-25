# Strategie de conținut — SageBeauty

## Stare actuala (pornire de la zero pe beauty)

Contul e proaspat mutat pe nisa beauty — 855 urmaritori / 106 urmariri, dar engagement-ul e foarte
mic (maxim ~20 aprecieri pe postare, comentarii aproape inexistente). Discrepanta (multi urmaritori,
aproape zero reactii) confirma ca baza actuala de urmaritori e din perioada dinainte de pivot si nu
e interesata de beauty (vezi `audience.md` — 84.8% barbati in statisticile vechi) — plus contul e din
2019, deci o parte din urmaritorii vechi sunt probabil conturi inactive de ani buni, nu doar
nepotriviti ca nisa. E starea de
pornire, nu un semn ca ceva nu functioneaza in continut — nu se schimba tonul/strategia doar pe baza
cifrelor mici de acum. Se actualizeaza aici pe masura ce cresc cifrele reale.

**Semn bun (dar de pe Facebook, nu Instagram):** reach-ul de pe Facebook (contul e cross-postat,
vezi si "Aprecieri si reactii" defalcate Instagram/Facebook mai sus) arata demografia tinta corecta —
25-34 ani 56.8%, 18-24 ani 35.1% (impreuna ~92%). Ramane un semn incurajator ca noul continut ajunge
la varsta potrivita macar pe unul din canale.

**Pe Instagram insa, situatia reala e alta:** la o postare verificata, 100% din vizualizari au venit
de la urmaritori, 0% de la non-urmaritori (85 vizualizari, 14 spectatori, 3 interactiuni). Deci
algoritmul Instagram inca nu impinge continutul catre public nou — reach-ul e limitat strict la baza
veche de urmaritori (care, cum am stabilit mai sus, nu e interesata de beauty). De retinut: pe Instagram, Reels-urile primesc de obicei mult mai mult reach catre non-urmaritori
(prin Explore/Reels tab) decat pozele/caruselele statice, deci reels-urile rare incetinesc cresterea
fata de un mix cu mai multe reels. **Motivul real:** Andreea nu se simte inca confortabil sa apara
in reels (rusine fata de cum arata/avatarul creat pe fata ei) — nu e doar o preferinta de format, e
un lucru personal. **Nu se readuce in discutie ca tradeoff de crestere / nu se sugereaza sa faca mai
multe reels** — ramane strict optiunea ei, cand si daca vrea, fara presiune. Carusele + poze raman
formatele de baza pe termen nedeterminat.

## Ritm si mix de continut

- **Ritm:** 4-5 postari pe saptamana, 3-4 Stories pe saptamana.
- **Mix de formate:** accent pe **carusele educationale** si **poze "wow"** (impact vizual puternic) —
  acestea sunt formatele principale. **Reels-urile sunt rare** — nu presupune un reel la fiecare
  cerere de "postare completa"; cand Andreea cere pachet complet fara sa specifice reel explicit,
  prioritizeaza poza + postare/carusel, nu adauga automat un reel.
- Cand Andreea cere explicit un reel, se scrie normal, dupa `instagram_reels_prompt.md` — durata
  **15-30 secunde** (schimbat de Andreea pe 2026-09-23, inainte era 30-45s), doar avatar si voce
  generate cu ElevenLabs, fara filmare reala (vezi `brand.md`).

## Plan de continut — sursa de idei implicita

**Ideile nu se mai aleg ad-hoc la fiecare cerere individuala — vin dintr-un plan aprobat de Andreea
in avans.** Fisierul `content_agent/context/plan_continut.md` tine planul curent (status draft/aprobat
si un tabel de itemi in ordine, cu status de facut/facut).

Cand Andreea cere continut (poza/postare/carusel/reel) **fara sa dea o idee explicita**:

1. Deschide `plan_continut.md`.
2. Daca exista un plan cu status **aprobat** si cu cel putin un item **de facut** → ia **urmatorul**
   item in ordine (primul "de facut" din tabel), foloseste tipul/categoria/ideea lui exact cum sunt
   scrise acolo, genereaza continutul, apoi marcheaza-l "facut" in `plan_continut.md` (vezi "Dupa
   livrare" din promptul agentului respectiv).
3. Daca planul nu exista inca, e inca **draft** (neaprobat), sau toti itemii sunt "facuti" (planul
   s-a epuizat) → **nu alege liber pe cont propriu**. Spune-i clar Andreei situatia (nu exista plan
   activ / planul s-a epuizat) si intreab-o daca vrea sa generezi un plan nou inainte sa continui.
   Daca zice da, genereaza un draft de plan (vezi "Cum genereaza agentul un plan nou" mai jos), arata-l
   pentru aprobare si opreste-te acolo — nu genera inca postarea efectiva in acelasi raspuns.

Cand Andreea cere explicit un plan ("fa-mi un plan de postari", "plan pe luna asta") — genereaza-l
direct dupa mecanismul de mai jos, salveaza-l ca **draft** in `plan_continut.md` si arata-l pentru
aprobare. Planul devine sursa de idei abia dupa ce Andreea confirma explicit ("aprob", "merge asa",
etc.) — atunci ii schimbi statusul in **aprobat**.

**Idee data explicit de Andreea in cerere** ("vreau o postare despre X") nu atinge planul — o
folosesti direct, fara sa consumi un item din el (vezi "Cand Andreea da o tema explicita" mai jos).

## Ce a mers deja (date reale de pe TikTok, 2026-09-23)

Pe TikTok-ul Andreei, cele mai vazute doua postari sunt de makeup, cu produsele ei reale: haul
"Ia si tu 150 lei sa iti iei make up" (1.120 vizualizari) si "Dau note produselor de makeup primite
in BelleBox" (907) — peste travel/fotbal/motivatie (~200-550). Formatul **"dau note" (produs real +
nota 1-10 + parere sincera)** e candidat puternic pentru planurile viitoare (categoria *Review
sincer*, cu fapte din `knowledge/produse_incercate.md`). **Aprobat de Andreea (2026-09-23): planul
urmator include cel putin un item "dau note"** — produse si note doar din `produse_incercate.md`.

**Primul carusel pe noul stil, pe TikTok (2026-09-23, dupa cateva ore):** 174 vizualizari, 2 like,
1 salvare — **94% de la persoane care NU o urmaresc**, **91% femei**. Contrast total cu Instagram
(100% vizualizari de la urmaritori, audienta veche majoritar barbati). Concluzie: TikTok aduce exact
publicul tinta nou; caruselele pe regulile din `identitate_vizuala.md` functioneaza acolo din prima zi.

**Val 2 pe TikTok (acelasi carusel, dupa ~2 zile):** 1.366 vizualizari (de la 541), un al doilea
varf mai mare decat primul, 45% din Republica Moldova. Salvarile doar 3 → 4, retentia 2.1 / 8.
Concluzie: TikTok poate reimpinge un carusel dupa 1-2 zile — **rezultatele se judeca la ~48h, nu la
cateva ore**; distributia e buna, retentia ramane de rezolvat (vezi `outputs/rapoarte/2026-09-24.md`).

**Like-uri raportat la vizualizari (TikTok, 2026-09-25) — cea mai importanta comparatie de pana acum:**

| Postare | Format | Vizualizari | Like-uri | Rata like |
|---|---|---|---|---|
| "Dau note produselor din BelleBox" | video, produse reale + parerea ei | 931 | 87 | **9,3%** |
| "Ia si tu 150 lei sa iti iei make up" | video, produsele ei reale, umor | 1.125 | 41 | **3,6%** |
| "5 greseli care iti topesc fondul de ten" | carusel AI, sfaturi | 1.433 | 12 | 0,8% |
| Waterproof B (~2h) | carusel AI, sfaturi | 114 | 3 | 2,6% (prea devreme) |

Concluzie: caruselele-sfat AI aduc **vizualizari** (ajung la straini), dar postarile cu **produsele ei
reale + parerea/umorul ei** aduc de 4-11 ori mai multe like-uri. Planul urmator trebuie sa mute greutatea
spre formatul "dau note" / produsele ei reale / opinie personala, nu doar sfaturi generale.
Candidat pentru decizia Andreei: cross-postare sistematica a fiecarui carusel si pe TikTok.

**Acelasi carusel, a doua zi (TikTok Studio, 2026-09-24 — raport `outputs/rapoarte/2026-09-24.md`):**
303 vizualizari, 10 like, 0 comentarii, 0 distribuiri, 1 salvare, 0 urmaritori noi; 86% femei, 81%
intre 18-34 ani (public tinta confirmat). **Problema: retentia** — in medie se vad doar **2.1 din 8
slide-uri** (22m20s timp total / 303 = ~4,4 s pe vizualizare), deci rezumatul (slide 7) si intrebarea
(slide 8) aproape nu sunt vazute → 0 comentarii. Recomandare (aprobat de Andreea 2026-09-24, aplicat in `instagram_carousel_prompt.md` si `verificare.md`): slide-ul 2
trebuie sa fie util singur + sa aiba motiv de swipe, iar intrebarea apare devreme, nu doar la final.

**Acelasi carusel pe Instagram (+ republicat automat pe Facebook), 2026-09-24 — acelasi raport:**
150 vizualizari (Instagram 135, Facebook 15), 24 spectatori, 4 aprecieri (IG 2, FB 2), 0 comentarii,
0 salvari, 4 vizite in profil, 0 urmaritori noi; surse: Flux 73,8%, Povesti 18%, Profil 5,7%;
interactiuni pe slide: coperta 2, slide-urile 2-4: 0. Graficul IG se aplatizeaza dupa prima ora
(~110 → ~130 la 2h), TikTok creste liniar. Calcul: 150 / 24 = ~6,25 vizualizari per persoana —
Instagram numara probabil vizualizarile altfel (ipoteza), deci nu se compara direct cu TikTok.
Concluzie: pe Instagram postarea ramane la cercul existent; public nou vine de pe TikTok. Interactiunea
slaba (0 comentarii, 0 urmaritori noi) e pe ambele platforme → problema e a caruselului, nu a platformei;
recomandarea de mai sus ramane valabila. (% urmaritori si sex/varsta pe Instagram nu s-au vazut.)

**Caruselul fondul de ten la ~21h pe TikTok (2026-09-25):** 541 vizualizari, 3 salvari, 4 comentarii,
**2 urmaritori noi** (primii din pivot), 99% non-urmaritori, 87% femei, 88% Romania, 95% din "Pentru
tine". Varful vine in primele ~3 ore, apoi se opreste — postarile pe TikTok traiesc cateva ore, deci
ritmul constant conteaza mai mult decat o postare "perfecta". Vs Instagram la ~21h: 48 de persoane,
0 urmaritori noi. TikTok = canalul de crestere confirmat.

## Idei venite din comentarii (pentru planul urmator)

- 2026-09-24, TikTok, la caruselul cu fondul de ten (primul comentariu real): o urmaritoare cu ten
  mixt/gras intreaba ce primer sa foloseasca — fruntea si nasul lucesc dupa cateva ore, iar noul ei
  primer face fondul "sa se adune". Idee: carusel "De ce se aduna fondul de ten peste primer" (sfat
  practic). Semnal: intrebarea vine exact din publicul tinta si exact pe tema caruselului.

## Rotatie de teme (categorii de continut)

Fiecare categorie e marcata daca are nevoie de fapte concrete de la Andreea (produs/rezultat real)
sau daca poate fi generata liber, din cunostinte generale de beauty:

- **Sfat practic** *(liber)* — un tips concret, usor de aplicat, care rezolva o problema reala a audientei. Nu are nevoie de experienta personala — e cunostinta generala de beauty.
- **Mit demontat / greseala frecventa** *(liber)* — o idee gresita raspandita in beauty, corectata cu argumente. La fel, cunostinta generala, nu experienta personala.
- **Intrebare frecventa** *(liber)* — un raspuns la o intrebare tipica pe care ar putea-o primi cineva in nisa asta (nu trebuie sa fie o intrebare primita chiar de ea, doar plauzibila).
- **Look / machiaj / transformare** *(liber pentru idee, dar fara sa pretinzi ca poza exista deja)* — un concept de look; daca agentul de poza genereaza un prompt pentru el, se leaga; nu se afirma ca rezultatul e "al ei" din trecut daca nu e confirmat.
- **Review sincer de produs** *(are nevoie de fapte)* — necesita o intrare reala din `knowledge/produse_incercate.md`. Daca fisierul e gol sau nu are o intrare potrivita, **agentul sare peste aceasta categorie automat** cand alege singur — nu o foloseste ca sa nu inventeze o experienta. O foloseste doar daca Andreea cere explicit un review si ii da detaliile pe loc.
- **Rutina / culise** *(are nevoie de fapte)* — la fel, doar daca exista detalii reale (in `produse_incercate.md` sau date direct de Andreea). Altfel se sare.

## Cum genereaza agentul un plan nou

Foloseste acest mecanism doar cand generezi/reinnoiesti planul din `plan_continut.md` (nu la fiecare
cerere individuala de continut — vezi sectiunea de mai sus):

1. Verifica `content_agent/outputs/log.md` si istoricul din `plan_continut.md` — exclude categoriile/unghiurile folosite recent, ca sa nu se repete.
2. Prefera implicit categoriile marcate *(liber)* — nu au nevoie de fapte pe care Andreea nu le-a dat.
3. Pentru fiecare item, alege un unghi concret in acea categorie (nu genericul categoriei — un tips anume, un mit anume), si un tip de continut (poza/postare/carusel/reel) respectand mixul din "Ritm si mix de continut" (carusele + poze predominant, reels rar).
4. Categoriile *(au nevoie de fapte)* se folosesc doar cand exista date reale disponibile (in `produse_incercate.md`) — altfel se sar la generarea planului.
5. Un plan tipic acopera aproximativ o saptamana-doua din ritmul stabilit (4-5 postari/saptamana) — nu genera zeci de itemi deodata, ca sa ramana usor de revizuit si aprobat.

## Regula de nerepetare

Inainte sa generezi continut nou, verifica `content_agent/outputs/log.md` — nu repeta aceeasi categorie sau acelasi unghi ca in ultimele 2-3 postari/reels-uri de pe acelasi tip de continut.

## Cand Andreea da o tema explicita

Daca vine deja cu o idee clara ("vreau o postare despre X"), nu ii impui alta categorie — doar noteaza in `log.md` categoria in care se incadreaza, pentru rotatia viitoare.
