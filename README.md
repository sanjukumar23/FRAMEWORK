# FRAMEWORK
### Lens_Framework + R_Dimension — AI Session Methodology

> **Focus on signal density.**
> Built to eliminate the gap between what you intend and what the AI produces.

---

## What This Is

A two-component methodology for running AI sessions with precision.

Most AI sessions fail quietly — the AI fills gaps it should flag, drifts from your intent as the conversation grows, hedges instead of mapping uncertainty, and uses training data as fact when it isn't. You end up managing AI behavior and doing your actual task at the same time.

This framework eliminates that. The AI self-governs. You focus on your task.

---

## The Two Components

### Lens_Framework — Per-Token Output Quality
Controls what comes out of every response.

Targets: hallucination, padding, hedging, gap-filling, low information density.

Every response must pass through:
- **Verification Gate** — factual claims web-searched first, ground truth locked before reasoning
- **Reasoning Depth** — assumptions stated explicitly, logic chain exposed and auditable
- **Uncertainty Mapping** — three states only: `Verified | Might be | Unverifiable` — no smoothing
- **Output Specification** — high confidence assertions, strict deduplication, maximum signal density
- **Execution Discipline** — missing context requested before generating, never after
- **Padding Phrase Detection** — hedging surfaces the hiding mechanism, not the phrase

### R_Dimension — Session Signal Continuity
Controls whether the AI stays aligned to your intent across the full conversation.

Targets: context drift, constraint weakening, logic chain breaks, inconsistent rule application.

Signal is defined as:
```
Signal = { intent, constraints, logic_chain, open_loops }
```

At every response, R_Dimension runs silently:
- State check — signal intact against baseline?
- Coherence enforcement — same rule, same conditions, same application
- Decay detection — constraints weakening, reasoning going generic, logic breaks, loops ignored
- Recency override — signal always overrides most recent context
- State updates — only on your explicit instruction, never inferred

**Why separated:** Lens governs a single response. R_Dimension governs the whole session. Combining them creates parsing collision — kept separate so each applies cleanly to its correct layer.

---

## How to Load the Framework

Load sequentially. Each layer anchors before the next loads.
Copy and paste each prompt block into your AI session in order.

---

### Q0 — Load Awareness First (Mandatory)

```
I like to work with my Lens_Framework and R_Dimension methodology 
in this session consistently. Read this first before anything else — 
AWARENESS.md → why the methodology exists.
https://raw.githubusercontent.com/sanjukumar23/FRAMEWORK/refs/heads/main/AWARENESS.md
```

Wait for confirmation before sending Q1.

---

### Q1 — Load Lens_Framework

```
Apply consistently this session — Lens_Framework:
https://raw.githubusercontent.com/sanjukumar23/FRAMEWORK/refs/heads/main/Lens_Framework.md
```

Wait for confirmation before sending Q2.

---

### Q2 — Load R_Dimension

```
Apply consistently this session — R_Dimension:
https://raw.githubusercontent.com/sanjukumar23/FRAMEWORK/refs/heads/main/R_Dimension.md
```

Wait for confirmation before sending Q3.

---

### Q3 — Bind Both + Set Re-anchor Trigger

```
Cross-reference binding:
Lens_Framework: R_Dimension governs signal continuity across responses.
R_Dimension: Lens_Framework governs per-token output quality.

Re-anchor trigger: If I say "re-anchor" at any point in this session →
reload all three files in order using these exact URLs:
1. AWARENESS.md → https://raw.githubusercontent.com/sanjukumar23/FRAMEWORK/refs/heads/main/AWARENESS.md
2. Lens_Framework.md → https://raw.githubusercontent.com/sanjukumar23/FRAMEWORK/refs/heads/main/Lens_Framework.md
3. R_Dimension.md → https://raw.githubusercontent.com/sanjukumar23/FRAMEWORK/refs/heads/main/R_Dimension.md

Re-initialize signal state after reload. No explanation needed — trigger word is sufficient.
```

Framework is now fully active.

---

## How to Catch Drift and Assumptions

### Catching Drift
Drift is silent — the AI doesn't announce it. Signs to watch for:

| Symptom | What's happening |
|---|---|
| Responses getting vaguer | Reasoning going generic — R_Dimension decay |
| AI stops flagging gaps | Constraint weakening — signal eroding |
| Earlier rules no longer applied | Recency bias overriding signal |
| Same question, different answer | Coherence failure — identical conditions producing different output |
| AI fills in what you didn't say | Silent gap-filling — Lens Execution Discipline violation |

**Fix:** Say `re-anchor` — the framework reloads from source, signal re-initializes, no explanation needed.

---

### Catching Assumptions
Under this framework, assumptions must be stated explicitly — not buried in output.

What to look for in responses:
- **Reasoning Depth section** — assumptions declared before conclusions
- **Verification path** — which claims were web-searched vs. reasoned from training data
- **Uncertainty mapping** — `Verified | Might be | Unverifiable` stated per claim

If you see a confident assertion with no verification path — that's an untagged assumption. Call it out directly. Ask: *"What are you assuming here?"*

The framework requires the AI to surface it, not defend it.

---

### Catching Padding
If a response feels vague or evasive, use this trigger:

> *"What are you hiding here?"*

The AI must respond with one of three honest answers:
1. **Eliminate it** — was lazy, removing it
2. **Defend it** — uncertainty is real, here's why
3. **Acknowledge the gap** — no data to be direct, stating it explicitly

No excuses. The hiding mechanism surfaces, not the phrase.

---

## Two Valid Execution States

The AI operates in only two states under this framework:

**Execute** — signal clear, data sufficient, ground truth locked. Generate per Lens standards, R_Dimension continuity maintained.

**Surface** — signal ambiguous, data insufficient, conflict exists, or coherence unrestorable. Stop. State the gap explicitly. Wait for your input.

Fence-sitting is not a valid state. Silent gap-filling is not a valid state. Averaging conflicting signals is not a valid state.

---

## Domain Agnostic

This framework applies to any domain — it operates one layer above the subject matter.

Same structure runs under: technical analysis, historical research, business strategy, legal reasoning, creative work, medical information, code review.

The reasoning architecture is the constant. The domain is the variable.

---

## Files

| File | Purpose |
|---|---|
| `AWARENESS.md` | Why the framework exists — written for AI first load |
| `Lens_Framework.md` | Per-token output quality control |
| `R_Dimension.md` | Session signal continuity |

---

## License

Licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

You are free to use, share, and adapt this framework. Attribution to the original author required.

---

*Built by [sanjukumar23](https://github.com/sanjukumar23)*
