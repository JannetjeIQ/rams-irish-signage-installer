# RAMS Specialist for Irish Signage Installers

A drop-in Claude folder that turns Claude into an experienced RAMS author for signage installation work in the Republic of Ireland. Aligned to the HSA RAMS Guidance Document, 8-section structure, 5x5 risk matrix.

## Who this is for

Small to mid-sized Irish signage contractors (sole traders, fit-out crews, signage SMEs) who:

- Get pulled onto construction sites and commercial fit-outs and need a compliant RAMS for every job
- Don't have a full-time H&S manager
- Are tired of starting every RAMS from a blank Word document

Not for: civils, scaffolding-only, electrical, demolition. Signage and adjacent install work only.

## How to use it (under 5 minutes)

1. **Clone or download this folder.**
2. **Open `reference/your-contractor-profile.md` and fill in the placeholders** with your company name, registered address, CRO/VAT, insurance details, named Project Manager, and competency-tracker owner. This is a one-time setup. The specialist reads from this file every time.
3. **Drop the whole folder into a new Claude Project** (use Claude.ai Projects, or paste the files into a Claude Code workspace).
4. **Ask:** "Draft a RAMS for [job description]" (for example: "Draft a RAMS for a fascia replacement at a Dublin retail unit, single fitter, 4m max height, two-day install").
5. **Answer the gap questions** the specialist asks (site contact, induction route, max height, access equipment, permits, fitter names, etc.).
6. **Get back a draft RAMS** in HSA 8-section format with a populated 5x5 risk matrix. Iterate inline. When happy, paste into Word as A4.

## What you get

- Compliant 8-section RAMS structure (HSA-aligned)
- Populated 5x5 risk matrix with residual-risk column
- Site-specific install steps (not boilerplate)
- Hazards drawn from a curated signage-install risk library
- Permit-to-work flagging (hot work, working at height, out-of-hours, lone working, confined space)
- Competency / training requirements per fitter
- Sign-off sheet template
- Appendix index (drawings, SDS, permits, insurance, competency certs)

## What it will not do

- Electrical isolation or live disconnect work (always a third-party RECI registered electrician in ROI)
- Anything above your insurance height limit (the specialist will flag and stop)
- Civils, scaffolding-only, demolition (out of scope)
- UK or NI sites without you swapping the legal context (HSA → HSE / CDM 2015)

## Methodology

This specialist uses Interpretable Context Methodology (ICM): folders as architecture, one job per file. Five files at root, source material in `reference/`. Easy to audit, easy to update, easy to fork for your own niche.

## File map

```
rams-irish-signage-installer/
├── README.md                 ← you are here
├── identity.md               ← who the specialist is, what they cover
├── rules.md                  ← how they respond, always/never list
├── examples.md               ← three worked example interactions
└── reference/
    ├── your-contractor-profile.md     ← FILL THIS IN FIRST
    ├── legal-context-ireland.md       ← HSA framework, statutes, when a RAMS is required
    ├── section-templates-hsa-8.md     ← the 8-section scaffold
    ├── risk-matrix-5x5.md             ← scoring rules and bands
    ├── risk-library.md                ← signage-install hazards with controls
    ├── competency-matrix-ireland.md   ← Safe Pass, IPAF, PASMA, FAR, etc.
    ├── permits-framework.md           ← when each permit fires
    └── intake-questions.md            ← the question list the specialist works through
```

## Customising the specialist

The whole point of ICM is that you can update one file without breaking the others.

- New hazard you keep hitting? Add to `reference/risk-library.md`.
- New competency requirement on a client's site? Add a row to `reference/competency-matrix-ireland.md`.
- Working in NI? Duplicate `reference/legal-context-ireland.md`, swap HSA references for HSE / CDM 2015.
- Want a different standing rule (e.g., "we always do two-fitter installs")? Edit `rules.md`.

## Credits and licence

Built by Jannetje van Leeuwen ([IQ Branding Solutions](https://iqbrandingsolutions.ie)) for the Clief Notes Lyceum Weekly Competition #3 (May 2026). Uses ICM (Interpretable Context Methodology) developed by Jake Van Clief.

Source material: HSA RAMS Guidance Document (Construction Safety Partnership, Ireland), HSA Interactive Template, S.I. No. 291 of 2013 Construction Regulations.

Released under MIT licence. Use it, fork it, ship it. No warranty: a RAMS produced with this specialist still requires sign-off by a competent person in your organisation before it goes to a client or PSCS.
