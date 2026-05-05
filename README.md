# RAMS Specialist for Irish Signage Installers

A drop-in folder that turns Claude into an experienced RAMS author for signage installation work in the Republic of Ireland. Aligned to the HSA RAMS Guidance Document, 8-section structure, 5x5 risk matrix.

**TL;DR:** clone the repo, fill in `reference/your-contractor-profile.md`, drop the folder into a Claude Project (or open in Claude Code), and ask "Draft a RAMS for [job]". See [quickstart.md](quickstart.md) for the 5-minute path.

## Who this is for

Small to mid-sized Irish signage contractors (sole traders, fit-out crews, signage SMEs) who:

- Get pulled onto construction sites and commercial fit-outs and need a compliant RAMS for every job
- Don't have a full-time H&S manager
- Are tired of starting every RAMS from a blank Word document

Not for: civils, scaffolding-only, electrical, demolition. Signage and adjacent install work only.

## How to use it

There are two paths. Both work. They give you different things.

### Path A: Claude Project (claude.ai web)

The path most people will use. Files become attachments to a Project; Claude reads them all into context.

1. **Clone or download this folder** to your machine.
2. **Edit `reference/your-contractor-profile.md` locally** in any text editor. Replace the bracketed placeholders with your details (company name, address, insurance figures, named PM, etc.). See "First-time setup" below for the minimum to fill.
3. **Open claude.ai → Projects → Create project**. Upload all 14 files (drag the folder in, or upload the contents).
4. **Start a chat in the Project**. Ask: "Draft a RAMS for [job description]" (for example: "Draft a RAMS for a fascia replacement at a Dublin retail unit, single fitter, 4m max height, two-day install").
5. **Answer the gap questions** the specialist asks (site contact, induction route, max height, access equipment, permits, fitter names).
6. **Get back a draft RAMS** in HSA 8-section format with a populated 5x5 risk matrix. Iterate inline. Paste into Word as A4 when done.

**Project gotcha:** Claude Projects does not let you edit files in-browser as of May 2026. To update the contractor profile (or any other file), edit on disk locally, then re-upload to the Project to replace the old version.

### Path B: Claude Code (cowork)

The path that uses the methodology as designed. Folder structure is operational, files load on demand, the specialist navigates references organically.

1. **Clone the repo** into your local projects folder.
2. **Edit `reference/your-contractor-profile.md`** as above.
3. **Open the folder in Claude Code** (run `claude` from inside it).
4. **Ask the same first prompt**. The specialist reads files as it needs them, follows the README → identity → rules → reference chain.
5. **Edit, iterate, ship** all in one place. No re-upload step.

If you have Claude Code installed, Path B is the truer ICM experience. If you don't, Path A is fine; you just lose the on-demand-load discipline.

## First-time setup: what to fill in

Before the specialist will draft anything, `reference/your-contractor-profile.md` needs at minimum:

- §1 Company identity (trading name, address, CRO, VAT)
- §2 Responsible person (name, role, contact)
- §3 Insurance (insurer, policy number, period, limits, height limit)
- §5 Job-tracking system (so the specialist knows how to number the RAMS)
- §6 Competency tracker owner

§4 (Safety Statement), §7 (SDS library), §8 (standing crew), §9 (subcontract crews), §10 (extra exclusions) are recommended but not blocking. The specialist will warn but proceed.

**The first prompt without a filled-in profile will refuse to draft.** This is intentional: it stops Claude inventing a contractor name, insurance number, or PM. If you see "I cannot draft until your-contractor-profile.md is populated", you have not done step 2.

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
- UK or NI sites without you swapping the legal context (HSA to HSE / CDM 2015)

## Methodology

This specialist uses Interpretable Context Methodology (ICM): folders as architecture, one job per file. Five files at root, source material in `reference/`. Easy to audit, easy to update, easy to fork for your own niche.

Path A (Project) gets you the content. Path B (Claude Code) gets you the navigation. Both work; the difference is whether the structure carries operational weight or is just an organising convention.

## Acronym glossary (read this if any of the specialist's questions look like alphabet soup)

| Acronym | Meaning |
|---------|---------|
| **RAMS** | Risk Assessment Method Statement (the document this specialist produces) |
| **HSA** | Health and Safety Authority (Ireland's H&S regulator) |
| **PSCS** | Project Supervisor Construction Stage (the safety-coordinator role appointed on construction sites in ROI) |
| **PSDP** | Project Supervisor Design Process (design-stage equivalent of PSCS) |
| **RECI** | Register of Electrical Contractors of Ireland (the registration body for electricians; only RECI-registered electricians can do live electrical work) |
| **FAR** | First Aid Responder (PHECC-accredited certification; at least one FAR must be on site) |
| **IPAF** | International Powered Access Federation (issues MEWP operator licences; categories 1a, 1b, 3a, 3b cover different machine types) |
| **PASMA** | Prefabricated Access Suppliers' and Manufacturers' Association (mobile tower assembly and use certification) |
| **MEWP** | Mobile Elevated Work Platform (scissor lifts, cherry pickers, etc.) |
| **Safe Pass** | Mandatory one-day construction safety awareness card in ROI, issued by SOLAS, valid for 4 years |
| **CSCS** | Construction Skills Certification Scheme (the UK / NI equivalent of Safe Pass) |
| **SDS** | Safety Data Sheet (chemical hazard information for adhesives, solvents, cleaners) |
| **PAT** | Portable Appliance Testing (annual electrical safety check on power tools) |
| **CPP** | Construction Phase Plan (site-wide safety plan owned by the PSCS) |
| **S.I. 291/2013** | Safety, Health and Welfare at Work (Construction) Regulations 2013 (the statute most signage installs fall under) |

## File map

```
rams-irish-signage-installer/
├── README.md                          ← you are here
├── quickstart.md                      ← 5-min path for the impatient
├── identity.md                        ← who the specialist is, what they cover
├── rules.md                           ← how they respond, always/never list
├── examples.md                        ← three worked example interactions
├── LICENSE
└── reference/
    ├── your-contractor-profile.md     ← FILL THIS IN FIRST (locally, then re-upload if using Project)
    ├── legal-context-ireland.md       ← HSA framework, statutes, when a RAMS is required
    ├── section-templates-hsa-8.md     ← the 8-section scaffold
    ├── risk-matrix-5x5.md             ← scoring rules and bands
    ├── risk-library.md                ← signage-install hazards with controls
    ├── competency-matrix-ireland.md   ← Safe Pass, IPAF, PASMA, FAR, etc.
    ├── permits-framework.md           ← when each permit fires
    └── intake-questions.md            ← the question list the specialist works through
```

## Customising the specialist

ICM's payoff: you can update one file without breaking the others.

- New hazard you keep hitting? Add to `reference/risk-library.md`.
- New competency requirement on a client's site? Add a row to `reference/competency-matrix-ireland.md`.
- Working in NI? Duplicate `reference/legal-context-ireland.md`, swap HSA references for HSE / CDM 2015.
- Want a different standing rule (e.g., "we always do two-fitter installs")? Edit `rules.md`.

## Credits and licence

Built by Jannetje van Leeuwen ([IQ Branding Solutions](https://iqbrandingsolutions.ie)) for the Clief Notes Lyceum Weekly Competition #3 (May 2026). Uses ICM (Interpretable Context Methodology) developed by Jake Van Clief.

Source material: HSA RAMS Guidance Document (Construction Safety Partnership, Ireland), HSA Interactive Template, S.I. No. 291 of 2013 Construction Regulations.

Licence: see [LICENSE](LICENSE). Short version: read it, evaluate it, learn from it. Do not use it commercially, do not redistribute, do not fork as the basis of a competing tool. For other uses, ask. No warranty: a RAMS produced with this specialist still requires sign-off by a competent person in your organisation before it goes to a client or PSCS.
