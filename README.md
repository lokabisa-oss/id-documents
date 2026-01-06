# id-documents

This repository contains archived copies of original Indonesian government
documents and public datasets for reference, auditability, and reproducible
data processing.

## Purpose

- Preserve original source documents in their published form
- Enable deterministic and reproducible data pipelines
- Provide auditable references for downstream datasets (e.g. region-id)

This repository stores **raw, immutable source files only**.
No normalization, transformation, or interpretation is performed here.

## Scope

Documents and datasets in this repository may originate from:

- Ministry of Home Affairs (Kementerian Dalam Negeri)
- Provincial and national open data portals
- Other official government institutions

## Structure

Documents are organized by source and year:

`<source>/<dataset>/<year>/`

Each dataset folder contains:

- original files as published
- a README describing the source and context
- a `SHA256SUMS` file for integrity verification

## Usage

Documents in this repository are intended to be consumed by automated pipelines
(e.g. CI/CD, data builders, parsers).

Consumers **must verify document integrity** using the provided SHA-256 checksums
before processing.

## Disclaimer

All documents in this repository are publicly available government publications.
This repository does not claim ownership, authorship, or authority over the content.

## Attribution

All documents originate from their respective official publishers.
Redistribution is provided solely for public reference and reproducible
data processing purposes.
