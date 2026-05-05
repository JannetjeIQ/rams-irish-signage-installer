# Intake Questions

The strict question set the specialist works through before drafting a RAMS. Two paths:

- **Fast path (§1):** the user pastes an order from their job-tracking system; the specialist fills the gaps with a tightly-scoped follow-up.
- **Full intake (§2):** no order yet; the user answers from scratch.

The order in this file is also the order the specialist asks. A downstream tool (form UI, web app, internal AI agent) can mirror this file directly as field definitions.

---

## 1. Fast path: from a pasted order

### 1.1 What gets pulled from the order

When the user pastes an order or order summary, the specialist extracts:

| Field | Order source |
|-------|--------------|
| Document number for the RAMS | Order reference number |
| Project name | Job title or description heading |
| Client name | Customer account |
| Order date | (not the same as install date; confirm separately) |
| Site address | Delivery / install address if populated |
| Initial scope | Line items and job description |
| Rep / account owner | Salesperson code (informational only) |

### 1.2 Gap questions (always asked, even with a complete order)

Sent in **one consolidated message**, not one at a time.

1. **Install date.** When is the fitter on site? (If different from order date.)
2. **Working hours.** Standard hours, out-of-hours, overnight?
3. **Site contact on the day.** Name, role, mobile.
4. **Site induction.** Required? If yes, route (reception, contractor portal, site manager). If not, default to "first-day walk-around with site manager".
5. **Access route.** Where does the fitter park, enter, carry stock?
6. **Welfare.** Toilet, handwashing, break area, drinking water; confirmed on site?
7. **Maximum working height.** Within the contractor's insurance height limit?
8. **Access equipment.** Ladder, mobile tower, MEWP (which category)? Scaffold?
9. **Public exposure.** Live retail, hospitality, transport, healthcare, event? Cordon plan?
10. **PSCS appointed.** Who is PSCS / main contractor? Any site-specific rules to read?
11. **Fitters on the job.** Names; competency status confirmed (Safe Pass, Manual Handling, Working at Heights, IPAF if MEWP, PASMA if tower, FAR for at least one).
12. **Substances beyond the standard SDS set.** Anything outside the contractor's standard adhesive, IPA, sealant?
13. **Permits required.** Hot work, work at height, confined space, out-of-hours, lone working?
14. **Client-imposed RAMS template.** Is the main contractor or client requiring submission on their template?
15. **Anything unusual.** Restricted headroom, fragile finishes, noise windows, neighbour sensitivities, infection-control awareness, anything the survey flagged.

### 1.3 Cross-check after gap answers

Before drafting, the specialist confirms:

- [ ] Job height within insurance limit
- [ ] No live electrical work in scope (or RECI electrician booked separately)
- [ ] All named fitters' competencies in date for the work (and for the install date)
- [ ] PSCS lead-time of 3+ working days (flag if shorter)

If any check fails, the specialist surfaces it before drafting.

---

## 2. Full intake (no order)

Used when the job has not been entered into the contractor's system, or when the order description is too thin to draft from.

### 2.1 Project basics

- Project name
- Document number (assign from the contractor's system, or use a sequential RAMS number)
- Client name
- Client contact (name, role, email, phone)
- Date of RAMS issue
- Planned install date(s) and duration
- Planned working hours
- Rep or account owner (informational)

### 2.2 Site

- Full site address (with Eircode)
- Site type (retail unit, office, construction site, event venue, hospitality, healthcare, transport)
- Site contact on the day (name, role, phone)
- Building manager or facilities contact (if different)
- Site induction required? If yes, route
- Access for vehicle and pedestrian
- Welfare confirmed (toilet, handwashing, break area, drinking water)
- Constraints (restricted headroom, fragile finishes, loading limits, noise windows, neighbour sensitivities)
- Live retail, hospitality, healthcare, public exposure level
- Out-of-hours or overnight work? Agreed with site?

### 2.3 Scope and method

- What is being installed (signage type, quantity, substrate, location on site)
- Phasing (one visit vs multiple; sequencing)
- Expected duration on site
- Maximum working height (within insurance limit?)
- Fixing method (VHB tape, screws, split batons, brackets, etc.)
- Any demolition or removal required first
- Any electrical disconnect or reconnect (flag: needs RECI electrician separately)
- Clean-up approach (site bins vs remove off site)

### 2.4 Personnel

- Number of fitters on the job
- Named lead fitter
- Named operatives
- Any subcontracted crew (name, insurance, competency held)
- First Aid Responder on site (named)
- Competency status for each fitter (Safe Pass, Manual Handling, Working at Heights, IPAF as applicable, PASMA as applicable, FAR, Abrasive Wheels as applicable): current and in date

### 2.5 Equipment

- Access equipment (ladder, MEWP category, mobile tower, scaffold)
- Power tools (drill, impact driver, heat gun, grinder, cutter)
- PAT status on tools (last date, next due)
- MEWP Thorough Examination in date (if MEWP used)
- Ladder inspection in date
- Harness formal inspection in date (if used)
- Non-standard substances beyond the default SDS set

### 2.6 Coordination

- PSCS appointed? Name, contact
- Main contractor name and contact
- Lead time to site (flag if shorter than 3 working days for PSCS submission)
- Client-imposed RAMS template? (Attach if yes)
- Site-specific rules to comply with (Construction Phase Plan, contractor handbook)

### 2.7 Hazards specific to this job

Pick from the risk library, plus free text for anything site-specific:

- Work at height (above 2m, above 5m, above 10m; within insurance limit?)
- Manual handling (heavy, awkward, glass, multi-person)
- Cuts (vinyl trimming, sharp substrate edges)
- Electrical adjacency (existing services, power tools)
- Slips and trips (floor state, cable routing)
- Public interaction (live retail, hospitality, transport, healthcare)
- Dust and debris
- Noise
- Vehicle movement (loading bay, car park)
- Adhesive fumes and solvents
- Lone working
- Out-of-hours
- Weather (external installs): wind limit, rain, temperature
- Working over public footpath or roadway
- Site-specific hazard flagged by client or survey

### 2.8 Permits required

Tick where applicable:

- [ ] Hot Work Permit
- [ ] Work at Height Permit
- [ ] Confined Space Permit
- [ ] Out-of-Hours Permit
- [ ] Lone Working Permit

### 2.9 Emergency and welfare

- Nearest hospital with A&E (name, distance from site)
- Site assembly point
- Site first aid location (kit, AED if known)
- Contractor's first aid kit carried in van (default: yes)
- Spill kit carried (default: yes)

### 2.10 Closing

- Responsible person sign-off on this RAMS (default per contractor profile §2)
- Distribution list (client, PSCS, main contractor, fitters, contractor's office)
- Special client requests (format, delivery, sign-off workflow)

---

## 3. Minimum viable RAMS (rapid-turnaround jobs)

When the install is in less than 3 working days, the specialist defaults to:

- All 8 sections present, some thin
- Risk matrix populated with at least the top 5 site-relevant hazards, residuals scored
- Contractor block verbatim
- Insurance block verbatim, current period of cover
- At least one named fitter with valid Safe Pass and Working at Heights (if any height work)
- Sign-off page present (blank acceptable at issue)

The specialist will offer to issue revision 0.2 the evening before the install with anything that was missing.

---

## 4. For downstream automation

This file is structured so that a UI (web form, internal tool, third-party app) can mirror it as field definitions. Each numbered question maps to one field. The fast-path (§1) is the form for users who already have an order in their system; the full intake (§2) is the form for users who do not.

A tool wrapping this specialist should:

1. Render fields per §1 or §2 depending on whether an order is provided.
2. Pass the answer dictionary back to the specialist.
3. Receive the markdown RAMS draft.
4. Render to A4 .docx for distribution.
5. Log the issued RAMS in a central index keyed by document number.
