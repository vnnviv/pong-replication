# Rubric v1 pilot: AI run (Nov 1)

Pilot scores are in `pilot_scores_ai.csv`. This is one AI read, not a human rater, so use it to find unclear anchors and not as data. Do not paste these into the Rater 1 or Rater 2 columns.

## What was scored

| Paper | Read | Items scored | Mean | Tier at 1.5 / 1.0 |
|---|---|---|---|---|
| Khajehnejad (DishBrain vs deep RL) | full text, arXiv v1 | 8 | 1.12 | Medium |
| Liu, Braille with organoids | full text, arXiv v3 | 9 | 0.78 | Low |
| Jordan, FinalSpark platform | full text through a summary tool | 8 | 0.62 | Low |
| Smirnova, OI roadmap (review rubric) | first 100k characters | 4 | 1.50 | High |
| Kagan 2022 | not read, team notes only | partial | not tiered | |

Not done: Kagan 2022 (publisher page blocked) and Promise and Potential (PubMed blocked). Someone needs to read both.

## Where the anchors are unclear

1. **RP is a floor effect.** New methods papers get 0 by default, so RP pushes honest small studies into Low. It also splits two ways: has this paper's result been replicated, or is this paper a follow-up to someone else's result? Khajehnejad is a same-group follow-up and I gave it 1. Decide which question RP asks.
2. **RB means two things.** The Braille paper tests robustness to noise added to the classifier features. The anchor means robustness across days, batches and labs. Say that classifier noise tests do not count.
3. **UA vs cross-validation.** Braille cross-validates 1300 trials from three organoids. I scored UA 0, but that could also be read as a leakage problem. Add a line to the UA anchor about repeated trials and cross-validation.
4. **CT on secondary analyses.** Khajehnejad reuses DishBrain data, so its controls are in the earlier paper. Should it get credit? I gave 1.
5. **NA vs 0 on comparators.** Jordan motivates with GPT-3 energy but compares no performance. I used NA for CF and 0 for EA. A second rater may flip either one.
6. **EA when "low-power" is only in the abstract.** Braille says low-power with no measurement. I scored 0, not NA. Write that down in the anchor.
7. **CC for roadmaps.** Aspirational is the genre. As written, the anchor penalises Smirnova for its title while its body is carefully hedged.
8. **Review rubric MP.** Smirnova separates projected from demonstrated in prose, not with labels. It is unclear whether implicit labelling earns a 2.

## Problems with the tiers

- **Honest and small scores like overreaching and small.** Braille is the most carefully hedged empirical paper here, and it lands Low (0.78) next to Jordan (0.62), which has weaker stats and some sloppy claims. The mean cannot tell them apart. Report the CC item and a claim-level view alongside the tier.
- **Cut-offs.** No empirical paper reaches 1.5, and the highest is 1.12. That could be a true finding or a miscalibrated scale. Look at the distribution after the human pilot. Do not tune cut-offs to produce a High tier, and write down the reason for any change.
- **The roadmap tiers High.** Reviews have their own tier list, so this is fine, but the 1.5 cut-off may be easier to hit with 4 items than with 9.

## Limits of this run

- Scores come from retrieved passages and one summary tool, not a full read of each PDF.
- Khajehnejad was read as the arXiv version, but the workbook lists the 2025 journal version. Check what changed.
- Jordan's details come from a summarisation tool. Verify the n values and the 95.5% figure in the PDF.
- Confidence in the CSV is the AI's own estimate.

## What the humans should do next

1. Score the same four papers independently, blind to this file.
2. Compare. Settle the 8 anchor questions above wherever your scores diverge.
3. Read Kagan 2022 and Promise and Potential.
4. Then freeze the rubric.
