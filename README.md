# Silent Retraction Corpus

A labeled, versioned, DOI-anchored dataset of silently-edited scientific papers detected across preprint-to-journal diffs. First greppable record of how the scholarly record quietly mutates.

## Scope (v0.0)

Clinical-trial preprints and their corresponding journal publications. Each pair is matched by Crossref `is_preprint_of` relations, title-and-author fuzzy match within an eighteen-month window, or shared ClinicalTrials.gov registry IDs. Each pair yields a typed diff across six categories: `numeric_shift`, `author_change`, `methods_change`, `limitations_change`, `data_availability_change`, `coi_change`.

Later versions expand to oncology RCTs, cardiology RCTs, and economics working papers.

## Sources

Only text-and-data-mining-licensed public sources enter the corpus. The ingestion layer reads arXiv (S3 requester-pays), bioRxiv and medRxiv (TDM API), and the PMC OA subset (NCBI FTP). The project never scrapes paywalled content, never bypasses account gates, and never redistributes material whose license forbids redistribution. The `LICENSES_AND_TDM.md` file lists every source and the written terms the project relies on.

## Licenses

Code: MIT. See `LICENSE`.

Data: CC-BY-4.0. Each release carries a Zenodo DOI and a Hugging Face dataset card.

## Status

Pre-v0.1. Day one: 2026-10-12. First end-to-end pipeline run on five hundred pairs: 2026-10-17. v1.0 target release: 2027-01-03.

Project page and roadmap live in the `docs/` folder once the pipeline runs. Issues and discussion welcome from day one.
