Dear Khaled,

Thank you for catching the missing figure references — you are right, it was not intentional. Academic convention requires every figure and every table to be cited in the text, and after you raised it I checked the whole document systematically: the same oversight also affects **Tables 3 and 4**.

Separately, I made the companion artifact repository public today (Apache-2.0, with Zenodo metadata prepared), so the paper also needs a short **Code and Data Availability** paragraph added to §Reproducibility, and Limitation **L8** needs to be updated (it currently states the code is not yet public, which is no longer accurate).

Rather than sending you a new revision — which would lose the edits you have already made — I have prepared a compact insertion table below covering all eight items. Each row gives a unique anchor phrase you can locate via Find (⌘-F / Ctrl-F) in your working copy, followed by the exact wording to add. Please feel free to rephrase.

---

## Insertion table — QANARY 3.0 (Paper 1)

### A. Orphaned figure/table citations (6 items)

| # | Find this anchor phrase | Insertion |
|---|---|---|
| **Figure 1** | "…and describes the tool pipeline and self-validation infrastructure." *(end of §3 Methodology intro, just before Figure 1)* | Append: " **Figure 1 shows the label lattice used throughout this analysis.**" |
| **Figure 2** | "SC-D1 identifies 59,061 structurally insecure wires across the 27 completed modules in 8.7 seconds total." *(opening of §4 Single-Cycle Results)* | Append: " **Figure 2 summarizes the module classification under SC-D1 and MC-D1.**" |
| **Figure 3** | "The ~8,500 convergence points across 1.17 million cells (approximately one per 140 cells on average) represent a non-trivial inspection effort…" *(§4 MC-D1)* | Insert after "on average" and before the closing parenthesis: "**, see Figure 3**" → "…(approximately one per 140 cells on average, see Figure 3) represent…" |
| **Figure 4** | "MC-D1 flags 614,126 structurally insecure wires in total…" *(opening of §4 Multi-Cycle Results)* | Append to that sentence (after "…a 10.4× increase"): " **Figure 4 decomposes these wires by root-cause category.**" |
| **Table 3** | "**DOM AND.** The four-stage pipeline resolves all structurally-flagged wires in the 16-cell reference gadget in under 0.1 seconds:" *(§ Benchmarks and Independent Confirmation, just before Table 3)* | Change the trailing colon to a period and add a sentence: "…in under 0.1 seconds. **Table 3 reports the stage-by-stage resolution.**" |
| **Table 4** | "Arithmetic SADC closes the residual completely." *(end of the ML-KEM Barrett paragraph, immediately before Table 4)* | Append: " **Table 4 summarizes the four-stage classification.**" |

### B. Artifact release (2 items)

| # | Find this anchor phrase | Insertion |
|---|---|---|
| **Code and Data Availability paragraph** | "We intend to submit to the TCHES artifact evaluation process." *(last sentence of §Reproducibility)* | After this sentence, add a new paragraph: "**Code and Data Availability.** The complete reproduction artifact is publicly available at `https://github.com/rayiskander2406/qanary-structural-dependency-analysis-arXiv-XXXX.XXXXX` under the Apache-2.0 license. The repository includes the single-command reproduction driver (`reproduce.py`), the Z3/CVC5 proof suite (theorems T1–T6), per-module evidence JSON for all 27 synthesized modules, synthesized netlists pinned to Adams Bridge commit `cdc9b1c`, and `repro_manifest.json` with pinned tool versions and SHA-256 hashes. A Zenodo DOI will be minted automatically upon publication; the `XXXX.XXXXX` placeholder in the repository name will be replaced with the final arXiv identifier once assigned." |
| **L8 row in the Limitations table** | "\| L8 \| Artifact evaluation readiness \| Tool/code not yet public \| Submit to TCHES AE post-acceptance \|" *(row L8 in the limitations table)* | Replace the full row with: "\| L8 \| Formal artifact evaluation pending \| Code is now public (Apache-2.0) but not yet AE-certified \| Submit to TCHES AE post-acceptance \|" *(Alternative: remove L8 entirely since public availability is no longer a limitation; your call.)* |

---

Each edit is a single sentence or one table row; nothing in the body text needs to be removed. If you prefer, I can send a diff-only Word document with just these eight changes applied via tracked changes, but the table should let you fold them in without disrupting your own revisions.

Thank you again for the careful review — the table audit was prompted entirely by your figure observation.

Best regards,
Ray
