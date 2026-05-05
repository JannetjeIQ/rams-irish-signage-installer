# Your Contractor Profile

**FILL THIS IN ONCE BEFORE USING THE SPECIALIST.** Replace every `[BRACKETED PLACEHOLDER]` with your actual details. The specialist reads this file every time it drafts a RAMS and uses it to populate the Contractor Details section.

If you leave placeholders in here, the specialist will refuse to draft until you complete it. That is intentional: it stops Claude inventing a company name, address, or insurance figure.

---

## 1. Company identity

```
Trading entity (verbatim, exact legal name): [YOUR LIMITED COMPANY LTD T/A YOUR TRADING NAME]
Registered address:                          [UNIT N, INDUSTRIAL ESTATE, TOWN, EIRCODE]
CRO number:                                  [CRO NUMBER]
VAT number:                                  [VAT NUMBER]
Business description (verbatim):             [E.G. SIGN PRODUCTION & INSTALLATION]
```

The trading-entity wording goes onto every RAMS verbatim. If the legal name is "Acme Holdings Ltd t/a Acme Signs", that is what appears, every time, no shortcut.

---

## 2. Responsible person (RAMS approver)

```
Name:                       [FULL NAME]
Role:                       [E.G. PROJECT MANAGER, OPERATIONS DIRECTOR]
Phone:                      [MOBILE]
Email:                      [EMAIL]
```

This is the person who signs off the RAMS before it leaves your office. Default approver named on every RAMS unless a job has been delegated to someone else.

---

## 3. Insurance

```
Insurer:                    [INSURER NAME]
Policy number:              [POLICY NUMBER]
Period of cover:            [DD/MM/YYYY] to [DD/MM/YYYY]
Employers Liability:        EUR [LIMIT] any one claim
Public Liability:           EUR [LIMIT] each and every occurrence
Products Liability:         EUR [LIMIT] each and every occurrence
Height limit:               [HEIGHT IN METRES] metres
Excess:                     EUR [EXCESS]
```

The full block goes verbatim into the Contractor Details section of every RAMS.

**Height limit is critical.** The specialist refuses to draft for jobs above this height. If you take on taller work via a broker extension or via a subcontracted crew with matching cover, do not change this number; that work needs special handling on the RAMS itself.

**Renewal cadence.** Set a calendar reminder 14 days before the period of cover end date so you have the new certificate in hand before the old one expires. Update this profile the same day you receive the new policy schedule.

---

## 4. Safety statement

```
Safety Statement document number / version:  [VERSION OR DOC ID]
Last reviewed:                                [YYYY-MM-DD]
Held at:                                      [LOCATION OR LINK]
```

Referenced in the Contractor Details block of every RAMS. If you don't have a Safety Statement yet, you need one before you take on any work classified as construction in ROI (Section 20, Safety Health and Welfare at Work Act 2005). The specialist will warn you if this is empty but will continue drafting.

---

## 5. Job-tracking system

```
System name:                [E.G. PRINTLOGIC, MONDAY, GOOGLE SHEET, WHATEVER]
Order number format:        [E.G. 5-DIGIT NUMERIC, P-PREFIX, ETC.]
Use order number as RAMS document number?:   [YES / NO]
```

If yes, the RAMS document number is the order number. This is the cleanest pattern: the same reference travels from quote to install to invoice to RAMS, and anyone in your office can find the RAMS by the order number. If no, set a sequential RAMS numbering scheme (e.g., RAMS-2026-001).

---

## 6. Competency tracker

```
Tracker maintained by:      [NAME, ROLE]
Tracker location:           [E.G. SHAREPOINT FOLDER, AIRTABLE, EXCEL ON SHARED DRIVE]
Cadence for expiry alerts:  [E.G. 60 DAYS BEFORE EXPIRY]
```

The person named here is the source of truth on which fitters are valid for a given job. The specialist will reference them when asking you to confirm fitter competency.

---

## 7. SDS library

```
Master SDS folder:          [LOCATION OR LINK]
Maintained by:              [NAME, ROLE]
Last reviewed:              [YYYY-MM-DD]
```

When the specialist drafts Appendix C of a RAMS, it pulls relevant SDS from this folder. If the folder doesn't exist yet, the specialist will draft Appendix C as a placeholder list of substances used on the job and prompt you to attach the SDS manually before issue.

---

## 8. Standing crew (optional but useful)

List your regular fitters. The specialist uses this to validate competency claims and to select named fitters for a job. Add or remove rows as your crew changes.

| Fitter name | Lead/operative | Safe Pass expiry | Manual Handling expiry | Working at Heights expiry | IPAF (categories) | PASMA expiry | FAR expiry | Notes |
|-------------|----------------|------------------|------------------------|---------------------------|-------------------|--------------|------------|-------|
| [Name 1]    | [L / O]        | [YYYY-MM-DD]     | [YYYY-MM-DD]           | [YYYY-MM-DD]              | [1a/1b/3a/3b]     | [YYYY-MM-DD] | [YYYY-MM-DD] |       |
| [Name 2]    |                |                  |                        |                           |                   |              |              |       |
| [Name 3]    |                |                  |                        |                           |                   |              |              |       |

If a row has no expiry filled, the specialist will not select that fitter for a job that requires that competency. It will ask you to confirm or update.

---

## 9. Subcontracted install crews (if you use them)

If you regularly use subcontract install crews for overflow or specialist work, list them here so the specialist can reference them by name. Each one needs to carry their own RAMS-relevant evidence (insurance, competency).

| Subcontractor name | Speciality | Insurance held | Competency cert held | Last verified |
|--------------------|------------|----------------|----------------------|---------------|
| [Crew name 1]      |            |                |                      |               |
| [Crew name 2]      |            |                |                      |               |

---

## 10. Standing exclusions (carried into every RAMS)

These get written into the cover page and the Method of Work section of every RAMS, so site managers and PSCSs know upfront what is not in scope.

- **Live electrical work.** All mains-power isolation, disconnection, termination, and re-energising of any signage product is performed by a third-party RECI registered electrician booked separately. IQ-style installers do not hold RECI registration and will not perform this work.
- **Anything above the insurance height limit** stated in §3.
- [Any other exclusion you want as default, e.g., "no roof work without a permit", "no demolition", etc.]

---

**Done? Save the file. The specialist will pick up your details from the next prompt.**
