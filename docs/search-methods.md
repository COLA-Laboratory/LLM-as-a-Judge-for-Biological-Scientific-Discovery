# Search and screening methods

[Project home](../README.md) · [Literature catalog](literature-catalog.md) · [Screening history](screening.md)

This evidence-mapping survey examines how large language models assess objects, processes, and outputs in biological research. The literature register counts studies. The evidence synthesis examines individual **judgment events**, each with an identifiable object, criterion, and verdict. A study can contain several events, such as a review of an analysis plan followed by an assessment of its output.

## Eligibility

- **Domain evidence.** An empirical study in biology, computational biology, or discovery-oriented biomedicine must report an identifiable LLM judgment tied to a research decision or assessment. We accept scores, pairwise preferences, rankings, labels, and critiques whose use in screening or revision can be traced. Study screening and evidence appraisal are included as adjacent research tasks.
- **Boundaries.** Generation, prediction, self-reported confidence, and performance scoring by people or rules alone fall outside the LLM judgment criterion. Ordinary clinical question answering, individual diagnosis, and patient recommendations fall outside the research scope. Reviews and commentaries may lead to original studies through their references.
- **Evidence status.** Identifiable judgment events can enter the register with limited independent validation. Studies supported provisionally by abstracts are marked separately. Reports awaiting an eligibility decision are tracked outside the study total. General evaluation research is counted separately when its approach to scoring, reliability, or bias assessment can transfer to this setting.

## Sources and search design

We combined two types of query. **Role-based queries** looked for terms such as *judge*, *evaluator*, or *reviewer*. **Task-based queries** looked for activities such as hypothesis assessment, candidate prioritization, workflow review, claim verification, or study screening. The task route was necessary because reports sometimes describe an evaluative step only in the methods or supplements. For example, all 22 domain studies newly included from the Web of Science batch were returned by the task query, which allowed records without explicit judge-role terms.

| Source or route | What was searched |
| --- | --- |
| PubMed | Database queries through E-utilities, followed by targeted reference and citing-record checks. |
| arXiv | Database queries through the Atom API and checks of report versions. |
| bioRxiv and Europe PMC | Europe PMC queries restricted to bioRxiv for preprint discovery. bioRxiv metadata were checked for versions, and Europe PMC supported targeted full-text and record checks. |
| Web of Science Core Collection | Two queries run on 19 November 2026, one role-based and one task-based. They yielded 242 distinct database records after removing query overlap. |
| Scopus | Two queries run on 19 November 2026, one role-based and one task-based. Deduplication and linkage yielded 481 distinct reports, 223 also found in the Web of Science batch. |
| Supplementary discovery | Backward and forward citation checks, selected conference proceedings and benchmark directories, and targeted searches for full reports, supplements, or author materials. The 20 November citation check recovered 98 PubMed records and 42 Crossref references, with seven report overlaps. |
| Embase | The planned search remains pending because database access could not be established. |

The eligibility rules accept reports in any language and impose no publication-date cutoff. The executed searches and accessible materials are predominantly English. The November 20 search snapshot and the focused November 21–22 checks cover different work. Later additions reflect targeted eligibility and version checks, so they leave the reported coverage of the earlier search runs unchanged.

## Screening and extraction

One reviewer screened titles and abstracts and consulted primary reports, supplements, or author materials when a decision required more detail. Overlapping database records were identified by platform identifiers, DOI, PMID, version-normalized arXiv identifier, or normalized title. Preprints, conference reports, and journal publications were linked when evidence indicated that they reported the same study. Where linked reports described distinct judgments, the synthesis retained the source of each judgment and marked known overlap.

For each judgment, the review records the object, criterion, evidence available to the model, verdict, and use in the research workflow. For evaluations, it also records the reference, unit of comparison, denominator, and limitations. These fields help distinguish repeated model responses and expert agreement from independent checks of scientific results or evidence that a judgment changed a decision. The detailed synthesis selects studies to span these different tasks and evaluation designs.

## Register and coverage

| Snapshot | Domain studies | General evaluation papers | Reports awaiting a decision |
| --- | ---: | ---: | ---: |
| 20 November 2026 search snapshot | 241 | 32 | 25 |
| 21 November 2026 after focused verification | 244 | 32 | 22 |
| 22 November 2026 after targeted additions and list reconciliation | 251 | 32 | 23 |

Of the 251 domain studies in the current register, 245 are recorded as included and six as provisionally included from abstracts. These are study-level counts after linking identifiable versions. The source table above gives counts for individual search batches at the record or report level. The same report can be returned by multiple routes.

The first two thematic PubMed queries missed 38 indexed studies in the set used to develop the search. Revised queries recovered all 38 in that development set. Independent retrieval testing and second-reviewer screening remain pending. Some search requests were incomplete, and judgments disclosed only in inaccessible full text or supplements may be underrepresented. The counts describe the current working register within the documented search coverage.
