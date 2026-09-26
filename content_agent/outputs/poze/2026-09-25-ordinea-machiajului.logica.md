# Corector de logica — Pudra de fixare, doar in doua locuri (item #5, runda 5)

> Verificat: `outputs/poze/2026-09-25-ordinea-machiajului.md` (textul de pe imagine, descrierea IG,
> TikTok, Threads, share in Story). Citit ca un strain care da scroll, in ordinea: imagine → IG →
> TikTok → Threads → Story. Context: `content_agent/CLAUDE.md`, `knowledge/produse_incercate.md`
> ("Rutina de machiaj de zi cu zi"), brief `outputs/briefuri/2026-09-25-item-5.md`.
> Nu am rescris continutul; reformularile de mai jos sunt propuneri pentru orchestrator.

## Verdict: **NECLAR**

Mesajul e unul singur si nu are contradictii (ordinea e prezentata ca a ei, nicio corectura, niciun
"de-asta"/"deci" fara baza). Problema e ca **pe TikTok (platforma prioritara) nu se intelege ce sunt
cei 12 pasi**, iar pe imagine legatura "cifra 9 = pudra de fixare" nu e spusa, ci trebuie ghicita.

## Probleme

### 1. TikTok — cei 12 pasi nu sunt numiti nicaieri (important)
- **Unde:** varianta TikTok (titlu + caption) + imaginea.
- **Text:** "Ordinea machiajului meu de zi cu zi are 12 pași, iar pudra de fixare vine la pasul 9…"
- **De ce e neclar:** pe imagine sunt doar cifre, fara numele pasilor (asa cere brief-ul), iar legenda
  cifra → produs exista doar in descrierea IG. Pe TikTok, unde vine publicul nou, cineva vede 12
  ambalaje numerotate si citeste "ordinea machiajului meu are 12 pași", dar nu afla care e ordinea —
  exact lucrul pe care il promite subrandul de pe imagine ("de la 1 la 12"). Pentru 7 produse fara nume
  pe ambalaj recunoscut, ordinea ramane de ghicit.
- **Propunere:** adauga in caption-ul TikTok, dupa intrebare sau inainte de hashtag-uri, aceeasi legenda
  scurta ca la IG (fapte deja in `produse_incercate.md`, nimic nou), de ex.:
  "1 primer · 2 fond de ten · 3 concealer · 4 gel de sprâncene · 5 pudră de sprâncene · 6 contur ·
  7 blush · 8 iluminator · 9 pudră de fixare · 10 creion de buze · 11 ruj · 12 luciu".
  (Daca asta depaseste regula de 2 propozitii din §5b, decide verificatorul/orchestratorul; alternativ,
  legenda poate merge ca prim comentariu fixat.)

### 2. Imagine — "cifra 9" evidentiata, dar nicaieri nu scrie ca 9 e pudra de fixare (mediu)
- **Unde:** textul de pe imagine.
- **Text:** "Pudra de fixare o pun doar în două locuri: pe frunte și jos pe obraz." / "rutina mea de zi
  cu zi, de la 1 la 12"
- **De ce e neclar:** in 2-3 secunde, strainul vede un hook despre pudra de fixare si un cerc plin cu 9,
  dar nimic nu leaga cele doua. Daca nu recunoaste ambalajul, nu stie ce produs e "pudra de fixare" din
  cele 12, deci evidentierea nu isi face treaba fara caption.
- **Propunere (subrandul, fara semnul "="):** "rutina mea de zi cu zi, de la 1 la 12 · pudra de fixare
  e nr. 9". Ramane un singur subrand scurt, cum cere brief-ul.

### 3. IG — "după … și nu o pun peste ele" se poate citi ca o contradictie (minor)
- **Unde:** descrierea IG, propozitia 2.
- **Text:** "E pasul 9 din rutina mea de zi cu zi, după contur, blush și iluminator, și nu o pun peste ele."
- **De ce:** "după" sugereaza la prima citire "deasupra lor"; abia a doua parte clarifica. Lipseste
  ideea ca merge pe alte zone. Pronumele "ele" e clar (contur, blush, iluminator).
- **Propunere:** "E pasul 9 din rutina mea de zi cu zi: vine după contur, blush și iluminator, dar pe
  alte zone, nu peste ele." (Acelasi fapt din `produse_incercate.md`.) Aceeasi nuanta, optional, in
  caption-ul TikTok: "…doar pe frunte și jos pe obraz, nu peste contur, blush și iluminator" e deja ok.

### 4. Story — intrebarea nu are variantele de raspuns (minor)
- **Unde:** share in Story.
- **Text:** „Pasul 9 e pudra de fixare. Tu unde o pui?”
- **De ce:** pe IG/TikTok/Threads intrebarea are cele doua variante ("toată fața / zone"); in Story e
  deschisa, deci se raspunde mai greu si nu se leaga de hook-ul "doar în două locuri".
- **Propunere:** „Pasul 9 e pudra de fixare. Tu o pui pe toată fața sau doar pe zone?”

### Observatie fara reformulare
- In legenda IG, "MUP" si "2 NBW" sunt prescurtari pe care un strain nu le intelege. Numele complet al
  brandului nu apare in `knowledge/produse_incercate.md`, deci nu propun o extindere (ar fi inventata);
  daca Andreea confirma numele complet, se poate scrie o data intreg.

## Ce e in regula
- Hook = o propozitie, se intelege din prima; "doua locuri" e urmat imediat de cele doua locuri.
- Intrebarea (IG, TikTok, Threads) se raspunde dintr-un cuvant si se leaga direct de mesaj.
- Nicio contradictie intre imagine, IG, TikTok, Threads (pas 9 din 12, frunte + jos pe obraz peste tot).
- Nicio legatura cauza-efect nemarcata; motivul (sebum) ramane doar in propunerea [DE APROBAT].
- Romana naturala, cu diacritice, ton de prietena.
