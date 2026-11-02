# Rubric v1.1 (proposed, Nov 1)

Changes from v1 come from the AI pilot (`pilot/`). Nothing here is frozen. The team approves it after the blind human pilot. Until then the workbook still uses v1.

## What changed

1. Replication (RP) is recorded but not averaged into the tier.
2. The eight remaining items are grouped into three domains and reported as a profile.
3. Each anchor has a short worked example from the pilot.
4. N/A and 0 have one rule.
5. Each paper gets a short claim log (1-3 claims, tagged) before scoring.

## Scoring rules

- Score 2, 1, 0 or NA.
- NA only if the item cannot apply to this kind of paper. Example: CF is NA if the paper makes no comparison to AI or silicon at all.
- If the item applies and the paper does not give the information, score 0.
- Score what the paper shows, not what the authors cite from an earlier paper. If controls or data come from earlier work, say so in the notes and score 1 at most for CT.
- Write the page or figure for every score.

## Claim log (before scoring)

For each paper write the headline claim and any efficiency or learning claim. Tag each: demonstrated, demonstrated under constraints, projected, illustrative, aspirational, not demonstrated. Use the tags when you score CC.

## Domain A: Design (SM, UA, CT, RB)

| Item | 2 | 1 | 0 | Notes from the pilot |
|---|---|---|---|---|
| SM System match | Claim is about the system actually tested | Gap between claim and system, acknowledged | Claim extends past the system with no acknowledgment | A 2D culture result called organoid evidence is a 0 |
| UA Unit of analysis | Stats at culture or organoid level, or a model for repeated sessions | Number of units given, independence unclear | Sessions or trials treated as independent, or n missing | Cross-validating many trials from 3 organoids as independent is a 0. 174 sessions from a few cultures is a 0 |
| CT Controls | Two or more fitting negative controls on the system studied | One control | None | Controls only in an earlier paper count for at most 1 |
| RB Robustness | Result shown across days, batches, lines or labs | One condition, limit stated | Not examined, or the paper's own data contradict it | Noise added to a classifier is not RB. It must be biological or lab variation |

## Domain B: Comparison (CF, EA)

| Item | 2 | 1 | 0 | Notes from the pilot |
|---|---|---|---|---|
| CF Comparator fairness | Same task and metric, matched inputs, baseline tuned or tuning shown, no cap that favors one side | Partly matched, limits stated | Comparator unmatched, untuned or unspecified | A same-classifier baseline on the raw stimulus is fair. "Competitive" with no named comparator is a 0 for that claim |
| EA Energy accounting | Whole-system energy measured, incubation and life support included | Part of the system measured | Energy appears only as motivation or as brain-level figures | "Low-power" in the abstract with nothing measured is a 0, not NA |

NA for EA only if the paper makes no energy claim anywhere, including the abstract.

## Domain C: Reporting (TR, CC)

| Item | 2 | 1 | 0 | Notes from the pilot |
|---|---|---|---|---|
| TR Transparency | Methods enough to repeat and data or code available | Methods enough, data or code on request only | Methods insufficient, no data or code | Proprietary platform with open analysis code is a 1 or 2, say which part is closed |
| CC Claim calibration | Title, abstract and headline match the evidence and the limits | Mild overreach | Headline contradicted by the paper's own limits | Use the claim tags. For roadmaps, score the gap between what is projected and how the title frames it, not the fact that it is aspirational |

## Recorded, not averaged

| Item | What it asks | Values |
|---|---|---|
| RP Independent reproduction | Has the result been reproduced by people with no author overlap? | 2 yes, 1 same group or overlapping authors only, 0 none known, NA never |

Also record: COI or affiliation, peer-review status, hypothesis stated up front, and whether the paper reuses data from an earlier one.

## Tier rule

- Mean of the scored items in Domains A-C (up to 8). RP is shown next to the tier, not inside it.
- Minimum 6 items scored, otherwise Unrated.
- Cut-offs set after the blind human pilot and before scoring the rest. Write down the reason for any change.
- Always report the three domain scores and CC next to the tier.

## Review rubric (reviews, roadmaps, company pages)

Items PS, HR, MP, CC as in v1. Added note for MP: implicit separation of measured and projected in prose scores 1, explicit labels or a table scores 2.
