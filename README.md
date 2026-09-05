# ozar

**ozar** is a local agent with a different kind of mind. Where today's coding and research agents (Claude Code, Codex, Gemini CLI, Qwen CLI) run a language model behind a tool loop, ozar runs an **organism**: a gradient-free linguistic core that reads a corpus once, **buys its laws** from what the corpus shows (a law needs a quorum of distinct shows, never a single example), and then answers only what it can **certify** — every answer carries its derivation, every silence carries its named reason. No weights, no sampling, no telemetry, no network: one binary and one crystal on your machine.

That is the claim we are building toward: an agent that researches, programs, executes and keeps learning on your own corpus, whose every step you can read and whose refusals are honest. Today the core is young. The releases here are the honest state of that core, measured on a held-out key the corpus never showed, and they will grow point by point.

## What ozar does today

- **Grounded question answering** on the GENESIS crystal: arithmetic, word problems, comparisons, verdict questions, definitions, why-questions — in the languages the corpus shows (English fully; eight more languages partially, growing with the frame markets).
- **A glass box.** `ozar ask "…" --why` prints the derivation: the facts read, the relation executed, the law each step rests on. When it cannot answer, it says why: which sentence it could not read, which road declined.
- **A cabin** (`ozar`): a terminal workspace with the transcript, the derivation tree, the organism's life signs, `/why`, `/self`, `/teach`, `/learn`.
- **Reading pages** (`ozar read <file> "question?"`): a page of prose becomes a corpus slice the organism answers from.
- **The doctor** (`ozar doctor`): the installation checked whole — binaries, crystal, schema, canon permissions.

## What is coming (the roadmap the releases follow)

1. **One carrier for stories in nine languages** — story frames bought by anti-unification, question frames bought by the executor that reproduces the shown answer; stories stop being an English-only road.
2. **Acts with a ledger** — tools (files, shell, http, git, build/test) as certified acts: a plan you can read, a cost you can see, a refusal by name.
3. **Continuous learning without forgetting** — every session is a corpus; laws are only added, courts remove; the held-out key is the honest measure.
4. **Identity** — a self-model read from the ledger of purchased laws, not from a prompt; slow personality variables with provenance.

## Install

1. Download the archive for your platform from the latest release and unpack `ozar` and `ozar-core` into a directory on your `PATH` (macOS arm64/x86_64, Linux x86_64/aarch64, Windows x86_64).
2. Download the crystal `GENESIS-<sha8>.crystal` into `~/.ozar/canon/`; `ozar canon use GENESIS-<sha8>` selects it.
3. `ozar doctor`, then:

```
ozar ask "Ann had 19 apples. Ann gave away 4 apples. how many apples does Ann have now?" --why
ozar
```

## How releases are cut

A release is cut only when the organism improves on the **held-out key** (questions the corpus never showed, nine languages, three depths): more right answers, no more wrong ones. Every release note states the crystal's signature, the key's signature and the counts — right, wrong, silent. A wrong answer costs more than a silence; the organism is scored so. Verify archives against `SHA256SUMS`.

## License

Proprietary. The binaries and the crystal are provided for use as released; reverse engineering, decompilation and redistribution of derived works are not permitted. See LICENSE.
