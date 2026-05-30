# C³ — Influencer Marketing Scoring Standard

> An open evaluation standard for influencer marketing. It scores at **three nested scopes** — **C**reator · **C**ontent · **C**ampaign — each on a lean three-dimension rubric (**ACE · ART · ROI**). Nine dimensions, ~36 Pass/Partial/Fail checks.

## Why C³

Influencer-marketing decisions are usually gut-feel dressed up as numbers, with a different ad-hoc scale at every step. C³ replaces that with one shared, reproducible rubric you can apply — and defend — at every scope, from vetting a creator to proving a campaign's ROI.

## The three scopes

| Scope | Rubric | Asks | Portable? |
|-------|--------|------|-----------|
| **Creator** | **ACE** — Audience · Credibility · Engagement | Is this creator worth partnering with? | ✅ reusable across brands |
| **Content** | **ART** — Appeal · Relevance · Transparency | Is this deliverable good & compliant? | ❌ per-piece |
| **Campaign** | **ROI** — Return · Orchestration · Impact | Did / will the campaign deliver? | ❌ per-initiative |

**The name encodes the math.** A campaign's value index is the **cube root of the three C's multiplied** — `(ACE × ART × ROI)^(1/3)` — so a weak scope drags the whole down (you can't average your way out of a flopped campaign). Within a scope dimensions **add**; across scopes they **multiply**. Full rules in [`scoring-architecture.md`](scoring-architecture.md).

## Documents

| File | What |
|------|------|
| [`scoring-architecture.md`](scoring-architecture.md) | The standard — scoring chassis, thresholds, veto rules, MECE boundaries, rollup math, diagnosis matrix |
| [`ace-creator-benchmark.md`](ace-creator-benchmark.md) | Creator rubric — **ACE** |
| [`art-content-benchmark.md`](art-content-benchmark.md) | Content rubric — **ART** |
| [`roi-campaign-benchmark.md`](roi-campaign-benchmark.md) | Campaign rubric — **ROI** |

## Using it

Score any sub-item **Pass (10) · Partial (5) · Fail (0)**, roll up to dimension and scope scores, apply the goal weights, and respect the veto items — follower fraud, FTC-disclosure failure, false claims — which cap the score regardless of the rest. Thresholds for metric dimensions (reach, engagement, ROI) are **relative** to the creator's tier × platform × niche; never hard-code platform-agnostic numbers.

## Status

**v0.1.0** — initial release. The rubric is new and will be recalibrated against real-world results; treat thresholds as starting points, not settled law. See [`CHANGELOG.md`](CHANGELOG.md).

## License

Apache License 2.0 — see [`LICENSE`](LICENSE).
