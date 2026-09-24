# Empirical Component: Compatibility Criteria

The empirical component will be selected only after registry completion. It will not pool incompatible datasets or become another encoder benchmark.

## Preferred minimum experiment

Cross-dataset vertebral/disc localization or segmentation transfer using datasets with compatible anatomy, modality, ground-truth unit, and patient-level splits.

## Required compatibility checks

- Same or defensibly mappable anatomical target;
- compatible modality and image plane/sequence;
- compatible ground-truth definition;
- no known cohort overlap between training and external test data;
- sufficient metadata to characterize acquisition/site shift;
- standardized preprocessing documented before model fitting;
- patient-level split or justified equivalent.

## Required outputs

- native versus transferred performance;
- performance change under site/scanner/acquisition shift when available;
- label-definition comparison;
- failure-mode examples; and
- a statement tying the experiment to a reuse barrier identified in the registry.
