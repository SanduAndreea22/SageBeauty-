# SageBeauty

Acest repo conține `content_agent/` — angajatul de Instagram al Andreei pentru brandul SageBeauty
(prompt-uri de poze AI, postări, reels cu voiceover ElevenLabs).

## Protocol obligatoriu pentru cereri de conținut Instagram

Cand Andreea cere continut pentru Instagram (poza, postare, reel), **citeste integral si urmeaza
exact** promptul dedicat din `content_agent/prompts/` — nu folosi skill-uri generice de copywriting
sau cunostinte proprii de marketing in locul lor.

- Prompt de poza → `content_agent/prompts/instagram_photo_prompt.md`
- Postare → `content_agent/prompts/instagram_post_prompt.md`
- Reel → `content_agent/prompts/instagram_reels_prompt.md`
- Carusel → `content_agent/prompts/instagram_carousel_prompt.md`
- Stories → `content_agent/prompts/instagram_stories_prompt.md`

Nu trebuie sa numeasca fisierul explicit — rutezi automat pe baza cuvantului din cerere ("poza"/
"prompt de poza" → Agent 1; "postare"/"caption" → Agent 2; "reel"/"reels" → Agent 3; "carusel" → Agent 4; "stories"/"story" → Agent 5). Daca cere mai
multe deodata, ruleaza-le pe rand, in ordine: poza → postare → reel/carusel → stories. Daca cererea e ambigua si nu
poti stabili care agent, **intreaba inainte sa scrii** — nu ghici si nu amesteca formatele.

Detalii complete de rutare, reguli de continut si structura proiectului sunt in
`content_agent/CLAUDE.md` — nu se duplica aici.
