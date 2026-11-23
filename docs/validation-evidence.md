# What validates an LLM judge?

These examples follow the judgment from its evidence and criterion to the decision it informs. The studies use different tasks and units, including hypotheses, rubric items, citations, response cells, and screening tasks. Each result describes the comparison reported in its source.

## Agreement about evidence

**SKiM-GPT.** Four specialists and the LLM rated support for 14 selected hypotheses using literature abstracts. The authors report quadratic-weighted Cohen’s κ of 0.84 with and without relevance filtering. Without filtering, median scores from the specialists and the system agreed in direction for 13 of 14 hypotheses. This measures agreement on the selected hypotheses and available literature. A test of the hypotheses themselves would require an outcome reference beyond those abstracts. [SKiM-GPT, Fig. 3](https://link.springer.com/article/10.1186/s12859-025-06350-7#Fig3)

**Citation checks in gene set interpretation.** Hu and colleagues used an LLM to check whether a proposed source supported a statement in a generated interpretation. In a manual audit, reviewers verified support for 383 of 489 retained citations. They also found that all facts were supported in 354 of 403 generated sentences. The first count describes citations after filtering. The second describes complete factual support at the sentence level. An audit of rejected citations would be needed to estimate how much valid evidence the filter discarded. [Hu et al., Methods and Extended Data Fig. 1](https://doi.org/10.1038/s41592-024-02525-x)

## Analysis quality and answer grading

**BIABench.** The adopted LLM judge and a blinded specialist agreed on 87% of the 922 process rubric items that both decided, out of 1,273 items across 20 bioimage analysis runs. Cohen’s κ was 0.67. The same runs informed judge selection. Five runs with expert process scores of 0.74–0.82 scored below 0.10 against the separate references for submitted outputs. The rubric tracks evidence about the analysis process, and the output reference checks what the analysis delivered. [BIABench, §3.3, Fig. 5 and Appendix E](https://arxiv.org/html/2609.34274v1#S3.SS3)

**LitBench.** An LLM panel graded whether answers to literature-synthesis questions supported reference facts. A clinician on the author team, blinded to the panel verdicts, independently rated 154 stratified response cells. Agreement was 89.0% (κ = 0.774), and the panel granted credit more often. The study also checked source identifiers and supporting text separately. The clinician comparison measures agreement about semantic support in the audited sample. The separate check verifies source matching. [LitBench, Methods and Table S4b](https://pmc.ncbi.nlm.nih.gov/articles/PMC13622311/)

## Screening and review decisions

**LEADS.** Fifteen specialists each completed ten literature-screening tasks and selected ten from a set of 30 citations per task. Assisted and unassisted recall against prior review inclusions was 0.81 and 0.78, respectively. Mean screening times were 449 and 580 seconds. The paired results characterize screening assistance for the tested case pool, selection quota, and reference. [LEADS, Fig. 5d](https://www.nature.com/articles/s41467-025-62058-5#Fig5)

**Automated abstract screening.** Sanghera and colleagues evaluated screening on 119,695 records with abstracts from 23 Cochrane reviews. Across five selected configurations, sensitivity ranged from 0.756 to 1.000 and precision ranged from 0.004 to 0.096. Prompt development used 800 balanced records from the same set of reviews. The verdicts were compared with prior review decisions and used to simulate screening workloads. The workload estimates depend on the prevalence of relevant records and how screened results are routed to reviewers. [Sanghera et al., Tables 3–4](https://doi.org/10.1093/jamia/ocaf050)

## Reproducibility and correctness

**All Verdicts are Not Equal.** This general evaluation study tested six models on four benchmarks with ten repeated judgments per condition and two presentation orders. The most deterministic judge agreed with reference labels on 51% of the evaluated items reported for that result. Repetition tests whether a model returns the same verdict, order swaps test sensitivity to presentation, and reference labels measure correctness. A judge that repeats its verdict can still be consistently wrong. [Kumar et al., AACL-IJCNLP 2026](https://aclanthology.org/2026.aacl-long.207/)

## What establishes decision value?

| Evaluation question | Evidence that addresses it |
| --- | --- |
| Does the judge apply the criterion reliably? | Repeat judgments under the same conditions. Track presentation sensitivity and the share of cases with a definite verdict. |
| Does the verdict agree with independent evidence? | Compare with specialist judgments, labeled references, or verified outputs. Report the unit, denominator, and any reuse of the cases during judge development. |
| Does the verdict change a research decision? | Record which cases were selected, revised, escalated, or excluded because of the verdict. Audit a sample of each decision where feasible. |
| Does the changed decision improve outcomes? | Compare selection or review policies on comparable inputs, resources, and outcome assessment. Distinguish outcomes of selected cases from the difference between policies. |

[Project home](../README.md) · [Literature catalog](literature-catalog.md) · [Search and screening methods](search-methods.md)
