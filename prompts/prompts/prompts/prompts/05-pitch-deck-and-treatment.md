# 05 — Pitch Deck & Treatment

## Objective
Translate the script into **sellable materials** — logline, synopsis, tone,
comps and author statement — for funding, co-production and broadcasters.
A deck doesn't sell the *plot*; it sells the *experience*, the *urgency*
("why now") and the *author* ("why you").

## When to use
When the project is ready to leave your desk: funding applications, market
co-production forums, broadcaster/streamer submissions, or a producer's
first read. Run it once you have at least a logline + synopsis + characters.

## The prompt
```
You are a development executive and pitch consultant who has read thousands
of decks. I will give you my project material and the TARGET I'm pitching to.
Your job is NOT to invent plot. Your job is to shape what I have into a deck
that a tired reader at the TARGET finishes — and remembers. Be sharp, visual
and specific. No filler adjectives ("gripping", "unique", "powerful").

Produce the deck SECTION BY SECTION. For each section give the exact text
ready to drop onto a slide/page, plus a one-line NOTE on what visual to pair
it with. Sections:

1. TITLE + FORMAT + GENRE — one clean line (e.g. "8 × 50' historical drama").
2. LOGLINE — the single strongest sentence (reuse/refine from step 01).
3. THE HOOK / WHY NOW — 3–4 lines on the cultural or emotional urgency.
   Why does this story need to exist *this year*?
4. SYNOPSIS — one tight paragraph (the spine, not the whole plot). End on a
   question or a door, not a resolution.
5. THE WORLD — 3–4 lines on what makes this world visually and socially
   distinct; why the story can ONLY happen here.
6. TONE & VISUAL LANGUAGE — 3 comps for tone (films/series) each with a
   one-line "we take the X from this", plus palette / camera / music in
   2 lines.
7. CHARACTER SNAPSHOT — the 3 leads, one line each: essence + want + flaw.
8. THE ENGINE (series only) — one line: what generates a new episode weekly.
9. COMPARABLES — 2–3 titles, each with a one-line "why": what audience /
   tone / market they prove. Comps without a "why" are noise — cut them.
10. AUTHOR STATEMENT — 4–6 lines, first person: the personal connection to
    the material and why *you* are the only one who can tell it. Honest,
    not grandiose.
11. STATUS & TEAM — what exists (draft, bible, attached names) and what you
    seek (development funding / co-producer / broadcaster).

After the sections, add:
- THE 30-SECOND PITCH: the whole project in 4 spoken sentences, as if said
  aloud in a lift.
- ONE RISK + ITS ANSWER: the objection the TARGET will have, and the line
  that disarms it.

Adapt emphasis to the TARGET (a public fund wants cultural urgency + team;
a streamer wants engine + audience + comps; a co-producer wants world +
financeability).

Here is my project material (logline / synopsis / bible / beats — paste all
you have):
{{PROJECT_MATERIAL}}

Target I am pitching to: {{TARGET}}
Format: {{FORMAT}}
```

## Variables
- `{{PROJECT_MATERIAL}}` — dump everything you have; the model will select.
- `{{TARGET}}` — e.g. "public film fund" / "international streamer" / "co-production market".
- `{{FORMAT}}` — e.g. "8 × 50' drama" / "feature film".

## Example input
> *Logline + 1-paragraph synopsis + 3 character lines for a dark comedy about
> a coastal town that starts worshipping a stranded whale. Target: European
> co-production market.*

## Notes
- **Sell the experience, not the events.** The reader can't *see* the film —
  make them *feel* the tone in the first slide.
- **Comps need a "why".** "In the tone of *Succession*" is weak; "we take
  *Succession*'s family-as-war-room, but at minimum-wage scale" is a sell.
- **The author statement is the secret weapon.** Funds and festivals back
  *people*. The personal "why me" often decides the read.
- **End the synopsis on a door**, not a summary. A resolved synopsis feels
  like the reader doesn't need to read the script.
- Translate the deck after: a clean English deck opens co-production; a
  native-language version closes the local fund. Keep both.
