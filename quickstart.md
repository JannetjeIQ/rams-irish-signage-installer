# Quickstart (5 minutes from clone to first useful response)

For judges, hiring managers, and anyone who wants to see this work cold without reading the README.

## What this folder is

A Claude specialist that drafts compliant RAMS (Risk Assessment Method Statements) for Irish signage installation jobs. HSA-aligned, 8-section, 5x5 risk matrix.

## The five steps

### 1. Get the folder

Either:
- **Clone:** `git clone https://github.com/JannetjeIQ/rams-irish-signage-installer.git`
- **Or download:** click the green Code button on GitHub, Download ZIP, unzip.

### 2. Edit `reference/your-contractor-profile.md`

Open it in any text editor. Replace the bracketed placeholders in **§1, §2, §3, §5, §6** with your actual details. Five sections, ~15 fields, takes 3 minutes if you have the info to hand.

The minimum:

- §1: company trading name, address, CRO, VAT
- §2: responsible-person name, role, phone, email
- §3: insurer, policy number, period of cover, EL/PL/Products limits, height limit, excess
- §5: how you number jobs (and whether the order number doubles as the RAMS document number)
- §6: who maintains the competency tracker

Save the file.

### 3. Drop into Claude

**Either:**

- **Claude Project (claude.ai web):** Projects → Create project → upload all 14 files (drag the folder contents in). Open a chat in the Project.
- **Claude Code (CLI):** open the folder in your terminal, run `claude`. Folder structure works on demand.

### 4. Ask the first question

Type:

> Draft a RAMS for [your job]: [client], [site], [date], [scope].

For example:

> Draft a RAMS for a fascia replacement at a Dublin retail unit. Single fitter, 4m max height, two-day install, install Wednesday.

### 5. Answer the gap questions

The specialist comes back with a single consolidated list of follow-up questions (site contact, induction route, access equipment, fitter competencies, permits, etc.). Answer them in one reply.

You then receive a draft RAMS in markdown, structured to the HSA 8-section template, with a populated 5x5 risk matrix. Iterate inline. Paste into Word as A4 to ship.

## What you should see (sanity check)

- The first prompt **without a filled-in profile will refuse to draft**. If you see "I will not invent contractor details", you skipped step 2.
- The specialist **will refuse out-of-scope work**: live electrical (RECI), work above the insurance height limit you set in §3.
- It will **not pad** with disclaimers, "let me know if you need anything else" closers, or generic boilerplate. If you get those, the folder is not loaded; reload.

## If you get stuck

- "I cannot draft until your-contractor-profile.md is populated" → step 2 not done.
- "This is above your stated insurance height limit" → either lower the height in your prompt or extend cover (it's working as designed).
- "I will not include live electrical work in scope" → exclude it from your prompt; book a RECI electrician separately (it's working as designed).
- Anything else looking off → see the [README acronym glossary](README.md#acronym-glossary-read-this-if-any-of-the-specialists-questions-look-like-alphabet-soup) for jargon, and `examples.md` for three worked interactions.

## What this folder is not

- Not a substitute for competent H&S advice. Sign-off by a competent person in your organisation is still required before the RAMS goes to a client or PSCS.
- Not a tool for civils, scaffolding-only, electrical, demolition, or sites outside Ireland (without swapping the legal context file).
