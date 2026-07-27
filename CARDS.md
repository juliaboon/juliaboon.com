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
| **Protection** 2019–2026 | Police → Child protection → Family Court → Public healthcare → Executive tribunals |
| **The assets** 2020–2026 | Police → Single expert valuation → Accounting body → Corporate regulator → Ombudsman |
| **Representation** 2021–2026 | Solicitors → Legal services commissioners → Costs assessment |

**Visual grammar:** institutions are boxes; what followed sits in the gap
between them, unboxed and unattributed, because it belongs to no one. Each bead
carries its year and its branch colour, so the reader can see a subject crossing
from executive to judicial and back.

**No causal claim is made.** The note above the chains says so explicitly:
*"only the order in which things happened."* A reader draws the inference; the
page does not assert it. That is both safer and more persuasive.

To add a bead: copy a `<li class="bead">` and the `<li class="link">` before it.
Colour is set per bead with `style="--c:#…"` so a chain can cross branches.
