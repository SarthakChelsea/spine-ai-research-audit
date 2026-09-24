# Protocol v0.1

## Review design

Systematic scoping review, resource registry, clinical fitness-for-use audit, technical accessibility/reproducibility audit, and focused empirical transfer study. Report according to PRISMA-ScR and preserve complete searches according to PRISMA-S.

## Primary objective

Determine whether publicly discoverable human spine-imaging datasets and pretrained AI models contain the imaging, labels, clinical context, and technical materials needed for specified research tasks.

## Clinical objectives

1. Quantify the availability of pain, functional, psychiatric/comorbidity, medication, treatment, response, complication, reoperation, and longitudinal follow-up data.
2. Determine whether individual imaging examinations can be linked to management decisions and later outcomes.
3. Determine whether datasets can support pain phenotyping, prognosis, treatment selection, treatment-response, or complementary/integrative-care research.

## Eligibility

### Include

- Human spine-focused imaging datasets with a verifiable public, registration-controlled, application-controlled, or historically public access path.
- Cervical, thoracic, lumbar, sacral, whole-spine, or spinal-cord imaging when the dataset is spine focused.
- Radiographs, CT, MRI, PET/CT, DXA/DEXA, EOS, fluoroscopy, or comparable clinical imaging.
- Publicly described pretrained models with a verifiable intended spine-imaging use; code and weights are audited separately rather than required for inclusion.

### Exclude

- Animal-only, phantom-only, or simulation-only resources.
- Synthetic data without identifiable human imaging.
- Non-spine datasets without a separable spine cohort.
- Papers without a verifiable underlying dataset/model.
- Duplicate publications describing the same resource, except as linked supporting evidence.

## Evidence sources

Literature databases: PubMed/MEDLINE, Embase, Scopus, Web of Science, IEEE Xplore, and ACM Digital Library when relevant.

Resource sources: TCIA, Grand Challenge, PhysioNet, Zenodo, Figshare, Kaggle, Hugging Face, GitHub, RSNA resources, Stanford AIMI, SpineWeb, and institutional portals.

## Unit of analysis and deduplication

Each unique dataset version and unique model version receives one primary registry ID. Secondary papers are linked in `dataset_publications.csv` or `model_publications.csv`. Potential cohort reuse is logged and adjudicated; publications must never be counted as independent cohorts by default.

## Outcomes

The primary result is a task-specific fitness classification, not a pooled performance metric. Absence of a required clinical element is a valid and reportable finding.

## Fitness gate

| Proposed use | Required evidence |
|---|---|
| Segmentation/localization | Imaging plus spatial ground truth |
| Finding detection/grading | Imaging plus explicit label definition and reference standard |
| Pain phenotyping | Imaging linked to pain presence, severity/location/duration, or a validated pain instrument |
| Prognosis | Baseline imaging linked to a future outcome and follow-up timing |
| Treatment selection | Imaging, defined treatment, timing, major confounders, and outcome |
| Treatment response | Baseline status, defined treatment/timing, post-treatment outcome, and follow-up completeness |
| Integrative care | Defined complementary/integrative treatment, timing/exposure, and outcome |

## Interpretation boundary

Availability of observational treatment data can support descriptive or association-focused analyses. It does not by itself establish causal treatment effects.
