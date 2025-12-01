# Livestock Language Skill

A Claude Skill for correctly using Australian livestock terminology

This skill teaches Claude how to understand and apply the terminology defined in the **National Bovine Livestock Language Guidelines**, published by **MLA, AUS-MEAT, and the Meat Industry Language and Standards Committee**.

Most large language models often default to US, Chinese or European livestock language. That leads to predictable problems: mixed scoring systems, incorrect assumptions, and advice that sounds confident but doesn’t match Australian practice. This skill provides AI Agents with a structured way to stay within the Australian standard.

The aim is simple: make livestock terminology clear, consistent, and usable inside an AI interface without changing or replacing the official Guidelines.

## What this skill does

* Keeps agents aligned with Australian livestock terminology
* Provides accurate definitions for classification, identification, physical assessment, welfare, reproduction, and trading specifications
* Prevents the model from drifting into international terms unless specifically asked
* Offers a foundation for future extensions, including calculator tools and vision-based assessment

It also gives industry professionals a starting point for building other AI tools that reflect how the Australian red meat sector actually communicates.

## How it works

This skill draws from the guideline files located in the `language/` directory. Each file covers a specific part of the National Livestock Language:

* **Classification & Identification** (sex classes, breed codes, NLIS traceability)
* **Physical Assessment** (fat score 0–6, muscle score A–E, frame scoring)
* **Health, Welfare & Reproduction**
* **Trading Terms & Specifications** (HSCW, dressing %, MSA, EUCAS)
* **Terminology Glossary** for quick lookups

Claude loads the relevant file, applies the definitions directly, and stays within the Australian standard unless the user explicitly requests a comparison with another system.

## Why a skill instead of fine-tuning?

Fine-tuning a model for this domain would require thousands of labelled examples and constant retraining every time standards shift. Skills avoid that overhead. They are:

* **Transparent** — anyone can read and review the logic
* **Easy to update** — a new file or correction is all it takes
* **Practical** — no datasets, GPUs, or infrastructure
* **A clean foundation** if the industry ever decides a dedicated livestock model is worth building

This keeps the barrier low while still delivering highly accurate, domain-specific behaviour.

## Current limitations

This skill doesn’t replace expertise. It can’t interpret images, assess an animal visually, or replicate real stockmanship. Some reference tables and state-level detail are trimmed to fit within the Skill specification constraints. These gaps are intended to be filled by complementary tools and eventually vision support.

## Future work

Planned additions include:

* Dressing %, frame score and weight calculators
* Fitness-to-load and welfare compliance checks
* Processor specification matching
* Vision-based assessment aligned with MLA visual standards

## License

See `LICENSE.txt` for full terms.
