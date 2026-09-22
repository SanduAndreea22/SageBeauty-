# Cum se folosește content_agent — SageBeauty

Direct în Claude Code, pe acest repo. Nu trebuie configurat nimic. Într-o conversație pe
`SageBeauty`, ceri direct, de exemplu:

```
Da-mi un prompt de poza pentru un review de ser cu vitamina C.
```

sau

```
Scrie-mi o postare despre [idee].
```

sau

```
Fa-mi un reel despre [idee].
```

sau

```
Fa-mi stories pentru caruselul cu [idee].
```

(Stories se fac mereu dintr-un continut deja generat — daca nu spui pentru care, se ia cel mai
recent din `outputs/log.md`.)

Claude citește fișierele din `context/`, `knowledge/` și `prompts/` direct din repo și rulează
agentul potrivit pe loc. Nu trebuie să numești fișierul explicit — Claude rutează automat pe baza
cererii (poza / postare / reel / carusel / stories), conform regulii din `/CLAUDE.md` (rădăcina repo-ului). Poți cere
și mai multe deodată ("vreau tot pachetul pentru ideea X") — atunci rulează agenții ceruți, în
ordine: poză → postare → reel/carusel → stories.

## Folosire zilnică

```
[Poza / Postare / Reel / Carusel / Stories] despre [idee]. [orice detalii despre produs/experienta, daca e cazul]
```

Daca nu dai destule detalii pentru un continut credibil (mai ales pentru postare/reel, unde nu se
inventeaza experiente), Claude te intreaba inainte sa scrie.

## Cand actualizezi contextul

Daca schimbi produse incercate sau reguli de ton, editezi fisierul din `content_agent/context/` sau
`content_agent/knowledge/` aici, in repo — repo-ul ramane sursa de adevar.

## Ce e automatizat prin Chrome

- **Generare efectiva in ElevenLabs** — dupa ce Agentul 3 livreaza scriptul de voiceover si il
  confirmi, Claude poate deschide ElevenLabs in Chrome-ul tau real (esti deja logata acolo) si
  genera efectiv audio/video — vezi sectiunea dedicata din `instagram_reels_prompt.md`. Te intreaba
  intotdeauna inainte sa apese butonul final de generare (consuma credite) si inainte sa descarce
  fisierul.

## Ce nu e construit inca

- **Postare directa pe Instagram** — agentii genereaza doar continutul, nu publica nimic automat.
  Publicarea ramane manuala (copy-paste) sau printr-un instrument separat (Buffer/Meta API), daca
  se decide ulterior.
- **Generare efectiva de imagine** — Agentul 1 produce doar promptul text; imaginea se genereaza
  manual, intr-un instrument de generare AI (Midjourney, Ideogram, DALL·E etc.).
