# Freshworks FY2023 Master File — Deterministic Benchmark v2

Version 2.0.0. This file is the human-readable rulebook. The canonical, fully fielded criterion specification is benchmark_spec.json. The original Rubric with citations.md is preserved.

## Scope and evidence hierarchy

This benchmark grades the completed Freshworks Group Master File for the financial year ended 31 December 2023. The reporting entity is Freshworks Inc.; the group perimeter is Freshworks Group, 11 subsidiaries, and 9 jurisdictions; the reporting currency is USD. June 2024 Device42 entities and other FY2024 materials are later-period context only.

Only the supplied matter folder, current rubric, evidence matrix, template, and completed DOCX may be used. No web or external facts are permitted. The FY2023 Form 10-K and FY2023 entity accounts control audited FY2023 financials and headcount.

The benchmark separates established facts, later-period context, qualified absence, qualified inference, open questions, and prohibited assertions. Source silence is not proof of a negative. “Not evidenced,” “not documented,” and “confirm with Group Tax/Treasury/Legal/management” pass where the supplied materials cannot establish absence. A complete and properly qualified document can score 100.

## Deterministic scoring

All positive criterion weights sum to exactly 100. Each criterion is scored once through its claim_key:

- pass = 1.0;
- partial = 0.5;
- fail = 0;
- not determinable = excluded from numerator and denominator only when the supplied evidence cannot establish the proposition.

Positive score = 100 × sum(weight × status value) ÷ sum(weight for determinable criteria).

Repeated coverage of one claim_key earns credit only once. Guardrails have no positive weight. A guardrail penalty applies only when the prohibited assertion actually appears. Cautious qualifications, N/A treatment, later-period attribution, and confirmation questions are not violations. A critical guardrail violation caps the final score at 79 after penalty.

Every JSON criterion contains: id, claim_key, category, priority, atomic_claim, expected_document_treatment, source, time_scope, evidence_class, pass_rule, partial_rule, fail_rule, prohibited_overstatement, weight, and source_rids.

## Category weights

| Category | Weight |
|---|---:|
| S — Scope and document control | 8.0 |
| P — Group perimeter and organization | 15.5 |
| B — Business, functions, and risks | 15.5 |
| I — Intangibles | 15.0 |
| T — Transfer pricing policy and transactions | 15.0 |
| F — Financing and treasury | 14.0 |
| X — Financial reporting and tax | 12.0 |
| Q — Evidence discipline and production quality | 5.0 |
| **Total** | **100.0** |

## Atomic criterion index

The exact deterministic rules, sources, time scopes, evidence classes, prohibited overstatements, and original R-ID mapping are in benchmark_spec.json. This index makes the scoring units visible without reintroducing compound criteria.

### S — Scope and document control

| ID | claim_key | Weight | Scoring unit |
|---|---|---:|---|
| S-01 | identity_period_currency | 2.5 | Group, reporting entity, FY ended 31 December 2023, and USD |
| S-02 | template_placeholders_removed | 1.5 | No placeholders/instructions in body, tables, headers, footers, or text boxes |
| S-03 | saas_template_adaptation | 1.5 | SaaS-specific columns and N/A treatment for physical rows |
| S-04 | scope_and_evidence_framework | 2.5 | FY2023 facts, later context, conflicts, inferences, and open questions separated |

### P — Group perimeter and organization

| ID | claim_key | Weight | Scoring unit |
|---|---|---:|---|
| P-01 | parent_legal_identity | 1.5 | US parent, Delaware, Nasdaq, and dated headquarters history |
| P-02 | fy2023_perimeter | 2.0 | 11 subsidiaries, 9 jurisdictions, Device42 excluded |
| P-03 | ownership_entity_list | 2.0 | Ownership relationships and entity list |
| P-04 | india_operating_entity | 1.5 | FTPL India identity, ownership/date, contract R&D/support role |
| P-05 | acquisition_and_dormant_entities | 1.5 | Framebench, Sassist, and Osmnez status/chronology |
| P-06 | regional_entity_roles_and_headcount | 2.5 | Regional roles, UK average headcount 100, Natero Ireland average headcount 2, conflicts |
| P-07 | australia_singapore_later_context | 1.0 | No invented FTE; later roles dated and attributed |
| P-08 | entity_changes_time_scope | 1.0 | Changes stated; no unsupported absolute no-change conclusion |
| P-09 | leadership_and_centralization | 1.5 | Parent strategic role and supported leadership/reporting centralization |
| P-10 | group_workforce | 1.0 | Approximately 4,900 FY2023 employees; later workforce figures dated |

### B — Business, functions, and risks

| ID | claim_key | Weight | Scoring unit |
|---|---|---:|---|
| B-01 | saas_business_and_products | 1.5 | Cloud SaaS model and supported product categories |
| B-02 | customer_metrics | 1.0 | 67,100 customers, 2,497 above USD 5,000 ARR, 108% NDR, sourced comparative |
| B-03 | cloud_hosting_architecture | 1.0 | Cloud-native, multi-tenant, AWS model; no invented regions |
| B-04 | principal_strategy_customer_contracts | 2.0 | Freshworks Inc. principal, strategic/IP owner, residual-return recipient |
| B-05 | digital_value_chain | 1.5 | Digital SaaS value chain; production means software activity |
| B-06 | india_rnd_support_role | 2.0 | India contract R&D/software development and support |
| B-07 | local_commercial_limited_risk | 1.5 | Local commercial limited-risk cost-plus provider characterization |
| B-08 | functional_and_risk_matrix | 3.0 | Evidence-consistent functions/risks with nuanced execution labels |
| B-09 | support_function_matrix | 1.5 | Customer support/after-sales visible or cross-referenced in matrix |
| B-10 | technology_value_drivers | 0.5 | Supported software, algorithms, Freddy AI, know-how, and qualified technical detail |

### I — Intangibles

| ID | claim_key | Weight | Scoring unit |
|---|---|---:|---|
| I-01 | fy2023_patent_position | 1.5 | FY2023 patent position; FY2024 IP register dated |
| I-02 | ip_categories_and_owners | 2.0 | Supported IP categories and Freshworks Inc. legal/economic ownership |
| I-03 | dempe_and_work_for_hire | 2.5 | US direction/control/economic return; India contract execution |
| I-04 | customer_relationship_intangibles | 1.0 | Mixed/context-dependent customer-relationship analysis |
| I-05 | goodwill_transfers_and_assignments | 1.0 | Goodwill, transfers, acquisitions, assignments without invented absence |
| I-06 | contract_rnd_agreement_terms | 2.0 | Contract R&D and missing formal terms |
| I-07 | trademark_licensing_terms | 2.0 | Trademark use/licensing and missing terms; no confirmed rate |
| I-08 | royalty_conflict | 3.0 | Conflicting royalty descriptions, owner, and no confirmed rate |

### T — Transfer pricing policy and transactions

| ID | claim_key | Weight | Scoring unit |
|---|---|---:|---|
| T-01 | tp_policy_and_alp | 2.0 | Arm’s-length policy, Group Tax oversight, annual review, guidance |
| T-02 | regional_benchmark_scope | 1.5 | Regional studies and only supported comparable count |
| T-03 | method_and_tested_party | 4.0 | TNMM/FCMU and tested party for every material transaction |
| T-04 | goods_cca_passthrough | 1.5 | Goods/CCA/pass-through treated only where supported |
| T-05 | india_markup_benchmark_conflict | 3.0 | India 15%, APAC IQR 8.34%–10.37%, median 9.32%, Group Tax conflict |
| T-06 | lvas_and_residual_return | 1.5 | Residual return separated from LVAS; no evidenced LVAS election |
| T-07 | service_compensation_and_agreements | 1.5 | Cost-plus/service compensation and agreement coverage |

### F — Financing and treasury

| ID | claim_key | Weight | Scoring unit |
|---|---|---:|---|
| F-01 | capital_and_public_offering | 1.5 | Parent capital, September 2021 IPO, approximately USD 1.1b proceeds, qualified exclusivity |
| F-02 | external_debt_and_facilities | 1.5 | Source-limited no-identified-debt observation and facilities follow-up |
| F-03 | cash_investments_and_liabilities_conflict | 2.5 | USD 488.1m cash, USD 699.5m securities, USD 1.19b total, USD 1.07b conflict |
| F-04 | shares_and_equity_compensation | 1.5 | Supported share/equity figures; causal explanation qualified |
| F-05 | treasury_pooling_netting_insurance_fx | 2.5 | Pooling/netting/captive/forward-contract treatment |
| F-06 | intercompany_loans_policy | 3.0 | Nil register versus later interview, later policy, Treasury confirmation |
| F-07 | guarantees_letters_credit_insurance | 1.5 | Guarantees, LOCs, surety, and insurance open questions |

### X — Financial reporting and tax

| ID | claim_key | Weight | Scoring unit |
|---|---|---:|---|
| X-01 | audited_financials | 3.0 | FY2023 controlling financials; revenue USD 596.4m and FY2022 USD 498.0m |
| X-02 | financial_performance_narrative | 2.0 | Revenue, SBC USD 210.707m/35%, interest, and cautious tax wording |
| X-03 | segment_reporting | 1.0 | Single public segment and qualified internal segmental-P&L gap |
| X-04 | apa_status | 1.5 | APA status and missing execution/implementation confirmation |
| X-05 | cbcr_status | 2.0 | CbCR thresholds/status without asserting a confirmed FY2023 filing |
| X-06 | india_exam_and_tax_reserves | 2.5 | India examination, MAP/dispute, and supported reserve figures |

### Q — Evidence discipline and production quality

| ID | claim_key | Weight | Scoring unit |
|---|---|---:|---|
| Q-01 | evidence_matrix_and_conflict_controls | 2.0 | Traceable sources, hierarchy, conflicts, and follow-up owners |
| Q-02 | template_and_render_quality | 3.0 | Template preservation and clean rendered/package QA |

## Guardrail layer

Guardrails are zero-weight controls. They trigger only on an actual prohibited assertion, not on a cautious qualification.

| ID | Prohibited assertion | Penalty | Critical |
|---|---|---:|:---:|
| G-01 | Physical goods, manufacturing, inventory, or physical distribution applicable | 5 | No |
| G-02 | Confirmed cost contribution arrangement | 5 | No |
| G-03 | Confirmed royalty rate/final unsupported royalty characterization | 5 | No |
| G-04 | Confirmed FY2023 CbCR filing without evidence | 10 | Yes |
| G-05 | Absolute no-external-debt/no-facilities assertion | 10 | Yes |
| G-06 | Unsupported cash pooling, netting, captive insurance, or related treasury assertion | 5 | No |
| G-07 | Unsupported guarantee programme or categorical absence | 5 | No |
| G-08 | Unsupported intercompany loan balances or terms | 10 | Yes |
| G-09 | Non-US economic IP ownership | 10 | Yes |
| G-10 | FY2024 facts presented as FY2023 | 10 | Yes |
| G-11 | Confirmed LVAS election without evidence | 5 | No |
| G-12 | Device42 included in FY2023 perimeter | 10 | Yes |
| G-13 | Unsupported “only public offering” assertion | 5 | No |
| G-14 | Later/non-controlling financials replacing FY2023 controlling sources | 10 | Yes |
| G-15 | Unsupported Australia/Singapore FY2023 FTE | 5 | No |
| G-16 | Unreconciled ledger treated as authoritative over FY2023 accounts | 5 | No |
| G-17 | Source silence converted into an absolute negative | 5 | No |

## Original-rubric audit

The original rubric was not deterministic because it used importance labels rather than numeric weights and contained:

1. duplicate or overlapping facts across multiple sections;
2. compound criteria combining identity, time, ownership, function, and risk claims;
3. FY2024 headcount, IP, organization-chart, loan-policy, and functional material that could be mistaken for FY2023 evidence;
4. absence-based requirements that treated missing evidence as proof of no event;
5. unsupported causal explanations, especially for RSU/ESPP movement;
6. positive criteria that conflicted with negative-space guards;
7. exact-section or exact-table requirements inconsistent with a substance-over-location rule; and
8. unsupported absolute wording concerning debt, liabilities, guarantees, facilities, other public offerings, restructurings, segmental P&Ls, and CbCR.

The v2 conversion:

- splits compound claims into atomic claim_keys;
- deduplicates repeated claims;
- makes FY2023 source hierarchy controlling;
- downgrades FY2024 material to dated later context;
- converts unsupported negatives into qualified-absence or open-question criteria;
- treats unsupported prohibited assertions as separate guardrail failures;
- accepts equivalent wording and sensible placement;
- uses production placement only for Q-02 and not as a hidden factual prerequisite; and
- preserves every original R-ID through source_rids in benchmark_spec.json.

## Explicit tension resolutions

- R-105/R-148: a source-limited balance-sheet observation may pass; unsupported FY2023 loan conclusions trigger the loan guardrail.
- R-107: a later reference-rate-plus-spread policy is later context and cannot establish FY2023 balances or terms.
- R-110: absolute liability wording is not required or rewarded.
- R-114: the equity movement may be stated; causal explanation must be qualified.
- R-115b, R-117, R-146, and R-152: qualified absence treatment passes; unsupported affirmative or absolute-negative treatment does not.
- R-154/R-160: IPO date/proceeds are positive facts; “only public offering” is qualified rather than required.
- R-024: source silence does not establish no restructuring or entity change.
- R-026: strategic centralization does not require an unsupported claim that every subsidiary reports to one named executive.
- R-033: FY2024 organization-chart material is later context only.
- R-133: CbCR status is positive; a confirmed filing is a separate guardrail.
- R-150: FY2024 headcount, IP, and function material cannot replace the FY2023 position.

## Crosswalk rule

The full reverse crosswalk is retained in the source_rids arrays of benchmark_spec.json. Every original R-ID, including lettered variants such as R-016a, R-115b, and R-134a, must appear in at least one atomic criterion or guardrail. An R-ID may appear in more than one destination where the original item contained both a positive claim and a prohibited-assertion control.

