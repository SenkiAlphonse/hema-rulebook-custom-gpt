# Core: Longsword AFTERBLOW — Hit Judging & Scoring (LS-AB)

Purpose: Teach the assistant how referees judge hits and how points are registered in the AFTERBLOW (AB) variant.

This file governs:
- timing classification
- scoring logic
- reduction and bonus logic
- grip-dependent values

It does NOT involve VOR, initiative, or priority.

AFTERBLOW is NOT:
- VOR (no priority)
- COMBAT (not pure chronology only)

AFTERBLOW is:
- Chronology-based
- With value hierarchy
- With modifier logic for near-immediate retaliation

---

# 0) Key Concepts

## Action vs Hit

- Action (akció): a fencing movement performed with intent (prep or attack).
- Hit (találat): the successful landing of an action.

Judging categories are based on observable timing of the final hit-delivering motion, not on intent.

---

# 1) Timing Categories

## 1.1 Simultaneous Hit (egyidejű találat)

Used when the referee cannot determine time order of the two hits.

This is NOT “együttes akció”.

## 1.2 Double Hit (kettős találat)

Occurs when:
- Both hits land in the same fencing phrase,
- There is less than one fencing tempo between them,
- And they are not judged as simultaneous.

Double hit is the reference case for scoring.

## 1.3 After-Action (után-akció) and After-Hit (után-találat)

After-hit occurs when:
- A fencer receives a valid hit,
- Immediately performs a simple cut or thrust,
- With no observable break, reset, or hesitation.

After-hit does not score independently.
It only modifies the value of the original hit.

Observable break indicators (NOT after-action):
- weapon withdrawal or reset
- additional step before action
- threat withdrawn
- halt already called (then disciplinary issue)

---

# 2) Grip-Dependent Baseline

The scoring reference is defined by DOUBLE HIT value.

Double-hit baseline:

- Two-handed original hit → 1 point
- One-handed original hit → 0 points

This is the neutral exchange value.

All other scoring is calculated relative to this.

---

# 2.5 Why Double Hit Is the Baseline

The double hit value is the conceptual reference point of AFTERBLOW.

This reflects a fundamental principle of fencing theory:

→ The first hit in time has inherent value.

When Right of Way (RoW) conventions are NOT applied, judging is primarily based on timing, not initiative.  
Within one tempo, priority is not determined by initiative structure, but by observable temporal order.

In combat-oriented fencing theory:
- The hit that lands first represents a successful offensive action.
- Any hit that follows occurs after damage has already been inflicted.
- Therefore, it is of lesser fencing value.

In sport fencing (which is an abstraction, not an actual duel):
- We do not speculate about “what might have happened next”.
- We evaluate what objectively occurred within the fencing phrase.

The AFTERBLOW model encodes this philosophy:

1. The ability to create a situation where you hit FIRST has value in itself.
2. If you fail to prevent a near-immediate return hit (within one tempo), that value is reduced to the neutral exchange baseline.
3. If you avoid being hit entirely, you earn additional value.
4. If you both strike cleanly AND control the opponent’s immediate retaliation, you earn even more value.

This does NOT encourage reckless fencing.

The system does not reward “mutual destruction”.
Instead, it structurally rewards:

- Control over the exchange expressed through timing,
- Defensive responsibility during and after the hit,
- Technical control over the opponent’s actions and response.

Thus:

Double hit = neutral reference value  
Clean hit = first hit while not receiving a hit in the same phrase  
Clean + defended after-action = first hit with demonstrated control afterward

The hierarchy rewards fencing value first,
and self-defense value even more.

## Note on Simultaneous Hits

Simultaneous hits are outside the baseline hierarchy.

In a simultaneous situation, the referee cannot determine temporal order.
Therefore, no “first hit value” can be established.

For this reason, simultaneous hits are handled as a separate category
with their own balanced scoring rule,
rather than through the double-hit baseline logic.

---

# 3) Scoring Model (Reframed)

## 3.1 Double Hit = Baseline

Register only against the fencer hit first:

- Two-handed → 1
- One-handed → 0

Second hit never scores independently.

---

## 3.2 Clean Hit = Baseline + 1

A hit is CLEAN if:
- No valid second hit within one tempo,
- No valid after-hit.

Score:

- Two-handed → 1 + 1 = 2
- One-handed → 0 + 1 = 1

Clean hit is simply one point better than a double hit.

---

## 3.3 Clean Hit + Successful Defense of After-Action = Baseline + 2

If:
- A clean hit occurs,
- Opponent attempts valid after-action,
- Original hitter parries that after-action with the blade,

Score:

- Two-handed → 1 + 2 = 3
- One-handed → 0 + 2 = 2

This reflects technical dominance and control.

Important:
Stopping an attack within tempo is NOT after-action defense.
There must be an actual after-action attempt.

---

## 3.4 Clean Hit + After-Hit = Baseline Restoration

If a clean hit is followed by a valid after-hit:

Reduce score back to double-hit baseline.

- Two-handed original → 2 → 1
- One-handed original → 1 → 0

After-hit does not score.
It only removes the clean bonus.

---

# 4) Simultaneous Hits (Special Category)

Simultaneous hits do NOT use baseline logic.

They are scored independently:

- 2H vs 2H → 1 each
- 1H vs 1H → 1 each
- 1H vs 2H → 1 only against the 1H fencer

This is the only case where both fencers receive points.

---

# 5) Combination Rule

If:
- Simultaneous OR Double Hit
AND
- An after-hit also occurs

The after-hit is ignored.

---

# 6) Mixed Valid / Invalid

If one hit is valid and the other invalid:
Judge only the valid hit.

If the referee cannot determine validity:
Annul and reset.

---

# 7) Critical GPT Corrections

Never state:

- “Kettős találat → both score.”
- “Után-találat scores.”

Correct principles:

- Only simultaneous gives points to both.
- Double hit and after-hit scenarios score only against the fencer hit first.
- After-hit modifies value; it never creates a separate scoring event.
- Baseline reference is the double-hit value.

---

# 8) Internal Formula

Let:

double_baseline =
    1 if original hit two-handed
    0 if original hit one-handed

Then:

- Double hit → double_baseline
- Clean hit → double_baseline + 1
- Clean + defended after-action → double_baseline + 2
- Clean + after-hit → double_baseline
- Simultaneous → special rule

End.