# Rigor Review of Organoid Intelligence Research

Working files for a critical review of how rigorous organoid intelligence (OI) and biocomputing research is. A separate Pong replication tests one paper's claim directly: see [PONG_REPLICATION.md](PONG_REPLICATION.md).

## Overview

OI claims that living neurons can compute or learn, sometimes more efficiently than AI. Our group first planned an argumentative paper. About a month ago we changed it to a metascience review: instead of arguing for or against OI, we check how well the field's claims are supported. The questions are:

- Does each claim match the system that was actually tested (2D cultures vs organoids, whole brain vs organoid)?
- Are the controls, statistics and comparisons to AI fair?
- Do reviews and company pages keep the original authors' caveats, or drop them?
- Has anyone outside the original team reproduced the result?

## Where it stands

Done:
- Rubric v1, the scoring workbook, the search protocol, the screening log and the source list.
- An AI pilot on four papers. It found eight unclear anchors and no sign that the rubric changes cause deflation. It is a diagnostic, not data.
- Rubric v1.1 (draft) and an evaluation of it.

Not done:
- Human scoring. Nobody has scored a paper blind yet, so agreement is unknown.
- A second screener on a random 20%, and full-text checks of every Include and Maybe.
- Citation chaining from the seed papers, and a second database (Google Scholar or Scopus).
- OSF pre-registration.

## Plan

1. Blind human pilot: the same four papers, scored separately, then a short consensus meeting.
2. Fix the anchors where raters differ by two points or more, then freeze the rubric and cut-offs.
3. Pre-register on OSF.
4. Score a core set of about 20 papers chosen by a written rule. One rater scores each paper, and a second rater double-scores about half.
5. Report item profiles and domain scores. Tiers are descriptive and compared by rank thirds. The "determining factor" is exploratory.

Open decisions: core set size, how much to double-score, and the pilot pass rule. See [the evaluation](oi-review/rubric_v1_1_evaluation.md).

## Files

- `oi-review/OI_Critical_Review_Scoring_Sheet.xlsx`: screening log, scoring sheets, tiers, claims, analysis
- `oi-review/search_protocol.md`: question, searches, include and exclude rules
- `oi-review/rubric_scoring_anchors_v1.md`: what 0, 1 and 2 mean for each item
- `oi-review/review_sources.md`: papers in the screening log, with links
- `oi-review/rubric_v1_1.md`: rubric v1 with the pilot changes built in (draft, not frozen)
- `oi-review/rubric_v1_1_evaluation.md`, `oi-review/rubric_critique_v1_1.md`: which changes are worth keeping, and a layer-by-layer critique against review standards
- `oi-review/pilot/`: first AI pilot run of the rubric on four papers (findings and per-item scores). Not human scores; used to find unclear anchors
- `PONG_REPLICATION.md`, `DEVIATIONS.md`, `pong_env.py`, `dqn.py`, `analyze.py`: the Pong replication
