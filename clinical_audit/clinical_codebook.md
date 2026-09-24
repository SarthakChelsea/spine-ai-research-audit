# Clinical Codebook: Pain, Treatment, and Integrative-Care Audit

## Status vocabulary

| Status | Meaning |
|---|---|
| `reported` | Explicitly available with enough detail for the stated field. |
| `partially_reported` | Present but incomplete, aggregate-only, untimed, or not linkable to index imaging. |
| `not_reported` | Checked in paper/supplement/official documentation and absent. |
| `unclear` | Mentioned ambiguously or insufficiently described. |

## Pain data

Record pain presence, location, duration, severity, measure/instrument, baseline timing relative to index imaging, and repeated time points. Examples of valid measures include NRS, VAS, PROMIS Pain Interference, and explicitly named pain scales. “Back pain cohort” alone is `partially_reported` unless individual pain data are available.

## Functional and patient-reported outcomes

Record ODI, NDI, PROMIS function, Roland-Morris, EQ-5D, SF-36, walking tolerance, work status, activities of daily living, or other explicitly defined outcomes. Record measurement timing and completeness.

## Psychiatric and biopsychosocial variables

Record depression, anxiety, PTSD, sleep disorder/insomnia, substance-use disorder, opioid-use disorder, chronic-pain history, pain catastrophizing/fear avoidance, socioeconomic factors, and occupational factors when available. State whether each is patient level and time-linked to imaging.

## Treatment categories

### Conventional

- medication: NSAIDs, acetaminophen, neuropathic agents, muscle relaxants, opioids;
- procedure: epidural steroid injection, nerve block, ablation, other intervention;
- surgery: decompression, discectomy, fusion, deformity correction, or defined alternative.

### Complementary/integrative

- physical therapy/rehabilitation;
- exercise therapy;
- yoga;
- acupuncture;
- chiropractic/manual therapy;
- massage;
- mindfulness/meditation;
- cognitive behavioral therapy/pain psychology;
- multidisciplinary pain program;
- cannabinoid treatment, when explicitly captured;
- other nonpharmacologic intervention exactly as stated.

Never assign “integrative” status based on assumption. Extract the stated intervention, intensity/dose, start time, duration, adherence/completion, co-interventions, and provider/setting if available.

## Response and follow-up

Record the response definition, baseline measure, post-treatment measure, time points, complications, reoperation/subsequent procedure, follow-up duration, and loss-to-follow-up/completeness. A treatment-response task requires baseline status, treatment/timing, post-treatment outcome, and follow-up completeness.

## Fitness interpretation

| Task | Minimum evidence | If absent |
|---|---|---|
| Pain phenotyping | Imaging linked to individual pain data | Not supported |
| Functional-outcome study | Imaging linked to functional/PRO data | Not supported |
| Prognosis | Baseline imaging linked to future outcome and time | Not supported |
| Treatment selection | Imaging, treatment, timing, confounders, outcome | Not supported |
| Treatment response | Baseline status, treatment/timing, post-treatment outcome, complete follow-up | Not supported |
| Integrative-care study | Defined intervention, timing/exposure, outcome | Not supported |
