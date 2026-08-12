---
title: "Gödel Machines: Self-Referential Universal Problem Solvers Making Provably Optimal Self-Improvements"
type: source
authors: Jürgen Schmidhuber
arxiv: cs/0309048
venue: "arXiv preprint, v1 25 Sep 2003; this summary cites v5 (last revised 17 Dec 2006, TR IDSIA-19-03); a same-title condensed chapter later appeared in Goertzel & Pennachin (eds.), Artificial General Intelligence, Springer, 2007"
source: ../../raw/papers/goedel-machines.pdf
updated: 2026-08-06
---
# Gödel machines — summary

## What it is

A Gödel machine is a formally specified agent that interacts with an environment under a fully
axiomatized utility function, and that **rewrites any part of its own code — including the proof
searcher that decides on rewrites — the moment, and only the moment, it has constructed a formal
proof that the rewrite raises expected utility** under its own axioms
([`raw/papers/goedel-machines.pdf`](../../raw/papers/goedel-machines.pdf), Abstract, p.1). It is not a
trained or evolved system: there is no population, no benchmark, no empirical trial. The entire
argument for why this produces good self-modifications is a theorem, not a measurement — the paper's
central claim is that a rewrite accepted this way is **globally optimal**, not merely locally better
than what came before, because the proof that justifies switching implicitly certifies the switch is
also better than every alternative self-rewrite the machine's own search could still find later
(Theorem 4.1, p.11). This is the paper the Darwin Gödel Machine (already in this wiki,
[`darwin-godel-machine.md`](darwin-godel-machine.md)) is named after and explicitly descends from.

## The mechanism: proof searcher, switchprog, and the Global Optimality Theorem

**Setup.** The machine's entire life is a sequence of discrete cycles acting on a single mutable
state string `s`, of which `x` (inputs), `y` (outputs), `time`, and `p` (the current program) are
named substrings (§2.1, p.3). `p(1)`, the initial software, bundles two things: `e(1)`, an ordinary
(and presumably suboptimal) policy for interacting with the environment, and a **proof searcher**
subroutine that runs concurrently (§2.2, p.4).

**Proof techniques and the axiomatic system A.** The proof searcher systematically tests **proof
techniques** — programs, written in a Forth/Prolog-like universal language `L`, that read parts of
`s` and emit theorems — using an online extension of Levin's Universal Search (§3.1, p.6). Every
theorem must be derived from an enumerable axiom scheme `A`, encoded in `p(1)` itself, with six
components the paper spells out concretely (§3.2 Item 1, pp.7–10): **(a)** hardware axioms
(how any instruction changes `s` from one cycle to the next — the paper works a real example for a
64-bit instruction pointer), **(b)** reward axioms (computational/physical costs and how inputs
translate into reward), **(c)** environment axioms (what, if anything, is assumed about the
distribution generating future inputs — e.g. computable, limit-computable, or Markovian), **(d)**
uncertainty/string-manipulation axioms (standard probability theory, needed to reason about
*expected* future utility), **(e)** initial-state axioms (how to reconstruct `s(1)`), and **(f)**
utility axioms — the formal utility function `u` itself, typically expected discounted future reward
(eq. 1, p.3–4).

**switchprog, target theorems, and check().** A proof technique may call `set-switchprog(m,n)` to
propose a candidate rewrite of `p` (`switchprog`), and `check()` to test whether the proof-in-progress
has become a **target theorem** — a symbolic statement of the exact form
`u[s(t1) ⊕ switchbit=1, Env] > u[s(t1) ⊕ switchbit=0, Env]` (eq. 2, p.9), i.e. "switching to
`switchprog` at time `t1` yields strictly higher utility than continuing to run unmodified `p`,
which would keep searching." The moment such a proof is found, `check()` flips `switchbit` and
transfers control to `switchprog`, which "may subsequently rewrite all parts of `s` … including `p`"
(§3.2 Item 5, p.11) — the proof searcher itself is not exempt.

**Why this is globally, not just locally, optimal.** Theorem 4.1 (p.11) is the paper's core result:
*"the utility of starting the execution of the present switchprog is higher than the utility of
waiting for the proof searcher to produce an alternative switchprog later."* The proof is almost a
one-liner once the target-theorem framing is seen clearly: the binary choice `check()` proves a fact
about is exactly *"execute now" vs. "keep the unmodified searcher running, which will consider all
(possibly infinitely many) future switchprogs"* — so a proof of the former beating the latter is, by
construction, a proof that beats every alternative the *unmodified* system could ever find (p.11–12).
Section 4.3 (p.12) draws out a striking corollary: because the target theorem being proved already
quantifies over all the machine's own future self-modifications, *"any proof of a target theorem
automatically proves that the corresponding self-modification is good for all further
self-modifications affected by the present one, in recursive fashion. In that sense all possible
'meta-levels' of the self-referential system are collapsed into one."* The paper also gives a relaxed
variant (target theorem 3, using `≥` instead of `>`, §4.2, p.12) and notes the same optimality
argument survives.

**The searcher is itself provably efficient, not just correct.** Section 5's Bias-Optimal Proof
Search (BIOPS) is a second, independent contribution: an online variant of Universal Search that is
proved *O()-optimal* — Theorem 5.1 (p.14) shows it needs at most `O(f(k))` steps whenever some
unknown proof technique could find a difficulty-`k` proof in `f(k)` steps, with no problem-dependent
constant hidden in the exponent the way brute-force provers (Hutter's HSEARCH, AIXI(t,l)) suffer from
(§6.4, p.19–20). Because the searcher is itself just more code in `p(1)`, its own proof techniques can
reason about *it*, so later self-rewrites can beat even O()-optimality once something better is
provably found (§2.3, p.4–5; §5.1, p.14).

## What the paper itself concedes it cannot do

The paper is explicit, in its own words, about two formal limits, both traced directly to Gödel's own
1931 incompleteness results (§2.4, p.5): *"Any formal system that encompasses arithmetics (or ZFC etc)
is either flawed or allows for unprovable but true statements. Hence even a Gödel machine with
unlimited computational resources must ignore those self-improvements whose effectiveness it cannot
prove … In particular, one can construct pathological examples of environments and utility functions
that make it impossible for the machine to ever prove a target theorem."* Section 4.4 (p.12–13)
extends this with Rice's theorem — *"any nontrivial property over general functions is undecidable"*
— conceding that under Rice's extreme notion of triviality *"only trivial improvements of a given
strategy may be provably useful,"* though the paper argues this notion of triviality is narrower than
what scientists intuitively mean by trivial. Concretely, this means the proof searcher can spend
unbounded time (in the worst case, forever, without ever halting on a target theorem) on an
environment/utility pair whose usefulness happens to be undecidable, and the machine has no way to
know in advance which pairs those are (§4.4, p.13; FAQ item 8, p.23).

> [!inferred] It is worth being precise about what the paper does **not** concede, because this is
> exactly where the Darwin Gödel Machine paper later pushes back. Schmidhuber's own FAQ section is
> notably confident that formalizing real-world utility and uncertainty is *not* a fundamental
> obstacle — "we just need to insert into `p(1)` the standard axioms for representing uncertainty…
> the machine learning literature is full of human-generated proofs of properties of methods for
> dealing with stochastic environments" (FAQ Q1, p.22) and "formal descriptions of non-computable
> objects do not at all present a fundamental problem" (FAQ Q4, p.23–24). The paper's acknowledged
> limitations are the Gödel/Rice-style **undecidability** ones above; the *practical* difficulty of
> actually writing down a real-world `u` and `A` rich enough to prove anything useful about, in a
> bounded amount of engineering effort, is not a concern the 2003/2006 paper itself dwells on — it is
> the concern the DGM paper raises against it fourteen years later (see below).

## Comparison to the Darwin Gödel Machine: what's kept, what's discarded

This is the single most important cross-reference for this page. The DGM paper
([`darwin-godel-machine.md`](darwin-godel-machine.md)) names itself directly after this one and states
its relationship explicitly: it keeps the Gödel machine's *self-referential core* but discards the
*provability requirement*, replacing it with empirical benchmark validation
([`raw/papers/darwin-godel-machine.pdf`](../../raw/papers/darwin-godel-machine.pdf), p.4) —
*"in practice, without restrictive assumptions … it is impossible to formally prove whether a
modification … will be beneficial."*

**What is kept: self-reference in the strict sense this paper defines it.** In both systems, the code
being edited is drawn from the same substrate as the code doing the editing. Here, `switchprog` — set
by the proof searcher, itself part of `p` — "may subsequently rewrite all parts of `s` … including
`p`" (§3.2 Item 5, p.11), so a self-rewrite can touch the very proof searcher that produced it. DGM's
coding agent is likewise built by evolving the same repository it is asked to edit: its
`self_improve_step` builds a container from *the parent agent's own code* and runs that same generic
agent against a problem statement pointing at that code
([`self-referential-code-rewriting.md`](../concepts/self-referential-code-rewriting.md)). Both papers
treat this as the defining, load-bearing property — not incremental parameter tuning, but the editor
and the edited sharing one identity.

**What is discarded: the proof requirement, and everything downstream of it.** This paper's whole
argument for *optimality* — Theorem 4.1 — is a deductive proof that a given `switchprog` beats every
alternative the unmodified searcher could ever find, contingent on the axiomatized `u` and `A` being
sound and rich enough to support that proof (§4.1, p.11; §4.4, p.12–13). DGM has no analogue of `u`,
`A`, target theorems, or `check()`: instead of *proving* a rewrite is beneficial, it *measures* one —
running the child agent on a coding-benchmark subset and keeping it only if the score improves
(archive-based, not proof-based, acceptance). That single substitution cascades:

- **Optimality guarantee → gone.** Theorem 4.1's "no local maxima" argument depends on the target
  theorem quantifying over *all* future switchprogs the unmodified searcher would ever consider
  (p.11–12). A benchmark score carries no such quantification — DGM's archive explicitly documents
  runs where a locally weaker child later unlocks a much stronger descendant (DGM paper, "stepping
  stones," p.4–5, Fig. 3) — i.e. DGM's search is knowingly *not* globally optimal in this paper's
  sense, and does not claim to be.
- **Meta-level collapse → gone.** §4.3 (p.12) shows a proven target theorem is automatically a proof
  that the change is good for *every* future self-modification it enables, recursively. DGM has no
  such transitive guarantee: each generation's benchmark score says nothing formally about whether the
  *next* generation's self-modification, built on top of it, will also be good — it is re-measured
  from scratch every time.
- **Formal `u`/`A` → an evaluation harness.** This paper's axioms (a)–(f) must be rich enough to prove
  facts about hardware, environment, and reward before anything can happen at all (§3.2, pp.7–10). DGM
  needs none of that machinery — only a benchmark and a scoring function — which is exactly the
  practical unlock that makes it a *running system* rather than a specification of one.
- **Scope of self-rewrite.** This paper's `switchprog` may rewrite essentially anything, including the
  axioms, the utility function itself (provided the new one is provably better under the *old* one —
  §6.1 item 4, p.16), or even the hardware (§6.1 item 8, p.16). DGM's self-modification scope is
  narrower and hand-drawn: the agent may edit its own tools/prompts/orchestration, but the
  archive/parent-selection loop that decides keep-vs-discard is fixed and human-owned, explicitly
  outside the agent's own edit scope
  ([`self-referential-code-rewriting.md`](../concepts/self-referential-code-rewriting.md)) — a much
  more circumscribed notion of "self" than this paper's `p`, which has no such carve-out in principle.

> [!inferred] Put in one line for cross-reference elsewhere in this wiki: the Gödel machine proves a
> rewrite is *globally* optimal before ever running it; the Darwin Gödel Machine runs a rewrite and
> *locally* keeps it if a benchmark says so. Both call the resulting property "self-referential" in
> exactly the same technical sense — same target, opposite direction of travel (deduction-first vs.
> execution-first) — and DGM's paper is explicit that it made this substitution because the proof
> requirement is not a design choice this paper leaves open; §2.4/§4.4 above are, in DGM's reading, why
> a literal Gödel machine cannot be built for a domain as informally specified as "write good code."

## Where this sits relative to this wiki's meta-evolution ladder

[`meta-evolution.md`](../concepts/meta-evolution.md) organizes this wiki's self-improving systems on a
four-rung ladder — Evolution → Self-evolution → Meta-evolution → Recursive Self-Improvement (RSI) —
where each rung is defined by *where the improvement is stored* (population, search state, model
weights, "everything, recursively") and is explicitly an **empirical**, execution-driven ladder: every
rung below RSI is characterized by a system that runs candidates and measures outcomes.

The Gödel machine does not belong on this ladder as one more rung, and forcing it onto one would
misrepresent both. It has no population (rung 1), no search-state archive that accumulates execution
experience (rung 2), and no trained model whose weights absorb outcomes (rung 3) — there is exactly
one running program `p` at a time, and it changes only on a proof, never on an observation of how well
a candidate performed. What it *does* share with the ladder's top rung is the **ambition**: rung 4 is
defined on that page as "each upgraded system further improves the process that produces its
successors" — and Section 4.3's meta-level collapse (p.12) is a formal proof of exactly that property,
for a Gödel machine, under the assumption that its axioms are sound and sufficient. In that narrow
sense this paper is not rung-4-*empirical* but rung-4-*adjacent in claim*: it is the only thing in this
wiki that formally proves the RSI property rather than gesturing at it or measuring a proxy for it —
and it buys that proof at the cost of requiring a fully specified formal world (§3.2's axioms a–f)
that no paper in this wiki's empirical lineage (including DGM) has been willing or able to write down
for a real task.

> [!inferred] A useful way to hold both facts at once: this paper is the **theoretical ceiling** the
> ladder's rung 4 gestures toward (formally guaranteed, recursively self-improving optimality), and
> every empirical system on the ladder — including DGM, which is named after it — is a *different
> route up*, trading the guarantee for a running system. The ladder measures "how much of RSI has been
> empirically demonstrated"; this paper answers a different question, "what would it take to *prove*
> RSI," and its own limitations section (§2.4, §4.4) is effectively an argument for why no rung of the
> empirical ladder can expect to inherit that proof for free.

## Where this fits in the wiki

This page grounds the theoretical half of
[`self-referential-code-rewriting`](../concepts/self-referential-code-rewriting.md), whose "Origin"
section previously cited this paper without a dedicated source page. See
[`../sources/darwin-godel-machine.md`](darwin-godel-machine.md) for the direct empirical descendant and
[`../concepts/meta-evolution.md`](../concepts/meta-evolution.md) for the ladder this paper's ambition
sits adjacent to but does not climb the same way.
