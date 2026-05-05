# 5x5 Risk Matrix

The scoring system used for every hazard in the Risk Prioritisation Table (Section 4 of the RAMS).

5x5 is the construction-industry norm in ROI and the UK and matches what most PSCSs expect to see.

## Likelihood scale

| Score | Label | Meaning |
|-------|-------|---------|
| 1 | Rare | Very unlikely; has not happened on similar jobs |
| 2 | Unlikely | Possible but unusual |
| 3 | Possible | Could happen occasionally |
| 4 | Likely | Happens regularly on similar jobs without controls |
| 5 | Almost certain | Expected unless actively controlled |

## Severity scale

| Score | Label | Meaning |
|-------|-------|---------|
| 1 | Negligible | No injury or trivial first aid |
| 2 | Minor | First aid, no lost time |
| 3 | Moderate | Lost-time injury, no lasting harm |
| 4 | Major | Serious injury, possible permanent effect |
| 5 | Catastrophic | Fatal or multi-casualty |

## Risk rating (Likelihood x Severity)

| Score range | Band | Action |
|-------------|------|--------|
| 1 to 4 | Low (green) | Acceptable with routine controls |
| 5 to 9 | Medium (yellow) | Additional controls if practicable |
| 10 to 14 | High (amber) | Controls mandatory before work starts |
| 15 to 25 | Very High (red) | Stop. Redesign method or do not proceed |

## Worked example

A fitter is installing flat-cut acrylic letters at 3.5m above a live retail shop floor on a Saturday morning.

**Hazard:** Fall from ladder.

**Initial scoring (no controls):**
- Likelihood: 3 (Possible)
- Severity: 4 (Major)
- Initial rating: 12 (High, amber)

**Controls applied:**
- Mobile tower in place of ladder for sustained work above 2m
- PASMA-certified fitter assembling tower
- Tower inspected before use, recorded
- Cordon at 2m radius, two A-frames, "Caution: overhead work" signage
- Two-fitter lift for any panel above 1m

**Residual scoring:**
- Likelihood: 1 (Rare, given tower + competent assembly + cordon)
- Severity: 3 (Moderate, residual fall from tower platform unlikely but not impossible)
- Residual rating: 3 (Low, green)

The residual moves from amber to green because the controls genuinely change the likelihood. If the controls had been "fitter to be careful", the likelihood score would not move and the residual would still be amber. That would be a flag back to the responsible person to either rework the method or escalate the hazard.

## Residual risk discipline

The most common 5x5 mistake is to apply controls and then score the residual the same as the initial. If controls do not move the score, they are not real controls.

Equally, if a residual score is dropped to 1/1 across the board, the matrix is being used as a comfort blanket. Honest residual scoring is the only reason the matrix earns its place in the document.

## Migration note from 3x3

Some legacy templates use a 3x3 matrix (Low / Medium / High on each axis). For reference:

| Old (3x3) | 5x5 equivalent |
|-----------|----------------|
| Low / Low | L=2, S=2, R=4, Band Low |
| Low / Medium | L=2, S=3, R=6, Band Medium |
| Medium / Medium | L=3, S=3, R=9, Band Medium |
| Medium / High | L=3, S=4, R=12, Band High |
| High / High | L=4, S=4, R=16, Band Very High |

When reviewing an old RAMS for repurpose, re-score the matrix from the hazard list rather than mapping cell-for-cell.
