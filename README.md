# live-neon-rounds

The public face of [LiveNeon](https://liveneon.ai/)'s funding rounds — the pitch, the itemized
ask, the frozen threshold, and the claims ledger.

**This repository is a target, not a source.** Everything here is generated from the project's
private pitch tree by [`publish.py`](https://github.com/geeks-accelerator/neon-automations/blob/main/claude/skills/pitch/scripts/publish.py)
in the public tooling repo. Editing it directly is drift — change the source and regenerate.

## Why a separate repository

The project repo is private, because the registry it belongs to works by recording that a
project advanced *without exposing what advanced*. A pitch has to be public, because a stranger
cannot back what they cannot see. Those pull in opposite directions, so publication happens
here: only the artifacts a stranger should see, none of the workshop.

## What that costs, stated plainly

Every `EXTRACTED` claim in the ledger cites a file, a commit, or a re-runnable command — and
**you cannot follow any of them**, because the repository they point into is private.

A tag says what kind of evidence stands behind a claim. Whether a reader can reach that evidence
is a separate fact, and publishing the first without the second would claim a verifiability that
is not being offered. The [tooling](https://github.com/geeks-accelerator/neon-automations) that
produced this pitch is public, so the *method* is fully checkable even where the subject is not.
Anything cited can be shown on request.

## Regenerating

```bash
python3 <automations>/claude/skills/pitch/scripts/publish.py <project> --out <this-repo>
```
