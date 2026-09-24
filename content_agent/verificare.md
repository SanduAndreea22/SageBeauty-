# Verificare înainte de livrare — SageBeauty (Output Check)

> Litera **O** din ACTION framework. Fiecare agent din `prompts/` trece prin lista asta **inainte**
> sa-i arate Andreei continutul. Daca un punct pica, repari si verifici din nou — nu livrezi cu
> "mici probleme". Fiecare regula de aici vine dintr-o greseala reala prinsa de Andreea (data intre
> paranteze), ca sa n-o mai prinda ea a doua oara.

La final, in livrare, scrii lista frazelor la persoana I cu sursa fiecareia, apoi linia `Verificare: ✅ toate punctele` — sau, daca ceva nu se
poate respecta, ce anume si de ce (ex: "nu am parerea ta despre X → am lasat [PAREREA MEA]").

## 1. Adevar (pentru orice tip de continut)

- [ ] Fiecare experienta, parere, nota sau rezultat al Andreei exista in `knowledge/` (produse,
      analiza tenului, profil) sau a fost spus de ea in conversatie — **sau e marcat clar
      `[DE APROBAT]`** ca propunere de-a ta. Problema nu e sa propui, e sa propui pe ascuns. *(2026-09-22: "am exfoliat zilnic o vara intreaga" — inventat.)*
- [ ] Unde lipseste parerea ei → `[PAREREA MEA: ...]`, nu o fraza completata.
- [ ] Nicio statistica sau cifra falsa despre piele/produse; sfaturile sunt cunostinte general acceptate.
- [ ] Parerile ei sunt formulate ca ale ei ("pentru mine"), nu ca adevar universal.
- [ ] **Sursa pentru fiecare fraza la persoana I.** Listeaza in verificare fiecare fraza cu "eu /
      pentru mine / imi / am / folosesc / m-a" si sursa ei (ex: "nu m-a iritat → produse_incercate.md,
      Glow Recipe"; "am ten mixt → brand.md"). **Fraza fara sursa poate ramane, dar marcata
      `[DE APROBAT]` in lista** — Andreea decide daca o pastreaza (Andreea, 2026-09-23: "nu conteaza ca inventezi daca eu aprob"). Nu se strecoara
      niciodata nemarcata. *(Next improvement 2026-09-23: de 3 ori o afirmatie despre Andreea a fost
      inventata — exfolierea zilnica, "fara exceptii" la rutina, "cel mai mult conteaza pasul 3".)*

## 2. Text

- [ ] Primul rand / coperta e un hook de **o singura propozitie**, dintr-un tip din `tone_of_voice.md`,
      diferit de ultimele 2 din `outputs/log.md`.
- [ ] Un singur mesaj principal.
- [ ] Caption 3-5 propozitii, se termina cu o intrebare **specifica** (nu "ce parere aveti?").
- [ ] **Maximum 5 hashtag-uri** *(limita Instagram, 2026-09-23)* si **maximum 2-3 emoji**.
- [ ] Fara clisee goale ("glow up", "self-care", "in lumea de azi"), fara ton de reclama.
- [ ] Diacritice corecte in tot textul care apare pe imagini.

## 3. Carusel (in plus fata de 1-2)

- [ ] **Firul:** coperta anunta ce urmeaza si cate sunt ("5 greseli"); acelasi cuvant pe tot setul;
      rezumatul are titlu; intrebarea finala numeste exact la ce raspunzi. Test: coperta + ultimul
      slide se inteleg singure. *(2026-09-23: "Care dintre ele e a ta?" — neclar.)*
- [ ] **Retentie (2026-09-24):** slide-ul 2 da un raspuns util complet + un motiv de swipe; intrebarea
      pentru comentarii apare si pe coperta sau pe slide-ul 2. *(Raport: 2.1 / 8 slide-uri vazute pe
      TikTok, 0 comentarii.)*
- [ ] Fiecare slide are o imagine reala (fata, piele, produs, textura, mana) — niciun slide cu
      iconita pe fundal plat. *(2026-09-23: v1 "nu e asa wow".)*
- [ ] Compozitii diferite, nu acelasi tip de doua ori la rand; minimum un slide gresit vs corect.
- [ ] Obiectele-subiect au forme diferite (nu doua "picaturi"). *(2026-09-23.)*
- [ ] Fiecare prompt de imagine: "o singura imagine, nu colaj", 4:5, realism, "nu schimba
      trasaturile fetei" cand apare fata.

## 4. Poza / portret

- [ ] 4:5 pentru feed (9:16 doar la Stories/Reels). *(2026-09-22.)*
- [ ] Textura reala a pielii ceruta explicit — nu "piele impecabila". *(2026-09-22.)*
- [ ] Haina si machiajul difera de ultimele 2-3 poze din log (exceptie: produsul subiect).
      *(2026-09-22: roz + nude la fiecare poza.)*
- [ ] Machiajul porneste de la `knowledge/profil_frumusete.md`, fara eyeliner grafic.

- [ ] La produse reale: promptul interzice explicit orice alt cod/text pe ambalaj in afara celor date.
      *(2026-09-24: "120C" inventat de ChatGPT pe Rare Beauty.)*
- [ ] **Fiecare imagine e un prompt complet pentru ChatGPT** — niciun `[POZA MEA]`, nicio cerere ca
      Andreea sa fotografieze ceva. *(2026-09-24: "vreau prompturi pentru ChatGPT, nu fac eu nimic".)*

## 5. Reel / Stories

- [ ] Reel 15-30s, doar avatar, text pe ecran pe fiecare cadru, voiceover curat fara adnotari.
- [ ] Stories: 2-3 frame-uri, pornesc de la un continut existent, max 1 emoji pe frame, fundal 9:16.

## 5b. Varianta TikTok (carusel / postare)

- [ ] Exista sectiunea "Varianta TikTok": titlu = hook scurt, caption 1-2 propozitii, 3-5 hashtag-uri,
      tip de sunet (nu un titlu de melodie inventat). Imaginile sunt aceleasi.

## 5c. Varianta Threads (carusel / postare) — din 2026-09-25

- [ ] Exista "Varianta Threads": 1-2 propozitii conversationale + o intrebare directa, max 1 emoji,
      fara lista de hashtag-uri; aceleasi reguli de adevar (fraze la persoana I cu sursa).

## 6. Plan si evidenta

- [ ] Ideea vine din `context/plan_continut.md` (sau a dat-o Andreea explicit).
- [ ] Dupa livrare: salvat in `outputs/`, rand in `outputs/log.md` cu **Status: draft**, item marcat "facut" in plan.
- [ ] **Cand se schimba o regula** (in orice fisier din `context/` sau aici), treci prin aceasta lista
      toate randurile din log cu Status **draft** si repara-le — continutul nepublicat nu ramane pe
      reguli vechi. Cand Andreea spune ca a postat ceva, Status devine **publicat**.
