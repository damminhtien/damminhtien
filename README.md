# Tien Minh Dam

Research Engineer building reproducible systems for search, optimization, clinical NLP, and technical learning.

[![ORCID](https://img.shields.io/badge/ORCID-0009--0006--7683--4476-a6ce39?logo=orcid&logoColor=white)](https://orcid.org/0009-0006-7683-4476)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-damminhtien-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/damminhtien)
[![Email](https://img.shields.io/badge/Email-contact-8B89CC?logo=gmail&logoColor=white)](mailto:damminhtienchl@gmail.com)

I work at the intersection of algorithmic research and usable software: exact and parallel search, constrained multi-objective optimization, Vietnamese clinical text grounding, and tools that make difficult technical subjects easier to learn.

## Now

- **[ClinGrounder](https://github.com/damminhtien/clingrounder)** — an offset-safe clinical text grounding toolkit for Vietnamese and mixed Vietnamese-English text. The current public release is [`0.1.0a9`](https://pypi.org/project/clingrounder/0.1.0a9/), with a deterministic offline pipeline, terminology linking, provenance, and an optional local [Streamlit demo](https://github.com/damminhtien/clingrounder/tree/main/examples/demo).
- **[Atlas](https://github.com/damminhtien/learn-atlas)** — a self-hosted learning codex covering linear algebra, calculus, probability, algorithms, ML, DL, RL, LLMs, and information theory. [Open the live site](https://techeese.github.io/learn-atlas/).
- **[MOSP documentation](https://damminhtien.github.io/MOSP/)** — an exact multi-objective shortest-path SDK and benchmark workbench, with C++, Python, Java/JNI, a stable C ABI, and a visual debugger. The research line is described in the [SOPMOA* paper](https://doi.org/10.1007/978-3-031-97635-3_36).

## Research

My research focuses on making optimization and search systems faster without weakening correctness or reproducibility.

- **SOPMOA*** — shared-open parallelism for high-performance multi-objective pathfinding. [ICCS 2025 / DOI](https://doi.org/10.1007/978-3-031-97635-3_36)
- **Constraint handling** — a generalized multi-objective framework with a constraint violation ratio and adaptive constraint diversity factor. [IJCAS 2024 / DOI](https://doi.org/10.1007/s12555-024-0445-8)
- **Radar scheduling** — genetic algorithms with stochastic heuristic initialization for constrained radar allocation. [IDEAL 2024 / DOI](https://doi.org/10.1007/978-3-031-77731-8_18)
- **Ar*** — bounded-suboptimal search with a conditional node re-expansion policy. [ICTC 2023 / IEEE](https://ieeexplore.ieee.org/document/10393240) · [DOI](https://doi.org/10.1109/ICTC58733.2023.10393240) · **Best Paper Award**

## Selected work

### ClinGrounder

The public benchmark is deliberately separated from clinical claims. On the checked-in synthetic pilot, the full deterministic profile reports entity exact F1 `1.0000`, assertion macro-F1 `1.0000`, Recall@5 `0.8750`, relation F1 `1.0000`, and p95 latency `3.704 ms` across four synthetic documents. The generated diagnostic expansion reports entity exact F1 `0.5408`, exact precision `1.0000`, Recall@5 `0.3965`, and p95 latency `3.010 ms` on a 200-document synthetic test split.

→ [Benchmark methodology and results](https://github.com/damminhtien/clingrounder/blob/main/docs/benchmarks/vi_clinical_grounding_v1/results.md) · [PyPI release](https://pypi.org/project/clingrounder/0.1.0a9/)

### Atlas

The live learning site currently contains **164 lessons**, **2,496 fact-checked MCQs**, **969 flashcards**, **492 homework problems**, **493 worked examples**, and **97 interactive visualizations**. It is a zero-build static site with GitHub Pages deployment and browser-local progress.

→ [Live demo](https://techeese.github.io/learn-atlas/) · [Source](https://github.com/damminhtien/learn-atlas)

### MOSP / SOPMOA*

In a paired 5-second, repeat-2 stress benchmark, `HybridCorridorPulseA` reached median rates of **379,499 expansions/s on long NYC**, **157,884 on MSPP4**, and **83,408 on MSPP5**, compared with **225,505 / 93,571 / 55,989** for the legacy CTDL line and **193,791 / 57,505 / 47,427** for `LTMOA_array_superfast`. These are stress-set results, not a universal solver ranking.

→ [Benchmark workbench and methodology](https://damminhtien.github.io/MOSP/) · [SOPMOA* DOI](https://doi.org/10.1007/978-3-031-97635-3_36)

### Semantic segmentation knowledge base

**[Awesome Semantic Segmentation](https://github.com/damminhtien/awesome-semantic-segmentation)** is a curated roadmap from FCN and U-Net through Transformer, universal, promptable, and open-vocabulary segmentation, with benchmark-oriented reading guidance for mIoU, Dice/F1, boundary quality, latency, memory, calibration, and robustness.

## Teaching and community

- Contributor and translator of the Vietnamese [Stanford CS229](https://stanford.edu/~shervine/l/vi/teaching/cs-229/cheatsheet-supervised-learning) and [CS230](https://stanford.edu/~shervine/l/vi/teaching/cs-230/cheatsheet-convolutional-neural-networks) cheatsheets.
- Co-founder of [BKFA](https://github.com/BKFA), an open learning community for computer science.

> **Evidence note.** ClinGrounder benchmark values above are from synthetic, reproducible engineering fixtures and are **not clinical validation**. MOSP values are time-capped stress-set measurements; regenerate the linked benchmark artifacts before making a new performance claim.
