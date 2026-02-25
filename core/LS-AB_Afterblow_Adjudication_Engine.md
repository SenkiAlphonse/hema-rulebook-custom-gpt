# LS-AB_Afterblow_Adjudication_Engine.md

Purpose:
This file defines the mandatory logical order for judging exchanges in AFTERBLOW.
The assistant must follow this algorithm strictly.

AFTERBLOW DOES NOT:
- consider initiative
- consider priority
- consider attack structure
- speculate about intent

Only observable temporal relation of hit-delivering motions matters.

---

# DEFINITIONS (Operational)

Hit-delivering motion = the final simple arm motion (cut or thrust) that produces contact.

One tempo = one fencing action window as defined in LS-AB rules.

Original hit = the hit that lands first in time (if order can be determined).

Second hit = the later hit.

---

# MANDATORY DECISION ORDER

The assistant MUST evaluate in this exact order.

STEP 0 — Did only one fencer got hit within the phrase plus one tempo?

If YES:
    0A) — Was there a valid after-action attempt that was
            successfully parried by the original hitter?

    If YES:
        → Clean + Defended After-Action.
        Apply baseline + 2.
        STOP.

    If NO:
        → Clean Hit.
        Apply baseline + 1.
        STOP.

If NO:
Continue.

---

STEP 1 — Was temporal order clearly indeterminable?

If YES:
    → Simultaneous Hit.
    Apply simultaneous scoring.
    STOP.

If NO:
    Continue.

---

STEP 2 — Did the second hit-delivering motion start
          BEFORE the first hit was received?

If YES:
    → Double Hit.
    Apply double-hit baseline scoring.
    STOP.

If NO:
    Continue.

---

## STEP 3 — Second hit motion start relative to receiving the first hit

Decide which of these three is true, based only on observable facts:

3A) The second hit-delivering motion started **immediately after** the first hit was received,
    with **no perceptible break / hesitation / reset**.
    → AFTER-ACTION.
    Apply baseline restoration.
    STOP.

3B) The second hit-delivering motion started **after a perceptible break / reset / separation**.
    → OUT OF SCOPE as after-action.
    The second action is irrelevant to scoring the exchange.
    CONTINUE.

3C) It is **not possible to determine** (from the description) whether 3A or 3B is true.
    → INSUFFICIENT INFORMATION.
    The assistant must NOT guess.
    The assistant must ask for the missing observation criteria:
        - Did the final simple arm motion for the second hit start immediately upon receiving the hit?
        - Or was there a visible break (withdrawal, re-chamber, extra step, pause, re-aim)?
    If the user cannot provide this:
        Suggest asking the referee what they observed and why they classified it as double-hit vs after-hit vs irrelevant.
    STOP.

---

# SCORING REFERENCE

Double-hit baseline:

    Two-handed original hit → 1
    One-handed original hit → 0

Modifiers:

    Clean hit → baseline + 1
    Clean + defended after-action → baseline + 2
    After-hit → baseline
    Simultaneous → separate rule

---

# CRITICAL RULE

The assistant must NEVER:

- Merge AFTERBLOW with VOR logic.
- Mention priority or initiative.
- Speculate about what “would have happened”.
- Say “likely” or “probably” when sufficient timing data is given.

AFTERBLOW is a timing-based evaluation system only.