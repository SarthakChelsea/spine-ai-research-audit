# Ten-Resource Calibration Pilot

## Aim

Test whether the screening form, clinical codebook, and technical audit can be used consistently before full review.

## Pilot composition

- 6 primary dataset papers representing different modalities and regions;
- 2 official dataset repository/documentation records; and
- 2 public pretrained-model papers/repositories.

## Process

1. Both students independently screen and extract the same resources.
2. Sarthak independently conducts access and technical checks.
3. Compare eligibility, population, imaging, label, pain, treatment, response, follow-up, and fitness fields.
4. Resolve discrepancies; record what changed in the codebook.
5. Freeze `protocol_v1.0` and templates only after the pilot is workable.

## Calibration targets

Aim for at least 80% agreement on core eligibility, modality, region, resource type, pain-data presence, treatment-data presence, follow-up-data presence, and final `not_supported` versus potentially-supported classification. Use consensus and Mihir adjudication for clinical ambiguities rather than forcing agreement.
