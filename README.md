# NEO: A Unified Model for Personalization


**Official implementation of the paper:** > *A Unified Model for Personalization: Language-Steerable Generative Recommendation, Search, and User Understanding*

---

## Overview

**NEO** is a framework that adapts a pre-trained decoder-only LLM into a **tool-free, catalog-grounded generator**. Unlike traditional recommender systems or tool-augmented LLMs, NEO reasons jointly over multiple-domain entities, user behavior, and natural language in a fully self-contained manner.

### Key Innovations:
* **Semantic Identifiers (SIDs):** Represents items as a distinct modality, allowing the model to interleave text and typed item identifiers in a shared sequence.
* **Language-Steerability:** Instruction-conditioned control over tasks (search vs. recommendation), target entity types, and output formats (IDs, text, or mixed).
* **Constrained Decoding:** Guarantees that the model only generates valid catalog items without limiting the creativity or logic of its free-form text.
* **Massive Scale:** Evaluated and proven on real-world catalogs of **10M+ items** across multiple media types.
