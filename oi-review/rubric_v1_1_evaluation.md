# Evaluation of rubric v1.1 and its changes

What this is: my own scoring of the design, in the style of your saved panel (ROI, No-BS, Referee). I did not run the full multi-agent council. The only data are the four AI-scored pilot papers, so everything here is a judgment, not a measurement. The Referee notes where I may be inflating.

## Does v1.1 deflate scores?

No. The changes barely move the numbers. The low scores come from what a 2 demands, not from the changes.

Pilot means (one AI rater, three empirical papers):

| Paper | v1 | v1.1 (RP out) | Tier |
|---|---|---|---|
| Khajehnejad | 1.12 | 1.14 | Medium |
| Braille (Liu) | 0.78 | 0.88 | Low |
| FinalSpark (Jordan) | 0.62 | 0.71 | Low |

- Removing RP raises each mean by 0.02-0.10. No paper changes tier.
- A strict reading of RB (noise on a classifier is not RB) would lower Braille to 0.75 and not change its tier.
- Of 22 scored items, 3 are 2s (14%), 14 are 1s (64%) and 5 are 0s. Scores pile up at 1, and the High band (1.5) needs mostly 2s. With these anchors, an empirical paper reaching High is rare, so the upper tier may stay empty.
- Four of eight items show no spread in this sample: UA is 0 for all three, CT, RB and CC are 1 for all three.
- The review rubric is the fragile part. Smirnova ranges from 1.25 (MP scored 1 under the new rule) to 1.75 (CC scored 2 under the roadmap rule) depending on how two anchors are read. That crosses a tier band either way.

## Each change: keep or cut

| Change | Effect on scores | Cost | Verdict |
|---|---|---|---|
| RP out of the mean, recorded | +0.02 to +0.10 | Low | Keep |
| Three domains, reported as a profile | None | Low | Keep |
| NA only if the item cannot apply, otherwise 0 | None in the pilot, pushes NA to 0 in general | Low | Keep. Count NA to 0 conversions in the main run |
| Worked examples in anchors | Slightly lower (up to -0.13) | Low | Keep, but test on new papers. The examples come from the same four pilot papers |
| CT: cap at 1 for inherited controls | None in the pilot | Low | Cut. Replaced by "score the chain, tick inherited". A cap penalizes proper reuse of data |
| Claim log (1-3 claims) | None | +10 min per paper | Keep, headline and efficiency claims only |
| Roadmap CC rule and MP explicit labels | Swings review scores by 0.25-0.5 | Low | Change. Drop review tiers, report item profiles |
| Minimum 6 items (of 8) | More papers Unrated than v1 (6 of 9) | None | Keep |
| Rank-based thirds for tier comparison | None to scores | Low | Add. Absolute bands stay as labels |

## Design layers, scored (0-100, fit to purpose and feasibility)

| Layer | Score | Why |
|---|---|---|
| Question and protocol | 80 | Written first, dated, ready to register |
| Search and screening | 55 | One screener, one database family, no citation chaining |
| Item set | 65 | Covers the right things. Reporting and design mixed in one mean |
| Anchors | 60 | Better with examples, still untested by humans |
| Scale and NA rule | 65 | Clear now, coarse |
| Raters and reliability | 50 | No human scores yet, and kappa on a few papers is unstable |
| Aggregation and tiers | 45 | High band probably unreachable, review tiers fragile |
| Determining factor | 35 | Built on the tiers it explains, small n, exploratory only |
| Claim layer | 55 | Light version only |
| AI pilot | 50 | Diagnostic, one rater, scores not gold |
| Reporting plan | 60 | PRISMA-ScR vs PRISMA 2020 still to choose |
| Overall | about 55 | Sound plan, unproven in practice |

## Advisor views

- **ROI:** the best payoff per hour is the blind human pilot, then rank-based tiers. Claim scoring for every paper is the worst return for the time.
- **No-BS:** you have four AI scores and a rubric nobody has tested. The risk is not deflation, it is that the tiers do not separate papers, and the "determining factor" is mostly an artifact.
- **Referee:** my scores are impressions from four papers and one AI rater. The 14% / 64% distribution could change entirely with a human or with a bigger sample. The worked examples were written after seeing these papers, so they are not independent tests.

## What to do

1. Blind human pilot on the same four papers, plus two new ones for testing the examples.
2. Track deflation by counting the share of 2s, 1s, 0s and NAs per rater in the pilot. If 2s stay under about 15% for humans too, the High band needs a rethink before preregistration.
3. Use rank-based thirds for the tier comparison.
4. Report review items as a profile.
5. Freeze, preregister, then score.
