# ozar

**ozar** is a local organism that answers what it can ground. It reads a corpus once, buys its laws from what the corpus shows, and then answers questions with a derivation you can read (`ozar ask "…" --why`) — or refuses, by name, when it cannot certify an answer. No network, no model weights, no telemetry: one binary, one crystal.

This repository holds **releases only**: binaries for macOS (Apple Silicon, Intel), Linux (x86_64, aarch64) and Windows (x86_64), and the **GENESIS crystal** (the forged state the binaries answer from). The source is closed.

## Install

1. Download the archive for your platform from the latest release and unpack `ozar` and `ozar-core` into a directory on your `PATH`.
2. Download the crystal `GENESIS-<sha8>.crystal` and place it under `~/.ozar/canon/` (`ozar canon use GENESIS-<sha8>` selects it; `ozar doctor` tells you if anything is missing).
3. Ask:

```
ozar ask "Ann had 19 apples. Ann gave away 4 apples. how many apples does Ann have now?" --why
ozar            # the cabin: type a question, Enter; /why, /self, /help
ozar doctor     # is the installation whole
```

## What a release is

A release is cut only when the organism measurably improves on the **held-out key** — questions the corpus never showed (nine languages, three depths). Every release note states the key's signature, the crystal's signature, and the counts: right, wrong, silent. A wrong answer costs more than a silence; the organism is scored so.

## Checksums

Every archive is listed in `SHA256SUMS`. Verify before you run.

## License

Proprietary. The binaries and the crystal are provided for use as released; reverse engineering, decompilation and redistribution of derived works are not permitted. See LICENSE.
