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

Claude citește fișierele din `context/`, `knowledge/` și `prompts/` direct din repo și rulează
agentul potrivit pe loc. Nu trebuie să numești fișierul explicit — Claude rutează automat pe baza
cererii (poza / postare / reel), conform regulii din `/CLAUDE.md` (rădăcina repo-ului). Poți cere
și mai multe deodată ("vreau tot pachetul pentru ideea X") — atunci rulează toți 3 agenții, în
ordine: poză → postare → reel.

## Folosire zilnică

```
[Poza / Postare / Reel] despre [idee]. [orice detalii despre produs/experienta, daca e cazul]
```

Daca nu dai destule detalii pentru un continut credibil (mai ales pentru postare/reel, unde nu se
inventeaza experiente), Claude te intreaba inainte sa scrie.

## Cand actualizezi contextul

Daca schimbi servicii, preturi sau reguli de ton, editezi fisierul din `content_agent/context/` sau
`content_agent/knowledge/` aici, in repo — repo-ul ramane sursa de adevar.

## Ce nu e construit inca

- **Postare directa pe Instagram** — agentii genereaza doar continutul, nu publica nimic automat.
  Publicarea ramane manuala (copy-paste) sau printr-un instrument separat (Buffer/Meta API), daca
  se decide ulterior.
- **Generare efectiva de imagine** — Agentul 1 produce doar promptul text; imaginea se genereaza
  manual, intr-un instrument de generare AI (Midjourney, Ideogram, DALL·E etc.).
- **Voce efectiva** — Agentul 3 produce doar scriptul; vocea se genereaza manual, in ElevenLabs.
