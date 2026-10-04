# Charisma Builds — Revised Outline

*Social Engineering for Influence and Self-Defense at Enterprise Scale*

> **Working draft, 2026-10-04.** The original outline is preserved unchanged in
> [`outline.md`](outline.md). This version keeps the original eight acts and fifty-two
> points in their original order, with each one fleshed out using the ideas developed in
> discussion. Sources added since the original are marked **(new)**. Each act opens with
> a status line saying how much it has shifted.

---

## Abstract (revised)

Most engineers treat charisma like a dump stat. Every point goes into combat, and the
story and character development get skipped. In an enterprise, the story is the org: your
manager, your peers, your career. This talk argues that charisma is a build you can spec
into. It treats social engineering as a toolkit engineers can use openly, and must learn to
recognize when it's used on them.

It starts from one belief: authority is granted by the governed. Organizations promote
people past their skills and abandon them there, and we call it Dunning-Kruger and give up.
The talk offers another option, **elicitation**: running the principles of a performance
improvement plan on your own work, informally and with empathy, through questions that turn
vague, unmeetable expectations into clear ones. Done well, your manager notices the pattern,
sees that it works, and adopts it.

It covers peer leadership modeled on the SRE and the blameless postmortem, how to ask
questions without judgment, and how the conditions a struggling manager creates mirror the
ones a scammer manufactures. Self-defense here means acting first, because no one else is
going to do it for you. The talk ends with a firm ethical limit: if a technique works only
when the other person doesn't know you're using it, don't use it. Wherever possible, each
claim is traced to the person who first stated the idea.

## The core belief

**Authority is granted by the governed.** Anyone practicing this has to actually believe it.
If you don't, the questions come out apologetic, and apologetic questions sound like stalling.

- **The corporate origin: Chester Barnard** (*The Functions of the Executive*, 1938). Authority
  doesn't sit with the person giving an order. It exists only when the person receiving the
  order accepts it.
- **The political origin:** John Locke grounded government in consent (1689) **(new)**, and
  before him Étienne de La Boétie's *Discourse on Voluntary Servitude* (c. 1550) **(new)**
  argued that a tyrant holds power only because people keep obeying.

---

## Act I: The Premise

*Status: holds. The title survived intact, and every word in it now means something specific.*

**1. Every technical system you've ever debugged is wrapped in a social system you never read the source for**
The longwall coal study found that new mining technology failed because it broke up the work
groups around it. Your org works the same way. And its social system has a failure mode
engineers will recognize: people promoted past what they can do and left there.
- Trist & Bamforth (1951)

**2. "Social engineering" is a neutral tool, and attackers borrowed it from salespeople, not the other way around**
Sharper now. The techniques split into two kinds. Some still work when the other person knows
about them: asking clarifying questions, restating someone's view, building support in the open.
Others only work when hidden: pretexting, fake urgency. This talk teaches the first kind and how
to recognize the second. Its signature technique, *elicitation*, is a word social engineers and
requirements engineers both use. And its success condition is the reverse of an attack's: it
works best once the other person discovers it.
- Popper (1945); Cialdini (1984)

**3. Charisma is not a personality trait you were issued at birth; it is a build you spec into**
The theme. In games where dialogue, story and companions run on Charisma, players dump it for
combat stats and miss the story. Engineers do the same thing: every point goes into technical
skill and none into the conversations where the org actually makes its decisions. In *Fallout*,
a high enough Speech skill lets you talk the final boss out of the fight entirely (the Master in
the first game, Legate Lanius in *New Vegas*). This talk is about your boss fight. Weber thought
charisma was an extraordinary gift that couldn't be taught; Antonakis showed it can be trained.
Put the old view and the evidence side by side.
- Weber (1922); Antonakis, Fenley & Liechti (2011)

**4. The enterprise is the hardest difficulty setting: high headcount, low bandwidth, no shared context**
Add the difficulty modifier. Organizations promote people for being good at their last job until
they land in one they can't do, and then provide no support. Across 214 firms, the top
salespeople were promoted and turned out to be worse managers. Most people meet the result as
their manager. On top of that, the unwritten deal at work, the psychological contract, is broken
so often that the paper documenting it is titled "Not the Exception but the Norm."
- Brooks (1975); Peter & Hull, *The Peter Principle* (1969) **(new)**; Benson, Li & Shue (2019) **(new)**; Robinson & Rousseau (1994) **(new)**

**5. What this talk will and will not teach you (and the line I will not help you cross)**
It will teach you how to get clarity from a manager who can't give it, how to lead peers with
facts, and how to recognize the conditions manipulation needs. It won't teach you to deceive
anyone. The line: if it only works when they don't know, don't do it. In the talk's own theme,
D&D has four Charisma skills: Persuasion, Performance, Intimidation and Deception. This build
puts no points in Deception.
- Kant (1795), Appendix II

---

## Act II: Systems, Both Kinds

*Status: core to the talk, and mostly not yet discussed point by point. It has a new job:
explaining why your manager is failing. The cause is the system, not the person.*

**6. You already think in systems; you just stopped at the network boundary**
You already run blameless postmortems on your services: you look for the conditions that
produced the failure, not a person to blame. This talk asks you to point that habit at people.
(Borrowing from Wiener: an analogy, not evidence.)
- Wiener (1948)

**7. Org charts are the documented API; the real call graph is informal and undocumented**
Barnard is the source of both ideas here: the informal organization, and the core belief that
authority is granted by whoever accepts it. The org chart shows who may give orders. The
informal graph shows whose orders actually get accepted.
- Barnard (1938)

**8. Conway's Law runs in both directions: your architecture is a confession about your relationships**
Where the team is tangled, the system is tangled. A manager who can't define "done" shows up in
the code as unclear interfaces and rework. Fixing the relationship is part of fixing the system.
- Conway (1968)

**9. Information in an enterprise obeys routing rules, and most of it is dropped at the first hop**
Bartlett's retelling experiments showed that a story degrades every time it's passed on. A
verbal instruction from your manager is already one retelling away from their boss's intent,
and one more away from what you'll remember of it. That's why elicitation always ends with a
written recap: it's the only copy that doesn't degrade.
- Bartlett (1932)

**10. Trust is the latency budget of an organization**
Where trust is high, a one-line request works. Where it's low, every request needs a spec, a
recap and a check-in. Elicitation is what you do while trust is low, and done well it rebuilds
the trust so that overhead can drop.
- Arrow (1972)

**11. Every org has a hidden dependency graph, and reputation is its service registry**
Reputation is how people decide whom to route work and trust through. The stance here is not to
chase credit or the raise. A reputation as a team player and an effective communicator doesn't
go unnoticed, and weak ties carry it further than your manager ever will.
- Granovetter (1973)

---

## Act III: The Mechanics of Influence

*Status: partly absorbed. Several points became the questions and the delivery style of
elicitation.*

**12. Influence is throughput, not volume: being heard beats being loud**
A good question has high throughput: it forces a specific answer. One clear ask with one piece
of evidence gets through where ten loud ones don't. (Borrowing from Shannon.)
- Shannon (1948)

**13. Attention is the scarcest resource in the building, and you are competing with 400 unread emails**
Your manager's attention is the bottleneck. That's why the elicitation questions come together
in one bundle rather than one at a time, and why the recap is short enough to actually get read.
- Simon (1971)

**14. Reciprocity, consistency, social proof, authority, liking, scarcity: the six primitives, and where each one fails at scale**
Each principle has an honest form and a hidden one: real scarcity versus a fake deadline, real
authority versus an impersonated one. The disclosure test sorts *within* each principle, not
between them. Elicitation uses the honest forms; the self-defense act teaches you to spot the
hidden ones.
- Cialdini (1984)

**15. Framing determines the answer more reliably than evidence does**
Framing is how the questions land. "So I don't waste your time" gets a different answer from
"you never told me." Present every question as learning and coaching, never as judgment.
- Tversky & Kahneman (1981)

**16. Specificity is charisma: vague asks get vague outcomes**
This is the engine of elicitation. Locke found that specific goals beat "do your best." When
your manager can't make the goal specific, you ask until it is: what does done look like, how
will we know it worked, and by when?
- Locke (1968)

**17. The highest-leverage sentence in any meeting is "Let me make sure I understand what you need"**
This is the opening move of every elicitation conversation. Restating their request in your own
words exposes the gaps without accusing anyone of leaving them.
- Rogers & Roethlisberger (1952)

**18. Status and status-signaling are real variables, and ignoring them does not zero them out**
A manager's status is at stake every time a question implies they didn't think something
through. Goffman described how people cooperate to help each other save face, and everyone
involved knows it's happening. So give the manager an ego escape: the gap becomes something
you're working out together, not something they missed. Saving face may be the clearest case of
a technique that works even though everyone knows it's being used.
- Weber (1922); Goffman (1959); Goffman, "On Face-Work" (1955) **(new)**

**19. Narrative beats data in the room; data beats narrative in the follow-up**
In the room, the story is "let's get this right together." In the follow-up, the recap is the
data: dates, decisions, priorities. Let the sting go in the room, and keep the facts in writing.
- Aristotle, *Rhetoric*, Book I.2

---

## Act IV: Peer Leadership Without Authority

*Status: defined. The model is the SRE and the blameless postmortem. Peer leadership happens at
the water cooler.*

**20. Most of your real leverage is lateral, and none of it comes with a title**
The model is an SRE who finds gaps in a system and brings metrics, with no authority beyond
facts and reasoning, and still drives results. That works because of the core belief: people
accept facts, so facts carry authority. Subordinates who influence their bosses mainly by
reasoning get the highest performance ratings.
- Barnard (1938); Kipnis, Schmidt & Wilkinson (1980) **(new)**; Kipnis & Schmidt (1988) **(new)**

**21. Credit is a renewable resource, and spending it on others compounds your own**
Credit flows upward too. Giving your manager credit for improvements leads to one of two good
outcomes: they adopt the pattern, or they get noticed and move to a role that suits them better.
The goal isn't to climb. One caution: the givers who finish last are the selfless ones, and the
ones who finish first are "otherish," generous but still protecting their own interests. The
written record and the end date are what keep you otherish.
- Gouldner (1960); Grant, *Give and Take* (2013)

**22. Being the person who makes other people's work legible is a full-time superpower**
The recap makes your manager's decisions legible to you, to the team and to their own boss.
That's why it reads as a gift and not as a file being built. It's also invisible glue work, and
the talk should say so.
- Scott (1998); Reilly, "Being Glue" (2019)

**23. Disagreement is a protocol, not an event: how to dissent and keep the connection open**
The blameless postmortem is that protocol in practice: no rank in the room, the situation over
the person, and everyone free to say what happened. Disagreeing with a manager works the same
way. It's about the plan, never the person.
- Rogers & Roethlisberger (1952); Asch (1951); Allspaw, "Blameless PostMortems and a Just Culture" (2012) **(new)**

**24. The "generous read" is a debugging technique for human behavior**
Labeling your manager "Dunning-Kruger" and giving up is the fundamental attribution error:
blaming someone's character for what their situation produced. Use Dunning-Kruger as a
framework, not a diagnosis. If they can't see the gap, don't ask them to see it; help them fill
it. Point it at yourself first, too: you probably can't see what your manager is being measured
on. Say early and out loud that the effect is disputed as a *measurement* (random data reproduces
the famous chart, and the "Mount Stupid" curve isn't in the paper). That's exactly why it's used
here as a framework.
- Heider (1958); Ross (1977); Kruger & Dunning (1999) **(new)**; Nuhfer et al. (2016) **(new)**

**25. Build the coalition before the meeting, because the meeting is a ratification ceremony**
The water cooler is where the coalition already forms, and usually it forms against the manager.
Peer leadership turns it around. When people complain about the boss, steer the conversation from
character to situation and share the questions, so the team helps its leader be their best self.
One person asking "what does done look like?" is a quirk; a whole team asking it makes clarity
the norm. In Milgram's variation where two fellow participants refused to continue, full
obedience dropped to about one in ten. Peers change what authority can do.
- Asch (1951); Milgram (1974)

**26. Mentorship is distributed caching: you are warming someone else's context**
Point it upward. This is, in effect, quietly mentoring your manager: warming their context on
what good management looks like, one question at a time.
- Kram (1985)

---

## Act V: Navigating Managerial Relationships

*Status: changed the most. It now has a single practice running through it.*

**The practice: elicitation.** Take the principles of a PIP (clear goals, measures, a deadline,
check-ins, a written record) and apply them informally to *your own* work, through questions.
The PIP is on you, not on them: you get the clarity a formal PIP would give you before anyone
needs one. Managers avoid formal PIPs partly because writing expectations down exposes that
they were never set. Done informally and with empathy, everyone improves. Social engineers use
"elicitation" for drawing information out through what looks like ordinary conversation, and
software engineers use it for gathering requirements. Here, it's both.
*Accuracy note for the stage:* in the US, at-will employment means a PIP usually isn't legally
required to fire someone. Companies use it as documentation in case the firing is challenged,
and rules differ elsewhere.

**27. Managing up is not flattery; it is reducing your manager's uncertainty**
Barnard named four conditions that must all hold before someone accepts an order as
authoritative: they understand it, it fits the organization's purpose, it's compatible with
their interests, and they can actually carry it out. The questions test those conditions:
"What does done look like?" (understanding), "What's driving this?" (purpose), "If I can only do
two of the three, which two?" (ability). A vague order fails the first test before anyone has
done anything wrong. The old line is "when I say jump, you say how high?", and "how high?" is
already a clarifying question; you're just asking the rest. Reinforce good behavior, not the
person: "Having the acceptance criteria up front saved me two days."
- Barnard (1938)

**28. Your manager is a lossy compression layer between you and the org, so control what gets compressed**
The recap gives your manager clean language to report upward. That's what makes it useful to
them, rather than a file kept against them. (Borrowing from Shannon.)
- Shannon (1948); Goffman (1959)

**29. Bad news early is a gift; bad news late is a liability transfer**
The check-in rhythm of elicitation is how bad news travels early: raised as learning, with the
facts in writing.
- Rosen & Tesser (1970)

**30. Translate your work into their units: risk, cost, headcount, and time-to-market**
Aim the questions at what makes your manager look good to their own boss. This works even with
ego-driven managers, because clarity that makes them look good upward is the one thing they
reliably want.
- Aristotle, *Rhetoric*, Book II

**31. Know what your manager is being measured on, or you are optimizing a function you can't see**
"What is your leadership asking you about this?" A manager who was promoted past their skills is
often being measured on things nobody explained to them either.
- Kerr (1975)

**32. Skip-levels, sponsors, and the difference between someone who likes you and someone who will spend capital on you**
These are the exit ramp. Elicitation, like a real PIP, has an end date. It should be longer than
HR's 30/60/90 days, because subtlety takes time, but set it before you start.
*Signs it's working:* they define done before you ask; your recap wording shows up in their
status reports; they start asking their own reports your questions.
*Signs it isn't:* questions meet hostility; recaps get disputed; blame keeps landing on you
despite the record.
When an organization fails its members, they can leave (exit) or try to fix it from inside
(voice); most default to neglect, now called quiet quitting. Elicitation is voice without a
formal channel, and the end date is where voice turns into exit. The next step is a skip-level,
a sponsor, or the door.
- Kram (1985); Hirschman, *Exit, Voice, and Loyalty* (1970) **(new)**

**33. Promotion is a lagging indicator of a story someone else has been telling about you**
This applies to your manager too. The two good outcomes: they adopt the pattern, or the credit
you've given them gets them noticed and moved into a role that fits. Peter & Hull named the bad
versions: "percussive sublimation" (being kicked upstairs) and the "lateral arabesque" (being
moved aside with a longer title). In both, the problem moves without being solved. A move to a
better fit is a fix; a kick upstairs exports your problem to someone else's team.
- Goffman (1959); Peter & Hull (1969) **(new)**

---

## Act VI: Self-Defense

*Status: redefined. Self-defense here is proactive, because no one else is going to do it. HR
exists to protect the company, not you, and a struggling manager can't protect you either. But
the corporate setting still helps: a manager's power comes from the organization's rules
(Weber's legal-rational authority), so those rules also limit it. Punishing someone for asking
what done looks like would need documentation, and the documentation would show a reasonable
question being punished. You ambush the ambiguity before it can be used against you, and the
target is always the situation, never the person.*

**34. The same techniques that make you effective make you a target**
This is the hinge between the two halves of the talk. Elicitation is a social engineering
technique, and once you've learned it, you can spot it being used on you. In D&D, a Deception
check is opposed by Insight. This act is your Insight check.
- Mitnick & Simon (2002)

**35. Urgency, authority, and isolation are the three-ingredient recipe for every manipulation you'll face**
This is the bridge. A struggling manager creates the same three conditions a scammer
manufactures, with no malice at all; their own panic flows downhill.
"I need this today" is urgency → "When do you need it, and what's driving that date?"
"Because leadership wants it" is authority → "What is your leadership actually asking about this?"
"Just get it done, don't pull anyone else in" is isolation → "Who else is involved?" (A single ally breaks the pressure.)
- Cialdini (1984); Milgram (1974); Asch (1951)

**36. Phishing and bad-faith persuasion share a threat model**
Reserved for the minority: managers who aren't struggling but use vagueness and blame on
purpose, often the ego-driven ones. With them, the threat model applies, because they are the
threat. You defend yourself; you don't manipulate back. *Open decision: keep this case or cut it.*
- Cialdini (1984); Mitnick & Simon (2002)

**37. Weaponized vagueness: how ambiguity is used to move accountability onto you**
This is now the problem elicitation solves. Ambiguity lets someone avoid committing and moves
the accountability onto you. A struggling manager may not be doing it on purpose, but the effect
on you is the same, so the defense is the same.
- Eisenberg (1984)

**38. The verbal commitment with no written trace is a durability problem, not a trust problem**
This is the written recap, and it's the shield. A poor manager can't blame you for missing vague,
unmeetable expectations when the record shows what you asked and what was agreed. Drop the
blame, keep the facts: "Timeline moved to the 14th after the scope change" records what happened
without accusing anyone.
- Bartlett (1932)

**39. "I'll get back to you" is a complete sentence and a security control**
Now part of elicitation: the pause between the ask and the recap. It breaks the urgency, buys
time to come back with a plan and the priority question, and keeps the questions from landing
while you're still standing in the doorway.
- Mitnick & Simon (2002)

**40. Spotting the difference between a request and a quota being transferred to you**
The priority question is the defense: "If I can only do two of these three, which two?" Vague
expectations get fixed by clarifying; impossible ones only get fixed by making the manager
choose. Once they've ranked the work in writing, they own the tradeoff.
- Oncken & Wass (1974)

**41. Burnout is often a social-engineering outcome, not a personal failing**
The emotional load is real, but you're already carrying it. That's the reason you're here: the
workplace's social contract isn't being honored. Strain comes from heavy demands combined with
little control, not from demands alone, and elicitation adds control. Name the cost honestly,
too: this is invisible, unpaid emotional labor, which is one more reason for the end date.
- Freudenberger (1974); Karasek (1979) **(new)**; Hochschild, *The Managed Heart* (1983) **(new)**

---

## Act VII: The AI Inflection

*Status: undecided. AI wasn't part of your own description of the topic. Options: shrink it to
a short "why now," or cut it. The security points here depend on whether the bad-faith case
stays.*

**42. AI collapsed the cost of producing competent-looking output to approximately zero**
If kept: a vague request now gets a fast, polished, wrong answer. That makes clarity worth more,
not less.
- Simon (1971); Noy & Zhang (2023)

**43. When everyone can generate the artifact, judgment and trust become the scarce goods**
This connects to reputation: what's scarce is the person whose name on the work means something.
- Simon (1971); Arrow (1972)

**44. Deepfakes and synthetic pretexting broke the heuristics your instincts were trained on**
Depends on the threat model. It shrinks or goes along with the bad-faith case.
- Turing (1950)

**45. The AI-assisted engineer's new job title is "person who vouches for this"**
Survives in any version. It's the reputation this talk is about building: team player, effective
communicator, someone whose word holds.
- Bainbridge (1983)

**46. AI is a persuasion amplifier: it drafts, tailors, and A/B tests the message against you**
Depends on the threat model.
- Weizenbaum (1976); Cialdini (1984)

**47. Verification rituals must now be out-of-band by default**
Survives only as "I'll get back to you," scaled up.
- Mitnick & Simon (2002)

**48. The skills AI cannot commoditize are the ones this talk is about**
Deming found that jobs requiring social skills have grown. Elicitation and peer leadership are
exactly those skills. This is the strongest candidate for a short "why now."
- Deming (2017)

---

## Act VIII: The Build

*Status: holds. The theme now fills in the gaps.*

**49. Your charisma build, speced: three stats to raise and one to respec out of**
Three to raise: Aristotle's components of credibility, which are good sense, good character and
goodwill. The one to respec out of: Deception. Of D&D's four Charisma skills, this build never
takes Deception.
- Aristotle, *Rhetoric*, Book II.1; Antonakis, Fenley & Liechti (2011)

**50. Week one: the smallest experiments that produce visible returns**
Start Monday with one question: "What does done look like?" Send one recap. Then, the next time
someone at the water cooler complains about the boss, share the question. Small wins compound.
- Weick (1984)

**51. The ethical floor: if it only works when they don't know you're doing it, don't do it**
Elicitation passes the test because its success condition is being discovered: the manager
notices the pattern, sees that it works, and adopts it. Clarifying questions pass. Leading
questions designed to make your idea seem like theirs don't. Plato's *Meno* shows both: Socrates
teaches entirely through questions, and he's been criticized ever since for leading. The
ego-driven manager is where the floor gets tested, because manipulation is easiest there, and
the floor still says no. Managing someone's ego is relationship debt that never gets paid down.
- Kant (1795), Appendix II; Plato, *Meno* **(new)**

**52. Leave with this: competence gets you in the room, charisma determines whether the room does anything about it**
Candidate closes:
(a) back to the theme: "In *Fallout*, you can talk the final boss out of the fight. Your boss
fight works the same way."
(b) "When the workplace contract breaks, you have more options than quitting and quiet quitting."
*Open decision.*
- Aristotle, *Rhetoric*, Book I.2; Casciaro & Lobo (2005)

---

## Sources added since the original

None of these are in [`bibliography.md`](bibliography.md) yet.
**Checked** means the citation was confirmed against a publisher, catalog record or the text
itself during discussion. **Recalled** means it still needs that check.

- Peter, Laurence J. & Raymond Hull. *The Peter Principle*. William Morrow, 1969. **Checked** ([archive.org](https://archive.org/details/peterprinciple0000pete))
- Benson, Alan, Danielle Li & Kelly Shue. "Promotions and the Peter Principle." *QJE* 134(4), 2019, 2085–2134. **Checked**
- Kruger, Justin & David Dunning. "Unskilled and Unaware of It." *JPSP* 77(6), 1999. Recalled
- Nuhfer, Edward, et al. "Random Number Simulations Reveal How Random Noise Affects the Measurements and Graphical Portrayals of Self-Assessed Competency." *Numeracy* 9(1), 2016. **Checked**
- Ross, Lee. "The Intuitive Psychologist and His Shortcomings." 1977. Recalled (already in further reading)
- Goffman, Erving. "On Face-Work." *Psychiatry* 18(3), 1955, 213–231. **Checked**
- Allspaw, John. "Blameless PostMortems and a Just Culture." Etsy Code as Craft, May 2012. **Checked**
- Plato. *Meno*, trans. Benjamin Jowett. **Checked** ([Gutenberg #1643](https://www.gutenberg.org/ebooks/1643))
- Kipnis, David, Stuart M. Schmidt & Ian Wilkinson. "Intraorganizational Influence Tactics." *JAP* 65(4), 1980, 440–452. **Checked**
- Kipnis, David & Stuart M. Schmidt. "Upward-Influence Styles." *ASQ* 33(4), 1988, 528–542. **Checked**
- Karasek, Robert A. "Job Demands, Job Decision Latitude, and Mental Strain." *ASQ* 24, 1979, 285–308. **Checked**
- Robinson, Sandra L. & Denise M. Rousseau. "Violating the Psychological Contract: Not the Exception but the Norm." *Journal of Organizational Behavior* 15(3), 1994, 245–259. **Checked**
- Hirschman, Albert O. *Exit, Voice, and Loyalty*. Harvard University Press, 1970. **Checked** ([archive.org](https://archive.org/details/exitvoiceloyalty0000hirs))
- Hochschild, Arlie Russell. *The Managed Heart*. University of California Press, 1983. Recalled
- Locke, John. *Second Treatise of Government*. 1689. Recalled
- La Boétie, Étienne de. *Discourse on Voluntary Servitude*. Written c. 1550. Recalled
- Grant, Adam. *Give and Take*. Viking, 2013. Recalled (already in further reading)

## Open decisions

1. **Act VII:** shrink it to a short "why now," or cut it.
2. **The bad-faith manager case** (phishing and bad-faith persuasion share a threat model): keep it or cut it.
3. **The close:** the *Fallout* boss fight, or "more options than quitting and quiet quitting."
4. **The word "ambush":** keep it as is, or use "ambush the ambiguity" so it stays aimed at the situation rather than the person.
