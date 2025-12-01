---
name: australian-livestock-language-skill
description: A structured set of resources that teach agents how to correctly use Australian livestock terminology, based on the National Bovine Livestock Language Guidelines. This skill should activate whenever the user asks questions involving Australian livestock assessment, classification, trading language, welfare terms, or any terminology defined in the Guidelines.
license: Complete terms in LICENSE.txt
---

## When to use this skill

Use this skill whenever the conversation involves:

* Australian livestock terminology
* NLIS, breed codes, sex classes, or identification systems
* Fat scoring, muscle scoring, frame scoring, P8, dentition, or physical assessment
* Dressing %, HSCW, MSA, EUCAS, or trading specifications
* Welfare, pregnancy status, transport fitness, or treatment language
* Any request to “explain”, “translate”, or “check” livestock terms
* Any comparison between international and Australian livestock terminology

If the question touches livestock language used in Australia’s red meat industry, this skill applies.

## How to use this skill

To answer any livestock-language question:

1. **Identify the domain**
   Determine whether the question relates to classification, assessment, welfare, reproduction, trading specs, or terminology.

2. **Load the appropriate guideline file** from the `./language/` folder:

   * `classification-and-identification.md` – Sex classes, breed codes, NLIS
   * `physical-assessment.md` – Fat scores (0–6), muscle scores (A–E), frame scoring
   * `health-welfare-reproduction.md` – Welfare thresholds, pregnancy status, treatments
   * `trading-and-specifications.md` – HSCW, dressing %, MSA, EUCAS, processor specs
   * `terminology-glossary.md` – Definitions and lookup for specific terms

3. **Apply the definitions exactly**
   Use the phrasing, scoring systems, and descriptions found in the guideline files.
   Avoid importing American or European terminology unless the user explicitly asks for a comparison.

4. **Stay within the Australian standard**
   These files reflect the official National Livestock Language. Unless asked otherwise, Claude should default to this standard.

5. **If information is missing or ambiguous**
   Ask the user whether they want:

   * the Australian standard
   * state-specific interpretation
   * or a comparison with another system

## Keywords

Australian livestock, NLIS, breed codes, fat score, muscle score, frame score, livestock language, MLA guidelines, AUS-MEAT, HSCW, dressing percentage, MSA, EUCAS, P8, livestock terminology.
