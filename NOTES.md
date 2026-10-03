# Working Notes

Observations and open questions on the outline. Nothing here changes
[`outline.md`](outline.md), which is a faithful transcription of the source document.

---

## 1. Citation spot-check

The source document already carries the author's own warning:

> **Verification:** These citations come from memory, not a live search. Check editions,
> volume/issue numbers and translations against the sources before publishing.

The pass below is **also from knowledge, not a live source check.** It is a triage list
for the real verification pass, not a substitute for it. These are the entries most
likely to need attention:

| Entry | Issue | Suggested correction |
|---|---|---|
| Shannon (1948) | Cited as *BSTJ* 27(3). The paper ran in **two parts**: 27(3), July 1948, pp. 379–423 and 27(4), October 1948, pp. 623–656. | Cite both parts, or cite the 1949 Shannon & Weaver book edition. |
| Wiener (1948) | Cited as "MIT Press/Wiley, 1948." The 1948 first edition was **Hermann & Cie (Paris) and John Wiley (New York)**; MIT Press published the 2nd edition in **1961**. | Pick one: "Wiley, 1948" for first publication, or "MIT Press, 1961" for the edition actually read. |
| Weber, *Economy and Society* | The Roth & Wittich translation was first published by **Bedminster Press, 1968**; the University of California Press printing is 1978. | Note both, or cite the UC Press printing explicitly as a reprint. |
| Conway (1968) | No volume/issue. | *Datamation* 14(5), April 1968, pp. 28–31. |
| Popper (1945) | "Routledge" — the original imprint was **Routledge & Kegan Paul**. | Minor; fix for consistency. |
| Salvi et al. (2024) | Listed as arXiv 2024, "later published in *Nature Human Behaviour*." | Confirm the journal version's year, volume and page range; cite the journal version as primary. |
| Cialdini (2021) | Unity is correctly noted as the seventh principle, but it was introduced in *Pre-Suasion* (2016) before being folded into the expanded *Influence*. | Optional refinement if the seventh principle gets any real weight. |

Everything else in the two origin tables matches what I know of the record, including
the details most likely to be wrong from memory — Asch in Guetzkow's *Groups, Leadership
and Men* (Carnegie Press, 1951), Goffman's 1956 Edinburgh / 1959 Anchor split, Arrow in
*Philosophy & Public Affairs* 1(4), Freudenberger in *Journal of Social Issues* 30(1),
and Kant's transcendental formula of public right sitting in Appendix II. That is a good
hit rate for citations recalled rather than looked up.

**Not yet done:** a live, source-by-source verification. Say the word and I'll run one
across all 39 origin entries and the 63 further-reading entries and record the results
here with page numbers and DOIs.

## 2. Structural observations

- **Act VIII is thin.** Four beats against eight each for Acts III and VI. In a talk this
  is survivable because the close carries it; in the book map it is the chapter with the
  most expansion work and the least raw material. See [`formats/book-outline.md`](formats/book-outline.md).
- **Beats 5 and 51 are a deliberate bookend** — the ethical limit promised early and paid
  off at the end. This is the single structure that does *not* survive translation to book
  form, for the reason given in the book map.
- **Every beat has at least one citation.** No gaps. Worth preserving as an invariant: if a
  new beat is added in expansion and cannot be traced to an origin, that is a signal about
  the claim, not about the bibliography.
- **Five beats rest on a single mid-century source with no modern companion.** Cross-checking
  the bibliography against the further-reading tags, every beat has at least one origin
  source, but beats **4, 15, 31, 37 and 40** have exactly one source each, all published
  1974–1984, and nothing contemporary behind them:

  | Beat | Claim | Sole source |
  |---|---|---|
  | 4 | The enterprise is the hardest difficulty setting | Brooks (1975) |
  | 15 | Framing determines the answer more reliably than evidence | Tversky & Kahneman (1981) |
  | 31 | Know what your manager is measured on | Kerr (1975) |
  | 37 | Weaponized vagueness moves accountability onto you | Eisenberg (1984) |
  | 40 | A request versus a quota being transferred to you | Oncken & Wass (1974) |

  At talk speed this is fine. In a book it is five places where a reviewer can ask "and has
  anyone shown this since 1984?" Beat 15 is the most exposed — framing has a large modern
  literature the outline doesn't touch — and beat 40 is the thinnest, since the monkey-transfer
  model is an *HBR* essay with no empirical base at all. Beats 42, 48 and 52 also lack modern
  companions, but correctly so: their origin source *is* the modern one, which the author
  already flagged.

- **Load-bearing sources.** Cialdini (5 beats), Aristotle (4), Mitnick & Simon (4), Asch
  (3), Barnard (3), Goffman (3), Simon (3). If any one of those readings is challenged, a
  lot of the outline moves at once. Cialdini and Mitnick & Simon are the two most likely to
  draw scrutiny from a security-literate audience.

## 3. Risks worth tracking

- **The Hadnagy problem**, already flagged in the source: DEF CON banned Christopher
  Hadnagy in 2022 over code-of-conduct complaints, and both his books are in the further
  reading (beats 2 and 5). A security audience may know. Options: drop both, keep with a
  footnote, or replace — the Ferreira, Coventry & Lenzini paper already in the list covers
  beat 2's ground academically. **Decision needed before the talk is given**, not before
  it is published.
- **Act VII will date.** It is the most time-sensitive material in the project and the
  gap between the talk and the book is where it will rot. The distribution proposal in the
  book map is partly a mitigation for this.
- **Origin-list composition.** Only a handful of the 39 origin entries have a woman as
  author or co-author (Kram, Bainbridge, Fenley & Liechti, Casciaro). The further-reading
  list is far more balanced. A reviewer of the book — and plausibly someone in a conference
  Q&A — will notice the contrast between the two lists. Worth having an answer ready, or
  worth revisiting whether some origins are genuinely the earliest statement of the idea.
- **The gaming metaphor is half-committed.** "Build," "spec," "stats," "respec" appear in
  beats 3 and 49 and in the title, and nowhere else in 52 beats. Fine at talk speed. In a
  book it needs to either run throughout or leave the title.

## 4. Open questions for the author

1. Is the 60-minute slot 60 minutes of content, or 50 plus Q&A? The whole timing plan in
   [`formats/talk-60min.md`](formats/talk-60min.md) turns on this.
2. Is the lightning talk a standalone piece or a trailer for the long talk? That decision
   picks between the two strategies in [`formats/lightning-5min.md`](formats/lightning-5min.md).
3. Which beats have a real story behind them? That list is the book's actual scope, and
   nothing else about the expansion can be planned until it exists.
4. Who is the audience for the 60-minute version — an engineering conference, an internal
   org, or a security conference? Act VI reads very differently to each.
