# juliaboon.com — structure

## The page

```
   ┌──────────────────────────────────────────────┐
   │  ABOVE — the constitutional diagram          │
   │  Crown → Parliament · Cabinet · Courts       │
   │  all converging on THE LAW                   │
   └──────────────────┬───────────────────────────┘
                      │
              ┌───────▼───────┐
              │  DUE PROCESS  │   grey, unlinked, humble
              └───────┬───────┘
                      │
   ┌──────────────────▼───────────────────────────┐
   │  BELOW — the record                          │
   │  Legislative · Executive · Judicial          │
   │  same three positions, mirrored              │
   ├──────────────────────────────────────────────┤
   │  OUTSIDE THE STRUCTURE  (dashed, no fill)    │
   │  professions that answer to no branch        │
   └──────────────────────────────────────────────┘
```

The upper diagram is fixed civics — it never needs editing.
The lower half grows as material is added.

## Palette — constitutional, not decorative

| Power | Fill | Line | Used for |
|---|---|---|---|
| Legislative | `#C9D9EC` | `#8FA9C4` | Parliament, above and below |
| Executive | `#F6E7C6` | `#CDB183` | Cabinet, public service, agencies |
| Judicial | `#F3D5D5` | `#C99A9A` | Courts, above and below |
| Outside | none | `#8A9099` dashed | professions — no counterpart above |

Cabinet is drawn in **both** legislative and executive shading, because ministers
are drawn from Parliament and sit in it. That fusion is the design.

The professional bodies are drawn with **no fill and a dashed edge**: they appear
nowhere in the diagram above.

## Cards below

| Column | Card | Folder |
|---|---|---|
| Legislative | Parliament | `/parliament/` |
| Executive | **Public healthcare** ● | `/healthcare/` |
| Executive | Health records | `/healthcare/#records` |
| Executive | Police & criminal | `/police/` |
| Executive | Executive tribunals | `/tribunals/` |
| Executive | Corporate regulators | `/corporate/` |
| Executive | Oversight bodies | `/oversight/` |
| Judicial | Family Court | `/family-court/` |
| Judicial | Supreme Court of NSW | `/supreme-court/` |
| Judicial | Judicial conduct | `/judicial-conduct/` |
| Judicial | Access to the court | `/access-to-justice/` |
| Outside | The legal profession | `/legal-profession/` |
| Outside | Health practitioner registration | `/registration/` |
| Outside | Accounting & valuation | `/accounting/` |

## Card anatomy

Every card below the hinge carries four things, in this order:

1. **Body** — the institution
2. **Role** — in monospace, in the branch colour, never a name
3. **Decision** — what was done, factually
4. **Date range** — in monospace

Add one by copying an `.ag` block into the right `.col`. It inherits the
branch colour automatically.

## Naming

No individual is named anywhere. Roles and decisions only.

Live proceedings run to 13 October. Australian defamation law puts the burden
of proving truth on the publisher, at the publisher's cost. And naming people
converts a structural argument into a personal one, which is weaker.

Names belong in filings, where they are protected by privilege.

## Folders

`/public_mental_health/` — holds the two manifestos. **Not wired to any page.**
For direct sharing only. Wire it after 13 October if at all.

`/documents/` — PDFs linked from section pages.
