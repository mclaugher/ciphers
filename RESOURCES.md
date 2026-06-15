# Ciphers Resources

Curated, high-trust sources. Knowledge for lessons is drawn from here — never from
memory. Wisdom comes from the communities at the bottom.

## Knowledge

- [Book: *The Code Book* — Simon Singh](https://simonsingh.net/cryptography/)
  The canonical popular history of cryptography, classical → modern, told as a story.
  Use for: the *why* and the narrative arc behind every cipher we study. Chapter 1 covers
  Caesar and the birth of cryptanalysis.
- [The Black Chamber — Simon Singh (interactive tools)](https://www.simonsingh.net/The_Black_Chamber/chamberguide.html)
  Browser tools to encode/decode and **break** substitution, Vigenère, and rail-fence
  ciphers, plus cryptograms to crack. Use for: checking by-hand work and extra practice.
- [Khan Academy — Journey into Cryptography (Brit Cruise)](https://www.khanacademy.org/computing/computer-science/cryptography)
  Free, beginner video series with interactive exercises. Use for: a gentle first look at
  each new idea. Direct: [The Caesar cipher (video)](https://www.khanacademy.org/computing/computer-science/cryptography/crypt/v/caesar-cipher).
- [Wikipedia — Caesar cipher](https://en.wikipedia.org/wiki/Caesar_cipher)
  Reliable reference for mechanics, history (Suetonius), and breakability. Use for:
  fact-checking specifics like keyspace size and the E(x) = (x + n) mod 26 formula.
- [Wikipedia — Kerckhoffs's principle](https://en.wikipedia.org/wiki/Kerckhoffs%27s_principle)
  Use for: the foundational idea that security must rest on the *key*, not on hiding the
  method ("the enemy knows the system").
- [dCode](https://www.dcode.fr/) — cipher *identification* + a tool for nearly every
  classical system. Use for: "what cipher is this?" and verifying answers.
- [Boxentriq — Frequency Analysis](https://www.boxentriq.com/code-breaking/frequency-analysis)
  Use for: letter-frequency tooling when we reach substitution-cipher cracking.
- [Wikipedia — Substitution cipher](https://en.wikipedia.org/wiki/Substitution_cipher)
  Use for: the one-to-one letter mapping and the 26! ≈ 4×10²⁶ keyspace figure.
- [English Letter Frequencies — Practical Cryptography](http://practicalcryptography.com/cryptanalysis/letter-frequencies-various-languages/english-letter-frequencies/)
  Canonical single-letter frequency table (E ≈ 12.7%, ETAOIN order). Use for: the
  frequency-reference card and any frequency claim in lessons.
- [English Letter & Bigram Counts — Peter Norvig (Mayzner revisited)](https://norvig.com/mayzner.html)
  Large-corpus letter, digraph, and word counts. Use for: digraph/word-shape facts (TH, HE, THE).
- [Arab Code Breakers — Simon Singh](https://simonsingh.net/media/articles/maths-and-science/arab-code-breakers/)
  & [al-Kindi's *Manuscript on Deciphering Cryptographic Messages* (c. 850 CE) — History of Information](https://historyofinformation.com/detail.php?id=3162)
  Use for: the origin of frequency analysis (al-Kindi, Baghdad, ~850 CE), Lesson 02's primary source.

## Wisdom (Communities)

- [American Cryptogram Association (ACA)](https://www.cryptogram.org/)
  Non-profit devoted to the *pencil-and-paper* cipher hobby since 1930 — a near-perfect
  match for the by-hand mission. Members construct and solve classical ciphers for each
  other. Use for: graded practice problems, the bi-monthly *Cryptogram*, and real solvers
  to learn from. See their [Cipher Types](https://www.cryptogram.org/resource-area/cipher-types/) guide.
- [r/codes](https://www.reddit.com/r/codes/)
  Reddit community for posting and collaboratively solving codes & ciphers. Use for:
  casual practice and second opinions on a stubborn cryptogram.

## Gaps
- No single vetted "classical → modern" textbook chosen yet beyond Singh. Revisit when we
  approach modern crypto.
- ~~No frequency-table reference doc built yet~~ — **done**: `reference/english-letter-frequency.html`
  (Lesson 02). Verify its percentages against a second corpus if precision ever matters.
- No Vigenère / Kasiski source vetted yet — find one before Lesson 03.
