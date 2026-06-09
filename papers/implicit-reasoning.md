# Implicit reasoning & agent orchestration

Papers on implicit / latent reasoning in LLMs — reasoning carried out *internally* (latent states, continuous or discrete "reasoning tokens") instead of as explicit chain-of-thought — and on orchestrating agents that reason implicitly.

**Open problem I'm chasing:** the *inverse mapping* — recovering explicit, interpretable reasoning from latent/implicit reasoning states (the inverse of compressing reasoning into latent tokens) is still not well solved. That's the bottleneck for orchestrating and auditing agents that reason implicitly.

## P1 — read soon

- [ ] **Li+2025** — *Implicit Reasoning in Large Language Models: A Comprehensive Survey* — the map of the field: taxonomy by execution paradigm (latent optimization, signal-guided control, layer-recurrent) and by where refinement happens (token / trajectory / internal-state level) — [arXiv](https://arxiv.org/abs/2509.02350)
- [ ] **Ramji+2026** — *Thinking Without Words: Efficient Latent Reasoning with Abstract Chain-of-Thought* — the recent "abstract reasoning token" paper I was pointed to: reasons through a reserved vocabulary of discrete *abstract* tokens instead of words, ~11.6× fewer reasoning tokens at comparable accuracy — [arXiv](https://arxiv.org/abs/2604.22709)
- [ ] **Hao+2024** — *Training Large Language Models to Reason in a Continuous Latent Space* (Coconut) — the seminal continuous-latent-thought method: feed the last hidden state back as the next input embedding; a latent thought can encode several next steps (BFS-like) — the ancestor of this whole thread — [arXiv](https://arxiv.org/abs/2412.06769)
- [ ] **Zou+2025** — *Latent Collaboration in Multi-Agent Systems* (LatentMAS) — agent orchestration moved into latent space: agents pass latent thoughts through working memory, training-free, far fewer tokens — the most direct hit on "agent orchestration with implicit reasoning" — [arXiv](https://arxiv.org/abs/2511.20639)

## P2 — this semester

- [ ] **Su+2025** — *Token Assorted: Mixing Latent and Text Tokens for Improved Language Model Reasoning* — earlier/related: abstracts early reasoning steps into latent discrete tokens (VQ-VAE) mixed with text — the predecessor to the abstract-token idea — [arXiv](https://arxiv.org/abs/2502.03275)
- [ ] **Chen+2025** — *Reasoning Beyond Language: A Comprehensive Survey on Latent Chain-of-Thought Reasoning* — broader survey of latent CoT; splits reasoning tokens into discrete (symbolic control cues) vs continuous (learned embeddings) — context for the token-abstraction angle — [arXiv](https://arxiv.org/abs/2505.16782)
- [ ] **Zhao+2026** — *Shorthand for Thought: Compressing LLM Reasoning via Entropy-Guided Supertokens* — splits reasoning tokens into structural vs organic, then merges recurring structural ones into "supertokens" (cross-word BPE) to compress traces — [arXiv](https://arxiv.org/abs/2604.26355)
- [ ] **Liu+2026** — *Thoughts-as-Planning: Latent World Models for Chain-of-Thoughts Optimization via Reinforcement Planning* — frames reasoning-chain optimization as sequential decisions over a latent semantic space, learning a world model of how chain edits change outputs — [arXiv](https://arxiv.org/abs/2605.28842)
- [ ] **Du+2025** — *Enabling Agents to Communicate Entirely in Latent Space* (Interlat) — inter-agent communication and task-solving fully in latent space; transmit and reason over latent states for large communication-efficiency gains — [arXiv](https://arxiv.org/abs/2511.09149)
- [ ] **Chen+2025** — *Latent Debate: A Surrogate Framework for Interpreting LLM Thinking* — maps latent reasoning to implicit internal "arguments" as a faithful surrogate — squarely the inverse-mapping problem — [arXiv](https://arxiv.org/abs/2512.01909)
- [ ] **Ramjee+2026** — *Ulterior Motives: Detecting Misaligned Reasoning in Continuous Thought Models* — monitorability / auditing of latent reasoning (the safety side of inverse mapping) — [arXiv](https://arxiv.org/abs/2604.23460)
- [ ] **Zhu+2025** — *A Survey on Latent Reasoning* — second survey of the area; complements Li+2025 and the Chen+2025 latent-CoT survey — [arXiv](https://arxiv.org/abs/2507.06203)

## P3 — on the radar

- [ ] **Liu+2026** — *The Vision Wormhole: Latent-Space Communication in Heterogeneous Multi-Agent Systems* — latent-space comms between agents via the VLM visual interface (continuous dense vectors) — niche but on-theme for agent orchestration — [arXiv](https://arxiv.org/abs/2602.15382)

## Done

_(empty)_
