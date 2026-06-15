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
