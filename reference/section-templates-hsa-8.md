# HSA 8-Section Templates

Fillable scaffolds for the 8-section HSA-aligned RAMS structure. Section order is fixed.

---

## Cover page

```
Risk Assessment Method Statement (RAMS)

Project:               [project_name]
Document number:       [order_number_from_contractor_profile §5]
Client:                [client_name]
Site:                  [site_address_with_eircode]
Document date:         [YYYY-MM-DD]
Revision:              0.1 (draft) | 0.2, 0.3 (review) | 1.0 (issued) | 1.1+ (post-issue revisions)
Prepared by:           [name from contractor profile §2]
Approver:              [name from contractor profile §2]
Distribution:          [list]

Standing exclusions on this RAMS:
- Live electrical work (RECI registered electrician engaged separately)
- Work above [height limit from contractor profile §3] (within insurance cover)
- [any other standing exclusion from contractor profile §10]
```

Checks:

- [ ] Document number tied to job-tracking reference
- [ ] Standing exclusions block present and accurate
- [ ] Revision number set

---

## Section 1: Contractor Details

```
Trading entity:        [verbatim, from contractor profile §1]
Registered address:    [from contractor profile §1]
CRO:                   [from contractor profile §1]
VAT:                   [from contractor profile §1]
Business description:  [from contractor profile §1]

Responsible person:    [name and role from contractor profile §2]
Contact:               [phone / email]

Insurance:
  Insurer:             [contractor profile §3]
  Policy number:       [contractor profile §3]
  Period of cover:     [contractor profile §3]
  Employers Liability: EUR [limit] any one claim
  Public Liability:    EUR [limit] each and every occurrence
  Products Liability:  EUR [limit] each and every occurrence
  Height limit:        [limit] metres
  Excess:              EUR [excess]

Safety Statement:      [doc number / version], last reviewed [date] (contractor profile §4)
```

Checks:

- [ ] Trading entity wording verbatim
- [ ] Insurance period of cover current at date of RAMS issue
- [ ] Height limit stated explicitly
- [ ] Safety Statement referenced

---

## Section 2: Site and Work Activity Information

```
Project name:          [name]
Document number:       [order number]
Client:                [client name]
Site address:          [full address with Eircode]

Scope of works:
  [one to three concrete paragraphs: what is being installed, where on site,
   any phasing, sequence, removal of existing items]

Planned start date:    [date]
Planned duration:      [duration]
Working hours:         [in-hours / out-of-hours / overnight]
Number of IQ personnel on site: [n]
Subcontractor crews on site:    [name(s) or "none"]

Site contact on the day:        [name, role, mobile]
Site induction:                 [first-day walk-around with site manager
                                 | formal induction at reception
                                 | formal induction via PSCS portal]
Access route:                   [where to park, enter, carry stock]
Welfare provision:              [toilet / handwashing / break / drinking water]
                                Confirmed with site: [yes / no]
Known constraints:              [restricted headroom, fragile finishes,
                                 noise windows, neighbour sensitivity]
Maximum working height:         [m]
                                Within insurance height limit: [yes / no]
```

Checks:

- [ ] Scope is concrete (not "signage install")
- [ ] Phasing noted if applicable
- [ ] Site contact captured (name + mobile)
- [ ] Welfare confirmed with site, not assumed
- [ ] Max working height within insurance limit

---

## Section 3: Method of Work

```
Check-in:
  [arrival procedure: reception, security, site contact name and phone]

Pre-start:
  - Lead fitter conducts RAMS briefing with all operatives.
  - Operatives sign acknowledgement sheet (Appendix E).
  - PPE donned per Section 6.
  - Dynamic risk assessment on arrival: lead fitter walks the area,
    confirms conditions match the survey, amends RAMS on the day if not.

Tasks:
  1. Check in with Security / Reception.
  2. Arrive on-site, locate work area.
  3. Complete site induction if not already done.
  4. Conduct dynamic risk assessment on arrival.
  5. Assess area for safety requirements.
  6. Cordon off area with barriers (not tape alone where public present).
  7. Set up access equipment ([ladder / mobile tower / MEWP category])
     and inspect before use.
  8. [HOLD POINT if applicable: confirm RECI electrician has isolated
     and locked off any existing mains-powered fitting before fitter
     touches it.]
  9. Apply fixings per manufacturer method ([fixing detail]).
  10. Attach signage to fixings.
  11. Clean as you go.
  12. Take photos (before, during, after).
  13. [HOLD POINT if applicable: hand back to RECI electrician for
      reconnection of new mains-powered unit.]
  14. Remove cordon and access equipment, reinstate the area.
  15. Check out with Security / Reception.

In-progress controls:
  - Cordon maintained throughout.
  - Public exclusion as required (see risk matrix entries for live retail
    / hospitality / public space).
  - Housekeeping: offcuts and packaging bagged immediately.

Clean-up:
  - Clean as you go: substrate wiped, debris bagged, no tools left
    on the floor.
  - Waste routed to site bins unless specified otherwise.
  - Old signage removal: [taken away on van | left in service yard
    for client disposal | not applicable].

Check-out:
  - Sign out at reception or with site contact.
  - All tools and equipment accounted for.
  - Photographs sent to project manager same day.

Estimated completion time: [hours / days, including contingency]
```

Checks:

- [ ] "Fitter" used in singular unless multi-fitter confirmed
- [ ] Blades specified as retractable (in tools list, Section 4)
- [ ] Cut-resistant gloves referenced (in PPE, Section 6)
- [ ] Steps tailored to the actual job (not generic boilerplate)
- [ ] Dynamic risk assessment on arrival present
- [ ] Hold points called out for RECI work if applicable

---

## Section 4: Hazard Identification and Plant / Equipment Requirements

### Risk Prioritisation Table (5x5)

| # | Activity | Hazard | Who affected | Initial L (1-5) | Initial S (1-5) | Initial Rating | Controls | Residual L | Residual S | Residual Rating |
|---|----------|--------|--------------|-----------------|-----------------|----------------|----------|------------|------------|-----------------|
| 1 |          |        |              |                 |                 |                |          |            |            |                 |
| 2 |          |        |              |                 |                 |                |          |            |            |                 |
| 3 |          |        |              |                 |                 |                |          |            |            |                 |

Seed from `risk-library.md`. Adjust likelihood and severity per site. Apply controls. Score residual. Anything residual-High or Very High is a flag back to the responsible person before work proceeds.

### Plant and Equipment Register

| Item | Inspection requirement | Last inspection | Next due |
|------|------------------------|-----------------|----------|
| Ladder ([type]) | Pre-use visual; quarterly recorded; annual formal | [date] | [date] |
| Mobile tower ([model]) | PASMA pre-use inspection; recorded weekly | [date] | [date] |
| MEWP ([category, model]) | Pre-use visual; Thorough Examination every 6 months (GA1-equivalent) | [date] | [date] |
| Power tools (drill, impact, etc.) | PAT every 12 months | [date] | [date] |
| Harness (if used) | Pre-use; formal inspection every 6 months | [date] | [date] |

### Tools list

- Retractable blades (always retractable)
- Drill / impact driver
- Spirit level / laser level
- Tape measure
- [Fixing components per spec]
- [Adhesives / tape per spec, e.g. 3M VHB]

Checks:

- [ ] At least top 5 site-relevant hazards listed
- [ ] Controls are specific (who does what, with what), not boilerplate
- [ ] Residual risk column populated
- [ ] Plant inspection records attached (Appendix B) or referenced

---

## Section 5: Training Requirements

For every fitter named on this RAMS, evidence held:

| Fitter | Safe Pass | Manual Handling | Working at Heights | IPAF (cat) | PASMA | Abrasive Wheels | FAR |
|--------|-----------|-----------------|--------------------|-----------:|-------|-----------------|-----|
| [Name 1] | [card no, expiry] | [expiry] | [expiry] | [cat, expiry] | [expiry] | [expiry] | [expiry] |
| [Name 2] |                  |          |          |          |       |                 |     |

At least one fitter on site must hold a current First Aid Responder certificate.

Records held by [tracker maintainer from contractor profile §6]. Certificates attached as Appendix G.

Checks:

- [ ] Every fitter row populated, no expired certifications
- [ ] At least one FAR present on site
- [ ] Card numbers captured (or "on file with [tracker maintainer], last verified [date]")

---

## Section 6: Personal Protective Equipment (PPE)

Baseline PPE (every install):

- Cut-resistant gloves
- Safety glasses
- Hi-vis vest
- Safety boots

Task-specific PPE for this job:

- [ ] Hard hat: active construction site, overhead work by others
- [ ] Hearing protection: sustained power tool use
- [ ] Dust mask (FFP2 minimum): drilling / cutting without extraction
- [ ] Respirator (half-mask A1P2 or A2P2): prolonged solvent use
- [ ] Harness (full body, energy-absorbing lanyard): height work without collective protection
- [ ] Knee pads: floor work
- [ ] Nitrile gloves: solvents / cleaners (over cut-resistant where needed)

PPE inspection responsibility: lead fitter, pre-use.

Checks:

- [ ] Baseline 4 items listed every time
- [ ] Task-specific items match hazards in Section 4
- [ ] Inspection responsibility named

---

## Section 7: Emergency Procedures and Welfare Requirements

Emergency contacts:

| Contact | Number |
|---------|--------|
| Site manager | [name, mobile] |
| Project Manager (contractor) | [name, mobile from contractor profile §2] |
| Emergency services | 112 / 999 |
| Nearest A&E | [hospital name and distance from site] |

First aid:

- Lead fitter holds current FAR certificate.
- First aid kit carried in van and on lead fitter's person.
- Site first aid point / AED location: [if known].

Fire:

- Evacuation route from work area to site assembly point: [described].
- Lead fitter familiar with assembly point (confirmed at induction or walk-around).

Spill:

- Small adhesive / solvent spill kit carried in van.
- Larger spills reported to site manager and contained.

Incident reporting:

- Any injury or dangerous occurrence reported to [responsible person from contractor profile §2] same day.
- Reportable incidents: HSA IR1 within 10 working days. Dangerous occurrences: IR3.
- Near-misses logged in contractor's near-miss register and reviewed at next toolbox talk.

Welfare:

- Toilet: [confirmed location]
- Handwashing: [confirmed]
- Break area: [confirmed]
- Drinking water: [confirmed available]
- Out-of-hours work: welfare confirmed available out of hours [yes / no]

Lone working (if applicable):

- Fitter checks in with [responsible person] on arrival and departure.
- Mobile charged, site contact number held.
- No lone working at height over 3m.

Checks:

- [ ] FAR named
- [ ] Site assembly point captured
- [ ] Welfare confirmed (each line), not assumed
- [ ] Incident reporting path named to a person, not a role

---

## Section 8: Sign-off and Appendices

```
RAMS Briefing and Acknowledgement

Project: ____________________    Document No: ____________
Date of briefing: ____________   Briefed by (lead fitter): ____________

Operatives below have received the RAMS briefing, understand the content,
and will comply with the method statement and controls.

| Name | Company | Role | Signature | Date |
|------|---------|------|-----------|------|
|      |         |      |           |      |

Responsible Person sign-off (contractor):
Name: [from contractor profile §2]
Signature: __________________    Date: ___________

PSCS / Main Contractor acknowledgement (where applicable):
Name: __________________    Role: __________________
Signature: __________________    Date: ___________
```

Appendices index (tick attached, leave blank if N/A):

- [ ] A. Site-specific drawings / layouts
- [ ] B. Plant and equipment inspection records
- [ ] C. SDS for substances used on this job (from contractor profile §7)
- [ ] D. Permit-to-work forms (hot work, work at height, out-of-hours)
- [ ] E. Toolbox talk record
- [ ] F. Insurance certificate (current)
- [ ] G. Competency certificates for named fitters

Checks:

- [ ] Sign-off page present (blank acceptable at issue)
- [ ] Appendices index present
- [ ] Permit forms attached if hot work / work at height / out-of-hours
- [ ] Current insurance certificate attached

---

## Pre-issue validation checklist

Run before producing the .docx. Anything failing is a blocker.

- [ ] All 8 sections present, in order
- [ ] Cover page with document number, revision, exclusions block
- [ ] Trading entity wording verbatim
- [ ] Insurance block current (period of cover not expired)
- [ ] Height limit stated and within job height
- [ ] Risk matrix populated, residuals scored, no Very High residuals unaddressed
- [ ] At least one named fitter with valid Safe Pass + Working at Heights (if any height) + Manual Handling
- [ ] At least one FAR on site
- [ ] Cut-resistant gloves listed in PPE
- [ ] Retractable blades specified in tools
- [ ] RECI exclusion stated on cover and in Method of Work hold-points if mains-powered work involved
- [ ] Sign-off page present
- [ ] Appendices index present, items attached or marked N/A
- [ ] Irish English throughout, no em-dashes
