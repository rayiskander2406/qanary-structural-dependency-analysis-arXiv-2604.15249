STATUS: ARXIV_V2_UPLOADED_AWAITING_MODERATION
SENT_DATE: 2026-04-17
UPLOADED_DATE: 2026-04-20 (Khaled uploaded ~2h before commit time)
LIVE_DATE: pending (arXiv moderation typically 2–24h)

## State machine

- 2026-04-17 — SENT (v2 replacement docx + arxiv_metadata.txt passed to Khaled for sanity-check + upload)
- 2026-04-20 — UPLOADED by Khaled to arXiv as v2 replacement of 2604.15249
- 2026-04-20 — Uploaded bytes (docx) + rendered PDF archived to ../../../arxiv/v2/
- → next expected: arXiv moderation completes (expected 2026-04-21); abs/2604.15249v2 becomes live

## What Khaled actually uploaded (vs. what we sent)

Zero content changes. Paragraph-level diff (after typographic normalization): 0 diffs on 907 paragraphs. The size delta (~370 KB → ~411 KB) is Word save-cycle metadata. Uploaded file archived at `../../../arxiv/v2/manuscript.docx` (SHA-256 `60de4742f1d0d282…`).

Khaled iterated the filename locally (`v2_for_Khaled` → `v4_for_Khaled`) across multiple open-save cycles, but content remained unchanged from the v2 draft we prepared.

## When arXiv v2 goes live (next action)

1. Verify `https://arxiv.org/abs/2604.15249v2` resolves with new abstract + Comments field.
2. Update this STATUS → `ARXIV_V2_UPLOADED_LIVE` with `LIVE_DATE`.
3. Update `../../../arxiv/v2/README.md` header: "uploaded, awaiting moderation" → "published on `<date>`".
4. Update `~/qanary/papers/registry.yaml` `paper1.arxiv.versions[]` v2 entry with real publication date; remove `arxiv_v2_pending: true`.
5. Tag `arxiv-v2` on the commit.
