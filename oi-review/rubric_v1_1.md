# Rubric v1.1 (draft, Nov 1)

This is v1 with the changes from the AI pilot built in. It is not frozen. The workbook still uses v1. Freeze this after the blind human pilot. See [the evaluation](rubric_v1_1_evaluation.md) for which changes are worth keeping.

## Rules for all items

- Score 2, 1, 0 or NA.
- NA only when the item cannot apply to this kind of paper. If it applies and the paper does not say, score 0.
- Score what is shown. If controls or data come from an earlier paper, score the chain: credit them only where the earlier source is cited and the data are the same, and tick "inherited" in the descriptors.
- Write the page or figure for every score.
- Before scoring, write a claim log: the headline claim and any efficiency or learning claim, each tagged demonstrated, demonstrated under constraints, projected, illustrative, aspirational or not demonstrated.

## Empirical papers

### Design

| Item | Asks | 2 | 1 | 0 | NA when | Look at |
|---|---|---|---|---|---|---|
| SM System match | Does the claim concern the system actually tested? | Claim is about the substrate tested | Gap acknowledged (2D vs organoid, etc.) | Claim extends past the system, no acknowledgment | Never | Abstract vs Methods, culture type |
| UA Unit of analysis | Are stats at the level of independent biological units? | Culture or organoid level, or a model for repeated sessions | Number of units given, independence unclear | Sessions or trials treated as independent, or n missing | No statistics reported | Figure legends, Methods statistics |
| CT Controls | Could the result come from artifact rather than neural activity or learning? | Two or more fitting negative controls on this system | One control | None | Never | Results, control figures |
| RB Robustness | Does it hold across days, batches, lines or labs? | Shown across days, batches, lines or labs | One condition, limit stated | Not examined, or contradicted by the paper's data | Never | Sessions, replicates, Limitations |

Pilot examples: 174 sessions from a few cultures analysed as independent = UA 0. Cross-validating many trials from 3 organoids as independent = UA 0. Noise added to a classifier is not RB.

### Comparison

| Item | Asks | 2 | 1 | 0 | NA when | Look at |
|---|---|---|---|---|---|---|
| CF Comparator fairness | If compared with AI or silicon, is it like-for-like? | Same task and metric, matched inputs, baseline tuned or tuning shown, no one-sided cap | Partly matched, limits stated | Unmatched, untuned or unspecified | The paper names no comparator at all | Baselines, input encoding, comparison figures |
| EA Energy accounting | If energy is claimed, was whole-system energy measured? | Whole system including incubation and life support, against a stated comparator | Part measured (electrode level only) | Energy only as motivation or brain-level figures | No energy claim anywhere, abstract included | Introduction, Discussion, any power table |

Pilot examples: a same-classifier baseline on the raw stimulus is fair. "Competitive" with no named comparator is a 0 for that claim. "Low-power" in an abstract with nothing measured is EA 0, not NA.

### Reporting

| Item | Asks | 2 | 1 | 0 | NA when | Look at |
|---|---|---|---|---|---|---|
| TR Transparency | Could another lab repeat it? | Methods enough, data or code available | Methods enough, data or code on request | Methods insufficient, no data or code | Never (grey sources with no methods = 0) | Methods, data statement, repositories |
| CC Claim calibration | Do title, abstract and headline match the evidence and limits? | Match | Mild overreach | Contradicted by the paper's own limits | Never | Title and abstract vs Results and Limitations |

### Recorded, not averaged

| Item | Asks | Values |
|---|---|---|
| RP Independent reproduction | Reproduced by people with no author overlap? | 2 yes, 1 same group or overlapping authors only, 0 none known |

Also record: COI or affiliation, peer-review status, hypothesis stated up front, data reused from an earlier paper (yes/no).

## Reviews, roadmaps, company pages

| Item | Asks | 2 | 1 | 0 | Look at |
|---|---|---|---|---|---|
| PS Primary sourcing | Do headline numbers trace to primary measurements? | Each cited to the study that measured it | Some second-hand | Uncited or only press or reviews | Reference list vs numbers in the text |
| HR Hedge retention | Does it carry the source authors' caveats forward? | Preserved | Some dropped | Caveated results stated as established | Each cited claim vs its source's Limitations |
| MP Measured vs projected | Does it separate measured from projected? | Explicit labels or a table | Separated in prose only | Blended | Efficiency, capacity and potential statements |
| CC Claim calibration | Does the headline match the evidence it presents? | Matches the evidence and stated limits | Mild overreach | Contradicted by its own hedges | Title and abstract vs body |

For a roadmap, score CC on the gap between what is projected and how the title frames it, not on the fact that it is aspirational.

## Tiers

- Empirical: mean of the scored items in Design, Comparison and Reporting (up to 8). Minimum 6 scored, else Unrated. RP shown beside it.
- Always report the three domain scores and CC with the tier.
- Absolute bands (High 1.5, Medium 1.0) are descriptive. For comparing tiers and the exploratory "most discriminating item" analysis, use rank-based thirds so no tier is empty. Decide and register this before main scoring.
- Reviews have 4 items, so one point moves the mean by 0.25. Report their item profile, not a tier.
