# Open Resources for AI in Spine Imaging

## Working title

**Open Resources for Artificial Intelligence in Spine Imaging: A Systematic Scoping Review and Empirical Fitness-for-Use Audit of Public Datasets and Models**

## Core question

Which publicly discoverable spine-imaging datasets and pretrained AI models are actually accessible, technically reusable, and clinically fit for specified imaging, pain, treatment, and integrative-care research questions?

## Why this project is different

This is not a narrative list of public datasets. It is a resource-level audit of:

- clinical fitness for pain, function, treatment, response, and complementary/integrative-care research;
- label definitions and cross-dataset harmonizability;
- actual access, licensing, documentation, and reproducibility;
- model code, weights, checkpoint loading, and sample inference; and
- one pre-specified, compatibility-aware transfer/generalization experiment.

The project is separate from the lumbar-MRI representation-benchmarking study. It does not compare encoders as its primary contribution.

## Main deliverables

1. PRISMA-ScR flow diagram and reproducible search record.
2. Registry of unique public spine-imaging datasets.
3. Registry of public pretrained spine-AI models.
4. Pain, treatment, outcome, and integrative-care availability audit.
5. Label ontology and harmonization map.
6. Dataset/model accessibility and reproducibility audit.
7. Task-specific fitness-for-use matrix.
8. Focused empirical cross-resource transfer study.

## Team roles

| Role | Responsibility |
|---|---|
| Medical students | Independent screening, full-text clinical extraction, clinical-label interpretation, cohort-reuse flags, and use-case classification. |
| Mihir Gupta | Senior clinical adjudication, clinical-variable definitions, interpretation of pain/integrative-care fitness, and manuscript oversight. |
| Sarthak Mahapatra | Resource discovery, dataset/model deduplication, access/download testing, reproducibility audit, ontology implementation, analysis, visualizations, empirical experiment, and computational documentation. |

## Repository rules

- The unit of analysis is a **unique dataset** or **unique model**, not a paper.
- Do not upload patient data, downloaded datasets, model weights, credentials, or protected health information.
- Do not upload publisher PDFs unless redistribution is explicitly permitted. Store citations and stable links instead.
- Every extraction must carry a source locator: page, table, supplement, README section, or repository file.
- Use `reported`, `partially_reported`, `not_reported`, or `unclear`; never leave a clinical field blank.

## Project status

Infrastructure and pilot materials prepared. The next milestone is a 10-resource calibration pilot before full screening.
