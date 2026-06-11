# LLM training

The training pipeline by stage — whole-pipeline surveys, pretraining / mid-training, post-training & alignment, the data angle — plus positioning papers situating LLMs in the broader AI landscape (read LeCun / Chollet / Bender / Bubeck as a four-way argument over whether LLMs are a destination or a way station).

> Entries without a link are cited by title/venue — confirm the exact identifier when ticking off.

## P1 — read soon

- [ ] **Zhao+2023** — *A Survey of Large Language Models* (frequently revised) — the most comprehensive single reference: pretraining, adaptation tuning, utilization, and alignment in one place; the scaffolding for everything else — [arXiv](https://arxiv.org/abs/2303.18223)

## P2 — this semester

- [ ] **Mo+2025** — *Mid-Training of Large Language Models: A Survey* — treats the in-between stage as a first-class paradigm: annealing-style phases refining data quality, optimization schedules, and context length, via gradient noise scale / information bottleneck / curriculum learning — [arXiv](https://arxiv.org/abs/2510.06826)
- [ ] **Wang+2024** — *A Comprehensive Survey of LLM Alignment Techniques: RLHF, RLAIF, PPO, DPO and More* — best pick for the alignment-algorithm zoo (breadth pick; the RL-lifecycle survey below is the frontier alternative) — [arXiv](https://arxiv.org/abs/2407.16216)
- [ ] **Bommasani+2021** — *On the Opportunities and Risks of Foundation Models* (Stanford CRFM) — coined "foundation model"; the homogenization argument is the key structural claim — [arXiv](https://arxiv.org/abs/2108.07258)
- [ ] **LeCun 2022** — *A Path Towards Autonomous Machine Intelligence* — canonical position paper arguing LLMs are not the road to autonomous intelligence; proposes JEPA — [OpenReview](https://openreview.net/forum?id=BZ5a1r-kVsf)
- [ ] **Chollet 2019** — *On the Measure of Intelligence* — skill-vs-generalization and the ARC benchmark; the conceptual counterweight to scaling-maximalism — [arXiv](https://arxiv.org/abs/1911.01547)
- [ ] **Bender+2021** — *On the Dangers of Stochastic Parrots* (FAccT 2021) — the skeptical position: form without grounding; reference point for the "do they understand?" debate
- [ ] **Bubeck+2023** — *Sparks of Artificial General Intelligence: Early Experiments with GPT-4* — the maximalist counterpoint; best read against Chollet and Bender — [arXiv](https://arxiv.org/abs/2303.12712)

## P3 — on the radar

- [ ] **RL-lifecycle survey (2025)** — *Reinforcement Learning Meets Large Language Models: A Survey … Across the LLM Lifecycle* — broader RL framing including post-training/test-time RL of reasoning systems (o1-style); swap into P2 if the reasoning-RL frontier matters more than alignment breadth — [arXiv](https://arxiv.org/abs/2509.16679)
- [ ] **Tie+2025** — *A Survey on Post-training of Large Language Models* — squarely post-training: SFT, reward modeling, RL-based alignment, with clear RLHF-loop diagrams (overlaps Wang+2024) — [arXiv](https://arxiv.org/abs/2503.06072)
- [ ] **Luo+2025** — *A Survey on Efficient LLM Training: From Data-centric Perspectives* — taxonomy of data-efficient post-training: selection, quality enhancement, synthetic generation, distillation, self-evolving data ecosystems — [arXiv](https://arxiv.org/abs/2510.25817)
- [ ] **Minaee+2024** — *Large Language Models: A Survey* — model-family-centric (GPT / LLaMA / PaLM lineages) plus training/fine-tuning/evaluation datasets; second opinion to Zhao+2023 — [arXiv](https://arxiv.org/abs/2402.06196)
- [ ] **Naveed+2023** — *A Comprehensive Overview of Large Language Models* — third broad overview, often cited alongside the two above — [arXiv](https://arxiv.org/abs/2307.06435)
- [ ] **Dawid & LeCun 2023** — *Introduction to Latent Variable Energy-Based Models* — gentler, pedagogical walk-through of the H-JEPA machinery — [arXiv](https://arxiv.org/abs/2306.02572)

## Done

_(empty)_
