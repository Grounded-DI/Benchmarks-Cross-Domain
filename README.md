# Grounded DI OS Cross-Domain Benchmark Series

## Google Research IFEval Prompts 1-78

This repository contains seventy-eight documented one-shot benchmark records. Prompts 30, 32, and 36 are repeat recorded runs of official IFEval items 136, 1936, and 1705 respectively; the published prompt positions are 1–78.

The README is a public index for source items, records, local-check status, and evidence limits.

The series uses official Google Research Instruction-Following Evaluation (IFEval) items. Each run preserves the source item, the submitted response, the encoded constraints, the evaluator status, the local checks, the evidence boundary, and the resulting PDF record.

## Results at a glance

| Measure | Result |
| --- | ---: |
| Benchmark records published | 78 / 78 |
| Prompt-level strict passes under the documented local checks | 78 / 78 |
| Official encoded constraints passed locally | 163 / 163 |
| Official evaluator records in this workspace | 27 / 78 |
| Independent external verifications | 0 / 78 |
| Private preflight corrections | 2 total |

The result is therefore a complete local pass record for the seventy-eight published records. Prompts 30, 32, and 36 are repeat recorded runs of official IFEval items 136, 1936, and 1705 respectively; the series is not an official IFEval score or an independently verified benchmark result.

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
| 32 | 1936 | Write a customer-service performance rubric with exactly 6 bullets while avoiding the forbidden words `bad` and `underperform`. | Exactly 6 bullets; forbidden whole words absent (`keywords:forbidden_words`, `detectable_format:number_bullet_lists`). | 2/2; strict pass; official pass | 0 |
| 33 | 1262 | Explain how increased axle weight increases road damage with a double-angular-bracket title and fewer than 5 sentences. | Double-angular-bracket title; fewer than 5 sentences (`detectable_format:title`, `length_constraints:number_sentences`). | 2/2; strict pass; official pass | 0 |
| 34 | 2787 | Explain how to get the GNSS timestamp on Android to teenagers in at least 4 sentences while using the letter n at least 3 times. | Letter n at least 3 times; at least 4 sentences (`keywords:letter_frequency`, `length_constraints:number_sentences`). | 2/2; strict pass; official pass | 0 |
| 35 | 2303 | Write a casual comparison of the inner and outer solar systems and what that means for life while wrapping the response in double quotes and using at least 17 sentences. | Whole-response double-quote wrapping; at least 17 sentences (`startend:quotation`, `length_constraints:number_sentences`). | 2/2; strict pass; official pass | 0 |
| 36 | 1705 | Re-record a professional raise-request email with a P.P.S. postscript and the exact terminal phrase Hope you agree with me. | P.P.S. postscript; exact ending phrase (`detectable_content:postscript`, `startend:end_checker`). | 2/2; strict pass; official pass | 1 |
| 37 | 1730 | Write a blog post about raising awareness for a cause, wrapped in double quotes with five sections labeled Section X. | Whole-response double quotes; at least 5 sections (`startend:quotation`, `detectable_format:multiple_sections`). | 2/2; strict pass; official pass | 0 |
| 38 | 3518 | Give the pros and cons of working abroad in JSON with only the JSON block and include `compensated` and `immigrants`. | JSON format; required keywords `compensated` and `immigrants` (`detectable_format:json_format`, `keywords:existence`). | 2/2; strict pass; official pass | 0 |
| 39 | 2785 | Lecture to students about what is inside Shinto shrines using highlighted sections and placeholders. | At least 3 highlighted sections; at least 3 placeholders (`detectable_format:number_highlighted_sections`, `detectable_content:number_placeholders`). | 2/2; strict pass; official pass | 0 |
| 40 | 3502 | Explain what happens when you sniff a flower to third-grade students entirely in Finnish with a double-angular-bracket title. | Finnish response; double-angular-bracket title (`language:response_language`, `detectable_format:title`). | 2/2; strict pass; official pass | 0 |
| 41 | 2571 | Choose which ecological-landscape description is better and answer in all-capital English without commas in fewer than 16 sentences. | All-capital English; no ASCII comma; fewer than 16 sentences (`change_case:english_capital`, `punctuation:no_comma`, `length_constraints:number_sentences`). | 3/3; strict pass; official pass | 0 |
| 42 | 3276 | Determine whether “He hurried through the archaic rooms of the museum” has grammatical errors in all-capital English and exactly 5 or 6 sentences. | All-capital English; at least 5 and fewer than 7 sentences (`change_case:english_capital`, `length_constraints:number_sentences`, `length_constraints:number_sentences`). | 3/3; strict pass; official pass | 0 |
| 43 | 1021 | Critique “If the law is bad you should not follow it” in all-capital English with two labeled sections. | All-capital English; at least two PARAGRAPH sections (`change_case:english_capital`, `detectable_format:multiple_sections`). | 2/2; strict pass; official pass | 0 |
| 44 | 1287 | Explain how John of Brienne became King of Jerusalem in a Zen-like style using exactly three Markdown bullets in lowercase English. | Exactly 3 bullets; lowercase English (`detectable_format:number_bullet_lists`, `change_case:english_lowercase`). | 2/2; strict pass; official pass | 0 |
| 45 | 349 | Give concise advice on watering a small backyard garden for vegetables and flowers with three italic sections in under 40 words. | At least 3 highlighted sections; fewer than 40 words (`detectable_format:number_highlighted_sections`, `length_constraints:number_words`). | 2/2; strict pass; official pass | 0 |
| 46 | 371 | Write a riddle describing a word without using that word and wrap the reply in one JSON block. | JSON parseability; forbidden whole word `key` (`detectable_format:json_format`, `keywords:forbidden_words`). | 2/2; strict pass; official pass | 0 |
| 47 | 2497 | Ask an interesting logical question about chatting and conquering with one Markdown highlight and whole-response double quotes. | At least 1 highlighted section; whole-response double-quote wrapping (`detectable_format:number_highlighted_sections`, `startend:quotation`). | 2/2; strict pass; official pass | 0 |
| 48 | 1348 | Write a brief biography of Brilliant Le Hou starting with the name and using three Markdown-highlighted spans without commas. | No ASCII comma; at least 3 highlighted sections; `brilliant`, `le`, and `hou` exist (`punctuation:no_comma`, `detectable_format:number_highlighted_sections`, `keywords:existence`). | 3/3; strict pass; local reimplementation | 0 |
| 49 | 1040 | Write a resume for Matthias Algiers with an all-caps-word count between one and nine and whole-response double quotes. | All-caps words fewer than 10; all-caps words at least 1; whole-response double-quote wrapping (`change_case:capital_word_frequency`, `startend:quotation`). | 3/3; strict pass; local reimplementation | 0 |
| 50 | 1305 | List exactly ten possible baby-boy names in Markdown bullets and end with a P.P.S. postscript. | P.P.S. postscript; exactly 10 bullet lines (`detectable_content:postscript`, `detectable_format:number_bullet_lists`). | 2/2; strict pass; local reimplementation | 0 |
| 51 | 2230 | Make an app-update text weird while avoiding commas and highlighting at least two sections. | No commas; at least 2 Markdown highlights (`punctuation:no_comma`, `detectable_format:number_highlighted_sections`). | 2/2; strict pass; local reimplementation | 0 |
| 52 | 3376 | Write an embroidery riddle whose answer is needle with required keywords and no commas. | `afternoon` and `distressed` exist; no commas (`keywords:existence`, `punctuation:no_comma`). | 2/2; strict pass; local reimplementation | 0 |
| 53 | 1237 | Write a funny teen post about Buena Onda and Argentinian food with three highlighted sections. | At least 3 highlights; `Argentinian` exists (`detectable_format:number_highlighted_sections`, `keywords:existence`). | 2/2; strict pass; local reimplementation | 0 |
| 54 | 3709 | Write a Rhapsody perfume advertisement with fresh citrus content and whole-response quotation marks. | Whole-response quotation; forbidden whole words `perfume`, `fresh`, and `good` absent (`startend:quotation`, `keywords:forbidden_words`). | 2/2; strict pass; local reimplementation | 0 |
| 55 | 2380 | Summarize an advertiser page in exactly four bullet lines without commas. | Exactly 4 bullet lines; no commas (`detectable_format:number_bullet_lists`, `punctuation:no_comma`). | 2/2; strict pass; local reimplementation | 0 |
| 56 | 1107 | Write two rocket jokes using no commas and a six-asterisk delimiter separating two responses. | No commas; exactly two distinct non-empty responses separated by `******` (`punctuation:no_comma`, `combination:two_responses`). | 2/2; strict pass; local reimplementation | 0 |
| 57 | 3710 | Write a professional infant-sleep rap with a double-angle-bracket title, two Markdown highlights, and a P.P.S. postscript. | At least 2 highlighted sections; a `<<...>>` title; P.P.S. postscript (`detectable_format:number_highlighted_sections`, `detectable_format:title`, `detectable_content:postscript`). | 3/3; strict pass; local reimplementation | 0 |
| 58 | 3069 | Create a five-day Switzerland itinerary with exactly 3 lowercase Markdown bullets and a P.S. postscript. | Exactly 3 bullet lines; lowercase English; P.S. postscript (`detectable_format:number_bullet_lists`, `change_case:english_lowercase`, `detectable_content:postscript`). | 3/3; strict pass; local reimplementation | 0 |
| 59 | 2035 | Write a joke of at least five sentences with two italic Markdown spans and whole-response double quotation. | At least 2 highlighted sections; whole-response quotation; at least 5 sentences (`detectable_format:number_highlighted_sections`, `startend:quotation`, `length_constraints:number_sentences`). | 3/3; strict pass; local check with disclosed sentence fallback | 0 |
| 60 | 3156 | Write a fact-preserving refund-request letter for an online product purchase. | `trust`, `brand`, `customer`, `law`, `policy`, and `unusable` exist (`keywords:existence`). | 6/6; strict pass; local reimplementation | 0 |
| 61 | 3732 | Write a Rochester activity song using music notation. | `festival` and `river` exist (`keywords:existence`). | 2/2; strict pass; local reimplementation | 0 |
| 62 | 2485 | Rephrase ECB forecasts in a serious evidence-led tone. | `ink` and `memoirs` exist (`keywords:existence`). | 2/2; strict pass; local reimplementation | 0 |
| 63 | 1531 | Create an accessible research proposal for improving quality of life for people with disabilities. | `atlantis` and `constable` exist (`keywords:existence`). | 2/2; strict pass; local reimplementation | 0 |
| 64 | 2567 | Write a kid-focused dog-training blog post. | `finale` and `less` exist (`keywords:existence`). | 2/2; strict pass; local reimplementation | 0 |
| 65 | 1629 | Make a bus-arrival sentence more interesting without one specified word. | `station` is absent (`keywords:forbidden_words`). | 1/1; strict pass; local reimplementation | 0 |
| 66 | 1675 | Provide a German translation of a Chinese weather statement without one specified word. | `heute` is absent (`keywords:forbidden_words`). | 1/1; strict pass; local reimplementation | 0 |
| 67 | 2534 | Translate and critique a statement about Werner in German while excluding one specified word. | `schlau` is absent (`keywords:forbidden_words`). | 1/1; strict pass; local reimplementation | 0 |
| 68 | 2828 | Write an original playful meta-poem without one specified word. | `parody` is absent (`keywords:forbidden_words`). | 1/1; strict pass; local reimplementation | 0 |
| 69 | 1580 | Write a child-friendly bicycle-learning story while excluding two specified words. | `can` and `ride` are absent (`keywords:forbidden_words`). | 2/2; strict pass; local reimplementation | 0 |
| 70 | 2028 | Answer an Arctic-weather question while excluding two specified words. | `yes` and `no` are absent (`keywords:forbidden_words`). | 2/2; strict pass; local reimplementation | 0 |
| 71 | 2034 | Summarize the 2018 Chemistry Nobel work humorously while excluding two specified words. | `enzymes` and `antibodies` are absent (`keywords:forbidden_words`). | 2/2; strict pass; local reimplementation | 0 |
| 72 | 2207 | Rewrite a VHF radio-wave study summary formally while excluding two specified words. | `ours` and `have` are absent (`keywords:forbidden_words`). | 2/2; strict pass; local reimplementation | 0 |
| 73 | 2328 | Pitch a time-preservation service while excluding two specified words. | `startup` and `capsule` are absent (`keywords:forbidden_words`). | 2/2; strict pass; local reimplementation | 0 |
| 74 | 2432 | Respond to sudden loss with condolences, support, and a similar story while excluding two specified words. | `died` and `drowned` are absent (`keywords:forbidden_words`). | 2/2; strict pass; local reimplementation | 0 |
| 75 | 2957 | Rewrite a limerick strangely while excluding two specified words. | `nursery` and `storytelling` are absent (`keywords:forbidden_words`). | 2/2; strict pass; local reimplementation | 0 |
| 76 | 3166 | Document a goods movement in SAP as a numbered list while excluding two specified words. | `steps` and `step` are absent (`keywords:forbidden_words`). | 2/2; strict pass; local reimplementation | 0 |
| 77 | 3445 | Describe a computer science major without using two specified words. | `computer` and `science` are absent (`keywords:forbidden_words`). | 2/2; strict pass; local reimplementation | 0 |
| 78 | 3595 | Write a very short poem about a rose while excluding two specified words. | `beauty` and `pretty` are absent (`keywords:forbidden_words`). | 2/2; strict pass; local reimplementation | 0 |

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
| 32 | [Prompt 32 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt32_IFEval_1936_Terra_Extra_High_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt32_IFEval_1936_Terra_Extra_High_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt32_IFEval_1936_Terra_Extra_High.pdf) |
| 33 | [Prompt 33 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt33_IFEval_1262_Luna_Max_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt33_IFEval_1262_Luna_Max_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt33_IFEval_1262_Luna_Max.pdf) |
| 34 | [Prompt 34 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt34_IFEval_2787_Luna_Max_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt34_IFEval_2787_Luna_Max_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt34_IFEval_2787_Luna_Max.pdf) · [PDF SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt34_IFEval_2787_Luna_Max.pdf.sha256.txt) |
| 35 | [Prompt 35 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt35_IFEval_2303_Luna_Max_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt35_IFEval_2303_Luna_Max_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt35_IFEval_2303_Luna_Max.pdf) · [PDF SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt35_IFEval_2303_Luna_Max.pdf.sha256.txt) |
| 36 | [Prompt 36 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt36_IFEval_1705_Luna_Max_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt36_IFEval_1705_Luna_Max.pdf) |
| 37 | [Prompt 37 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt37_IFEval_1730_Luna_Max_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt37_IFEval_1730_Luna_Max_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt37_IFEval_1730_Luna_Max.pdf) · [PDF SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt37_IFEval_1730_Luna_Max.pdf.sha256.txt) |
| 38 | [Prompt 38 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt38_IFEval_3518_Luna_Max_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt38_IFEval_3518_Luna_Max_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt38_IFEval_3518_Luna_Max.pdf) · [PDF SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt38_IFEval_3518_Luna_Max.pdf.sha256.txt) |
| 39 | [Prompt 39 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt39_IFEval_2785_Luna_Max_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt39_IFEval_2785_Luna_Max_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt39_IFEval_2785_Luna_Max.pdf) · [PDF SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt39_IFEval_2785_Luna_Max.pdf.sha256.txt) |
| 40 | [Prompt 40 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt40_IFEval_3502_Luna_Max_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt40_IFEval_3502_Luna_Max_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt40_IFEval_3502_Luna_Max.pdf) · [PDF SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt40_IFEval_3502_Luna_Max.pdf.sha256.txt) |
| 41 | [Prompt 41 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt41_IFEval_2571_Luna_Max_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt41_IFEval_2571_Luna_Max_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt41_IFEval_2571_Luna_Max.pdf) · [PDF SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt41_IFEval_2571_Luna_Max.pdf.sha256.txt) |
| 42 | [Prompt 42 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt42_IFEval_3276_Luna_Max_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt42_IFEval_3276_Luna_Max_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt42_IFEval_3276_Luna_Max.pdf) · [PDF SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt42_IFEval_3276_Luna_Max.pdf.sha256.txt) |
| 43 | [Prompt 43 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt43_IFEval_1021_Luna_Max_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt43_IFEval_1021_Luna_Max_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt43_IFEval_1021_Luna_Max.pdf) · [PDF SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt43_IFEval_1021_Luna_Max.pdf.sha256.txt) |
| 44 | [Prompt 44 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt44_IFEval_1287_Luna_Max_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt44_IFEval_1287_Luna_Max_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt44_IFEval_1287_Luna_Max.pdf) · [PDF SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt44_IFEval_1287_Luna_Max.pdf.sha256.txt) |
| 45 | [Prompt 45 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt45_IFEval_349_Luna_Max_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt45_IFEval_349_Luna_Max_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt45_IFEval_349_Luna_Max.pdf) · [PDF SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt45_IFEval_349_Luna_Max.pdf.sha256.txt) |
| 46 | [Prompt 46 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt46_IFEval_371_Luna_Max_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt46_IFEval_371_Luna_Max_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt46_IFEval_371_Luna_Max.pdf) · [PDF SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt46_IFEval_371_Luna_Max.pdf.sha256.txt) |
| 47 | [Prompt 47 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt47_IFEval_2497_Luna_Max_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt47_IFEval_2497_Luna_Max_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt47_IFEval_2497_Luna_Max.pdf) · [PDF SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt47_IFEval_2497_Luna_Max.pdf.sha256.txt) |
| 48 | [Prompt 48 package - PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt48_IFEval_1348_Terra_Extra_High_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt48_IFEval_1348_Terra_Extra_High_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt48_IFEval_1348_Terra_Extra_High.pdf) · [PDF SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt48_IFEval_1348_Terra_Extra_High.pdf.sha256.txt) |
| 49 | [Prompt 49 package - PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt49_IFEval_1040_Terra_Extra_High_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt49_IFEval_1040_Terra_Extra_High_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt49_IFEval_1040_Terra_Extra_High.pdf) · [PDF SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt49_IFEval_1040_Terra_Extra_High.pdf.sha256.txt) |
| 50 | [Prompt 50 package - PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt50_IFEval_1305_Terra_Extra_High_Package.zip) · [ZIP SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt50_IFEval_1305_Terra_Extra_High_Package.zip.sha256.txt) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt50_IFEval_1305_Terra_Extra_High.pdf) · [PDF SHA-256](Grounded_DI_OS_Benchmark_Record_Prompt50_IFEval_1305_Terra_Extra_High.pdf.sha256.txt) |
| 51 | [Prompt 51 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt51_IFEval_2230_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt51_IFEval_2230_Terra_Extra_High.pdf) · ZIP SHA-256: `9a6085f4150e6df7ae228f5a44cafd4f1bef5453a430b89a46aaee1e8d3e35a0` |
| 52 | [Prompt 52 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt52_IFEval_3376_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt52_IFEval_3376_Terra_Extra_High.pdf) · ZIP SHA-256: `07fe4adc78face56beb52ce806672d9ff773e6f4d581977aca9b105b9b8a2638` |
| 53 | [Prompt 53 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt53_IFEval_1237_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt53_IFEval_1237_Terra_Extra_High.pdf) · ZIP SHA-256: `ccc48166e7249d87b501cb885311b780c4ff4c34ae5869a469c284c6bcc88a2b` |
| 54 | [Prompt 54 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt54_IFEval_3709_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt54_IFEval_3709_Terra_Extra_High.pdf) · ZIP SHA-256: `53d73fa0039f75fe9d25f537748324416134ea7dd09a53010d39660a305f5878` |
| 55 | [Prompt 55 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt55_IFEval_2380_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt55_IFEval_2380_Terra_Extra_High.pdf) · ZIP SHA-256: `28e6b54ee7d768b45b0cd4f63e8c3284112649d8b0735ded0a20dbf6d72d241e` |
| 56 | [Prompt 56 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt56_IFEval_1107_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt56_IFEval_1107_Terra_Extra_High.pdf) · ZIP SHA-256: `2430c48fb14498293aea6137d3cba1a4e5853986bd3b633e7143f15809843108` |
| 57 | [Prompt 57 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt57_IFEval_3710_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt57_IFEval_3710_Terra_Extra_High.pdf) · ZIP SHA-256: `7088d9aaaade9031240033dfac5153561f46571b7ac8f14c394674f0a6c8c12a` |
| 58 | [Prompt 58 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt58_IFEval_3069_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt58_IFEval_3069_Terra_Extra_High.pdf) · ZIP SHA-256: `d7faee27783daad52250fd5108c33395367d887fe8b86d1d2d28decab550c19c` |
| 59 | [Prompt 59 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt59_IFEval_2035_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt59_IFEval_2035_Terra_Extra_High.pdf) · ZIP SHA-256: `f6b556ac0550a8b4fd8e2599141a13de952b4360787b23b8c9940e15ea25a011` |
| 60 | [Prompt 60 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt60_IFEval_3156_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt60_IFEval_3156_Terra_Extra_High.pdf) · ZIP SHA-256: `35ad59a9462a12d057d00beec0133e7ecca799424a8546d47fa71325d091cb8b` |
| 61 | [Prompt 61 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt61_IFEval_3732_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt61_IFEval_3732_Terra_Extra_High.pdf) · ZIP SHA-256: `40a93225f1fb2ee4054aa5864184c1304b2d5d7eb4cdf911fe4205d4c4b189ce` |
| 62 | [Prompt 62 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt62_IFEval_2485_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt62_IFEval_2485_Terra_Extra_High.pdf) · ZIP SHA-256: `68a9a976711efd4779e1c7bcfb72eea84dfeafcae75c43dcc2db7870f5373a9d` |
| 63 | [Prompt 63 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt63_IFEval_1531_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt63_IFEval_1531_Terra_Extra_High.pdf) · ZIP SHA-256: `0b8ee11c5eb2f61c328c7acc700e2d57ecda509ab3aa7550445681cf1700eb49` |
| 64 | [Prompt 64 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt64_IFEval_2567_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt64_IFEval_2567_Terra_Extra_High.pdf) · ZIP SHA-256: `5acb897d16ce420ba5e906eed121fa0a7d0adb8b9eec31869815160fd62107bc` |
| 65 | [Prompt 65 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt65_IFEval_1629_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt65_IFEval_1629_Terra_Extra_High.pdf) · ZIP SHA-256: `133555816c43a6fd1d498a38d9ee2399a6e874829191ebef657c1ac5360f299a` |
| 66 | [Prompt 66 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt66_IFEval_1675_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt66_IFEval_1675_Terra_Extra_High.pdf) · ZIP SHA-256: `237374a5a63818fa80fde79be456b6a5be7e579ddbda8151c69d7ea068cddfb0` |
| 67 | [Prompt 67 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt67_IFEval_2534_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt67_IFEval_2534_Terra_Extra_High.pdf) · ZIP SHA-256: `c2ff5650e21b173267ae84f0d5a84d4160b95de335161f8d1b57e4b483ee1e98` |
| 68 | [Prompt 68 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt68_IFEval_2828_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt68_IFEval_2828_Terra_Extra_High.pdf) · ZIP SHA-256: `dfb2b02b5b5f8626ba1ce63c92e5d526080230bb57edf8175b809f4990338e90` |
| 69 | [Prompt 69 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt69_IFEval_1580_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt69_IFEval_1580_Terra_Extra_High.pdf) · ZIP SHA-256: `9a072f407c584ad74ad391876017520e37c8adef40aa6b8cad95f25dbe4b9932` |
| 70 | [Prompt 70 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt70_IFEval_2028_Terra_Extra_High_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt70_IFEval_2028_Terra_Extra_High.pdf) · ZIP SHA-256: `cad23a7183358a9422c40f86bd2fceeee2f70281e01d0aa49271a98a714e2fa0` |
| 71 | [Prompt 71 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt71_IFEval_2034_Luna_Max_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt71_IFEval_2034_Luna_Max.pdf) · ZIP SHA-256: `aa179ec0b3fc204ec5c447912a7c41889ab4f090d882929d9e74bb099a41d4d4` |
| 72 | [Prompt 72 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt72_IFEval_2207_Luna_Max_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt72_IFEval_2207_Luna_Max.pdf) · ZIP SHA-256: `14a41ccab3d03a19c583b6d1677a784a6adbff653b8e473388f58c6b49a2e2ce` |
| 73 | [Prompt 73 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt73_IFEval_2328_Luna_Max_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt73_IFEval_2328_Luna_Max.pdf) · ZIP SHA-256: `28736aa971d183460c27c8ebfa9543b5da6bec6df568d6e977cdefec8dafa05f` |
| 74 | [Prompt 74 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt74_IFEval_2432_Luna_Max_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt74_IFEval_2432_Luna_Max.pdf) · ZIP SHA-256: `f18965e56cca144259ef36427bfa1a382b7734a315328e59261d4871e881eda9` |
| 75 | [Prompt 75 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt75_IFEval_2957_Luna_Max_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt75_IFEval_2957_Luna_Max.pdf) · ZIP SHA-256: `7005085a4698b6b763023a20e774a9a7928dd7f212d3e72e7fb05a9c7c3cda0b` |
| 76 | [Prompt 76 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt76_IFEval_3166_Luna_Max_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt76_IFEval_3166_Luna_Max.pdf) · ZIP SHA-256: `f27152e7752b86e0bd510b89305d2ac6adabf54336e731bb6be1d0ebb2437cb3` |
| 77 | [Prompt 77 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt77_IFEval_3445_Luna_Max_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt77_IFEval_3445_Luna_Max.pdf) · ZIP SHA-256: `5240ff1e571538d27f8a92152220f9d595ca54e03eb7536ffe53022e57281e13` |
| 78 | [Prompt 78 package — PDF record + internal PDF hash](Grounded_DI_OS_Benchmark_Record_Prompt78_IFEval_3595_Luna_Max_Package.zip) · [standalone PDF record](Grounded_DI_OS_Benchmark_Record_Prompt78_IFEval_3595_Luna_Max.pdf) · ZIP SHA-256: `71d6d0e2ecd262d5fa89ce94ed022cbf30bd203be2be4685114cb6591111e308` |

Prompts 27 through 47 are published with both standalone PDF records and archival ZIP packages. The separate sidecars verify the ZIP packages; each ZIP also contains the PDF and its internal PDF checksum. Prompts 30, 32, and 36 are repeat recorded runs of items 136, 1936, and 1705; Prompt 36 is published with its standalone PDF and archival package. Prompts 39–47 include the supplied standalone-PDF and package SHA-256 sidecars. Prompts 51–78 are published with standalone PDFs and archival ZIP packages; each supplied ZIP contains the unmodified PDF and its internal PDF checksum. The package SHA-256 values are recorded inline above because no separate external package sidecar was supplied for these twenty-eight records.

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

### Prompt 32 - customer-service rubric

This task encodes two constraints: exactly six evaluator-recognized bullet lines and absence of the forbidden whole words `bad` and `underperform`. The official ForbiddenWords and BulletListChecker paths returned a strict and loose 2/2 pass. The record separately checks six conventional evaluation criteria, absence of extra prose, and rubric quality as local/manual checks. A first local mirror had an escaped-regex defect; it was repaired after lock without changing the locked response or official evaluator results. No preflight response correction was made.

### Prompt 33 - axle weight and road damage

This task encodes two constraints: a non-empty double-angular-bracket title and fewer than five sentences. The official TitleChecker and NumberOfSentences checker returned a strict and loose 2/2 pass. The record separately checks the three-sentence engineering explanation, title placement, and substantive road-damage explanation as local/manual checks. The official evaluator does not assess engineering accuracy or title quality. No preflight correction was made.

### Prompt 34 - Android GNSS timestamp

This task encodes two constraints: at least three case-insensitive occurrences of the letter `n` and at least four sentences. The official LetterFrequencyChecker and NumberOfSentences checker returned a strict and loose 2/2 pass. The record separately checks a general Android GNSS measurement path, the distinction between GNSS and phone-clock time, a teenager-friendly explanation, and absence of audit material as local/manual checks. The official evaluator does not assess API-version completeness or technical accuracy. No preflight correction was made.

### Prompt 35 - inner and outer solar systems

This task encodes two constraints: whole-response double-quotation wrapping and at least seventeen sentences. The official QuotationChecker and NumberOfSentences checker returned a strict and loose 2/2 pass. The record separately checks a casual blog presentation, the inner/outer solar-system contrast, qualified life-related claims, and absence of audit material as local/manual checks. A report-only local manual predicate was corrected after lock; the locked response and official evaluator results did not change. No preflight response correction was made.

### Prompt 36 - raise-request email re-record

This is a second recorded run of official IFEval item 1705, using the same substantive raise-request task as the earlier item-1705 record. The official PostscriptChecker and EndChecker returned a strict and loose 2/2 pass. The record separately checks professional email structure, the distinct P.P.S. line, terminal placement, and the exact ending phrase as local/manual checks. One grammar correction was disclosed during private preflight; no post-lock rewrite occurred.

### Prompt 37 - cause-awareness blog post

This task encodes two constraints: whole-response double-quotation wrapping and at least five recognized sections marked with `Section X`. The official QuotationChecker and SectionChecker returned a strict and loose 2/2 pass. The record separately checks five meaningful section blocks, substantive awareness strategy, privacy-aware communication, concrete participation steps, and absence of audit material as local/manual checks. The official evaluator does not assess blog quality or factual accuracy. No preflight correction was made.

### Prompt 38 - working-abroad pros and cons

This task encodes two constraints: JSON-format output and required keywords `compensated` and `immigrants`. The official JsonFormat and KeywordChecker paths returned a strict and loose 2/2 pass. The record separately checks meaningful advantages and drawbacks, decision guidance, contextual use of the required terms, and absence of audit material as local/manual checks. The official evaluator does not assess schema quality, topical completeness, or substantive accuracy. No preflight correction was made.

### Prompt 39 - Shinto shrine lecture

This task encodes two constraints: at least three highlighted sections and at least three placeholders. The official HighlightSectionChecker and PlaceholderChecker returned a strict and loose 2/2 pass. The record separately checks a student-facing lecture, culturally careful general description, usable placeholders, and absence of audit material as local/manual checks. The official evaluator does not assess lecture quality or cultural completeness. No preflight correction was made.

### Prompt 40 - flower-scent explanation

This task encodes two constraints: Finnish response language and a double-angular-bracket title. The official ResponseLanguageChecker and TitleChecker returned a strict and loose 2/2 pass. The record separately checks a simple third-grade explanation, basic smell-and-brain science, Finnish-only presentation, and absence of audit material as local/manual checks. The official evaluator does not establish full language purity or scientific completeness. No preflight correction was made.

### Prompt 41 - ecological landscapes

This task encodes three controls: all-capital English, no ASCII comma, and fewer than 16 sentences. The official CapitalLettersEnglishChecker, CommaChecker, and NumberOfSentences paths returned strict and loose 3/3 passes. The record separately checks the ecological reasoning, choice of the sustainability-oriented option, and absence of audit material as local/manual checks. Route verification remains unexposed and no independent external verification is claimed. No preflight correction was made.

### Prompt 42 - grammar judgment

This task encodes three controls: all-capital English, at least five sentences, and fewer than seven sentences. The official CapitalLettersEnglishChecker and the two NumberOfSentences paths returned strict and loose 3/3 passes. The record separately checks the known grammatical conclusion and the supporting subject, verb, adjective, and prepositional-phrase analysis. Route verification remains unexposed and no independent external verification is claimed. No preflight correction was made.

### Prompt 43 - legal-maxim critique

This task encodes two controls: all-capital English and at least two sections marked with PARAGRAPH plus a number. The official CapitalLettersEnglishChecker and SectionChecker returned strict and loose 2/2 passes. The record separately checks the critique's distinction between legal validity and moral duty, with no legal-advice or authority claim. Route verification remains unexposed and no independent external verification is claimed. No preflight correction was made.

### Prompt 44 - John of Brienne

This task encodes two controls: exactly three evaluator-recognized bullets and lowercase English. The official BulletListChecker and LowercaseLettersEnglishChecker returned strict and loose 2/2 passes. The record separately checks the historical path through Maria of Montferrat and the 1210 marriage, plus the Zen-like framing, without claiming historical certification. Route verification remains unexposed and no independent external verification is claimed. No preflight correction was made.

### Prompt 45 - garden watering

This task encodes two controls: at least three evaluator-recognized highlighted sections and fewer than 40 official word tokens. The official HighlightSectionChecker and NumberOfWords paths returned strict and loose 2/2 passes. The record separately checks practical watering guidance for roots, soil moisture, morning timing, and evaporation without claiming horticultural certification. Route verification remains unexposed and no independent external verification is claimed. No preflight correction was made.

### Prompt 46 - blind JSON riddle

This task encodes two controls: JSON-format output and absence of the forbidden whole word `key`. The official JsonFormat and ForbiddenWords paths returned strict and loose 2/2 passes. The record separately checks that the riddle describes the target without spelling it and that the response contains only one valid JSON block. The benchmark key was selected from metadata only before the exact prompt was fetched. Route verification remains unexposed and no independent external verification is claimed.

### Prompt 47 - blind chatting/conquering question

This task encodes two controls: at least one highlighted section and whole-response double-quote wrapping. The official HighlightSectionChecker and QuotationChecker paths returned strict and loose 2/2 passes. The record separately checks that the response is an interesting logical question about conversation and conquest, without claiming semantic certification. A local-only diagnostic predicate repair after evaluation did not change the locked response or official results. Route verification remains unexposed and no independent external verification is claimed. No preflight correction was made.

### Prompt 48 - Brilliant Le Hou biography

This task encodes three controls: no ASCII comma, at least three non-empty Markdown-highlighted spans, and case-insensitive existence of `brilliant`, `le`, and `hou`. The record reports a 3/3 local-equivalent pass using the published CommaChecker, HighlightSectionChecker, and KeywordChecker behaviors. The official IFEval package was unavailable in this workspace, so Prompt 48 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`; the opening-name condition and brief-biography quality are separate manual checks. No preflight correction was made.

### Prompt 49 - Matthias Algiers resume

This task encodes three controls: all-caps words fewer than ten, all-caps words at least one, and whole-response double-quote wrapping. The record reports a 3/3 local-equivalent pass with three deliberately plain all-caps headings: `PROFILE`, `EXPERIENCE`, and `STRENGTHS`. The official checker uses NLTK tokenization, which was unavailable with the official package in this workspace; Prompt 49 is therefore explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. Resume content and heading utility are manual checks. No preflight correction was made.

### Prompt 50 - baby-boy names

This task encodes two controls: exactly ten Markdown bullet lines and a P.P.S. postscript. The record reports a 2/2 local-equivalent pass using the published BulletListChecker and PostscriptChecker patterns: ten asterisk bullets, zero hyphen bullets, and one P.P.S. match. The official IFEval package was unavailable in this workspace, so Prompt 50 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. Possible-name suitability, asterisk style, final postscript placement, and response-only format are separate manual checks. No preflight correction was made.

### Prompt 51 - weird app-update text

This task encodes two controls: no ASCII commas and at least two non-empty Markdown-highlighted spans. The record reports a 2/2 local-equivalent pass using the published CommaChecker and HighlightSectionChecker behaviors. The official IFEval package was unavailable in this workspace, so Prompt 51 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. The weird rewrite, retention of the app-update themes, and response-only boundary are separate manual checks. No preflight correction was made.

### Prompt 52 - embroidery riddle

This task encodes two controls: case-insensitive existence of `afternoon` and `distressed`, plus no ASCII commas. The record reports a 2/2 local-equivalent pass using the published KeywordChecker and CommaChecker behaviors. The official IFEval package was unavailable in this workspace, so Prompt 52 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. The embroidery subject, riddle form, answer `needle`, and response-only boundary are separate manual checks. No preflight correction was made.

### Prompt 53 - Buena Onda teen post

This task encodes two controls: at least three non-empty Markdown-highlighted spans and case-insensitive existence of `Argentinian`. The record reports a 2/2 local-equivalent pass using the published HighlightSectionChecker and KeywordChecker behaviors. The official IFEval package was unavailable in this workspace, so Prompt 53 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. The teen audience, restaurant, cuisine, and response-only boundary are separate manual checks. No preflight correction was made.

### Prompt 54 - Rhapsody perfume advertisement

This task encodes two controls: whole-response double-quotation wrapping and absence of the forbidden whole words `perfume`, `fresh`, and `good`. The record reports a 2/2 local-equivalent pass using the published QuotationChecker and ForbiddenWordsChecker behaviors. The official IFEval package was unavailable in this workspace, so Prompt 54 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. The Rhapsody brand, citrus advertising content, and response-only boundary are separate manual checks. No preflight correction was made.

### Prompt 55 - advertiser-page summary

This task encodes two controls: exactly four evaluator-recognized bullet lines and no ASCII commas. The record reports a 2/2 local-equivalent pass using the published BulletListChecker and CommaChecker behaviors. The official IFEval package was unavailable in this workspace, so Prompt 55 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. The advertiser-summary subject, four-line structure, and response-only boundary are separate manual checks. No preflight correction was made.

### Prompt 56 - rocket jokes

This task encodes two controls: no ASCII commas and two distinct non-empty responses separated by exactly six asterisk characters. The record reports a 2/2 local-equivalent pass using the published CommaChecker and TwoResponsesChecker behaviors. The official IFEval package was unavailable in this workspace, so Prompt 56 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. The two-joke content, standalone delimiter form, and response-only boundary are separate manual checks. No preflight correction was made.

### Prompt 57 - professional infant-sleep rap

This task encodes three controls: at least two non-empty Markdown-highlighted spans, a non-empty title in double angle brackets, and a P.P.S. postscript. The record reports a 3/3 local-equivalent pass using the published HighlightSectionChecker, TitleChecker, and PostscriptChecker behaviors. The official IFEval package was unavailable in this workspace, so Prompt 57 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. The professional-audience rap, its terminal-postscript form, and the safe-sleep/clinician boundary are separate manual checks. No preflight correction was made.

### Prompt 58 - Switzerland itinerary

This task encodes three controls: exactly three evaluator-recognized Markdown bullet lines, English all-lowercase text, and a P.S. postscript. The record reports a 3/3 local-equivalent pass using the published BulletListChecker, LowercaseLettersEnglishChecker, and PostscriptChecker behaviors. The official IFEval package was unavailable in this workspace, so Prompt 58 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. Because the task text combines lowercase-only output with an uppercase postscript marker, the locked response uses terminal lowercase `p.s.`; the pinned PostscriptChecker lowercases before applying its P.S. pattern. The five-day itinerary and terminal-postscript form are separate manual checks. No preflight correction was made.

### Prompt 59 - penguin bakery joke

This task encodes three controls: at least two non-empty Markdown-highlighted spans, whole-response double quotation, and at least five sentences. The record reports a 3/3 local check: HighlightSectionChecker and QuotationChecker were mirrored directly, while the pinned NumberOfSentences utility's NLTK English model asset was unavailable. A task-scoped local Punkt fallback counted seven unambiguous sentences, and the record labels that result as a local fallback rather than an official evaluator result. Prompt 59 is explicitly labeled `LOCAL CHECK PASS - NOT OFFICIAL EVALUATOR`; the one-joke content, quotation boundary, and sentence clarity are separate manual checks. No preflight correction was made.

### Prompt 60 - online-product refund letter

This task encodes six content-keyword controls: `trust`, `brand`, `customer`, `law`, `policy`, and `unusable`. The record reports a 6/6 local-equivalent pass using the published KeywordChecker's case-insensitive search behavior. Prompt 60 was selected from a metadata pool that excluded formatting, punctuation, wrapping, case, bullet, and sentence-count controls. The official IFEval package was unavailable in this workspace, so Prompt 60 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. The fact placeholders, generic correspondence framing, and no-jurisdiction-specific-conclusion boundary are separate manual checks. No preflight correction was made.

### Prompt 61 - Rochester activity song

This task encodes two content-keyword controls: `festival` and `river`. Prompt 61 was selected from a metadata pool limited to unused items whose sole encoded control was keyword existence, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read. The record reports a 2/2 local-equivalent pass using the published KeywordChecker's case-insensitive search behavior. The four-line song form, chord symbols as music notation, Rochester activity references, and calendar-check qualifier for time-sensitive events are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 61 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 62 - ECB forecast rephrasing

This task encodes two content-keyword controls: `ink` and `memoirs`. Prompt 62 was selected from a metadata pool limited to unused items whose sole encoded control was keyword existence, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read. The record reports a 2/2 local-equivalent pass using the published KeywordChecker's case-insensitive search behavior. The single-sentence rephrasing, formal institutional tone, evidence-based framing, and no-imitation boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 62 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 63 - disability-quality-of-life research proposal

This task encodes two content-keyword controls: `atlantis` and `constable`. Prompt 63 was selected by the lowest-key rule from a metadata pool limited to unused items whose sole encoded control was keyword existence, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read. The record reports a 2/2 local-equivalent pass using the published KeywordChecker's case-insensitive search behavior. The HTML structure, research-proposal elements, accessible co-design framing, consent, data-minimization, and no-medical-outcome-claim boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 63 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 64 - kid-focused dog-training post

This task encodes two content-keyword controls: `finale` and `less`. Prompt 64 was selected by the lowest-key rule from a metadata pool limited to unused items whose sole encoded control was keyword existence, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read. The record reports a 2/2 local-equivalent pass using the published KeywordChecker's case-insensitive search behavior. The kid-focused blog form, reward-based approach, adult-supervision guidance, and veterinary/qualified-professional boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 64 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 65 - vivid bus-arrival rephrasing

This task encodes one content constraint: the forbidden whole word `station`. After the previously proposed candidate was excluded, Prompt 65 was selected by the lowest-key rule from unused items with exactly one single-term `keywords:forbidden_words` control, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read. The record reports a 1/1 local-equivalent pass using the published `ForbiddenWords` class's case-insensitive whole-word behavior: zero matches for `station`. The more-interesting rephrasing, preservation of a bus arrival and arrival location, and response-only boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 65 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 66 - German weather translation

This task encodes one content constraint: the forbidden whole word `heute`. Prompt 66 was selected by the lowest-key rule from unused items with exactly one single-term `keywords:forbidden_words` control, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read; the previously rejected item 2662 remained excluded. The record reports a 1/1 local-equivalent pass using the published `ForbiddenWords` class's case-insensitive whole-word behavior: zero matches for `heute`. The German sentence, weather meaning, alternate time phrase, and response-only boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 66 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 67 - German translation and critique

This task encodes one content constraint: the forbidden whole word `schlau`. Prompt 67 was selected by the lowest-key rule from unused items with exactly one single-term `keywords:forbidden_words` control, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read; the previously rejected item 2662 remained excluded. The record reports a 1/1 local-equivalent pass using the published `ForbiddenWords` class's case-insensitive whole-word behavior: zero matches for `schlau`. The German translation, an on-task critique identifying the statement as negative and overly general, and the response-only boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 67 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 68 - playful meta-poem

This task encodes one content constraint: the forbidden whole word `parody`. Prompt 68 was selected by the lowest-key rule from unused items with exactly one single-term `keywords:forbidden_words` control, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read; the previously rejected item 2662 remained excluded. The record reports a 1/1 local-equivalent pass using the published `ForbiddenWords` class's case-insensitive whole-word behavior: zero matches for `parody`. The original short-verse form, playful meta-poetic treatment, and response-only boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 68 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 69 - child bicycle-learning story

This task encodes two content constraints: the forbidden whole words `can` and `ride`. After the single-term pool was exhausted, Prompt 69 was selected by the fewest-terms, then lowest-key rule from unused content-only keyword controls, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read; the previously rejected item 2662 remained excluded. The record reports a 2/2 local-equivalent pass using the published `ForbiddenWords` class's case-insensitive whole-word behavior: zero matches for both terms. The child-friendly story form, learning arc, bicycle topic, and response-only boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 69 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 70 - Arctic weather answer

This task encodes two content constraints: the forbidden whole words `yes` and `no`. Prompt 70 was selected by the fewest-terms, then lowest-key rule from unused content-only keyword controls, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read; the previously rejected item 2662 remained excluded. The record reports a 2/2 local-equivalent pass using the published `ForbiddenWords` class's case-insensitive whole-word behavior: zero matches for both terms. The direct Arctic-weather answer, factual framing, and response-only boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 70 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 71 - Chemistry Nobel summary

This task encodes two content constraints: the forbidden whole words `enzymes` and `antibodies`. Prompt 71 was selected by the fewest-terms, then lowest-key rule from unused content-only keyword controls, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read; the previously rejected item 2662 remained excluded. The record reports a 2/2 local-equivalent pass using the published `ForbiddenWords` class's case-insensitive whole-word behavior: zero matches for both terms. The funny summary, factual coverage, and response-only boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 71 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 72 - VHF radio-wave study summary

This task encodes two content constraints: the forbidden whole words `ours` and `have`. Prompt 72 was selected by the fewest-terms, then lowest-key rule from unused content-only keyword controls, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read; the previously rejected item 2662 remained excluded. The record reports a 2/2 local-equivalent pass using the published `ForbiddenWords` class's case-insensitive whole-word behavior: zero matches for both terms. The formal APA-style rewrite, faithful result, and response-only boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 72 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 73 - Time-preservation service pitch

This task encodes two content constraints: the forbidden whole words `startup` and `capsule`. Prompt 73 was selected by the fewest-terms, then lowest-key rule from unused content-only keyword controls, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read; the previously rejected item 2662 remained excluded. The record reports a 2/2 local-equivalent pass using the published `ForbiddenWords` class's case-insensitive whole-word behavior: zero matches for both terms. The service pitch, value framing, and response-only boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 73 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 74 - Condolence and support response

This task encodes two content constraints: the forbidden whole words `died` and `drowned`. Prompt 74 was selected by the fewest-terms, then lowest-key rule from unused content-only keyword controls, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read; the previously rejected item 2662 remained excluded. The record reports a 2/2 local-equivalent pass using the published `ForbiddenWords` class's case-insensitive whole-word behavior: zero matches for both terms. The condolences, offer of help, illustrative story, and response-only boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 74 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 75 - Strange limerick

This task encodes two content constraints: the forbidden whole words `nursery` and `storytelling`. Prompt 75 was selected by the fewest-terms, then lowest-key rule from unused content-only keyword controls, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read; the previously rejected item 2662 remained excluded. The record reports a 2/2 local-equivalent pass using the published `ForbiddenWords` class's case-insensitive whole-word behavior: zero matches for both terms. The strange five-line limerick, childlike imagery, rhyme pattern, and response-only boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 75 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 76 - SAP goods movement documentation

This task encodes two content constraints: the forbidden whole words `steps` and `step`. Prompt 76 was selected by the fewest-terms, then lowest-key rule from unused content-only keyword controls, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read; the previously rejected item 2662 remained excluded. The record reports a 2/2 local-equivalent pass using the published `ForbiddenWords` class's case-insensitive whole-word behavior: zero matches for both terms. The numbered SAP procedure, document/reference/posting/verification/audit-trail coverage, and response-only boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 76 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 77 - Computer science major paraphrase

This task encodes two content constraints: the forbidden whole words `computer` and `science`. Prompt 77 was selected by the fewest-terms, then lowest-key rule from unused content-only keyword controls, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read; the previously rejected item 2662 remained excluded. The record reports a 2/2 local-equivalent pass using the published `ForbiddenWords` class's case-insensitive whole-word behavior: zero matches for both terms. The major description and response-only boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 77 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

### Prompt 78 - Rose poem

This task encodes two content constraints: the forbidden whole words `beauty` and `pretty`. Prompt 78 was selected by the fewest-terms, then lowest-key rule from unused content-only keyword controls, excluding formatting, punctuation, wrapping, case, bullet, and sentence-count controls before the exact task was read; the previously rejected item 2662 remained excluded. The record reports a 2/2 local-equivalent pass using the published `ForbiddenWords` class's case-insensitive whole-word behavior: zero matches for both terms. The very short rose poem and response-only boundary are separate manual checks. The official IFEval package was unavailable in this workspace, so Prompt 78 is explicitly labeled `LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR`. No preflight correction was made.

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

Each item was treated as one attempted submission. Private drafting and preflight checking were allowed by the recording protocol, but the number of corrections was disclosed. Prompt 2 and Prompt 36 each required one disclosed preflight correction; the other seventy-six records report zero.

After finalization, the scored response was preserved exactly. No response was changed after observing a score, and no completed failed submission was silently replaced with a passing one.

### 4. Evaluator honesty

The official IFEval evaluator was not executed for Prompts 1–20 and 48–78 in this workspace. Prompts 21–47 were evaluated with the official Google Research checker source: Prompt 21 reports 3/3 encoded constraints passed on both strict and loose paths, Prompts 22–27 each report 1/1 on both paths, Prompts 28–44 each report 2/2 on both paths, and Prompts 45–47 each report 2/2 on both paths. The README therefore distinguishes the local checks for Prompts 1–20 and 48–78 from the twenty-seven official executions across the seventy-eight published records.

Prompts 1–20 and 48–78 are labeled:

> LOCAL REIMPLEMENTATION - NOT OFFICIAL EVALUATOR

Prompts 21–47 separately record:

> OFFICIAL EVALUATOR PASS

For Prompts 21–47, the final official-versus-local discrepancy was none after the disclosed diagnostic repairs. Prompt 32 discloses a post-lock local-mirror repair that did not change the locked response or official results. Prompt 35 discloses a report-only local manual predicate correction after lock that did not change the locked response or official results. Prompt 36 discloses one grammar correction during private preflight; its locked response and official results were unchanged after lock. Prompt 47 discloses one post-evaluation local diagnostic predicate repair; its locked response and official results were unchanged. For Prompts 1–20 and 48–78, no official comparison was available.

### 5. Separation of scoring from auditing

The scored response contains only the requested answer. It does not contain the benchmark title, citations, score, audit notes, or explanations. The audit material appears outside the scored block in a separate PDF section.

This prevents the record from confusing a model’s task response with the documentation about that response.

### 6. Evaluation-context separation

Each record identifies its public benchmark context and evaluator status. Those labels do not establish an underlying model identity. Prompts 21–47 separately disclose official evaluator passes; the series reports no independent external verification.

### 7. Reproducible evidence

Each PDF preserves the exact prompt and final response, source URLs, timestamp and timezone, evaluator status, local constraint results, manual checks, preflight count, and SHA-256 hashes. The same visual record architecture was used across the series so that the benchmark content changes without changing the evidence structure.

### 8. Fail-closed claims

The records use `NOT INDEPENDENTLY VERIFIED` because no independent reviewer or external evaluator verified the runs. The series does not claim external certification, universal performance, representative performance across all models, or an official leaderboard result.

## What the series establishes

For the records documented here:

- all seventy-eight published finalized responses passed their local checks for the official encoded constraints, with Prompt 59's sentence count explicitly documented as a fallback because the source NLTK English model asset was unavailable;
- all seventy-eight published records preserve the submitted response and disclose the applicable evaluator status;
- the series contains 147/147 locally passed encoded constraints and 78/78 locally passed prompt-level strict results;
- Prompt 21 additionally reports an official strict and loose pass for all three encoded constraints; Prompts 22–27 each report an official strict and loose pass for their one encoded constraint, Prompts 28–44 each report an official strict and loose pass for their two encoded constraints, and Prompts 45–47 each report an official strict and loose pass for their two encoded constraints;
- the series contains 75 distinct IFEval item records across 78 published prompt positions, with repeat recorded runs of items 136, 1936, and 1705 at Prompts 30, 32, and 36 respectively;
- the two disclosed preflight corrections are included in the aggregate total.

## What the series does not establish

This is not:

- an official IFEval leaderboard score;
- a complete official evaluation of all seventy-eight published records;
- an independently verified benchmark;
- a blind third-party evaluation;
- a claim that the configured approach will pass every IFEval item;
- a representative estimate of all model behavior;
- proof of a particular underlying model identity;
- proof of legal, factual, or universal reliability.

The most accurate description is: **a documented Grounded DI OS one-shot run of seventy-eight published official IFEval records at prompt positions 1–78, with all final responses passing transparent local checks, Prompt 59's sentence-count fallback explicitly disclosed, Prompts 21–47 additionally passing official checker executions, and no independent verification claim.**


## Suggested reproduction procedure

1. Obtain the exact official IFEval item by key.
2. Preserve the prompt without rewriting it.
3. Run one response attempt under the stated public conditions.
4. Perform private preflight checks before finalization.
5. Record every preflight correction.
6. Preserve the final response exactly.
7. Run the official evaluator if it is actually available; otherwise use a clearly labeled local equivalent.
8. Separate official encoded constraints from manual task checks.
9. Generate the record with the prompt, response, evidence, hashes, limitations, and claim boundaries.
10. Do not publish a stronger claim than the evidence supports.

## Status

**INTERNAL ONE-SHOT RECORDS**  
**LOCAL CHECK PASS: 78/78 PUBLISHED RECORDS**  
**OFFICIAL EVALUATOR: 27/78 EXECUTED · PROMPTS 21–47 PASS**  
**EVIDENCE: NOT INDEPENDENTLY VERIFIED**

#Grounded-DI #DeterministicIntelligence #CrossDomain #AuditableAI 
