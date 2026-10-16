# Grounded DI — Benchmark and Evaluation Index

This is the central navigation point for Grounded DI's published benchmark, local-audit, replay, and comparison records. The original IFEval records remain at the repository root. Additional public benchmark materials are preserved in the folders below and linked to their original repositories at specific source commits.

**Snapshot: October 16, 2026.** This consolidation preserves published records; it does not rerun or regrade them.

## Benchmark and review records

| Collection | Recorded result | Evidence status | Materials |
| --- | --- | --- | --- |
| Google Research IFEval | 83/83 local prompt passes; 188/188 encoded constraints; 80 distinct items across 83 positions | 27/83 official evaluator executions; 0 independent verifications; two disclosed preflight corrections | [Full record and source links](README.md#google-research-ifeval-prompts-1-83) |
| Harvey LAB — BriefWise 501/501 | 501/501 criteria locally audited — provisional | provisional local criterion audit | [Files and scope](benchmarks/harvey-lab/README.md) · [Original repository](https://github.com/Grounded-DI/briefwise-di-performance-on-harvey-lab-benchmark-audit) |
| Overfitting Dicta / Legora — Freshworks FY2023 | 89/89 applicable review-weight points; separate Deterministic v2 grade: 89.75/100 | retrospective original-mission review | [Files and scope](benchmarks/overfitting-dicta-freshworks/README.md) · [Original repository](https://github.com/Grounded-DI/benchmarks-briefwise-di2-freshworks-fy2023-review) |

The Harvey 501/501 count is a local criterion-audit checkpoint. The Freshworks 89/89 count is a retrospective applicable-weight review with a reconstructed denominator and a reservation. These use different units from IFEval prompt positions and encoded constraints. **Do not combine them into one pass rate.**

## Replay, historical, and qualitative records

| Collection | Recorded subject | Evidence class | Materials |
| --- | --- | --- | --- |
| VerdictBridge — synthetic controlled replay | Lane v. Apex: two identical archives; separate sealed speed-branch record: three executions | synthetic closed-world replay | [Files and scope](benchmarks/verdictbridge-replay/README.md) · [Original repository](https://github.com/Grounded-DI/VerdictBridge) |
| Visual assessments and handbag comparison | Preserved phenotype, product-riddle, and handbag comparison records; no standardized aggregate score | qualitative comparison and diagnostic demonstrations | [Files and scope](benchmarks/visual-comparisons/README.md) · [Original repository](https://github.com/Grounded-DI/Deterministic-VIsual-Assessments-) |
| DI² — historical determinism benchmark | August 14, 2025 command-sequence and stability-scan record | historical self-reported benchmark artifact | [Files and scope](benchmarks/di2-historical/README.md) · [Original repository](https://github.com/Grounded-DI/DI-2) |
| BatteryWise and ClarityWise — historical diagnostic demos | Battery-efficiency prompt/template and ClarityWise diagnostic demonstration | historical diagnostic prompts and illustrative outputs | [Files and scope](benchmarks/legacy-diagnostics/README.md) · [Original repository](https://github.com/Grounded-DI/deterministic-intelligence) |
| Harvey LAB — earlier August packages and Ridgeline stages | Four-task 188/188 coverage checkpoint; Ridgeline baseline 36/50 and rubric-aware remediation 50/50 | earlier provisional local-audit packages | [Files and scope](benchmarks/harvey-earlier-packages/README.md) · [Original repository](https://github.com/Grounded-DI/-Social-Media-Posts-August-2026) |
| Ulam prime-density — three-execution artifact reproducibility | Three preserved execution packets with reported CSV, PNG, and ZIP identity | bounded artifact byte-reproducibility record | [Files and scope](benchmarks/ulam-reproducibility/README.md) · [Original repository](https://github.com/Grounded-DI/-Social-Media-Posts-August-2026) |

Earlier Harvey packages overlap the later audit sequence. Mirrored certificates, historical screenshots, comparison images, and multiple copies of the same record are not new trials. The root `1_Benchmark_Score_50_of_50_and_Estimated_Relevant_Statistics.jpeg` is retained as a historical capture, without adding a separate independently established score. The Harvey certificate already at the root remains in place; its original-source copy and sidecar are now collected under `benchmarks/harvey-lab/`.

## Related evidence repositories

These provide context, audit records, or navigation; they are not added to the scored benchmark totals.

| Repository | Role and scope |
| --- | --- |
| [BriefWise DI²](https://github.com/Grounded-DI/BriefWise_DI2) | Historical citation/authority audit checkpoints. Its 501/501 case-citation certificate is a different record from Harvey LAB 501/501. |
| [Replay Certificate Registry](https://github.com/Grounded-DI/grounded-di-replay-certificate-registry) | Bounded replay demonstrations, verification artifacts, and provenance. Preserve each demo's local or synthetic scope. |
| [MathWise Deterministic Replay Certificates](https://github.com/Grounded-DI/MathWise-Deterministic-Replay-Certificates) | Curated mathematical certificates and source index; mathematical proof/replay records are not model benchmark pass counts. |
| [DI System Evaluation — Top-5](https://github.com/Grounded-DI/DI-System-Eval-Top5) | Review framework and analysis archive, not an executable or empirical benchmark suite. |
| [Release-Control Challenge v1](https://github.com/Grounded-DI/Release-Control-Challenge-v1) | Documentation stub at the inspected snapshot; no benchmark inputs, verifier, or recorded result published. |
| [Evidence and Decision Library](https://github.com/Grounded-DI/START_HERE_DI_EXHIBIT_BOOKS) | Harvey audit book and Cross-Domain 83/83 companion-volume navigation. Books summarize source evidence and are not additional runs. |

## Inventory, provenance, and maintenance

- [Machine-readable collection registry](BENCHMARK_REGISTRY.json)
- [Copied-asset manifest](BENCHMARK_ASSETS.json): original repository, exact source commit/path, pinned URL, Git blob identity, SHA-256, and size
- [Discovery scope](BENCHMARK_DISCOVERY.md): public-repository search coverage, inclusions, and exclusions

The source repositories remain canonical for their publication chronology and later corrections. Each collection folder is a dated byte-preserved snapshot with a separate navigation README. Existing source rights and attributions remain applicable; consolidation grants no additional license.

For updates, verify the new source commit and evidence status, copy the changed public artifacts, refresh the manifest and collection entry, and preserve superseded score interpretations explicitly. A checksum establishes byte identity, not source truth, benchmark correctness, filing readiness, or independent validation.

### Known publication gaps

The Freshworks source refers to a completed Master File PDF/DOCX and an original-mission review JSON that are absent from its inspected public tree. Its published certificate, Markdown review, later-v2 rubric, specification, change log, and grade are included here. Missing materials are not reconstructed. See the [Freshworks folder](benchmarks/overfitting-dicta-freshworks/README.md) for the denominator history and drafting reservation.
