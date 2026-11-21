---
name: wsjf-cost-of-delay
description: Ranks work by WSJF (Weighted Shortest Job First) with a split of roles. The sponsor, the person who owns priorities, scores only cost of delay as three parts (business value, time criticality, opportunity enablement or risk reduction) on a small Fibonacci-style scale and adds them. The team estimates job size and computes WSJF as cost of delay divided by job size. Ties go to the shorter job. Each score carries a date, its inputs and its assumptions. Use when ordering goals, features or a backlog, when a priority argument keeps restarting, or when the person who wants something is also sizing it.
---

# WSJF with a cost-of-delay split

## Purpose
WSJF asks one question of every candidate: how much does waiting cost per unit of effort? The answer orders the work. This version separates who judges what. The sponsor knows what delay costs and says so. The team knows how big the job is and says that. Neither scores the other's half, so the ranking resists wishful thinking.

Background: WSJF comes from SAFe, a published framework, and rests on Reinertsen's cost-of-delay idea. The rule that the sponsor scores only cost of delay is a variation used in practice. It is not the published standard.

## When to use
- You have more candidates than capacity and need an order you can defend.
- Priority debates repeat because nobody wrote down why one item beats another.
- The person asking for an item is also the person estimating it.
- Skip it for a list of three small items where the order is obvious, or where one item is a legal deadline and nothing else competes.

## Steps
1. Pick the layer where the sponsor actually decides, usually goals or large features, and score there. Do not score every small item. Score a smaller item only as a last resort, and note the reason beside the score.
2. The sponsor scores three parts for each candidate on the scale 1, 2, 3, 5, 8: business value (what it is worth if delivered), time criticality (how fast that worth decays or a deadline bites), and opportunity enablement or risk reduction (what it unlocks or what danger it removes).
3. Add the three parts. That sum is the cost of delay. The sponsor does not score job size, because people who want something tend to shrink its size.
4. The team estimates job size for each candidate on the same kind of scale, 1, 2, 3, 5, 8, using its usual method. The team does not score value, time criticality or enablement.
5. Compute WSJF as cost of delay divided by job size. Round to one decimal.
6. Rank from highest WSJF to lowest. When two items tie, the shorter job goes first, because it frees capacity sooner and returns feedback sooner.
7. Write next to each score its date, the inputs it rested on, and what it assumes (for example, "assumes the partner contract is signed by March"). A score with no assumption written down cannot be rechecked.
8. Rescore when a fact changes: a deadline moves, a dependency lands, a size estimate grows. Do not rescore on a calendar alone.
9. Until the sponsor has scored, show the team's best guess at cost of delay and label the resulting order "model only". Replace it when the sponsor scores. Never present a model-only order as the sponsor's.
10. Read the ranking as a proposal. Check it for dependencies and capacity before work starts.

## Example
Invented data. Product team "Pebble Notes", scored 2026-03-09. Columns on the scale 1, 2, 3, 5, 8.

| Item | Value, time, enablement, size | Cost of delay, WSJF, rank |
|---|---|---|
| Import from other note apps | 5, 3, 5, size 3 | 13, 4.3, rank 1 |
| Share by link | 3, 2, 2, size 2 | 7, 3.5, rank 2 |
| Dark theme | 2, 1, 1, size 2 | 4, 2.0, rank 3 (tie, shorter job) |
| Search rebuild | 5, 3, 2, size 5 | 10, 2.0, rank 4 (tie, longer job) |
| Offline mode | 5, 2, 5, size 8 | 12, 1.5, rank 5 |

Worked row in prose: value 5, time 3, enablement 5 gives cost of delay 13. With job size 3, WSJF is 13 divided by 3, which is 4.3.

Check the others the same way. Share by link: 3 + 2 + 2 = 7, and 7 divided by 2 is 3.5. Dark theme: 2 + 1 + 1 = 4, and 4 divided by 2 is 2.0. Search rebuild: 5 + 3 + 2 = 10, and 10 divided by 5 is 2.0. Offline mode: 5 + 2 + 5 = 12, and 12 divided by 8 is 1.5.

Offline mode has the second-highest cost of delay and still ranks last, because it is the biggest job. That is the method working, and the sponsor may still choose to start it early for a reason the scores do not hold. If so, write the reason down.

## What this does not verify
- Scores are judgments, not measurements. A 5 is someone's opinion with a number on it.
- WSJF ranks work; it does not decide. The sponsor and team still choose.
- It can hide dependencies. A low-scoring item that blocks a high-scoring one may need to go first.
- With small scales and few items, the inputs are noisy. A gap of 0.2 between two items is not a real difference.
- Adopted, not measured: no result is claimed for better ordering or faster delivery.

## Common failure modes
- The sponsor scores size. The ranking now reflects what the sponsor hopes the effort is. Hand size back to the team.
- Scoring everything. Dozens of scored small items cost more attention than they save. Score at the decision layer.
- Stale scores. A score from last quarter that nobody dated or rechecked orders work by old facts. Rescore on change.
- False precision. Quoting WSJF to two decimals from 1-to-8 inputs implies accuracy the inputs lack. Treat near-ties as ties.
- Gaming time criticality. Every item becomes urgent when urgency buys priority. Ask for the date and the consequence behind any 5 or 8, and write them next to the score.

## Licence and version
CC BY 4.0. Attribution: Drew Podwal. Version 0.1, 2026-11-21. Adopted, not measured: no result has been measured yet.
