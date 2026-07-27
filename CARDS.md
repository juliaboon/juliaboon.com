# juliaboon.com — structure

## The page

Three views: **Above** the structure · **Below** the record · **Across** the sequence.


```
   ABOVE — the constitutional diagram          full-bleed
   Crown → Parliament · Cabinet · Courts
   all converging on THE LAW
                  │
          ┌───────▼───────┐
          │  DUE PROCESS  │   grey, unlinked, humble
          └───────┬───────┘
                  │
   BELOW — the record
   Legislative · Executive · Judicial
   same three positions, mirrored
```

Everything sits under the law and belongs to one of the three branches.
There is no "outside".

## Palette

| Power | Fill | Line |
|---|---|---|
| Legislative | `#C9D9EC` | `#8FA9C4` |
| Executive | `#F6E7C6` | `#CDB183` |
| Judicial | `#F3D5D5` | `#C99A9A` |

Cabinet is shaded in both legislative and executive because ministers are drawn
from Parliament and sit in it.

## Cards

| Column | Card | Nested under | Folder |
|---|---|---|---|
| Legislative | Parliament | — | `/parliament/` |
| Executive | Public healthcare | — | `/healthcare/` |
| Executive | Health records | healthcare | `/healthcare/#records` |
| Executive | Practitioner registration | healthcare | `/registration/` |
| Executive | Police & criminal | — | `/police/` |
| Executive | Executive tribunals | — | `/tribunals/` |
| Executive | Corporate regulators | — | `/corporate/` |
| Executive | Accounting & valuation | corporate | `/accounting/` |
| Executive | Oversight bodies | — | `/oversight/` |
| Judicial | Family Court | — | `/family-court/` |
| Judicial | Supreme Court of NSW | — | `/supreme-court/` |
| Judicial | Judicial conduct | — | `/judicial-conduct/` |
| Judicial | Access to the court | — | `/access-to-justice/` |
| Judicial | The legal profession | access to the court | `/legal-profession/` |

Nested cards use `class="ag sub"` and draw their own tick to the parent.

## Card anatomy

1. **Body** — the institution
2. **Role** — monospace, branch colour, never a name *(top-level cards only)*
3. **Decision** — what was done, factually
4. **Years** — no exact dates on the public page

## Standing rules

**No individual is named anywhere.** Roles and decisions only. Live proceedings
run to 13 October; Australian defamation law puts the burden of proving truth on
the publisher; and naming people converts a structural argument into a personal
one. Names belong in filings, where privilege protects them.

**Years, not dates.** Precision belongs in the filings.

**The record is stated as partial** in the note above the cards, so an incomplete
picture is not mistaken for the whole one.

**The healthcare card says "a patient represented by the author"** so no reader
infers the author was the person detained.

## Folders

`/public_mental_health/` — the two manifestos. **Not linked from any page.**
For direct sharing only. Publicly readable by anyone who guesses the path, so
treat the URL itself as the access control until after 13 October.

`/documents/` — PDFs linked from section pages.

Section pages are intentionally blank pending the filings.

---

## ACROSS — the sequence

Three subjects, each carried from one institution to the next over seven years.

| Chain | Beads |
|---|---|
| **Not in the best interest of children** 2019–2026 | Police *(→LECC)* → Child protection → Family Court *(→ICL)* → Public healthcare → Executive tribunals |
| **Non-equitable** 2020–2026 | Police → Single expert valuation → Accounting body → Corporate regulators (ATO · ASIC) → Ombudsman |
| **Legal protections** 2021–2026 | Solicitors → Legal services commissioners → Costs assessment |

### Visual grammar

- **Beads** are institutions — boxed, with year and branch colour.
- **Links** are what followed — unboxed, in the gap between beads, because
  they belong to no one.
- **Branches** hang *beneath* a bead: an oversight body that was asked and
  returned nothing. A branch is a dead end, not a step forward, so it drops
  down rather than continuing across.

Two branches at present:

| Parent | Branch | Tail |
|---|---|---|
| Police 2019 | LECC 2024 | referred to internal investigation; police closed it without investigating |
| Family Court 2021 | Independent children's lawyer 2021 | police records not disclosed; professional complaint not investigated |

The ICL hangs from the Family Court rather than sitting in the legal-profession
column, because the appointment is the court's.

### No causal claim

The note above the chains says so: *"only the order in which things happened."*
A reader draws the inference. One they make themselves is one they defend;
one that is asserted for them is one they argue with.

### Adding to a chain

Copy a `<li class="stack">` and the `<li class="link">` before it. Colour is set
per bead with `style="--c:#…"` so a chain can cross branches. To add a dead-end
branch, copy an `<div class="off">` block inside the stack.
