# arXiv v2 — published 2026-04-21

**arXiv URL:** https://arxiv.org/abs/2604.15249v2
**Uploaded:** 2026-04-20 (by Khaled Kirah)
**Publicly live:** 2026-04-21
**Status:** PUBLISHED

## Files

| File | SHA-256 (first 16) | Purpose |
|---|---|---|
| `manuscript.docx` | `60de4742f1d0d282…` | FROZEN — exact bytes uploaded to arXiv as v2 (~411 KB) |
| `manuscript.docx.ots` | — | OpenTimestamps proof of upload bytes (Bitcoin, pending confirmation) |
| `manuscript.pdf` | `8a656c7361057e65…` | arXiv-rendered v2 PDF (the file Khaled downloaded back from arXiv after upload) |
| `manuscript.pdf.ots` | — | OpenTimestamps proof of the rendered PDF (Bitcoin, pending confirmation) |
| `arxiv_metadata.txt` | — | Literal text of the Abstract + Comments fields Khaled pasted at upload time |

## Changes vs. arXiv v1

Per `arxiv_metadata.txt` Comments field:

> v2: added Zenodo artifact DOI (10.5281/zenodo.19625392); minor abstract revision to reference FIPS 203/204 explicitly; resolved artifact-repository URL placeholder in the Code and Data Availability section. No changes to the methodology, results, or references.

Specifically:
- **Abstract** revised opening sentence to reference PQC, ML-KEM (FIPS 203), ML-DSA (FIPS 204) explicitly.
- **Code and Data Availability** section now cites Zenodo concept DOI `10.5281/zenodo.19625392` (Paper 1's own artifact archive, minted 2026-04-17 as v1.0.0).
- **No text changes** in methodology, results, bibliography, or citation numbering.

## Zenodo (no new version needed)

The v1 README's note about "a new Zenodo version should auto-mint via the GitHub webhook" was an over-anticipation. The Zenodo artifact (`10.5281/zenodo.19625393`, minted 2026-04-17 with Paper 1 v1.0.0) was always the target — arXiv v2 simply ADDED the in-text reference to it. No new Zenodo mint is required or occurring. Registry's `paper1.zenodo.versions[]` remains as-is.

## Source authoring history

Khaled iterated the Word source between receiving our v2 draft (2026-04-17) and uploading to arXiv (2026-04-20). Local iteration names visible on his side: `v2_for_Khaled_2026-04-17` → `v4_for_Khaled_2026-04-17`. Paragraph-level diff (after typographic normalization): **0 content changes**. The size delta (~370 KB → ~411 KB) is Word save-cycle metadata.

## Live-transition actions (completed 2026-04-21)

1. ✓ Verified https://arxiv.org/abs/2604.15249v2 resolves with new abstract + Comments field.
2. ✓ README header flipped from `awaiting moderation` → `published 2026-04-21`.
3. ✓ `../../correspondence/khaled/2026-04-17_sent_paper1_v2/STATUS.md` updated: AWAITING_MODERATION → ARXIV_V2_UPLOADED_LIVE.
4. ✓ `~/qanary/papers/registry.yaml` `paper1.arxiv.versions[]` v2 entry: `live_date` set to 2026-04-21; `manuscript_git_sha` filled; `repo.arxiv_v2_pending` removed.
5. ✓ Tag `arxiv-v2` applied.
