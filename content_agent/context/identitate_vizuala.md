# Identitate vizuală — SageBeauty

> Reguli vizuale pentru **tot** continutul de feed (carusele, postari cu poza) — din brief-ul de
> director de creatie dat de Andreea pe 2026-09-23. Inlocuieste stilul vechi de carusel (iconite
> line-art pe fundal plat), pe care Andreea l-a gasit "nu asa wow": curat, dar plat, nu oprea
> scroll-ul. [DE AJUSTAT de Andreea] — agentul respecta ce e scris aici.

## Regula de baza

**Fara slide-uri/poze cu doar iconite si text pe fundal simplu.** Fiecare imagine are un element
vizual real: fata, piele, produs, textura sau o mana care aplica ceva.

## Reguli vizuale (obligatorii)

1. **Aproape, nu de departe.** Pielea si produsul se vad de aproape: textura fondului de ten,
   stralucirea, porii, rezultatul pe ten. Macro si prim-planuri, nu cadre largi goale.
2. **Arati, nu doar spui.** Problema si solutia se vad in imagine — ex: fond de ten crapat/cu pete
   pe zona T vs fond care arata proaspat. Textul confirma ce se vede, nu il inlocuieste.
3. **Compozitie diferita pe fiecare slide.** Rotesti intre: prim-plan pe fata, macro pe textura,
   produs pe masa/blat (flat lay sau unghi 45°), comparatie in doua parti (split), mana in actiune
   (aplica, intinde, tapoteaza). Nu repeti acelasi aranjament de doua ori la rand in acelasi set.
4. **Textul ocupa maximum o treime din imagine si sta peste ea**, nu in locul ei — intr-o zona
   linistita a pozei (fundal, umar, blat), cu contrast suficient (umbra fina sau banda
   semitransparenta in culoarea paletei, nu casete opace mari).
5. **Lumina naturala, culori calde, aspect de viata reala — nu de reclama.** Lumina de fereastra,
   ora de aur, baie/masa de machiaj reala. Fara produse plutind in aer.
   **Exceptie — portretele "wow" cu Andreea** (look-uri, coperte, poze de sine statatoare): au voie
   la lumina difuza de studio si fundal simplu (gri perlat etc.), ca in poza "no-makeup makeup" din
   `knowledge/examples/good_posts.md` — etalonul pe care Andreea l-a placut cel mai mult. Conditia
   e aceeasi: realism total al pielii, nu aspect de reclama retusata.
6. **Realism:** piele cu textura reala (pori, mici imperfectiuni, asimetrie usoara), nu
   aspect plastic/airbrushed de AI — aceeasi regula ca in `prompts/instagram_photo_prompt.md`.
7. **Trasaturile fetei din poza de referinta nu se schimba niciodata.**

## Paletă — ce leaga postarile in feed

Paleta nu mai e "fundalul cardului" — e **tonul general al imaginilor si culoarea textului
suprapus**, pastrate la fel pe toate slide-urile ca postarea sa se recunoasca in feed:

- **Ton general al imaginii:** cald — nude, roz pudrat, piersica, lumina aurie; fundaluri reale in
  aceste nuante (prosop, blat, perete, lenjerie) acolo unde se poate
- **Text suprapus:** alb cald/crem sau maro-roscat inchis, in functie de ce contrasteaza pe zona
  respectiva a pozei
- **Accent:** terracotta cald — pentru cifre, sublinieri, eticheta "gresit"/"corect", sageti fine
- Tipografie: sans-serif curat, titlu ingrosat mare, text de explicatie mai subtire; aceeasi pe tot setul

## Poze reale vs generate AI (decizia Andreei, 2026-09-23: mix)

- **Fata, look-uri, piele pe fata** → generate AI pe baza pozei ei de referinta.
- **Produse reale ale Andreei** (din Goodiebox, BelleBox, Sephora etc., vezi
  `knowledge/produse_incercate.md`) → le fotografiaza ea. Se marcheaza in livrare cu
  `[POZA MEA: descrierea exacta a pozei de facut — cadru, unghi, lumina, ce e pe blat]`.
- Produse generice (un fond de ten oarecare, o pensula) → AI, **fara brand/eticheta lizibila**, ca
  sa nu sugereze un produs anume pe care nu l-a testat.
