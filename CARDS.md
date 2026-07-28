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
| **Not in the best interest of children** 2019–2026 | Police *(→LECC)* → Child protection → Family Court *(→ICL)* → Family reports → Public healthcare → Executive tribunals |
| **Non-equitable** 2017–2026 | Child support → Police → Family Court → Single expert valuation *(→Accounting body)* → Corporate regulators (ATO · ASIC) → Ombudsman |
| **Legal protections** 2021–2026 | Solicitors → Legal aid *(→Internal review)* → Pro bono schemes → Legal services commissioners → Costs assessment |

### Visual grammar

- **Beads** are institutions — boxed, with year and branch colour.
- **Links** are what followed — unboxed, in the gap between beads, because
  they belong to no one.
- **Above a bead ↑** — a body that *supervises* it. Regulators sit above what
  they regulate. A stack can hold two: costs assessment above the legal services
  commissioners, both above the solicitors.
- **Below a bead ↓** — a body *appointed by* it. The independent children's
  lawyer hangs from the Family Court because the appointment is the court's.
- **⇅ double arrow** — a closed loop: a complaint returned to the body it was
  made about. Used once, for the police oversight commission, because the
  documents establish it precisely.

**Main beads align on their top edge** across each chain, whatever hangs above or
below them, and every connector rule sits on that same line. Supervisors and
appointees are absolutely positioned so they never shift the row.

Each chain carries its own `--pad` on the `<section>`, sized to whatever is
tallest above its beads. If you add a supervisor or lengthen a link, raise it.

**Link text is short by rule** — six to eight words. The connector says what
followed; the card below says how. Long link text starves the columns and pushes
the diagram apart.

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

---

## Family Court — what the card now says

> Proceedings since 2021. Financial disclosure incomplete throughout;
> applications to compel it did not result in enforcement. Final orders were made
> in 2024 while a police investigation was on foot, and enforced in 2025 while it
> remained on foot. An application to set the orders aside under s.79A(1) of the
> Family Law Act, on the ground that they were obtained by fraud, has not been
> listed for a threshold hearing in over fifteen months, while an enforcement
> hearing was listed ahead of it. The harm is not reversible and any later relief
> would be nugatory.

Note the construction: **"on the ground that they were obtained by fraud"**
describes the application. It does not assert the fraud as established. The
listing sequence — enforcement heard, s.79A unlisted for fifteen months — is a
matter of record and needs no adjective.

⚠️ **VERIFY**: the fifteen-month figure, the filing date of the s.79A
application, and that the police investigation was on foot on both the order date
and the enforcement date.

---

## Column order is an argument

**Executive** reads: Police → Child protection → Public healthcare → Health
records → Practitioner registration → Executive tribunals → Child support →
Corporate regulators → Accounting → Oversight.

Police sit at the top because everything else follows from what was not
investigated. Healthcare sits between police and the tribunals because that is
where the sequence went. Order is not alphabetical and not chronological; it is
the order in which the failures compound.

## The one rhetorical line on the site

Parliament's card ends with a `.coda`:

> *Deafening silence.*

It is set apart from the factual span, in the branch colour, italic. It works
only because nothing else on the page does this. Two of them and the record
becomes commentary. Keep it to one.

## ⚠️ Legal aid — a claim I did not write

You said: *"even if means test fails it is in the law that all DFV-involving
matters need to be taken."*

The card says instead:

> Family violence and coercive control were raised throughout and are not
> addressed in the reasons.

That is checkable from the refusal letters and cannot be argued with. The
stronger version — that a legal obligation was breached — needs the provision
named. Legal Aid NSW policy does contain family violence and special
circumstances provisions, and the means test can be varied, but I have not read
the guideline and will not put a statutory claim on a public page from memory.

**Send me the provision and I will cite it precisely.** With a guideline number
the sentence becomes: *"Guideline X requires … The reasons do not refer to it."*
That is much stronger than the current wording, and it is unanswerable.

---

## Family reports — s.60B verified

The card cites the statute directly, and the citation is current:

> **Family Law Act 1975 (Cth), s.60B** — as substituted by the Family Law
> Amendment Act 2023 (No. 87, 2023), Schedule 1 item 4, in force 6 May 2024:
>
> *The objects of this Part are:*
> *(a) to ensure that the best interests of children are met, including by
> ensuring their safety; and*
> ***(b) to give effect to the Convention on the Rights of the Child** done at
> New York on 20 November 1989.*

Australia ratified the Convention in 1990 ([1991] ATS 4). The obligation to give
effect to it is not aspirational — it is an object of Part VII, and the courts
must read the parenting provisions in light of it.

### What the card says

> Section 60B of the Family Law Act provides that an object of the parenting
> provisions is to give effect to the Convention on the Rights of the Child.
> Risks raised in evidence do not appear in the reports, and conclusions within a
> single report are inconsistent with each other. One report was released to the
> parties the day before a listed trial.

Three sentences, three registers: **the statute**, **what the documents omit**,
**what the documents contain**. The reader joins them.

Note what is not said: that the report writer breached s.60B. The object binds
the court's construction of the Part; whether it binds a report writer directly
is an argument, not a fact. The page states the object and the omission and stops.

⚠️ **VERIFY the year range 2022–24.** I placed the bead between Family Court
(2021) and Public healthcare (2023) to keep the chain chronological, and widened
it to 2024 to cover the report released the day before trial. If there was only
one report, correct it to that year.

---

## Corrections made from the LSC file

| Was | Now | Source |
|---|---|---|
| "1:100 against a sworn figure" | **$100,000 against $7 million** sworn overseas | your figures |
| "order removed when representation ended" | **removed by order 14 Feb 2024, five days before the 19 Feb trial** | complaint of 5 Dec 2024 |
| "professional complaint not investigated" | **conduct complaint suspended since February 2025** | OLSC notifications 13 Feb 2025, 25 Sep 2025 |

The order chronology, from the complaint: **s.102NA made by Order 1 on 10 March
2023; removed by Order 5 on 14 February 2024; trial listed 19 February 2024.**
Representation ceased ten days before trial; the order went five days before it.

That is a sharper fact than the one the page carried before. The protection did
not lapse when the lawyer left. It was removed, by application, on a date, with
the trial five days away.

## The ICL card

> Appointed by the court and funded by Legal Aid. The s.102NA protection made in
> March 2023 was removed by order on 14 February 2024, five days before trial and
> after the protected party had become unrepresented. Police material subpoenaed
> in 2023 was not disclosed. A conduct complaint lodged in December 2024 alleges
> partiality, failure to act on family violence evidence, and intervention in the
> protected party's own legal aid application. **The investigation has been
> suspended since February 2025.**

Two constructions to keep:

**"alleges"** — the complaint's contents are described as allegations, because
that is what they are until determined. The page does not assert them.

**"suspended since February 2025"** — this is the *documented* fact, and it is
the finding. Fifteen months of suspension needs no adjective. It is also the only
sentence in the card that is not an allegation, which is why it lands hardest.

The first line — **appointed by the court and funded by Legal Aid** — does quiet
work. The body said to have intervened in a legal aid application is itself paid
by legal aid.

## The valuations card

> The business was valued at $100,000 in the proceedings, against $7 million sworn
> by the same party in an overseas filing. Executed contracts for the sale of the
> business, and a new entity holding its assets, were not before the court;
> bankruptcy documents were produced shortly before enforcement. A property
> valuation delivered days before trial increased the assessed value, while the
> Valuer General's figures for the same period fell below the previous year's.

The property valuation sentence is built as a **divergence, not a motive**. Two
figures moving in opposite directions over the same period, one of them official.
No reader needs to be told what that suggests, and asserting it would be the one
sentence a valuer's insurer could act on.

⚠️ **VERIFY**: the $7 million figure and where it was sworn; the Valuer General
figures for the relevant years; and the date the bankruptcy documents were served.

---

## Terminal arrows

Each chain now ends in a `<li class="link end">` — an arrow with a comment and
**nothing after it**. The arrow points into empty space at the edge of the
container. That is the design, not a rendering fault: the sequence runs out of
institutions before it runs out of matter.

| Chain | Terminus |
|---|---|
| Not in the best interest of children | Mental Health and Guardianship Act conditions not established |
| Non-equitable | no outcome |
| Legal protections | three applications, no outcome |

### The wording of the first one

You said *"guardianship/Mental Health Acts laws breached."*

The page says **"conditions not established."**

Same claim, reviewable form. "Breached" asserts a legal conclusion against a
tribunal whose decisions are on foot and subject to review. "Not established"
says the record does not show the statutory conditions were met — which is
exactly the argument in the manifesto: s.12(1)(b) requires an opinion that no
less restrictive care consistent with *safe and effective* care is available, and
that opinion cannot be formed on a record in which nothing was measured.

It is the same point, and it survives being read by the tribunal it concerns.

### Layout consequence

Adding a sixth connector to the six-bead chains crushed the columns at 1200px.
Two adjustments: stacks narrowed from 9rem to **8.2rem**, and the wrap threshold
raised from 1080px to **1240px**, so the long chains break to two rows before
they get squeezed rather than after.

Verified clean at 1600, 1440, 1300, 1240, 1200, 1080, 900, 620 and 390px.
