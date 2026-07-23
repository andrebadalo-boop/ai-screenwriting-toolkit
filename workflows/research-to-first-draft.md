# Workflow — Research → First Draft

> This is the **pipeline**: the order in which the prompts and templates are
> meant to be used, and how the output of each step becomes the input of the
> next. Don't skip ahead — a weak logline poisons every step after it.
> The model is a writing partner at each stage; **you** own the voice and the
> final call. Works with Claude or any LLM.

## The shape of the pipeline

```
[0] RESEARCH  →  [1] LOGLINE  →  [2] CHARACTERS  →  [3] STRUCTURE
        →  [4] OUTLINE  →  [5] SCENE-BY-SCENE DRAFT  →  ([6] PITCH, in parallel)
```

Each arrow means: *copy the agreed output of the left step and paste it as
context at the top of the right step's prompt.* That hand-off is the whole
method. It keeps the model working from **your** decisions, not its guesses.

---

## Step 0 — Research (ground the story before you invent it)

> Especially for **historical, true-story or procedural** material (e.g. a
> period drama about a real trial), do this *first*. Inventing on top of
> unverified facts costs you rewrites later.

- Collect sources and **keep a running "facts vs fiction" note**:
  - ✅ **Fact** — verified, with source (archive, law text, interview, press).
  - 🔁 **Dramatised** — based on a fact but compressed/changed for drama.
  - ✨ **Invented** — wholly fictional, added for theme or engine.
- Decide, in one line, your **contract with the truth**: e.g. *"faithful to the
  event, free with the private lives"* — so every later choice is consistent.
- Output of this step: a **1–2 page research brief** (world, rules, real
  figures, the one historical question your story will answer). This brief is
  the first thing you paste into every later prompt.

> Tip for period work: research the **texture** (objects, prices, slang, what
> people couldn't say aloud) as much as the events. Texture is what makes a
> world feel lived-in on screen.

---

## Step 1 — Logline & premise

- Open: [`../prompts/01-logline-and-premise.md`](../prompts/01-logline-and-premise.md)
- **Input:** your research brief (step 0) + your raw idea.
- **Do:** generate the 3 loglines, pick the strongest, run the stress test.
- **Exit gate (don't proceed until true):** the chosen logline passes the
  "any film" test *and* has a visible stake. If not, loop here — cheap to fix
  now, expensive on page 60.
- **Output to carry forward:** the chosen logline + its element breakdown.

---

## Step 2 — Character bibles

- Open: [`../prompts/02-character-bible.md`](../prompts/02-character-bible.md)
- **Input:** the logline (step 1) + a rough sketch per main character.
- **Do:** run the prompt **once per main character and once for the antagonist**.
  The antagonist gets a bible too — a villain without a want/need is a weather
  event, not a character.
- **Exit gate:** every lead has a clear **want ≠ need** gap and at least one
  contradiction. If want and need match, the arc is flat — push harder.
- **Output to carry forward:** the set of character bibles (essence, want,
  need, wound, flaw-in-action, arc, voice lines).

---

## Step 3 — Beat sheet & structure

- Open: [`../prompts/03-beat-sheet-and-structure.md`](../prompts/03-beat-sheet-and-structure.md)
- **Input:** logline (step 1) + a merged paragraph of the character arcs
  (step 2) + your research brief (step 0).
- **Do:** build the beat grid; for series, build the **season spine** *and* the
  **pilot** grid, plus the one-line engine statement.
- **Exit gate:** the **Stakes Ladder** climbs at beats 4 → 9 → 11 → 13, and the
  midpoint is a true reversal (changes meaning, not just "more plot").
- **Output to carry forward:** the beat sheet + the engine statement (series).

---

## Step 4 — Outline (turn beats into pages-worth of scenes)

- Open the matching template:
  - Feature / pilot body → [`../templates/one-page-synopsis.md`](../templates/one-page-synopsis.md)
    (write the spine as prose first — it exposes plot holes the grid hides).
  - Per-episode breakdown (series) → [`../templates/episode-outline.md`](../templates/episode-outline.md)
- **Input:** the beat sheet (step 3).
- **Do:** expand each beat into scenes/blocks, each with a function and a turn.
  For series, make sure the pilot's final image **opens a door**, not closes one.
- **Exit gate:** every block/scene turns; A- and B-stories cross; the end hook
  opens a *new* question.
- **Output to carry forward:** the scene-by-scene outline (your shooting map).

---

## Step 5 — First draft, scene by scene (then rewrite each scene)

- Write the draft **from the outline**, one scene at a time, in your own voice.
  Let the model draft *with* you if useful, but the voice on the page is yours.
- Then, scene by scene, run the rewrite prompt as a **doctor's pass**:
  - Open: [`../prompts/04-scene-and-dialogue-rewrite.md`](../prompts/04-scene-and-dialogue-rewrite.md)
  - **Input:** the drafted scene + its goal (from the outline) + the characters'
    one-line essences (from step 2).
  - **Do:** take the diagnosis, accept the cuts, rewrite for subtext and voice.
- **Exit gate per scene:** it enters late / leaves early, it turns, and the
  dialogue passes the "cover the lines, read the action" subtext test.
- **Output:** a complete first draft that already had one surgical pass.

---

## Step 6 — Pitch materials (run in parallel, from step 3 onward)

- Open: [`../prompts/05-pitch-deck-and-treatment.md`](../prompts/05-pitch-deck-and-treatment.md)
- **Input:** everything above (logline, bibles, beat sheet, synopsis).
- **Do:** generate the deck tuned to the **target** (public fund vs streamer vs
  co-production market — the emphasis changes; the prompt handles this).
- **When:** you don't need a finished draft to pitch — a strong bible + synopsis
  + deck is often what gets the draft *funded*. Start this as soon as step 3
  holds, and refresh it after step 5.
- **Output:** a target-specific deck + the 30-second spoken pitch.

---

## The hand-off rule (the part people skip — don't)

At every step, **paste the agreed outputs of the previous steps at the top of
the new prompt**, under a line like `--- CONTEXT FROM PREVIOUS STEPS ---`.
This is what makes the model consistent across a long project instead of
re-inventing your characters every time. A 10-minute context paste saves hours
of contradiction-hunting.

## End-of-pipeline checklist

- [ ] Logline survived the "any film" test (step 1).
- [ ] Every lead has want ≠ need + a contradiction (step 2).
- [ ] Stakes ladder climbs; midpoint is a real reversal (step 3).
- [ ] Every scene/block turns; A & B cross; hook opens a new question (step 4).
- [ ] Each scene passed the subtext + late-entry/early-exit test (step 5).
- [ ] The deck matches the target and ends the synopsis on a door (step 6).
- [ ] The **voice on the page is yours** — the model sped you up, it didn't
      write you.

## A note on authorship

This pipeline is a scaffold, not an author. The craft decisions — what to cut,
what hurts, what's true — are human and they are *yours*. Use the model to
think faster and to pressure-test; use your judgement to decide. The goal is
not an AI-written script. The goal is **your** script, reached with fewer dead
ends — and a method you can hand to a student and they can run on day one.

---

*Built and maintained in the open by André Badalo —
[github.com/SEU-USER/ai-screenwriting-toolkit](https://github.com/SEU-USER/ai-screenwriting-toolkit).
Reuse, remix, translate, teach (CC BY 4.0).*
