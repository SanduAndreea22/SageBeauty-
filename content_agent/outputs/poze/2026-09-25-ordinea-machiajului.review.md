# Review — poze/2026-09-25-ordinea-machiajului.md (runda 3)

**Verdict: RESPINS**

Verificator independent, 2026-09-25. Am verificat cu `verificare.md` (§1, §2, §4, §5b, §5c, §5d, §6), cu brief-ul `outputs/briefuri/2026-09-25-item-5.md`, cu `knowledge/produse_incercate.md`, `context/identitate_vizuala.md`, `context/tone_of_voice.md`, `prompts/instagram_photo_prompt.md` si `outputs/log.md`.

Punctele 2, 3, 4, 5, 6 si 7 din review-ul rundei 2 sunt rezolvate. Doua puncte pica.

## Puncte picate

### 1. Fapt despre produs distorsionat si marcat "fapt ok" (verificare §1: "Fapte despre produse ... nu se inventeaza deloc"; brief: nota "citata exact")
- Citat din sectiunea optionala: „La pasul 5 am o poveste: Brow Powder Duo nu mi-a plăcut deloc la început, acum e 100/10.”
- Sursa, `produse_incercate.md`: "Initial nu mi-a placut deloc **culoarea**. Dupa prima aplicare insa... m-am indragostit de ea."
- Formularea propusa scoate "culoarea". Asa, neplacerea se muta de la culoare la tot produsul. In plus, "acum" sugereaza o evolutie in timp care nu e in sursa: ea s-a indragostit dupa prima aplicare.
- In tabelul de verificare, randul are statusul "fapt ok; formularea [DE APROBAT]", iar in livrare scrie "**nu e propunere inventata**". Faptul nu e ok, e modificat. Daca Andreea aproba formularea pe baza acestei etichete, faptul distorsionat ajunge in continut.
- Remediu: fie citatul exact ("initial nu mi-a placut deloc culoarea"), fie propunerea se scoate.

### 2. Sapte produse neconfirmate apar in imagine fara sa fi fost intrebata Andreea (verificare §4, 2026-09-25: "Produsele din imagini sunt produsele reale ale Andreei (din `produse_incercate.md`, cu poza de referinta) ... lipseste unul → intrebi"; `produse_incercate.md`: "Neconfirmate inca: pudra de fixare, ruj, luciu ... se intreaba inainte de a le pune in imagine"; contur/blush/iluminator: "produsele exacte nu sunt numite")
- Citat din prompt: "Folosește exact cele 12 produse din pozele de referință atașate". Citat din nota: "3 concealerul tau · 6 pudra ta de fixare · 7 conturul tau · 8 blush-ul tau · 9 iluminatorul tau · 11 rujul tau · 12 luciul tau".
- Asta inseamna 7 din 12 produse care nu exista in `produse_incercate.md`. Regula din knowledge cere ca intrebarea sa se puna **inainte** de a le pune in imagine. Livrarea da insa promptul gata de generat, cu o conditie pasiva ("Daca ... nu ai o poza ..., spune-mi"). Si "Pasul urmator" e generarea, nu intrebarea.
- Brief-ul directorului ("in imagine apar din pozele ei de referinta") contrazice regula scrisa de Andreea in `knowledge/` si in `verificare.md`. Un brief nu poate anula o regula a Andreei. Conflictul il rezolva orchestratorul, cu o intrebare directa catre Andreea: "Ai poze cu concealerul, pudra de fixare, conturul, blush-ul, iluminatorul, rujul si luciul pe care le folosesti zilnic? Cum se numesc?" Raspunsul se trece in `produse_incercate.md`. Pana atunci, pasul urmator e intrebarea, nu generarea.

## Observatii minore (nu blocheaza)
- Cercurile crem cu cifre stau pe un blat crem, deci contrastul e slab. Cifrele terracotta se citesc, dar cercurile se pierd. De luat in calcul un contur fin terracotta.
- Sunetul TikTok, "în trend pe beauty", e vag, dar nu e un titlu de melodie inventat, deci trece de §5b.

## Ce trece
- **Hook:** de tip curiozitate, o propozitie, livrat de imagine (cifra 6 marcata). Difera de ultimele doua hook-uri din log (mit contrazis, adresare directa). Nu contine "pe dos", "gresit", "secret", "am aflat" sau "mi-am dat seama".
- **Mesaj si fapte:** un singur mesaj. Ordinea respecta brief-ul (6 = pudra de fixare). Sprancenele gel → pudra nu sunt comentate. Faptul general despre pudre e formulat fara cifre.
- **Descriere IG:** 3 propozitii plus legenda ceruta de brief, 1 emoji, 3 hashtag-uri. Intrebarea, care se raspunde dintr-un cuvant, e permisa de brief.
- **Imagine (§4):** format 4:5, 4K, ultrarealist, "o singura imagine, nu colaj", grila 4 x 3, fara obiecte in plus. Interdictia explicita de coduri si texte pe ambalaje e prezenta. Textul ocupa maximum 1/3 din imagine si nu acopera produsele. Diacriticele sunt corecte. Promptul e complet pentru ChatGPT. Nu apare fata, deci trasaturile, haina si machiajul nu se aplica.
- **TikTok (§5b):** titlu = hook, caption de 2 propozitii, 4 hashtag-uri, tip de sunet.
- **Threads (§5c):** 2 propozitii si o intrebare directa, 1 emoji, fara hashtag-uri.
- **Restul:** amintirea §5d e prezenta. Log-ul are randul actualizat, cu Status draft. Exista un singur pas urmator.

## Fraze la persoana I (si afirmatii despre Andreea)

| Fraza | Unde | Sursa | Status |
|---|---|---|---|
| "rutina mea de zi cu zi, de la 1 la 12" | imagine | `produse_incercate.md`, rutina de machiaj + hook-ul "un singur pas mutat" pe acelasi ecran (conditia din brief) | ok |
| "E rutina mea de zi cu zi, cu o singură mutare" | IG | ca mai sus + brief | ok |
| "Ordinea machiajului meu de zi cu zi are 12 pași, iar singura mutare e pudra de fixare" | TikTok | ca mai sus + brief | ok |
| "Rutina mea de machiaj de zi cu zi are 12 pași și un singur pas mutat" | Threads | ca mai sus + brief | ok |
| "concealerul tau / pudra ta de fixare / conturul tau / blush-ul tau / iluminatorul tau / rujul tau / luciul tau" | nota catre Andreea + imagine | lipsa in `produse_incercate.md` (neconfirmate / nenumite) | [DE APROBAT] — trebuie confirmate inainte de generare (punctul 2) |
| „De acum pun pudra de fixare înainte de blush.” | doar propunere optionala | lipsa in `knowledge/` | [DE APROBAT] (marcata corect) |
| „La pasul 5 am o poveste: Brow Powder Duo nu mi-a plăcut deloc la început, acum e 100/10.” | doar propunere optionala | `produse_incercate.md` spune "nu mi-a placut deloc **culoarea**" | [DE APROBAT] + fapt distorsionat (punctul 1) |
