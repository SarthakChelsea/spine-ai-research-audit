# Medical Student Screening and Extraction Manual

## Purpose

Your role is to determine whether each public spine-imaging resource contains clinically meaningful information needed for pain, function, treatment, and outcome research—not simply whether it has images and labels.

## Three rules

1. Extract only what is evidenced in the paper, supplement, or official documentation.
2. Use one of four status values for every clinical field: `reported`, `partially_reported`, `not_reported`, or `unclear`.
3. Cite the exact evidence location for every decision: page, table, supplement, README heading, or data dictionary field.

## Phase 1: title/abstract screen

Include for full text if the source plausibly describes a human spine-imaging dataset or public pretrained model with an identifiable resource. Mark `unclear` if a dataset may be present but cannot be identified from the abstract. Exclude animal, phantom, synthetic-only, non-spine, private-only, and duplicate resources.

## Phase 2: full-text extraction

For each resource, complete the dataset/model identity fields, cohort fields, imaging fields, annotation/reference-standard fields, and all clinical-audit fields in the templates.

### Required clinical checks

Check separately for:

- pain presence, location, duration, severity, instrument, and time point;
- disability/function and quality of life;
- neurologic findings;
- depression, anxiety, PTSD, sleep disorder, substance-use disorder, opioid-use disorder, and other relevant comorbidities;
- medication exposure, especially opioids and non-opioid analgesics;
- conservative management, injections, procedures, and surgery;
- physical therapy, exercise, acupuncture, chiropractic/manual therapy, massage, yoga, mindfulness/CBT, pain psychology, multidisciplinary pain care, and other stated complementary/integrative treatment;
- treatment timing relative to index imaging;
- response definition and timing;
- complications, reoperation/subsequent procedure, and follow-up duration/completeness.

## Do not infer

- A surgery label does **not** establish treatment response.
- A medication list does **not** establish treatment timing, exposure duration, or response.
- A diagnosis label does **not** establish pain severity or functional impairment.
- A longitudinal imaging series does **not** establish clinical follow-up unless linked outcome data are present.
- Similar label names are not automatically equivalent across datasets.

## Final two statements for each dataset

Write both statements using evidence from the resource:

1. **Supported use:** “This dataset is suitable for ___ because it contains ___.”
2. **Unsupported use:** “This dataset is not suitable for ___ because it lacks ___.”

## Independent review and adjudication

Two students extract independently. Keep original entries. Resolve straightforward discrepancies by consensus. Escalate clinical-definition or clinical-use disagreements to Mihir. Escalate technical-access questions to Sarthak.
