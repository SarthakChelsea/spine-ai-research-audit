# Open Resources for AI in Spine Imaging

## What we are trying to find

This project asks a practical clinical question:

> Which publicly available spine-imaging datasets and pretrained AI models can answer particular research or clinical questions, and which important questions can they *not* answer?

We are not making a list of datasets. We are mapping what each resource genuinely contains and whether it is fit for use. A key priority is whether resources link imaging to pain, function, psychiatric or other relevant comorbidities, medications, treatment, complementary/integrative care, treatment response, and follow-up.

The likely gap we are testing is that public resources may be useful for image-analysis tasks (for example segmentation or localization) but usually cannot support treatment-selection, prognosis, pain, or treatment-response research.

## The only folders and files students need

- `papers/` — save the PDF of each paper and any important official dataset/model documentation. Name files `P001_short-title.pdf`, `P002_short-title.pdf`, etc.
- `PAPERS_TO_REVIEW.xlsx` — update this daily. It assigns papers and shows progress.
- `EXTRACTION_FORM.xlsx` — enter one row for every *unique dataset or model*, not one row for every paper.
- `MIHIR_DECISIONS.md` — do not answer these yourself. Flag a paper as needing discussion instead.

## What sources should be reviewed?

### 1. Primary dataset papers and official dataset pages

Include human spine-imaging datasets that are publicly available or accessible after registration/application. Look for MRI, CT, radiographs, DEXA, PET/CT, or other human spine imaging.

For each unique dataset, extract:

- dataset name, official link, and access type;
- number of unique patients **separately** from number of examinations/scans/images;
- cohort: age group, diagnoses, setting, country/site(s), and whether pre- or post-operative;
- spine region and imaging modality;
- labels/annotations and their level (patient, study, vertebra, disc, image);
- clinical information, especially the pain/treatment/follow-up fields below;
- one sentence on what it is suitable for and one sentence on what it cannot support.

### 2. Supporting publications for an already-known dataset

These may add information about cohort, labels, or follow-up. Do **not** create a second extraction row if it is the same underlying dataset. Add the paper to the tracker and note the existing dataset name.

### 3. Pretrained spine-AI model papers and official code/model pages

Include a model only if it is intended for spine imaging and has a paper, public code, public weights, or a clear official model page.

For each unique model, extract:

- model name and official link;
- intended task, spine region, modality, inputs, and outputs;
- training dataset(s) stated by the authors;
- whether code and weights are publicly available;
- internal/external validation stated in the paper;
- what it is suitable for and what it is not suitable for.

Students should only report what the source states. Sarthak will later test installation, checkpoints, and inference.

### 4. Reviews

Use reviews to find candidate datasets/models and references. Do not treat a review as proof that a resource is public or usable; verify the primary publication or official page.

## What must be extracted about clinical information

For every field below, choose exactly one status in the extraction sheet:

- **Reported** — clearly available and described.
- **Partly reported** — some information is available, but incomplete or only for a subset.
- **Not reported** — no information found after reading the paper/supplement/official documentation.
- **Unclear** — the source hints at it but does not allow a confident decision.

Add a brief detail and a page/table/supplement location. “Not reported” is an important result, not a missing entry.

Required clinical fields:

- pain measurements or symptoms;
- function/disability or patient-reported outcomes;
- psychiatric and other relevant comorbidities;
- medication information;
- treatments received;
- complementary/integrative treatments (for example acupuncture, chiropractic care, yoga, mindfulness, massage, or other non-pharmacologic care, when explicitly stated);
- timing of treatment relative to imaging;
- response to treatment;
- complications, reoperation, or subsequent procedure;
- follow-up duration and completeness.

Do not infer response merely because a patient had surgery, or infer treatment timing because a dataset contains postoperative scans.

## Simple screening protocol

1. Read the title and abstract. Mark **Exclude** only if it is clearly not a human spine-imaging dataset/model.
2. Read the full paper plus supplement and official source page. Save the PDF/documentation in `papers/`.
3. Check whether the paper describes a new unique dataset/model or a secondary use of one already listed.
4. Enter the resource in `EXTRACTION_FORM.xlsx` only if eligible. Cite the exact supporting page/table.
5. If unsure, mark `Needs discussion` in the tracker rather than guessing.

## Basic exclusions

Exclude animal-only resources, synthetic-only data, non-spine datasets without a separable spine cohort, papers with no identifiable resource, and duplicate descriptions of the same resource. Do not exclude a dataset simply because it lacks outcomes; record that absence.

## Two required conclusion sentences for every resource

Complete both fields in the extraction form:

1. **Suitable for:** the actual use supported by its imaging, labels, and metadata.
2. **Not suitable for:** the clinical/computational use it cannot validly support, especially if pain, treatment, response, or follow-up are absent.

## Review process

Two students independently screen and extract priority papers. Resolve disagreements by discussion; Mihir decides clinical interpretation when needed. Sarthak handles resource verification, deduplication, technical model testing, analysis, and any empirical experiment.
