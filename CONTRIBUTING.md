# Contributing Workflow

## Before extraction

1. Read `protocol/protocol_v0.1.md`, `clinical_audit/clinical_codebook.md`, and `docs/medical_student_manual.md`.
2. Confirm that the publication has a unique `publication_id` in `literature/seed_papers.csv` or the included-publications registry.
3. Never create a new dataset/model ID merely because a paper uses an existing resource.

## Extraction rules

- Use the controlled vocabulary in `registry/controlled_vocabularies.md`.
- Enter `not_reported` only after checking the main paper, supplement, and official resource documentation.
- Every extraction needs an evidence locator.
- Do not modify another reviewer's row. Add your own row using your reviewer ID.
- Flag suspected cohort reuse rather than resolving it yourself.

## Review rules

- Student clinical disagreements: discuss first, then flag for Mihir adjudication.
- Technical access/reproducibility issues: flag for Sarthak review.
- Protocol/codebook changes require a dated entry in the amendments log.

## Data and copyright

Do not commit images, patient data, raw datasets, credentials, model weights, or restricted-access material. Cite papers and link to official resources; do not upload publisher PDFs without explicit redistribution permission.
