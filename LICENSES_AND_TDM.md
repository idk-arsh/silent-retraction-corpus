# Source licenses and TDM posture

This project ingests scientific papers only from sources whose text-and-data-mining terms the project can point to in writing. It never scrapes paywalled content. It never bypasses an account gate. It never redistributes full paper text whose license forbids redistribution.

Each source below carries the exact URL for the terms the project relies on. If a term changes, the project pauses that ingestion arm until the new terms are read and documented here.

## arXiv

Bulk access via the Kaggle snapshot and the arXiv S3 requester-pays bucket. Terms: https://info.arxiv.org/help/bulk_data_s3.html.

## bioRxiv and medRxiv

TDM API. Terms: https://api.biorxiv.org/.

## PubMed Central Open Access subset

NCBI FTP, Open Access subset only. Terms: https://pmc.ncbi.nlm.nih.gov/tools/openftlist/.

## Crossref

Metadata via the public REST API. Terms: https://www.crossref.org/documentation/retrieve-metadata/rest-api/.

## OpenAlex

Full snapshot and REST API. Terms: https://docs.openalex.org/download-all-data/openalex-snapshot.

## ClinicalTrials.gov

Full study record download. Terms: https://clinicaltrials.gov/data-api/about-api.

## Posture

The corpus records DIFFS between versions, together with the DOIs that identify the source papers. The corpus does not redistribute full paper text. Downstream users who want the underlying text follow the DOI to the original source and comply with that source's terms.
