# Mission: Ciphers

## Why
You want to genuinely understand *how ciphers work* — not just use them, but see the
ideas, history, and reasoning that make a code secure or breakable. This is
curiosity-driven: the payoff is the repeated "aha" of watching secret-writing evolve
from a shift of three letters into the mathematics that secures the modern world.

## Success looks like
- Look at a piece of ciphertext and reason about what kind of cipher likely produced it.
- Encrypt, decrypt, and **crack the classic pen-and-paper ciphers by hand** — Caesar,
  monoalphabetic substitution, Vigenère, transposition.
- Explain *why* each cipher is strong or weak, in terms of keys, keyspace, and the
  patterns an attacker exploits.
- Trace the throughline from classical ciphers to the core ideas behind modern
  cryptography (keys, Kerckhoffs's principle, the one-time pad, public keys).

## Constraints
- **By hand first.** Pencil-and-paper intuition is the preferred mode; tools come second.
- **Classical → modern.** Start with pen-and-paper ciphers; build toward modern ideas as
  understanding compounds (era was "both / unsure" — let the path reveal itself).
- Lessons stay short, self-contained, and tied to building real intuition.

## Out of scope (for now)
- Writing cipher-breaking *code* / programming implementations — revisit if the goal
  shifts toward building (e.g. if the `ciphers/` project here becomes the driver).
- Heavy formal number theory and security proofs.
- Competitive CTF / security-engineering tooling.
