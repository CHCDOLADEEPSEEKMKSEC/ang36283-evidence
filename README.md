# ANG36283 — evidence trail site

Public list of the documents and photographs behind the #OPWFM documentation project.
Each item: title, date, source, grade, SHA-256 hash, and (where publishable) the file itself.

**Publish rules**
1. **Public-record documents only** (Registers of Scotland sheets/plans, FOI responses, Companies House public filings).
2. **Our own photographs** — public ground, no faces, no plates.
3. **Never**: internal notes, personal data, member details, keys, or unverified allegation as fact.
4. **Corrections are published, not quietly edited** — a changed file gets a new hash and a dated note.

**Adding an item**
```bash
python3 /mnt/ledger/vault/tools/evidence_publish.py \
  --file "/path/to/file.pdf" --title "RoS title sheet ANG36283" \
  --grade PROVEN --date 2026-11-03 --source "Registers of Scotland" --kind pdf
```
Then commit + push — Pages updates in ~60s.
