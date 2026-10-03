# Working Notes

Observations and open questions on the outline. Nothing here changes
[`outline.md`](outline.md), which is a faithful transcription of the source document.

---

## 1. Citation spot-check

The source document already carries the author's own warning:

> **Verification:** These citations come from memory, not a live search. Check editions,
> volume/issue numbers and translations against the sources before publishing.

A partial live verification has since been run against the actual texts and library
catalog records. Results are below; digital locations for every origin source are in
[`sources-digital.md`](sources-digital.md). **Status** marks what was checked against a
source rather than recalled.

| Entry | Issue | Resolution | Status |
|---|---|---|---|
| Shannon (1948) | Cited as *BSTJ* 27(3). The paper ran in **two parts**: 27(3), July 1948, pp. 379–423 and 27(4), October 1948, pp. 623–656. | Cite both parts, or cite the 1949 Shannon & Weaver book edition. | **Confirmed** |
| Wiener (1948) | Cited as "MIT Press/Wiley, 1948." The 1948 first edition was **John Wiley (New York)**; MIT Press published the 2nd edition in **1961**. | Pick one: "Wiley, 1948" for first publication, or "MIT Press, 1961" for the edition actually read. | **Confirmed** — archive.org catalogues the 1948 edition as "New York, J. Wiley" |
| Weber, *Economy and Society* | The Roth & Wittich translation was first published by **Bedminster Press, 1968**; the University of California Press printing is 1978. | Note both, or cite the UC Press printing explicitly as a reprint. | Partly — the 1922 German original is confirmed as Tübingen: Mohr |
| Conway (1968) | No volume/issue. | **Leave it out.** Conway's own site gives only "*Datamation*, April 1968"; secondary sources split between 14(4) and 14(5). Cite month, year and the author's page. | **Unresolved** — my earlier suggestion of 14(5) is not supportable |
| Popper (1945) | "Routledge" — the original imprint was **Routledge & Kegan Paul**. | Minor; fix for consistency. | **Confirmed** |
| Salvi et al. (2024) | Listed as arXiv 2024, "later published in *Nature Human Behaviour*." | Confirm the journal version's year, volume and page range; cite the journal version as primary. | Not yet checked |
| Cialdini (2021) | Unity is correctly noted as the seventh principle, but it was introduced in *Pre-Suasion* (2016) before being folded into the expanded *Influence*. | Optional refinement if the seventh principle gets any real weight. | Not yet checked |
| Aristotle *Rhetoric* II.1 | Does II.1 actually name the three components of ethos? | Yes, verbatim: "good sense, good moral character, and goodwill." Beat 49's "three stats" is sound. | **Confirmed** |
| Kant, Appendix II | Does the transcendental formula sit in Appendix II? | Yes. Full title: "Concerning the Harmony of Politics with Morals According to the Transcendental Idea of Public Right." | **Confirmed** |
| Cialdini (1984) | First edition cited as William Morrow, 1984. | The 1984 first edition is **not digitised** — archive.org has 1993 and later, and the principles were reworded between editions. Don't quote a later printing as 1984. | **New issue found** |

Several details that were most likely to be wrong from memory checked out against
sources: Asch in Guetzkow's *Groups, Leadership and Men* (Carnegie Press, 1951, pp. 177–190),
Trist & Bamforth at *Human Relations* 4(1), 3–38, Granovetter at *AJS* 78(6), May 1973,
Kram at Scott, Foresman 1985, Scott at Yale UP 1998, Mitnick & Simon at Wiley 2002, and
Barnard's 1938 Harvard UP first edition. That is a high hit rate for citations recalled
rather than looked up.

One caveat on Goffman: the 1956 Edinburgh / 1959 Anchor split is correct as a
bibliographic fact, but the 1956 Edinburgh monograph does not appear to be digitised
anywhere, so only the 1959 text can actually be consulted.

**Still outstanding:** the 16 origin sources in Tier 4 of
[`sources-digital.md`](sources-digital.md) are paywalled and have not been checked against
print, and none of the 63 further-reading entries has been verified at all. The journal
details for those were recalled, not looked up.

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
