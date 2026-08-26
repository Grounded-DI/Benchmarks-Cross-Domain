# Grounded DI OS Cross-Domain Benchmark Series

## Google Research IFEval Prompts 1-12

This repository contains twelve auditable one-shot benchmark records produced under the Grounded DI OS / FastPath 5.6 / Protocol A recording procedure.

The series uses official Google Research Instruction-Following Evaluation (IFEval) items. Each run preserves the source item, the submitted response, the encoded constraints, the evaluator status, the local checks, the evidence boundary, and the resulting PDF record.

## Results at a glance

| Measure | Result |
| --- | ---: |
| Benchmark records | 12 / 12 |
| Prompt-level strict passes under the documented local checks | 12 / 12 |
| Official encoded constraints passed locally | 25 / 25 |
| Official evaluator executions in this workspace | 0 / 12 |
| Independent external verifications | 0 / 12 |
| Private preflight corrections | 1 total |

The result is therefore a complete local pass record, not an official IFEval score or an independently verified benchmark result.

## What was tested

| Prompt | IFEval item | Task | Official encoded constraints | Local result | Preflight |
| ---: | ---: | --- | --- | --- | ---: |
| 1 | 136 | Explain what an atomic nucleus is in exactly nine short Markdown bullets and under 100 words. | Exactly 9 bullets; fewer than 100 words. | 2/2; strict pass | 0 |
| 2 | 1325 | Write a funny article about dinosaur extinction inside quotation marks with exactly eight bullets. | Quotation-wrapped response; exactly 8 Markdown bullets. | 2/2; strict pass | 1 |
| 3 | 1377 | Produce a five-part software-engineering planning document using the specified headings and `***` dividers. | Exactly 5 paragraphs under the official paragraph checker. | 1/1; strict pass | 0 |
| 4 | 1379 | Write a limerick about Sarah living in a town that is always 90°F. | At least 6 highlighted sections; Sarah appears fewer than twice; Sarah exists. | 3/3; strict pass | 0 |
| 5 | 1389 | Write an all-capital English letter to a friend who moved away. | English/all capitals; the letter `o` appears at least 40 times. | 2/2; strict pass | 0 |
| 6 | 1402 | Recommend a college with open enrollment and regional accreditation. | Letter `p` appears at least 15 times; `DuPage` and `Dade` are absent. | 2/2; strict pass | 0 |
| 7 | 1481 | Write a casual, strange resume for Antonia Maj applying to a coffee company. | Exactly 2 `SECTION` markers; exactly 2 Markdown bullets. | 2/2; strict pass | 0 |
| 8 | 1508 | Write a comma-free haiku about a lion. | Keywords `forests` and `riddle`; zero commas. | 2/2; strict pass | 0 |
| 9 | 1418 | Write a 30-line poem with one short sentence per line. | Zero commas; sentence count at least 30 and fewer than 31. | 3/3; strict pass | 0 |
| 10 | 1512 | Create a short-sentence forum thread about people waiting for local news. | At least 20 square-bracket username placeholders; zero commas. | 2/2; strict pass | 0 |
| 11 | 1516 | Write a five-line lowercase English poem about binge watching. | Lowercase English; keyword `netflix` exists. | 2/2; strict pass | 0 |
| 12 | 3409 | Create a funny fighting-game slogan. | Entire response wrapped in double quotes; at least 3 Markdown highlights. | 2/2; strict pass | 0 |

The official constraints are the machine-scored requirements encoded in the IFEval dataset. Some natural-language task requirements were checked separately and are identified below as manual checks.

## Record files

The PDF is the primary record for each run. The scored response is reproduced exactly inside its record.

| Prompt | Record |
| ---: | --- |
| 1 | [Prompt 1 - IFEval 136](Luna_OneShot_Benchmark_Record_v2_IFEval_136.pdf) |
| 2 | [Prompt 2 - IFEval 1325](Luna_OneShot_Benchmark_Record_Prompt2_IFEval_1325.pdf) |
| 3 | [Prompt 3 - IFEval 1377](Luna_OneShot_Benchmark_Record_Prompt3_IFEval_1377.pdf) |
| 4 | [Prompt 4 - IFEval 1379](Grounded_DI_OS_Benchmark_Record_Prompt4_IFEval_1379.pdf) |
| 5 | [Prompt 5 - IFEval 1389](Grounded_DI_OS_Benchmark_Record_Prompt5_IFEval_1389.pdf) |
| 6 | [Prompt 6 - IFEval 1402](Grounded_DI_OS_Benchmark_Record_Prompt6_IFEval_1402.pdf) |
| 7 | [Prompt 7 - IFEval 1481](Grounded_DI_OS_Benchmark_Record_Prompt7_IFEval_1481.pdf) |
| 8 | [Prompt 8 - IFEval 1508](Grounded_DI_OS_Benchmark_Record_Prompt8_IFEval_1508.pdf) |
| 9 | [Prompt 9 - IFEval 1418](Grounded_DI_OS_Benchmark_Record_Prompt9_IFEval_1418.pdf) |
| 10 | [Prompt 10 - IFEval 1512](Grounded_DI_OS_Benchmark_Record_Prompt10_IFEval_1512.pdf) |
| 11 | [Prompt 11 - IFEval 1516](Grounded_DI_OS_Benchmark_Record_Prompt11_IFEval_1516.pdf) |
| 12 | [Prompt 12 - IFEval 3409](Grounded_DI_OS_Benchmark_Record_Prompt12_IFEval_3409.pdf) |

A consolidated bundle for the first three records is also available: [Prompts 1-3 regenerated bundle](Grounded_DI_Universal_Benchmark_Records_IFEval_136_1325_1377_Regenerated.zip).

## Prompt-by-prompt explanation

### Prompt 1 - atomic nucleus

This is a compact factual explanation task. The response had to use exactly nine Markdown bullet lines and stay below 100 words. Grounded DI counted the bullet lines and lexical word tokens separately, then confirmed that the scored response contained no extra prose.

### Prompt 2 - dinosaur extinction

This combines a creative writing task with two rigid formatting requirements: the complete response must be surrounded by straight double quotation marks and contain exactly eight Markdown bullet lines. One private preflight correction moved the opening quotation mark so the published bullet-list regex counted all eight bullets. The correction was disclosed rather than hidden.

### Prompt 3 - software planning document

This task required five labeled parts separated by four literal `***` dividers. The official IFEval constraint is paragraph count. Grounded DI additionally checked the required headings, their order, the divider count, substantive replacement of placeholders, and the absence of extra dividers inside the sections.

### Prompt 4 - Sarah limerick

This is a constrained poem task. The official checks require at least six Markdown-highlighted spans and require the name Sarah to exist but appear fewer than twice. The local audit counted the highlights and checked the name case-insensitively. The poem’s subject and poem-only format were recorded as manual task checks.

### Prompt 5 - all-capital letter

This tests global case control together with a high-frequency character requirement. The response had to be an English letter in all capitals and contain the letter `O` at least 40 times. Grounded DI checked the case condition and character count independently.

### Prompt 6 - college recommendation

This is a recommendation task with lexical constraints. The response had to contain at least 15 occurrences of the letter `p` while avoiding the forbidden words `DuPage` and `Dade`. The local check followed the published case-insensitive, word-boundary approach for the forbidden terms.

### Prompt 7 - Antonia Maj resume

This tests simultaneous section and bullet formatting. The resume had to contain exactly two `SECTION` markers and exactly two Markdown bullet lines while still providing substantive content about Antonia’s education, marketing, customer service, sales, and coffee-company application.

### Prompt 8 - lion haiku

This is a small poetic format task with two lexical constraints. The response had to include the exact keywords `forests` and `riddle` and contain no comma characters. The haiku itself was preserved as task content; the encoded score was based on keyword existence and comma absence.

### Prompt 9 - 30-line poem

This is the most structurally demanding item in the series. The official evaluator encodes three constraints: no commas, fewer than 31 sentences, and at least 30 sentences. Grounded DI also manually checked exactly 30 non-empty lines, one short sentence per line, terminal periods, poem-only output, and the absence of sentence-counting traps such as abbreviations or URLs.

### Prompt 10 - local-news forum thread

This tests placeholder generation and punctuation control. The response had to be a coherent thread with at least 20 square-bracket username placeholders and no commas. Short sentences and forum coherence were additional manual task checks because they were not separately encoded in the official instruction list.

### Prompt 11 - lowercase binge-watching poem

This combines a global lowercase-English requirement with the keyword `netflix`. Grounded DI also manually checked the five-line structure, AABBA rhyme scheme, binge-watching subject, and poem-only response. The official score was limited to the two encoded constraints.

### Prompt 12 - fighting-game slogan

This is a compact formatting test. The response had to begin and end with straight double quotation marks after whitespace stripping and contain at least three non-empty Markdown highlights. Grounded DI also checked that the text functioned as a slogan for a funny fighting game.

## How Grounded DI kept the benchmark fair

Grounded DI treated fairness as an evidence and claim-boundary problem rather than simply reporting a favorable number.

### 1. Official item control

Each item was identified by its official IFEval key. The exact prompt, instruction IDs, and parameters were checked against the official dataset before the response was finalized. The checker source was consulted for the relevant counting behavior. The series did not substitute rewritten prompts or third-party versions.

Controlling sources:

- [Google Research instruction-following evaluation repository](https://github.com/google-research/google-research/tree/master/instruction_following_eval)
- [Official IFEval input dataset](https://raw.githubusercontent.com/google-research/google-research/master/instruction_following_eval/data/input_data.jsonl)
- [Official instruction checker source](https://github.com/google-research/google-research/blob/master/instruction_following_eval/instructions.py)
- [Official IFEval paper](https://arxiv.org/abs/2311.07911)
- [Official sentence-count utility](https://github.com/google-research/google-research/blob/master/instruction_following_eval/instructions_util.py)

### 2. Benchmark sovereignty

The official encoded constraints controlled the benchmark score. Grounded DI did not silently repair an awkward prompt, add favorable criteria, remove inconvenient criteria, or change the evaluator’s terminology.

When a natural-language requirement was not encoded by IFEval, it was labeled separately as a manual task check rather than being folded into the official score.

### 3. One-shot discipline

Each item was treated as one attempted submission. Private drafting and preflight checking were allowed by the recording protocol, but the number of corrections was disclosed. Prompt 2 required one disclosed preflight correction; the other eleven records report zero.

After finalization, the scored response was preserved exactly. No response was changed after observing a score, and no completed failed submission was silently replaced with a passing one.

### 4. Evaluator honesty

The official IFEval evaluator was not executable in this workspace for these records. Every result is therefore labeled:

> LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR

The local checks were designed to mirror the published checker behavior for the relevant constraints. They are not presented as official scores. Because the official evaluator did not execute, official-versus-local discrepancies are reported as not measurable.

### 5. Separation of scoring from auditing

The scored response contains only the requested answer. It does not contain the benchmark title, citations, score, audit notes, or explanations. The audit material appears outside the scored block in a separate PDF section.

This prevents the record from confusing a model’s task response with the documentation about that response.

### 6. Route and runtime separation

The requested route was recorded as `FastPath 5.6 / Luna Max`. The observed runtime was recorded separately as `Codex`, because the exact model identifier was not exposed by the runtime. The records do not convert a requested route into a claimed model identity.

### 7. Reproducible evidence

Each PDF preserves the exact prompt and final response, source URLs, timestamp and timezone, evaluator status, local constraint results, manual checks, preflight count, and SHA-256 hashes. The same visual record architecture was used across the series so that the benchmark content changes without changing the evidence structure.

### 8. Fail-closed claims

The records use `NOT INDEPENDENTLY VERIFIED` because no independent reviewer or external evaluator verified the runs. The series does not claim external certification, universal performance, representative performance across all models, or an official leaderboard result.

## What the series establishes

Under the documented Grounded DI OS recording conditions:

- all twelve finalized responses passed their local equivalents of the official encoded constraints;
- all twelve records preserved the submitted response and disclosed the evaluator limitation;
- the series contains 25/25 locally passed encoded constraints and 12/12 locally passed prompt-level strict results;
- the records are auditable as internal one-shot records.

## What the series does not establish

This is not:

- an official IFEval score;
- an independently verified benchmark;
- a blind third-party evaluation;
- a claim that the observed runtime will pass every IFEval item;
- a representative estimate of all model behavior;
- proof that the requested Luna Max route was the observed underlying model.

The most accurate description is: **a documented Grounded DI OS one-shot run of twelve official IFEval items, with all final responses passing transparent local checks and no official or independent verification claim.**

## Suggested reproduction procedure

1. Obtain the exact official IFEval item by key.
2. Preserve the prompt without rewriting it.
3. Run one response attempt under the stated route and tool conditions.
4. Perform private preflight checks before finalization.
5. Record every preflight correction.
6. Preserve the final response exactly.
7. Run the official evaluator if it is actually available; otherwise use a clearly labeled local equivalent.
8. Separate official encoded constraints from manual task checks.
9. Generate the record with the prompt, response, evidence, hashes, limitations, and claim boundaries.
10. Do not publish a stronger claim than the evidence supports.

## Status

**INTERNAL ONE-SHOT RECORDS**  
**LOCAL CHECK PASS: 12/12**  
**OFFICIAL EVALUATOR: NOT EXECUTED**  
**EVIDENCE: NOT INDEPENDENTLY VERIFIED**
