# Critique of the review design, layer by layer

Compared with the standards a metascience or methods review is usually held to. I could not open the standards documents themselves in this run (search returned links only), so check each point below against PRISMA 2020, PRISMA-ScR, AMSTAR 2, Cochrane's risk-of-bias guidance and GRADE before citing them in the paper.

Rating: **Keep** (meets the bar), **Change** (fix before scoring), **Defer** (do it if time allows, state as a limitation if not).

| # | Layer | Where we are | Standard it is compared with | Verdict |
|---|---|---|---|---|
| 1 | Question and protocol | Written before searching, dated | Pre-registration (OSF, or PROSPERO if it qualifies) and PRISMA protocol items | Keep. Register on OSF after the human pilot and before scoring the rest |
| 2 | Search | PubMed, bioRxiv, medRxiv, arXiv plus manual grey literature | At least two or three databases, a search string reported, citation chaining, grey literature stated | Change. Add Google Scholar or Scopus and do citation chaining from the seed papers |
| 3 | Selection | One screener, title and abstract | Two independent screeners, at least on a sample, with agreement reported | Change. Second screener on a random 20% now. Full-text check on every Include and Maybe |
| 4 | Selection by claim, not quality | Papers are included if they make an in-scope claim | Fine for a methods review. Risk: the corpus is also shaped by what gets published and indexed | Keep. State the publication bias limit |
| 5 | What the items measure | Mix of reporting quality (TR, CC) and design validity (SM, UA, CT, RB, CF, EA) | Standards separate reporting quality from risk of bias. Mixing them in one score makes it unclear what a low score means | Change. Group into domains and report each, which v1.1 does |
| 6 | Item definitions | Anchors for 0, 1, 2 | Risk-of-bias tools use signaling questions and domain judgments, not single-line anchors | Change. Add worked examples (v1.1) and test them on new papers |
| 7 | Scale and N/A | 0/1/2 or NA | Three levels is coarse but matches common practice. N/A needs a stated rule | Change. One N/A rule, counted per rater |
| 8 | Raters and reliability | Two raters, kappa in the sheet | Two independent raters, consensus process, agreement reported. Kappa with a few papers is unstable | Change. Use weighted kappa and report disagreements, not only kappa |
| 9 | Adding items into a mean and tiers | Mean of items, cut-offs 1.5 and 1.0 | Risk-of-bias guidance generally avoids numeric composite scores and uses domain judgments. Weighting is arbitrary and results can change with the scale | Change, with a trade-off. Keep a mean because the team needs tiers to compare, but report domain scores beside it and run a sensitivity check (drop each item, try other weights) |
| 10 | Tier cut-offs | Fixed in advance | Prespecified thresholds are good. Changing them after seeing results is a researcher degree of freedom | Keep. Set after the blind pilot and before the main scoring, log changes |
| 11 | Determining factor | Item with the biggest High-Low gap | A post hoc analysis on the same scores that built the tiers. With a small n, a ranking tells you nothing causal | Change. Call it exploratory, "most discriminating item", report leave-one-out |
| 12 | Claim-level view | Claims sheet, tags | GRADE rates certainty per outcome, not per study. Per-claim assessment is closer to what a methods review needs | Defer the full version. Keep the lightweight claim log in v1.1 |
| 13 | Replication item | Scored 0/1/2 | Almost always 0 in a young field, so it adds no spread | Change. Record it, don't average it |
| 14 | AI pilot | One AI pass, four papers | A model scorer needs a gold set, a dev/test split, and a stop rule before it counts as data | Keep as a diagnostic only. Defer any AI scoring until humans have scored |
| 15 | COI and affiliation | Descriptor, tested against scores | Fine as a descriptive comparison. Groups will be small and confounded | Keep, report counts and use exact tests |
| 16 | Reporting our own review | Plan to follow PRISMA 2020 (27 items) | PRISMA 2020 is written for reviews of interventions. PRISMA-ScR (22 items) fits a scoping or methods review better | Change. Pick one, say why, and list the items that do not apply |
| 17 | Our own bias | The group started with an argumentative paper and has views on OI | Disclose priors and how scoring avoids them (blind scoring, written anchors) | Add a short reflexivity paragraph |

## Where the balance falls

The team has one semester and three students. The design has to be defensible, not perfect.

Do before scoring the rest:
- blind human pilot on the same four papers, then fix the anchors (v1.1 draft is ready)
- second screener on 20%
- Google Scholar or Scopus plus citation chaining
- pre-register the protocol, rubric and cut-offs on OSF
- RP out of the mean, domain scores reported

Do if time allows:
- claim-level scoring for all papers, weighted kappa and sensitivity analysis in the workbook, second full-text reviewer

State as limitations if not done:
- single database family, small n, tiers are descriptive, no causal claim about what makes a paper rigorous

## What this means for the paper's claims

The tiers show how well each paper reports and justifies its claims by this rubric, using our judgments. They do not show whether the underlying science is right. Say that plainly in the abstract and the limitations.
