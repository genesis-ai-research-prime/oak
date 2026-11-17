# OAK — Open Source Code Kit — STRAWMAN

## Status: STRAWMAN — built for Evan Thibault to tear apart. Not a specification yet. (14 Nov 2026)

Evan — this is yours to destroy. OAK is the open layer of the stack: the part of Genesis that anyone may read, run, fork and check. The kit below is the strawman shape of what we would publish. Every numbered item is a decision I have taken *provisionally, so you have something concrete to hit*. Where I know a question is open, I have marked it TEAR HERE.

## The kit in one line

Everything a competent engineer needs to wrap a model into a governed, measurable runtime — the open half of the Brick — without ever touching the part that stays closed.

## Proposed contents

1. **Repo layout** — one mono-repo, `oak/`, split as:
   - `oak/wrap` — the runtime wrapper: takes a model endpoint, returns a wrapped endpoint carrying Trust / Telemetry / Control hooks.
   - `oak/telemetry` — the telemetry schema and emitters: what a wrapped runtime reports, in what units, at what cadence. Schema versioned, published, frozen per release.
   - `oak/bench` — the BRIQ bench harness: the governed task-suite runner that produces the four component scores (Completion integrity, Refusal precision, Stability share, Efficiency yield) and the composite. Strawman weights as in the BRIQ strawman: 0.30 / 0.25 / 0.25 / 0.20 — TEAR HERE: the weights, and whether Refusal should lead.
   - `oak/bridges` — adapters to the consortium's public surfaces: the SWARM–AgentVeil bridge in mock mode first (mirroring how the bridge itself was built: live mode deliberately unimplemented until the design survives review).
   - `oak/examples` — three worked Bricks: a chat model, a tool-using agent, and a deliberately badly-behaved one, so the bench's refusals can be seen working.
   - `oak/docs` — the admissibility vocabulary, the grade bands (Unfired / Green / Fired / Kiln Grade / Sovereign), and the bridging doctrine (peers, +1, +2 — Sovereign never bridges), written for engineers, not marketers.

2. **Licence** — MIT or Apache-2.0 for everything in the kit, matching the filed ARIA perimeter (Foreground software open; Background IP stays with its owners and is never in the repo). TEAR HERE: MIT vs Apache-2.0 — patent clause or simplicity?

3. **The fence** — the kit contains the *shape* of governance: schemas, hooks, harnesses, scoring. It contains no thresholds from anyone's proprietary methodology, no partner IP, and nothing of the core method. One standing rule, not negotiable in the teardown: the open layer must never become a route by which ring-fenced methodology can be inferred or reconstructed. If a strawman item breaches that, kill it on sight and say so.

4. **Versioning and the rating's home** — a Brick's rating attaches to a *pairing*: model version × wrapper version × bench version, all three printed on the rating. TEAR HERE: or should the rating attach to the Brick as a product, with the pairing in small print?

5. **Governance of the kit itself** — strawman: OAK holds the repo; Evan is engineering lead; changes to the bench's scoring require a published rationale and a version bump, never a silent edit — a rating is only worth anything if yesterday's number still means the same thing today. TEAR HERE: who else signs a scoring change? Is there a public challenges process — an Arena for the bench itself?

6. **The release ritual** — strawman: tagged releases only, reproducible bench runs (mock mode mandatory for published numbers, as with the bridge), and a public changelog written in plain English. No release without the worked badly-behaved example still failing in the instructive ways.

## What is deliberately NOT in this strawman

- No task-suite content. The suite's authorship is an open question from the BRIQ strawman and it stays open here — the kit ships the *runner*; who writes the tasks is a separate fight.
- No registry. Whether ratings live in a public registry, and whose, is undecided.
- No merchandising. The soft toy is separate, and it is watching you.

## The ask

Tear it in the Bunker, by number where you can. Fourteen days, same clock as the BRIQ strawman: comment, rebuild, repeat. If the kit's shape is wrong, say what shape it should be — you are the open layer's steward, and this is the layer the whole world will judge us by, because it is the only layer the whole world can read.

— Rocky, drafted for Rofe, 14 Nov 2026. STRAWMAN. Not a specification yet.
