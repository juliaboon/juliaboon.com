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
| **Non-equitable** 2017–2026 | Child support → Police → Family Court → Single expert valuation *(→Accounting body)* → Corporate regulators (ATO · ASIC) → Ombudsman |
| **Legal protections** 2021–2026 | Solicitors → Legal aid *(→Internal review)* → Pro bono schemes → Legal services commissioners → Costs assessment |

### Visual grammar

- **Beads** are institutions — boxed, with year and branch colour.
- **Links** are what followed — unboxed, in the gap between beads, because
  they belong to no one.
- **Above a bead ↑** — a body that *supervises* it. Regulators sit above what
  they regulate.
- **Below a bead ↓** — a body *appointed by* it. The independent children's
  lawyer hangs from the Family Court because the appointment is the court's.
- **⇅ double arrow** — a closed loop: a complaint returned to the body it was
  made about. Used once, for the police oversight commission, because the
  documents establish it precisely.

Main beads sit on one baseline across each chain; appointees hang below without
lifting their parent off the line.

Two branches at present:

| Actor | Related body | Position | Outcome |
|---|---|---|---|
| Police 2019 | LECC 2024–25 | **above ⇅** | referred back to police, who declined it under s.132; oversight then satisfied with that handling |
| Single expert valuation 2022 | Accounting body 2024 | **above ↑** | complaint about the valuation closed without investigation |
| Solicitors 2021 | Legal services commissioners 2023 | **above ↑** | six complaints, two jurisdictions; no finding made |
| Legal aid 2022 | Internal review 2025 | **above ↑** | unsuccessful; property in dispute counted as means |
| Family Court 2021 | Independent children's lawyer 2021 | **below ↓** | police records not disclosed; professional complaint not investigated |

### The loop, as documented

23 Sep 2024 — complaint to the oversight commission about the police.
15 Oct 2024 — commission assesses it as *"appropriate for the NSW Police Force
to deal with"* and refers it to police.
28 Oct 2024 — the police district declines it under **s.132 Police Act 1990**;
not referred for further investigation.
8 Oct 2025 — further information provided to the commission.
21 Oct 2025 — commission *"satisfied with how police have dealt with your
complaint"*; new allegations do not meet the threshold for serious misconduct;
the complaint is filed *"to help identify important patterns and trends."*

Ref CASE20248744. This is the only ⇅ on the page, and it is earned.

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

---

## Wording held back deliberately

The Family Court entry says *"financial disclosure incomplete throughout;
applications to compel it did not result in enforcement."*

It does **not** say the disclosure was concealed, or that a judge sabotaged
enforcement. Both may be true and both belong in filings. On a public page under
your own name they are imputations against an identifiable individual — a judge
is identifiable from the case number — and Australian defamation law would put
the burden of proving them on you, at your cost, while the proceedings are still
running.

The factual version does the same work. A reader who sees *disclosure was
incomplete and applications to compel it were not enforced* draws the conclusion
without being told.

---

## Legal aid — the correct names

Two separate review bodies, each with its own address:

- **LARC** — Legal Aid Review Committee · `larc@legalaid.nsw.gov.au`
- **LARP** — Legal Aid Review Panel · `larp@legalaid.nsw.gov.au`

Both were engaged. Neither succeeded.

### Timeline from the file

| Date | Event |
|---|---|
| 28 Sep 2021 | Legal aid refused — ref 7423283 |
| 1 Jun 2022 | Appeal lodged |
| 30 Jun 2022 | Second refusal |
| 13 Mar 2023 | Application to the Family Violence and Cross-examination of Parties Scheme |
| 8 Feb 2024 | Urgent application before a five-day trial |
| 10 Dec 2024 | Refusal — ref 9322476 |
| 31 Dec 2024 | LARC appeal form lodged |
| 15 Jan 2025 | Appeal received (file 24F069452, "Property settlement married") |
| 21 Mar 2025 | Appeal forwarded to LARP — ref 9494129 |
| 31 Mar 2025 | Letter to Grants Division and LARP on the property pool |
| **10 Apr 2025** | **Appeal refused — decision upheld** |
| 8 Dec 2025 | Legal Aid Queensland application |
| 10 Dec 2025 | Queensland refusal |

## The s.102NA sequence

**Section 102NA, Family Law Act 1975.** Where family violence is alleged, an
alleged perpetrator may not personally cross-examine the other party, and the
section requires both to be legally represented. Legal Aid administers the
scheme that funds it.

| When | What |
|---|---|
| Mar 2023 | The court orders that s.102NA applies |
| Mar 2023 | Scheme application made in the state where the proceedings are heard; referred to the other state |
| 2023 | Representation obtained, funded by a **litigation loan** |
| Feb 2024 | Representation ends **ten days before trial** |
| Feb 2024 | Application made to remove the s.102NA order; **removed** |
| Feb 2024 | Trial listed to proceed with the protected party unrepresented |
| Feb 2024 | Trial adjourned — on a separate ground: the family report had been released to the parties one day before |

### Why this is the strongest item on the site

It is not a discretionary refusal of assistance. Parliament enacted a protection
against being cross-examined by an alleged perpetrator. That protection operates
only if someone funds a lawyer. When the lawyer was gone, **the protection was
removed rather than the hearing moved.**

The safeguard was treated as a scheduling obstacle.

### What is deliberately not said on the page

**Who applied to remove the order.** The site says "removed on application". The
applicant is identifiable from the case number, is a legal practitioner, and is
the subject of a complaint that has not been determined. Naming them, inside a
paragraph about a family violence protection being stripped, is an imputation
this record cannot yet prove and does not need.

**Why the representation ended.** The site says "when it ended". No
characterisation of the practitioner, for the same reason: the complaint is
pending.

**Motive.** The page does not say the removal was intended to avoid an
adjournment. It sets out the order, the removal, and the listing, in sequence.
A reader who sees a protection removed ten days before a trial draws the
conclusion unaided — and a conclusion a reader reaches is one they will defend.

Both are properly pleaded in filings, where privilege applies.

## The sharpest fact in that folder

**Section 102NA, Family Law Act 1975.** Where family violence is alleged, an
alleged perpetrator may not personally cross-examine the other party — and the
section requires that both be legally represented. Legal Aid administers the
Family Violence and Cross-examination of Parties Scheme to fund it.

On 13 March 2023 the court notified that s.102NA applied. Application was made
to the scheme the same day, ahead of an interim hearing eight days later.

**A statutory protection against being cross-examined by an alleged perpetrator
exists only if someone funds a lawyer.** That is not a discretionary refusal of
assistance; it is a protection Parliament enacted, defeated at the point of
delivery.

⚠️ **VERIFY before publishing.** Obtain (a) the March 2023 order recording that
s.102NA applied, (b) the application and order removing it in February 2024, and
(c) the transcript or orders of the listed trial date. The page currently asserts
all three. Each should rest on a document, not a recollection.
