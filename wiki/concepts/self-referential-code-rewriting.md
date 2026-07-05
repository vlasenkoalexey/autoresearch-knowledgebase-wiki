# Self-referential code rewriting

**Self-referential code rewriting** describes a system whose self-modification target is the very code that
constitutes its own problem-solving apparatus — its tools, prompts, and control/orchestration logic — such
that a successful edit also improves the system's own ability to make its *next* edit. This is distinct from
a system that merely tunes external parameters or a downstream artifact: the thing being changed is the thing
doing the changing.

## Origin: the theoretical Gödel machine

The term traces to Schmidhuber's 2007 **Gödel machine**, which required a *formal proof* that a candidate
self-rewrite would be beneficial before adopting it — a requirement the Darwin Gödel Machine paper notes is
practically impossible to satisfy without highly restrictive assumptions.

## In this wiki's papers

- [**Darwin Gödel Machine**](../sources/darwin-godel-machine.md) keeps the Gödel machine's self-referential
  core but relaxes "provably beneficial" to "empirically validated on a benchmark." Concretely, its base
  agent is a frozen foundation model wired to two tools (`bash`, whole-file view/edit) plus one prompt; the
  self-modification scope is narrowly defined as editing the agent's *own* component files (the edit tool,
  the bash tool, the `forward()` orchestration, the prompts) — explicitly excluding the archive/parent-
  selection machinery itself, which stays fixed and human-owned in this version of DGM (flagged as future
  work to make self-referential too). Across an 80-iteration SWE-bench run this self-referential loop
  discovered, among other changes, a unique-match `str_replace` edit command and a multi-candidate-patch-
  plus-ranking workflow — improvements to the agent's own editing apparatus made *by* that same apparatus.
- [**Bilevel Autoresearch**](../sources/bilevel-autoresearch.md) is a useful *contrastive* case: its outer
  "Level 2" reads and rewrites the inner autoresearch loop's search-mechanism code at runtime — a genuine
  self-modification — but it is not self-referential in DGM's sense. The thing doing the rewriting (Level
  2's 4-round Explore→Critique→Specify→Generate dialogue, and Level 1.5's freeze/unfreeze rules above it)
  is fixed and human-authored throughout the paper's experiments; only Level 1 is rewritten, never Level 2
  itself. The authors name this gap directly: "if a discovered mechanism reliably improves Level 1, the same
  mechanism-discovery principle can in principle be applied to Level 2 itself," but demonstrating that
  recursive bootstrapping is left as explicit future work, not a result of this paper. So where DGM's
  editor and edited are the same code from iteration one, Bilevel Autoresearch currently has a strict,
  un-rewritten level *above* the level being rewritten — one bilevel step, not (yet) an open recursion. See
  [`mechanism-level-self-improvement`](mechanism-level-self-improvement.md) for the more general concept
  this instantiates.

> [!inferred] `autoresearch`'s ratchet ([`../code/autoresearch/overview.md`](../code/autoresearch/overview.md))
> is explicitly **not** self-referential in this sense: the agent may edit `train.py`, but the ratchet logic
> deciding keep-vs-discard (`program.md`) and the frozen evaluation substrate (`prepare.py`) are authored and
> owned by the human, not by the agent, and are not themselves in the agent's edit scope. DGM collapses that
> distinction — the evolving artifact and the evolving mechanism are the same code.

## See also
- [`evolutionary-self-improvement`](evolutionary-self-improvement.md)
- [`../sources/darwin-godel-machine.md`](../sources/darwin-godel-machine.md)
