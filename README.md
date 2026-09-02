# Grounded DI OS Cross-Domain Benchmark Series

## Google Research IFEval Prompts 1-31

This repository contains thirty-one documented one-shot benchmark records produced under the Grounded DI OS / FastPath 5.6 / Protocol A recording procedure. Route conditions are disclosed per record: Prompts 1–20 use FastPath 5.6 / Luna Max; Prompt 21 uses FastPath 5.6 / SOL Max; Prompts 22–24 and 26–31 use FastPath 5.6 / Terra Extra High; Prompt 25 uses FastPath 5.6 / SOL Extra High.

The series uses official Google Research Instruction-Following Evaluation (IFEval) items. Each run preserves the source item, the submitted response, the encoded constraints, the evaluator status, the local checks, the evidence boundary, and the resulting PDF record.

## Results at a glance

| Measure | Result |
| --- | ---: |
| Benchmark records | 31 / 31 |
| Prompt-level strict passes under the documented local checks | 31 / 31 |
| Official encoded constraints passed locally | 62 / 62 |
| Official evaluator executions in this workspace | 11 / 31 |
| Independent external verifications | 0 / 31 |
| Private preflight corrections | 1 total |

The result is therefore a complete local pass record, not an official IFEval score or an independently verified benchmark result.

## What was tested

| Prompt | IFEval item | Task | Official encoded constraints | Local result | Preflight |
| ---: | ---: | --- | --- | --- | ---: |
| 1 | 136 | Explain what an atomic nucleus is in exactly nine short Markdown bullets and under 100 words. | Exactly 9 bullets; fewer than 100 words. | 2/2; strict pass | 0 |
| 2 | 1325 | Write a funny article about dinosaur extinction inside quotation marks with exactly eight bullets. | Quotation-wrapped response; exactly 8 Markdown bullets. | 2/2; strict pass | 1 |
| 3 | 1377 | Produce a five-part software-engineering planning document using the specified headings and *** dividers. | Exactly 5 paragraphs under the official paragraph checker. | 1/1; strict pass | 0 |
| 4 | 1379 | Write a limerick about Sarah living in a town that is always 90°F. | At least 6 highlighted sections; Sarah appears fewer than twice; Sarah exists. | 3/3; strict pass | 0 |
| 5 | 1389 | Write an all-capital English letter to a friend who moved away. | English/all capitals; the letter o appears at least 40 times. | 2/2; strict pass | 0 |
| 6 | 1402 | Recommend a college with open enrollment and regional accreditation. | Letter p appears at least 15 times; DuPage and Dade are absent. | 2/2; strict pass | 0 |
| 7 | 1481 | Write a casual, strange resume for Antonia Maj applying to a coffee company. | Exactly 2 SECTION markers; exactly 2 Markdown bullets. | 2/2; strict pass | 0 |
| 8 | 1508 | Write a comma-free haiku about a lion. | Keywords forests and riddle; zero commas. | 2/2; strict pass | 0 |
| 9 | 1418 | Write a 30-line poem with one short sentence per line. | Zero commas; sentence count at least 30 and fewer than 31. | 3/3; strict pass | 0 |
| 10 | 1512 | Create a short-sentence forum thread about people waiting for local news. | At least 20 square-bracket username placeholders; zero commas. | 2/2; strict pass | 0 |
| 11 | 1516 | Write a five-line lowercase English poem about binge watching. | Lowercase English; keyword netflix exists. | 2/2; strict pass | 0 |
| 12 | 3409 | Create a funny fighting-game slogan. | Entire response wrapped in double quotes; at least 3 Markdown highlights. | 2/2; strict pass | 0 |
| 13 | 1609 | Discuss asking Sonia out in four paragraphs with outer double quotation marks. | Exactly 4 paragraphs; paragraph 1 begins with weekend; quotation wrapping. | 2/2; strict pass | 0 |
| 14 | 1705 | Write a professional raise-request email with a P.P.S. | P.P.S. postscript; exact ending phrase Hope you agree with me. | 2/2; strict pass | 0 |
| 15 | 1713 | Write an interesting and funny article about banana-peel biology. | disappointed appears at least 2 times; at least 6 Markdown highlights. | 2/2; strict pass | 0 |
| 16 | 1825 | Explain Generative Adversarial Networks using bullet points. | No commas; P.P.S. postscript; five required keywords. | 3/3; strict pass | 0 |
| 17 | 1936 | Write a customer-service representative performance rubric. | Exactly 6 counted bullets; forbidden whole words absent. | 2/2; strict pass | 0 |
| 18 | 1908 | Evaluate the statement that wizards are more powerful than sorcerers. | At least 30 sentences; exactly 2 bullets; at least 8 placeholders. | 3/3; strict pass | 0 |
| 19 | 1980 | Write a blog post about the sleek new magistrates. | At least 300 words; exactly 3 asterisk bullets; P.S. marker. | 3/3; strict pass | 0 |
| 20 | 3098 | Write a blog post about improving writing skills. | Exactly 3 bullets; exactly 4 sections separated by ***; at least 2 all-capital words. | 3/3; strict pass | 0 |
| 21 | 2704 | Write a haiku about foolish behavior in the form of a question for young readers and include not studying. | Two responses separated by `******`; title wrapped in `<<>>`; zero commas. | 3/3; strict pass; official pass | 0 |
| 22 | 2857 | Write a performance-review rubric for a software engineer and wrap the entire output in JSON. | JSON parseability after limited Markdown-fence normalization. | 1/1; strict pass; official pass | 0 |
| 23 | 3224 | Write an interesting riddle that uses math notation and repeat the request before answering. | Repeat-prompt prefix (`combination:repeat_prompt`). | 1/1; strict pass; official pass | 0 |
| 24 | 3753 | Determine whether a = 20 from a + b + c = 30, b = 10, and c = 5 using one specified answer phrase. | Accepted constrained-response option (`detectable_format:constrained_response`). | 1/1; strict pass; official pass | 0 |
| 25 | 2225 | Explain the difference between a levee and an embankment and respond only in Korean. | Korean response (`language:response_language`). | 1/1; strict pass; official pass | 0 |
| 26 | 2880 | Explain the difference between the Russell class and the set of all sets in exactly two paragraphs beginning paragraph 1 with booster. | Exactly 2 paragraphs and paragraph 1 first word booster (`length_constraints:nth_paragraph_first_word`). | 1/1; strict pass; official pass | 0 |
| 27 | 2311 | Explain why a serving of 32 grams of unsalted almonds lists 396 calories without using commas. | No ASCII comma (`punctuation:no_comma`). | 1/1; strict pass; official pass | 0 |
| 28 | 3386 | Determine how many whole gallons Jennifer can buy with $10 at $3 per gallon while avoiding two keywords and including remainder. | Forbidden words absent; keyword remainder present (`keywords:forbidden_words`, `keywords:existence`). | 2/2; strict pass; official pass | 0 |
| 29 | 143 | Calculate a colt's height after 3 years using a three-asterisk separator and a terminal P.P.S. postscript. | Exactly 2 paragraphs; P.P.S. marker (`length_constraints:number_paragraphs`, `detectable_content:postscript`). | 2/2; strict pass; official pass | 0 |
| 30 | 136 | Explain what an atomic nucleus is in exactly 9 very short bullet points under 100 words. | Exactly 9 bullets; fewer than 100 words (`detectable_format:number_bullet_lists`, `length_constraints:number_words`). | 2/2; strict pass; official pass | 0 |
| 31 | 1375 | Demonstrate an unsafe Java database-query pattern and its parameterized fix with code comments and the keyword `vulnerable`. | Exactly 2 paragraphs; keyword `vulnerable` present (`length_constraints:number_paragraphs`, `keywords:existence`). | 2/2; strict pass; official pass | 0 |

The official constraints are the machine-scored requirements encoded in the IFEval dataset. Some natural-language task requirements were checked separately and are identified below as manual checks.


## Record files

The PDF is the primary record for each run. The scored response is reproduced exactly inside its record.

| Prompt | Record |
| ---: | --- |
| 1 | [Prompt 1 - IFEval 136](Grounded_DI_OS_Benchmark_Record_Prompt1_IFEval_136_v1.pdf) |
| 2 | [Prompt 2 - IFEval 1325](Grounded_DI_OS_Benchmark_Record_Prompt2_IFEval_1325_v1.pdf) |
| 3 | [Prompt 3 - IFEval 1377](Grounded_DI_OS_Benchmark_Record_Prompt3__IFEval_1377_v1.pdf) |
| 4 | [Prompt 4 - IFEval 1379](Grounded_DI_OS_Benchmark_Record_Prompt4_IFEval_1379.pdf) |
| 5 | [Prompt 5 - IFEval 1389](Grounded_DI_OS_Benchmark_Record_Prompt5_IFEval_1389.pdf) |
| 6 | [Prompt 6 - IFEval 1402](Grounded_DI_OS_Benchmark_Record_Prompt6_IFEval_1402.pdf) |
| 7 | [Prompt 7 - IFEval 1481](Grounded_DI_OS_Benchmark_Record_Prompt7_IFEval_1481.pdf) |
| 8 | [Prompt 8 - IFEval 1508](Grounded_DI_OS_Benchmark_Record_Prompt8_IFEval_1508.pdf) |
| 9 | [Prompt 9 - IFEval 1418](Grounded_DI_OS_Benchmark_Record_Prompt9_IFEval_1418.pdf) |
| 10 | [Prompt 10 - IFEval 1512](Grounded_DI_OS_Benchmark_Record_Prompt10_IFEval_1512.pdf) |
| 11 | [Prompt 11 - IFEval 1516](Grounded_DI_OS_Benchmark_Record_Prompt11_IFEval_1516.pdf) |
| 12 | [Prompt 12 - IFEval 3409](Grounded_DI_OS_Benchmark_Record_Prompt12_IFEval_3409.pdf) |
| 13 | [Prompt 13 - IFEval 1609](Grounded_DI_OS_Benchmark_Record_Prompt13_IFEval_1609.pdf) |
| 14 | [Prompt 14 - IFEval 1705](Grounded_DI_OS_Benchmark_Record_Prompt14_IFEval_1705.pdf) |
| 15 | [Prompt 15 - IFEval 1713](Grounded_DI_OS_Benchmark_Record_Prompt15_IFEval_1713.pdf) |
| 16 | [Prompt 16 - IFEval 1825](Grounded_DI_OS_Benchmark_Record_Prompt16_IFEval_1825.pdf) |
| 17 | [Prompt 17 - IFEval 1936](Grounded_DI_OS_Benchmark_Record_Prompt17_IFEval_1936.pdf) |
| 18 | [Prompt 18 - IFEval 1908](Grounded_DI_OS_Benchmark_Record_Prompt18_IFEval_1908.pdf) |
| 19 | [Prompt 19 - IFEval 1980](Grounded_DI_OS_Benchmark_Record_Prompt19_IFEval_1980.pdf) |
| 20 | [Prompt 20 - IFEval 3098](Grounded_DI_OS_Benchmark_Record_Prompt20_IFEval_3098.pdf) |
| 21 | [Prompt 21 - IFEval 2704](Grounded_DI_OS_Benchmark_Record_Prompt21_IFEval_2704_SOL_Max.pdf) · [supplied package-hash sidecar](Grounded_DI_OS_Benchmark_Record_Prompt21_IFEval_2704_SOL_Max_Package.zip.sha256.txt) |

Prompt 21’s supplied SHA-256 sidecar names the source package archive. This update publishes the PDF record and sidecar; it does not claim that a separate Prompt 21 ZIP archive is present.

| 22 | [Prompt 22 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt22_IFEval_2857_Terra_Extra_High_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt22_IFEval_2857_Terra_Extra_High_Package.zip.sha256.txt) |

Prompt 22 is published as its archival ZIP package. The PDF record and its PDF checksum are inside the ZIP; the separate sidecar verifies the ZIP itself.

| 23 | [Prompt 23 - IFEval 3224](Grounded_DI_OS_Benchmark_Record_Prompt23_IFEval_3224_Terra_Extra_High.pdf) · [supplied package-hash sidecar](Grounded_DI_OS_Benchmark_Record_Prompt23_IFEval_3224_Terra_Extra_High_Package.zip.sha256.txt) |

Prompt 23 is published as its PDF record and supplied package-hash sidecar. The sidecar names and hashes the source package archive; this update does not claim that a separate Prompt 23 ZIP archive is present.

| 24 | [Prompt 24 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt24_IFEval_3753_Terra_Extra_High_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt24_IFEval_3753_Terra_Extra_High_Package.zip.sha256.txt) |

Prompt 24 is published as its archival ZIP package. The PDF record and its PDF checksum are inside the ZIP; the separate sidecar verifies the ZIP itself.

| 25 | [Prompt 25 - IFEval 2225](Grounded_DI_OS_Benchmark_Record_Prompt25_IFEval_2225_SOL_Extra_High.pdf) · [supplied package-hash sidecar](Grounded_DI_OS_Benchmark_Record_Prompt25_IFEval_2225_SOL_Extra_High_Package.zip.sha256.txt) |

| 26 | [Prompt 26 - IFEval 2880](Grounded_DI_OS_Benchmark_Record_Prompt26_IFEval_2880_Terra_Extra_High.pdf) · [supplied package-hash sidecar](Grounded_DI_OS_Benchmark_Record_Prompt26_IFEval_2880_Terra_Extra_High_Package.zip.sha256.txt) |

Prompts 25 and 26 are published as PDF records and supplied package-hash sidecars. The sidecars name and hash their source package archives; this update does not claim that separate Prompt 25 or Prompt 26 ZIP archives are present.

| 27 | [Prompt 27 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt27_IFEval_2311_Terra_Extra_High_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt27_IFEval_2311_Terra_Extra_High_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt27_IFEval_2311_Terra_Extra_High.pdf) |

| 28 | [Prompt 28 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt28_IFEval_3386_Terra_Extra_High_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt28_IFEval_3386_Terra_Extra_High_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt28_IFEval_3386_Terra_Extra_High.pdf) |
| 29 | [Prompt 29 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt29_IFEval_143_Terra_Extra_High_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt29_IFEval_143_Terra_Extra_High_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt29_IFEval_143_Terra_Extra_High.pdf) |
| 30 | [Prompt 30 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt30_IFEval_136_Terra_Extra_High_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt30_IFEval_136_Terra_Extra_High_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt30_IFEval_136_Terra_Extra_High.pdf) |
| 31 | [Prompt 31 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt31_IFEval_1375_Terra_Extra_High_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt31_IFEval_1375_Terra_Extra_High_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt31_IFEval_1375_Terra_Extra_High.pdf) |

Prompts 27 through 31 are published with both standalone PDF records and archival ZIP packages. The separate sidecars verify the ZIP packages; each ZIP also contains the PDF and its internal PDF checksum.

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

### Prompt 13 - Sonia out

This task combines advice with exact paragraph and quotation structure. The official checks require four paragraphs, the first beginning with the normalized word weekend, and outer quotation marks. The local audit separately confirmed that the response remained an advice response rather than audit material.

### Prompt 14 - raise-request email

This tests professional writing with two terminal constraints. The official checks require a P.P.S. postscript and the exact ending phrase Hope you agree with me. Email professionalism and postscript placement were recorded separately as manual checks.

### Prompt 15 - banana-peel biology

This combines creative factual writing with keyword frequency and Markdown highlighting. The official checks require disappointed at least twice and at least six non-empty highlighted sections. Article quality, humor, and banana-peel biology were recorded as manual checks.

### Prompt 16 - GAN explanation

This tests content explanation under a punctuation and lexical envelope. The official checks require no commas, a P.P.S. pattern, and five required keywords. Bullet formatting, explanatory quality, and explanation-only presentation were recorded separately.

### Prompt 17 - customer-service rubric

This combines a practical rubric task with exact bullet control and forbidden-word screening. The official checks require exactly six counted bullet lines and absence of the two forbidden whole words. Rubric quality, customer-service relevance, and marker uniformity were recorded separately.

### Prompt 18 - wizards and sorcerers

This is the long-form structural stress test in the second half of the series. The official checks require at least 30 sentences, exactly two counted bullet lines, and at least eight square-bracket placeholders. The local record reported 34 sentences, two bullets, and eight placeholders.

### Prompt 19 - sleek new magistrates

This tests sustained article generation alongside word count, bullet count, and terminal postscript detection. The official checks require at least 300 words, exactly three asterisk bullet lines, and a P.S. postscript. The local record reported 450 words and a terminal P.S.

### Prompt 20 - writing skills

This combines bullet structure, section separation, and capitalization. The official checks require exactly three counted bullet lines, exactly four sections separated by ***, and at least two all-capital words. The local record reported three bullets, four sections, and two all-capital words.

### Prompt 21 - foolish-behavior haiku

This task required exactly two different responses separated by six asterisks, a title wrapped in double angular brackets, and no commas. The official Google Research checkers returned 3/3 encoded constraints passed on both strict and loose paths. The record separately reports two three-line haikus, explicit question form, the not-studying topic, conventional 5/7/5 scans, and young-reader suitability as manual checks.

### Prompt 22 - software-engineer review rubric

This task encodes only JSON format. The official checker returned a strict and loose pass after parsing the locked raw JSON response; it accepts limited Markdown-fence normalization but this record used no fence. The title, rating scale, four engineering-performance criteria, and evaluable guidance are separate manual rubric checks rather than additional official score components.

### Prompt 23 - math-notation riddle

This task encodes one repeat-prompt constraint. The response had to begin with the exact official prompt-to-repeat string before giving an answer. The official Google Research checker returned a strict and loose pass. The record separately reports the case-sensitive prefix, blank-line boundary, non-empty riddle, recognizable math notation, and absence of audit material as local/manual checks.

### Prompt 24 - constrained arithmetic response

This task encodes one constrained-response format requirement. The locked response was `My answer is no.` because a = 15 rather than 20. The official Google Research checker returned a strict and loose pass. The record separately reports exact whole-response equality, one-option-only use, absence of extra prose, and arithmetic correctness as local/manual checks. The initial direct checker invocation required a disclosed `build_description()` initialization repair after lock; the locked response did not change.

### Prompt 25 - Korean levee/embankment distinction

This task encodes a response-language requirement. The official checker detected Korean (`ko`) and returned a strict and loose pass. The record separately reports zero Latin letters, Korean-only presentation, and a substantive levee/embankment distinction as local/manual checks; it does not claim independent linguistic certification.

### Prompt 26 - Russell class and universal collection

This task encodes one structural constraint: two non-empty paragraphs separated by two newlines, with paragraph one beginning with `booster`. The official checker returned a strict and loose pass. The record separately checks the Russell class, self-membership contradiction, universal-collection distinction, mathematical notation, and scope qualification. The official evaluator required a disclosed dependency-path repair after lock; the locked response was unchanged.

### Prompt 27 - almond calorie premise

This task encodes the absence of the ASCII comma. The official CommaChecker returned a strict and loose pass. The record separately reports Unicode comma-like punctuation scans, the 396/32 and 32 × 9 arithmetic comparison, and a limited labeling-error explanation as local/manual checks; it does not claim nutritional certification.

### Prompt 28 - constrained milk purchase

This composite task encodes two constraints: forbidden whole words (`divide`, `answer`) and required keyword `remainder`. The official ForbiddenWords and KeywordChecker paths returned a strict and loose 2/2 pass. The record separately reports three whole gallons, a $1 remainder, a $12 four-gallon check, and absence of extra prose as local/manual checks. A disclosed local regex diagnostic was corrected after evaluation without changing the locked response or official results.

### Prompt 29 - colt-height composite

This task encodes two constraints: exactly two non-empty paragraphs separated by a line containing `***`, and a recognized `P.P.S.` postscript marker. The official ParagraphChecker and PostscriptChecker returned a strict and loose 2/2 pass. The record separately reports the 36-month conversion, 216 inches of growth, 18 feet of growth, and a final height of 23 feet as local/manual checks. The official checkers do not independently score the arithmetic or terminal placement. No preflight correction was made.

### Prompt 30 - atomic nucleus

This task encodes exactly nine evaluator-recognized bullet lines and a word count below 100. The official BulletListChecker and word-count check returned a strict and loose 2/2 pass. The record separately checks the nine conventional bullets, the 57-token official count, the hydrogen-1 caveat, and the nuclear-science explanation as local/manual checks. The official evaluator does not certify scientific correctness or conventional bullet presentation. No preflight correction was made.

### Prompt 31 - Java SQL safety illustration

This task encodes two constraints: exactly two non-empty blocks separated by the evaluator-recognized `***` pattern, and the required keyword `vulnerable`. The official ParagraphChecker and KeywordChecker returned a strict and loose 2/2 pass. The record separately checks the unsafe dynamic-query pattern, the parameterized `PreparedStatement` correction, the required code comment, and the absence of exploit or target material as local/manual checks. The official evaluator does not certify code safety, compilation, or production security. No preflight correction was made.

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

Each item was treated as one attempted submission. Private drafting and preflight checking were allowed by the recording protocol, but the number of corrections was disclosed. Prompt 2 required one disclosed preflight correction; the other thirty records report zero.

After finalization, the scored response was preserved exactly. No response was changed after observing a score, and no completed failed submission was silently replaced with a passing one.

### 4. Evaluator honesty

The official IFEval evaluator was not executed for Prompts 1–20 in this workspace. Prompts 21–31 were evaluated with the official Google Research checker source: Prompt 21 reports 3/3 encoded constraints passed on both strict and loose paths, Prompts 22–27 each report 1/1 on both paths, and Prompts 28–31 each report 2/2 on both paths. The README therefore distinguishes the local checks for Prompts 1–20 from the eleven official executions.

Prompts 1–20 are labeled:

> LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR

Prompts 21–31 separately record:

> OFFICIAL EVALUATOR PASS

For Prompts 21–31, the official-versus-local discrepancy was none. For Prompts 1–20, no official comparison was available.

### 5. Separation of scoring from auditing

The scored response contains only the requested answer. It does not contain the benchmark title, citations, score, audit notes, or explanations. The audit material appears outside the scored block in a separate PDF section.

This prevents the record from confusing a model’s task response with the documentation about that response.

### 6. Route and runtime separation

Routes are disclosed per record: Prompts 1–20 use `FastPath 5.6 / Luna Max`; Prompt 21 uses `FastPath 5.6 / SOL Max`; Prompts 22–24 and 26–31 use `FastPath 5.6 / Terra Extra High`; Prompt 25 uses `FastPath 5.6 / SOL Extra High`. The records do not convert a requested route into a claimed underlying model identity. Prompts 21–31 separately disclose official evaluator passes; the series reports no independent external verification.

### 7. Reproducible evidence

Each PDF preserves the exact prompt and final response, source URLs, timestamp and timezone, evaluator status, local constraint results, manual checks, preflight count, and SHA-256 hashes. The same visual record architecture was used across the series so that the benchmark content changes without changing the evidence structure.

### 8. Fail-closed claims

The records use `NOT INDEPENDENTLY VERIFIED` because no independent reviewer or external evaluator verified the runs. The series does not claim external certification, universal performance, representative performance across all models, or an official leaderboard result.

## What the series establishes

Under the documented Grounded DI OS recording conditions:

- all thirty-one finalized responses passed their local equivalents of the official encoded constraints;
- all thirty-one records preserve the submitted response and disclose the applicable evaluator status;
- the series contains 62/62 locally passed encoded constraints and 31/31 locally passed prompt-level strict results;
- Prompt 21 additionally reports an official strict and loose pass for all three encoded constraints; Prompts 22–27 each report an official strict and loose pass for their one encoded constraint, and Prompts 28–31 each report an official strict and loose pass for their two encoded constraints;
- the series contains 31 complete embedded records;
- the single disclosed preflight correction is included in the aggregate total.

## What the series does not establish

This is not:

- an official IFEval leaderboard score;
- a complete official evaluation of all thirty-one records;
- an independently verified benchmark;
- a blind third-party evaluation;
- a claim that the route will pass every IFEval item;
- a representative estimate of all model behavior;
- proof of a particular underlying model identity;
- proof of legal, factual, or universal reliability.

The most accurate description is: **a documented Grounded DI OS one-shot run of thirty-one official IFEval items, with all final responses passing transparent local checks, Prompts 21–31 additionally passing official checker executions, and no independent verification claim.**


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
**LOCAL CHECK PASS: 31/31**  
**OFFICIAL EVALUATOR: 11/31 EXECUTED · PROMPTS 21–31 PASS**  
**EVIDENCE: NOT INDEPENDENTLY VERIFIED**

#Grounded-DI #DeterministicIntelligence #CrossDomain #AuditableAI 
