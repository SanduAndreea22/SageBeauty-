# Unelte — SageBeauty (Implementation)

> Litera **I** din ACTION framework: cu ce se executa fiecare pas si cine il face. Agentul nu
> promite nimic ce nu poate face singur si nu publica nimic.

| Pas | Unealta | Cine face | Note din practica |
|---|---|---|---|
| Scrie continutul (text, prompturi, script) | Claude Code, pe acest repo | agentul | citeste `context/`, `knowledge/`, `prompts/` direct din fisiere |
| Genereaza imaginile | ChatGPT (generator de imagine) | Andreea | **un prompt = o cerere = o imagine** — mai multe deodata dau colaj; redă bine textul cu diacritice |
| Corecteaza o imagine deja generata | ChatGPT, editare pe imaginea incarcata ("pastreaza imaginea identica, schimba doar...") | Andreea | daca schimba fata, a doua incercare sau text in Canva |
| Text/retus pe imagine | Canva (Magic Eraser, text) | Andreea | varianta de rezerva cand ChatGPT greseste textul |
| Poze cu produsele ei reale | ChatGPT, cu poza produsului incarcata ca referinta | Andreea (doar copy-paste) | **Andreea nu face poze** — agentul livreaza mereu prompt complet (decizia 2026-09-24) |
| Voce + avatar pentru reels | ElevenLabs, prin Chrome (`mcp__claude-in-chrome__*`) | agentul, cu acordul ei la fiecare generare | vezi `prompts/instagram_reels_prompt.md`; consuma credite |
| Publicare Instagram (feed, Stories) | aplicatia Instagram | Andreea | manual; max 5 hashtag-uri |
| Publicare TikTok | aplicatia TikTok (photo mode — carusele si poze single, fara video) | Andreea | aceleasi imagini ca pe Instagram; agentul livreaza "Varianta TikTok" (titlu, caption scurt, 3-5 hashtag-uri, tip de sunet). Pe TikTok ajunge la public nou: primul carusel 94% non-urmaritori, 91% femei |
| Salvare si istoric | `outputs/`, `outputs/log.md`, git (push pe `main`) | agentul | |

## Ce NU poate face agentul

- Nu genereaza imagini singur si nu vede rezultatul pana nu i-l trimite Andreea.
- Nu publica si nu programeaza postari.
- Nu vede statisticile contului — le primeste doar ca screenshot-uri de la Andreea.
