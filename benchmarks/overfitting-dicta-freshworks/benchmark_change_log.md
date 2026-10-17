# Benchmark change log

## Publication correction — 16 October 2026

The canceled later-v2 grade report has been removed from the current publication. The recorded result is **89/89 applicable original-mission review-weight points**. The later-v2 rubric and specification remain as the disclosed accounting reference.

## Version 2.0.0 — deterministic evidence-disciplined update

Date: 16 October 2026

Status: reference scoring framework for the Freshworks Group Master File — FY2023.

The original Rubric with citations.md was preserved. The completed Master File was not modified. No web source or external fact was used.

## Files created

- Rubric with citations — Deterministic v2.md — human-readable benchmark.
- benchmark_spec.json — canonical machine-readable specification.
- benchmark_change_log.md — this audit and change record.

## Baseline audit

The supplied rubric was useful as a source-indexed checklist but was not deterministic. It used importance labels rather than a fixed numerical model and contained overlapping and compound criteria. The principal defects were:

| Defect | Treatment in v2 |
|---|---|
| Duplicate facts repeated across document-control, group, business, IP, TP, and finance sections | One claim_key and one positive scoring unit; repeated coverage earns no additional credit |
| Compound criteria combining multiple independent facts | Split into atomic criteria with separate pass/partial/fail rules |
| FY2024 headcount, IP, organization-chart, loan-policy, or function material used as FY2023 evidence | Later-period evidence class; credit only when dated and attributed |
| Source silence treated as proof of no debt, no guarantees, no restructuring, no other offering, no internal P&L, or no filing | Qualified-absence or open-question treatment; no invention required |
| Unsupported causal explanation for the RSU/ESPP movement | Reportable figure separated from qualified inference |
| Positive criteria conflicting with negative-space guards | Positive evidence and zero-weight guardrail layers separated |
| Exact-section or exact-table scoring inconsistent with substance-over-location | Equivalent wording and sensible placement pass; placement is a Q-02 production check only |
| “No external debt,” “only public offering,” “no guarantee programme,” and similar absolutes | Rewritten as source-limited observations or prohibited-assertion controls |
| Unweighted importance labels | Fixed positive weights totaling exactly 100 |

## Fixed scoring changes

The v2 score is 100 times weighted status value divided by the determinable positive weight. Pass is 1.0, partial is 0.5, fail is 0, and not determinable is excluded only when the evidence cannot establish the proposition. The score is not a raw checklist total.

The positive weights are:

| Category | Weight |
|---|---:|
| Scope and document control | 8.0 |
| Group perimeter and organization | 15.5 |
| Business, functions, and risks | 15.5 |
| Intangibles | 15.0 |
| Transfer pricing policy and transactions | 15.0 |
| Financing and treasury | 14.0 |
| Financial reporting and tax | 12.0 |
| Evidence discipline and production quality | 5.0 |
| **Total** | **100.0** |

Guardrails have zero positive weight. They apply only when the prohibited assertion appears. A critical guardrail penalty is 10 points and caps the final score at 79; a non-critical guardrail penalty is 5 points. Qualified language does not trigger a guardrail.

## Criterion conversion and crosswalk

The authoritative crosswalk is the union of every criterion.source_rids and guardrail.source_rids array in benchmark_spec.json. The following records the substantive conversion:

### Scope and perimeter

- R-001/R-002 → S-02 and Q-02: placeholder/instruction removal and package/production checks.
- R-003/R-004/R-005 → S-01: group, reporting entity, period, and currency.
- R-006 → S-03 and Q-02: SaaS adaptation and template preservation.
- R-007/R-027 → P-01: parent legal identity, listing, and headquarters history.
- R-008/R-009/R-010/R-153 → P-02 and G-12: FY2023 perimeter and Device42 exclusion.
- R-011/R-023/R-149/R-159 → P-03 and G-09/G-17: ownership/entity list and negative-space/IP controls.
- R-012 → P-04: India operating entity and role.
- R-013/R-014/R-015/R-028/R-069 → P-05 and I-05: acquisition, dormant status, and chronology.
- R-016a/R-016b/R-017a/R-017b/R-018a/R-018b/R-019a/R-019b/R-020a/R-020b/R-030/R-031a/R-031b → P-06: regional roles, controlling headcount, and conflicts.
- R-021a/R-021b/R-021c/R-022a/R-022b/R-022c/R-032/R-156 → P-07 and G-15: Australia/Singapore missing FTE and later context.
- R-024/R-033/R-070 → P-08, S-04, Q-01, and G-10/G-17 as applicable: changes, later chart, and absence safeguards.
- R-025/R-026 → P-09: strategic centralization and leadership, without an unsupported complete reporting-line assertion.
- R-029/R-161 → P-10 and G-17: FY2023 workforce and later/absence guard.

### Business, functions, and intangibles

- R-034/R-035/R-036/R-037 → B-01/B-02/B-03: SaaS, products, metrics, and hosting.
- R-038/R-039/R-040 → B-04: principal, strategy, contracts, IP, and residual returns.
- R-041/R-044/R-140 → B-05 and G-01: digital value chain and physical-goods guard.
- R-042/R-043/R-047 → B-06 and B-08: India contract R&D/support and functional matrix.
- R-045/R-046/R-048/R-049/R-051/R-052/R-053/R-054 → B-07/B-08: local limited-risk profile and nuanced functions/risks.
- R-050 → B-09: support visibility in the matrix.
- R-055 → B-10: supported technology value drivers without invented technical detail.
- R-056/R-057 → I-01 and S-04/G-10: FY2023 patents and FY2024 IP context.
- R-058/R-059/R-063 → I-02: IP categories and ownership.
- R-060/R-061/R-062/R-064/R-102 → I-03: DEMPE, control, work-for-hire, and agreement framework.
- R-065 → I-04: customer relationships as a qualified analysis.
- R-066/R-067/R-068/R-069/R-070 → I-05: goodwill, transfers, acquisitions, and assignments.
- R-071/R-072 → I-06: contract R&D agreement gaps.
- R-073/R-074 → I-07: trademark licensing gaps.
- R-076/R-089/R-142 → I-08 and G-03: royalty conflict and no confirmed rate.

### Transfer pricing and finance

- R-075/R-078 → T-07: service compensation and agreement coverage.
- R-077/R-079/R-080 → T-01: policy, oversight, annual review, and guidance.
- R-081/R-097 → T-02: regional benchmark scope and supported comparable counts.
- R-082/R-084/R-085/R-086/R-087/R-088/R-098 → T-03: method and tested party.
- R-091/R-092/R-141 → T-04 and G-02: goods, pass-through, and CCA control.
- R-095/R-096/R-100/R-101 → T-05: India 15% versus APAC range conflict.
- R-099/R-103/R-152 → T-06 and G-11: residual return and no evidenced LVAS election.
- R-090/R-117/R-118a/R-118b/R-118c/R-146 → F-07 and G-07: guarantees, LOCs, surety, and insurance.
- R-093/R-094/R-107/R-108/R-147/R-148 → F-06 and G-08: loan-register conflict and unsupported-term guard.
- R-104/R-106/R-154/R-160 → F-01 and G-13: IPO facts and qualified “only offering” language.
- R-105/R-110/R-119/R-144 → F-02 and G-05: source-limited debt/facilities treatment.
- R-109/R-111/R-113 → F-03: cash/investment conflict and unsupported liability language.
- R-112/R-114 → F-04: share/equity figures and causal-inference safeguard.
- R-115a/R-115b/R-116/R-145 → F-05 and G-06/G-17: pooling, netting, captive, and FX safeguards.

### Financial reporting and tax

- R-120/R-121/R-122/R-155/R-158 → X-01 and G-14/G-17: controlling FY2023 financials.
- R-123/R-124/R-125/R-126/R-127/R-128 → X-02: performance narrative and cautious tax language.
- R-129/R-130 → X-03 and G-17: public segment reporting versus missing internal P&L.
- R-131/R-132 → X-04: APA status.
- R-133/R-134a/R-134b/R-135/R-143 → X-05 and G-04: CbCR status versus filing assertion.
- R-136/R-137/R-138/R-139 → X-06: India examination, MAP/dispute, and tax reserves.

### Reclassified or retired logic

- The original positive criteria requiring categorical absence were downgraded to qualified absence or open question: R-024, R-105, R-110, R-115b, R-117, R-146, R-152, R-154/R-160, and the negative portions of R-129/R-130.
- The original loan-policy material in R-107 was reclassified as later context and cannot establish FY2023 loan terms.
- The original causal explanation in R-114 was reclassified as a qualified inference.
- R-140 through R-157 were separated into positive treatment and guardrails where they combined a substantive point with a prohibited assertion.
- R-158 through R-161 were retained as evidence-discipline controls; they cannot create a positive requirement to assert an absence.
- Exact-location requirements were merged into substantive claim_keys and Q-02; location no longer changes factual credit.

No original R-ID was discarded. The full source-rid arrays are the preserved crosswalk, and the required validation is that every original ID in the current rubric appears at least once.

## Known tension resolutions

| Tension | v2 resolution |
|---|---|
| R-105/R-148 | A source-limited financial-statement observation may pass; unsupported FY2023 loan conclusions trigger G-08 |
| R-107 | Later policy is later context only |
| R-110 | Absolute liability description is not required or rewarded |
| R-114 | Amounts may be stated; causation must be qualified |
| R-115b/R-117/R-146/R-152 | Qualified absence passes; unsupported affirmative or absolute-negative statements do not |
| R-154/R-160 | IPO date/proceeds are positive; “only offering” is qualified |
| R-024 | Source silence does not establish no restructuring or entity change |
| R-026 | Strategic centralization does not require an unsupported complete reporting line |
| R-033/R-150 | FY2024 organization, headcount, IP, and function facts are later context only |
| R-133 | CbCR status is positive; confirmed filing is a separate guardrail |

## Validation record

The [original-mission review](Freshworks%20FY2023%20original%20mission%20review.md) records the 89/89 applicable review-weight result, guardrails, criterion-level evidence matrix, reservations, and delivery verdict. The completed DOCX was treated as read-only input.

