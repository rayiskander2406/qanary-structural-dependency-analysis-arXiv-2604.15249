# Email to Khaled — QANARY Paper v2 ready for review

**Subject:** QANARY Paper v2 — ready for your review (3 metadata-only edits, arXiv:2604.15249)

---

Dear Khaled,

arXiv has assigned ID **2604.15249** to our paper (uploaded yesterday), and the reproduction artifact is now live on GitHub and permanently archived on Zenodo with DOI **10.5281/zenodo.19625392** (concept DOI — always resolves to the latest version).

Attached is **v2** of the paper. The revision is metadata-only — **no changes to methodology, results, references, figures, or tables**. Three surgical edits:

1. **Abstract opening sentence.** Added "(PQC)", "ML-KEM (FIPS 203)", and "ML-DSA (FIPS 204)" so these high-intent search terms appear on the arXiv landing page (they are currently missing from the abstract, which hurts discoverability on Scholar/arXiv search).

2. **Keywords line** (under the title). Consolidated three existing keywords to inline their acronym / standard number (no change to keyword count):
   - `Post-Quantum Cryptography` → `Post-Quantum Cryptography (PQC)`
   - `ML-KEM` → `ML-KEM (FIPS 203)`
   - `ML-DSA` → `ML-DSA (FIPS 204)`

3. **Code and Data Availability paragraph.** Resolved the `XXXX.XXXXX` placeholder in the GitHub URL to the final `arXiv-2604.15249` suffix; added the Zenodo concept DOI and version DOI as clickable hyperlinks; removed the obsolete sentence "A Zenodo DOI will be minted automatically upon publication…" which no longer applies.

A complete diff-view (before → after) for each of the three edits is available on request if helpful.

## Attachments

- **`QANARY_Paper_v2_for_Khaled_2026-04-17.docx`** — the revised paper
- **`QANARY_Paper_v2_arXiv_metadata_2026-04-17.txt`** — copy-paste-ready material for the arXiv v2 upload form

## Important note on the arXiv v2 upload

arXiv stores the abstract in **two** places: (1) inside the PDF, and (2) in a separate metadata field shown on the paper's landing page (this is what Google Scholar and Semantic Scholar index). arXiv does **not** auto-extract the abstract from an uploaded PDF. For the abstract edit to take effect on the landing page, the metadata abstract field must also be updated during the v2 submission — the companion `.txt` file contains the exact text to paste.

Suggested `Comments` field for the arXiv v2 upload (appears under the title on the landing page):

> v2: added Zenodo artifact DOI (10.5281/zenodo.19625392); minor abstract revision to reference FIPS 203/204 explicitly; resolved artifact-repository URL placeholder in the Code and Data Availability section. No changes to the methodology, results, or references.

If the revisions look correct to you, please upload v2 to arXiv at your convenience. Happy to jump on a quick call if anything looks off.

Best regards,
Ray
