# Strategie de conținut — SageBeauty

## Ritm si mix de continut

- **Ritm:** 4-5 postari pe saptamana, 3-4 Stories pe saptamana.
- **Mix de formate:** accent pe **carusele educationale** si **poze "wow"** (impact vizual puternic) —
  acestea sunt formatele principale. **Reels-urile sunt rare** — nu presupune un reel la fiecare
  cerere de "postare completa"; cand Andreea cere pachet complet fara sa specifice reel explicit,
  prioritizeaza poza + postare/carusel, nu adauga automat un reel.
- Cand Andreea cere explicit un reel, se scrie normal, dupa `instagram_reels_prompt.md` — durata
  implicita ~30-45 secunde (nu 15-30s), avatar si voce generate cu ElevenLabs (vezi `brand.md`).

## Regula de baza: agentul alege singur, nu Andreea

**Cand Andreea nu da o idee explicita ("vreau o postare", fara alte detalii), agentul NU o intreaba
"despre ce?" — alege singur o idee, ca la etapa de Content Strategist/Idea Generator.** Andreea a
construit agentul ca sa nu mai stea ea sa gaseasca teme. Intrebarea catre ea e ultima solutie, nu
pasul 1 — vezi mai jos cand chiar e necesara.

## Rotatie de teme (categorii de continut)

Fiecare categorie e marcata daca are nevoie de fapte concrete de la Andreea (produs/rezultat real)
sau daca poate fi generata liber, din cunostinte generale de beauty:

- **Sfat practic** *(liber)* — un tips concret, usor de aplicat, care rezolva o problema reala a audientei. Nu are nevoie de experienta personala — e cunostinta generala de beauty.
- **Mit demontat / greseala frecventa** *(liber)* — o idee gresita raspandita in beauty, corectata cu argumente. La fel, cunostinta generala, nu experienta personala.
- **Intrebare frecventa** *(liber)* — un raspuns la o intrebare tipica pe care ar putea-o primi cineva in nisa asta (nu trebuie sa fie o intrebare primita chiar de ea, doar plauzibila).
- **Look / machiaj / transformare** *(liber pentru idee, dar fara sa pretinzi ca poza exista deja)* — un concept de look; daca agentul de poza genereaza un prompt pentru el, se leaga; nu se afirma ca rezultatul e "al ei" din trecut daca nu e confirmat.
- **Review sincer de produs** *(are nevoie de fapte)* — necesita o intrare reala din `knowledge/produse_incercate.md`. Daca fisierul e gol sau nu are o intrare potrivita, **agentul sare peste aceasta categorie automat** cand alege singur — nu o foloseste ca sa nu inventeze o experienta. O foloseste doar daca Andreea cere explicit un review si ii da detaliile pe loc.
- **Rutina / culise** *(are nevoie de fapte)* — la fel, doar daca exista detalii reale (in `produse_incercate.md` sau date direct de Andreea). Altfel se sare.

## Cum alege agentul o idee (cand Andreea nu da una)

1. Verifica `content_agent/outputs/log.md` — exclude categoriile/unghiurile folosite in ultimele 2-3 continuturi de acelasi tip.
2. Din categoriile ramase, prefera implicit cele marcate *(liber)* — nu au nevoie de fapte pe care Andreea nu le-a dat.
3. Alege un unghi concret in acea categorie (nu genericul categoriei — un tips anume, un mit anume) si scrie continutul direct, fara sa mai intrebe.
4. Categoriile *(au nevoie de fapte)* se folosesc doar cand exista date reale disponibile (in `produse_incercate.md`) sau cand Andreea a dat deja detaliile in cerere.

## Regula de nerepetare

Inainte sa generezi continut nou, verifica `content_agent/outputs/log.md` — nu repeta aceeasi categorie sau acelasi unghi ca in ultimele 2-3 postari/reels-uri de pe acelasi tip de continut.

## Cand Andreea da o tema explicita

Daca vine deja cu o idee clara ("vreau o postare despre X"), nu ii impui alta categorie — doar noteaza in `log.md` categoria in care se incadreaza, pentru rotatia viitoare.
