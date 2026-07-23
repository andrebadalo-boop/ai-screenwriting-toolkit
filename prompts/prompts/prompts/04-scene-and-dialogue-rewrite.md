# 04 — Scene & Dialogue Rewrite

## Objective
Rewrite a scene for **subtext**, **conflict**, **late entry / early exit** and
**distinct character voices** — and cut every on-the-nose line. A good scene
ends in a different place than it began; a good line says one thing and
means another.

## When to use
In the rewrite stage, scene by scene. Also as a warm-up exercise: paste your
weakest scene and let it get dismantled. The model is a ruthless editor here —
that's the point.

## The prompt
```
You are a script doctor and dialogue editor working with a professional
screenwriter. I will give you a scene and its purpose in the story. Your job
is NOT to add plot. Your job is to make this scene earn its place on the page
through conflict, subtext and voice. Be unsentimental — cut what is soft.

First, DIAGNOSE the original scene. In a short list, name:
- the ON-THE-NOSE lines (where a character says exactly what they feel/know),
- the EXPOSITION dumps (information the audience doesn't need *here*),
- the MISSING CONFLICT (where two characters agree too easily),
- the ENTRY/EXIT problem (does it start too early or linger too long?),
- the VOICE problem (could the lines be swapped between characters?).

Then, REWRITE the scene in proper screenplay format. Apply these rules:
- Enter LATE, leave EARLY. Start as close to the turn as possible.
- Give each character a SCENE OBJECTIVE and an OBSTACLE to it.
- The scene must TURN: end in a different power/emotional state than it began.
- Convert feelings into ACTION and SUBTEXT — what is *not* said does the work.
- Make each voice distinct: rhythm, vocabulary, what they avoid saying.
- Cut at least 20% of the dialogue. Silence is a line.

Finally, add a CHANGE LOG: 4–6 bullet points, each = "I changed X → because Y
(craft principle)".

Here is the scene text:
{{SCENE_TEXT}}

What this scene MUST accomplish in the story:
{{SCENE_GOAL}}

Characters in the scene (with one-line essence each):
{{CHARACTERS_IN_SCENE}}
```

## Variables
- `{{SCENE_TEXT}}` — paste the scene as-is (rough is fine).
- `{{SCENE_GOAL}}` — e.g. "the protagonist must lose an ally without saying why".
- `{{CHARACTERS_IN_SCENE}}` — e.g. "MARTA — proud, never asks; TOMÁS — jokes to hide fear".

## Example input (intentionally on-the-nose, to show the before/after)
> *INT. KITCHEN — NIGHT*
> *MARTA: I am very angry at you because you lied to me.*
> *TOMÁS: I am sorry, I feel guilty and I love you.*
> *MARTA: I don't know if I can forgive you.*
> *Goal: Marta decides to leave, but cannot say it aloud.*

## Notes
- **Subtext test:** cover the dialogue and read only the action lines. If the
  scene's meaning still comes through, you've got subtext. If not, the
  dialogue is doing the exposition's job.
- **Conflict test:** in every exchange, ask "what does each want *right now*?"
  If both want the same thing, the scene is dead — give one of them a secret.
- **Voice test:** read the lines without the character names. If you can't
  tell who's speaking, the voices are the same voice in different fonts.
- A scene that only *reveals information* is not a scene — it's a memo.
  Make the information cost someone something.
