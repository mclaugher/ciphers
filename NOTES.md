# Teaching Notes — Ciphers

Working notes on how to teach this learner. Not a journal — preferences and conventions.

## How they like to learn
- Prefers learning **by hand** (pencil & paper) over code. Build intuition first.
- Goal is **understanding for its own sake** (curiosity-driven) — no deadline or deliverable.
- Responded comfortably to structured multiple-choice prompts during setup.

## Pacing
- Era: **start classical, build toward modern** ("both / unsure"). Let the path reveal itself.
- Keep lessons short and self-contained; one tangible win each. Mind working memory.

## Open questions to revisit
- Is the `ciphers/` software project in this directory related to this learning goal?
  (User didn't say.) If a build goal emerges, the "no code" scope may change.
- Math appetite unknown. Gauge from their reaction to mod-26 arithmetic in Lesson 1; if
  they enjoy it, lean into the arithmetic view of ciphers (affine, Hill, RSA later).

## Conventions for this workspace
- **Cite every factual claim** in lessons; link back to sources in RESOURCES.md.
- **Quiz options: equal word count**, no formatting tells, no length clues.
- Promote a term to GLOSSARY.md only **after** the user can use it correctly (not on first
  exposure). Candidates waiting on evidence: *cipher, plaintext, ciphertext, key, keyspace,
  substitution, Kerckhoffs's principle*.
- Each lesson: one primary source to read/watch, cross-links to reference docs, and a
  reminder that I (the agent) am their teacher — ask followups.

## Progress
- Lesson 01 — The Caesar Cipher: created. (Awaiting evidence of mastery before LR + glossary.)
- Lesson 02 — Substitution & Frequency Analysis: created, with interactive frequency-analysis
  cracker (intercept solves to a Kerckhoffs-themed quote; key = QWERTY layout). Built the
  `english-letter-frequency.html` reference card alongside it.
  - Mission throughline reinforced: big keyspace ≠ secure; ciphertext must not leak plaintext
    structure. Teed up Lesson 03 (Vigenère) as the deliberate answer to frequency analysis.
  - Still **awaiting evidence of mastery** before writing the first learning record or promoting
    glossary terms. Watch for: can they crack the intercept *without* the "starter" button, and
    do they reach for E→most-common unprompted? Math-appetite question (NOTES, open) still open —
    they met 26!/factorial here; gauge reaction.
- Lesson 03 — The Vigenère Cipher: created. Three interactives: encrypt/decrypt with repeating-key
  alignment; a frequency-flattening demo (plain vs substitution vs Vigenère bars — the visual
  "why it's strong"); and a Kasiski key-length finder (intercept key=LEMON, "WE ARE SURROUNDED…",
  GCD of gaps 60/45/20 = 5). Built `vigenere-tableau.html` reference card alongside.
  - Deliberate structure: Lesson 03 teaches the cipher + the *idea* of the break (repeating key
    leaks its length) but stops before the full column-by-column crack — that's **Lesson 04**, to
    keep within working memory. Throughline made explicit: Vigenère = Caesar with a moving shift;
    breaking it = key-length (Kasiski) + Lesson-02 frequency analysis per column.
  - User said "keep building lessons" — proceeded straight from L02 to L03 without a mastery check.
    Still no learning records / glossary promotion (no direct evidence yet). If they keep saying
    "continue," consider a light retrieval check before L04 to avoid building on sand.

- Lesson 04 — Breaking the Vigenère Cipher: created. Column-by-column cracker on a 388-letter
  intercept (key LEMON); "solve by frequency" auto-fills each column's key letter via most-common=E,
  with live full-message decode and a manual-nudge path for columns whose top letter isn't E. Built
  `breaking-vigenere.html` playbook reference. Closes the classical-cryptanalysis thread: Caesar →
  substitution/frequency → Vigenère → breaking Vigenère.
  - Next deliberate beat: **Lesson 05 — one-time pad & perfect secrecy** (teed up in L04). This is the
    classical→modern hinge the MISSION calls out. Will need real sourcing on Shannon (see RESOURCES gap).

## Pacing observations
- 2026-06-15: User is in "keep building" mode (batch-consuming lessons) rather than working through
  the interactives between sessions. Lessons are accumulating faster than evidence of mastery. Not a
  problem yet, but the first learning record should wait for a real signal (a solved intercept, a
  question that shows a misconception, or an explicit "I've got this").
- 4 lessons + 4 reference cards now exist with ZERO learning records and an empty glossary. Before
  Lesson 06, strongly consider pausing to (a) run a cross-lesson retrieval check, (b) write the first
  learning record, (c) seed GLOSSARY.md with the terms the user has clearly absorbed. Flag this to the
  user rather than building indefinitely on unverified mastery.
