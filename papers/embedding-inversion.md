# Embedding inversion & perturbation defenses

Text → embedding is easy; recovering the text from a (possibly perturbed) embedding is hard. Three angles: **attacks** (forward inversion), **defenses** (perturbing embeddings), and the **formal-guarantee / statistical framing** of the privacy–utility tradeoff.

**Open thread I'm chasing:** a worst-case (information-theoretic) recoverability bound for text — "above this noise level, no adversary wins" — grounded in embedding geometry (manifold reach, Jacobian conditioning). The empirical privacy–utility curves and the metric-DP mechanism guarantees exist; the minimax-style converse for *discrete text recovery* does not yet.

> Entries without a link are cited by title/venue — confirm the exact identifier when ticking off.

## P1 — read soon

- [ ] **Morris+2023** — *Text Embeddings Reveal (Almost) As Much As Text* (EMNLP 2023) — the **vec2text** attack that defines the problem: iterative re-embed-and-correct recovers ~92% of 32-token sequences exactly — [arXiv](https://arxiv.org/abs/2310.06816)
- [ ] **ZSinvert (2024)** — *Universal Zero-shot Embedding Inversion* — the adaptive-attack counterpoint: vec2text degrades on Gaussian-perturbed embeddings, but semantic content is recovered anyway, without a per-embedding trained model — why noise alone isn't a guarantee — [arXiv](https://arxiv.org/abs/2504.00147)
- [ ] **Mitigating Privacy Risks in LLM Embeddings from Embedding Inversion (2024)** — most on-point defense study: defense vs. downstream performance under embedding perturbation, plus dimensionality reduction and quantization as alternatives
- [ ] **SPARSE (2026)** — *Concept-Aware Privacy Mechanisms for Defending Embedding Inversion Attacks* — argues standard DP wastes noise by assuming uniform per-dimension sensitivity; Mahalanobis mechanism with elliptical noise — [arXiv](https://arxiv.org/abs/2602.07090) · [OpenReview](https://openreview.net/forum?id=bcOD0CLgBb)

## P2 — this semester

- [ ] **Feyisetan+2020** — multivariate Laplace mechanism for text — the d_X-privacy text instantiation; the guarantee-side entry point
- [ ] **Du+2023** — *Sanitizing Sentence Embeddings (and Labels) for Local Differential Privacy* (CCS 2023) — Purkayastha and Normalized Planar Laplace (directional-noise) mechanisms
- [ ] **Duchi+2013** — *Local Privacy and Statistical Minimax Rates* (FOCS 2013 / JASA 2018) — the template for turning "noise added before release" into estimation-rate lower bounds via privatized Fano/Le Cam — the machinery to port to discrete text recovery under embedding noise
- [ ] **Song & Raghunathan 2020** — *Information Leakage in Embedding Models* (CCS 2020) — foundational; first showed embeddings leak, though only to approximate bag-of-words recovery
- [ ] **GEIA (2023)** — *Sentence Embedding Leaks More Information than You Expect* — generative inversion reconstructing whole sentences, not just word sets
- [ ] **DPPN (2024)** — *Detecting and Perturbing Privacy-Sensitive Neurons to Defend Embedding Inversion Attacks* — perturbs only a small set of privacy-sensitive neurons instead of all dimensions — [OpenReview](https://openreview.net/forum?id=DF5TVzpTW0)
- [ ] **A Differentially Private Text Perturbation Method Using a Regularized Mahalanobis Metric** (ACL PrivateNLP 2020) — anisotropic-noise predecessor on the mechanism side — [ACL](https://aclanthology.org/2020.privatenlp-1.2)
- [ ] **EntroGuard (2025)** — *Safeguarding LLM Embeddings in End-Cloud Collaboration via Entropy-Driven Perturbation* — plug-in perturbation for black-box on-device embedding models — [arXiv](https://arxiv.org/abs/2503.12896)

## P3 — on the radar

- [ ] **Andrés+2013 / Chatzikokolakis+2013** — geo-indistinguishability — roots of metric differential privacy (d_X-privacy), the formalism behind "perturb the vector, get indistinguishability"
- [ ] **LAGO (2025)** — *Few-shot Crosslingual Embedding Inversion Attacks* — newer attack variant; useful DP-defense evaluation section — [arXiv](https://arxiv.org/abs/2505.16008)
- [ ] **ALGEN (2025)** — *Few-shot Inversion Attacks on Textual Embeddings via Alignment and Generation*
- [ ] **Reproducibility study of vec2text (2025)** — caveat on how robust the headline inversion numbers are
- [ ] **Morris+ — Language Model Inversion** — recovers prompts from output distributions; same inversion philosophy, different target

## Done

_(empty)_
