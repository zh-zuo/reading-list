# Implicit reasoning & agent orchestration

Papers on implicit / latent reasoning in LLMs — reasoning carried out *internally* (latent states, continuous or discrete "reasoning tokens") instead of as explicit chain-of-thought — and on orchestrating agents that reason implicitly.

**Open problem I'm chasing:** the *inverse mapping* — recovering explicit, interpretable reasoning from latent/implicit reasoning states (the inverse of compressing reasoning into latent tokens) is still not well solved. That's the bottleneck for orchestrating and auditing agents that reason implicitly.

## P1 — read soon

- [ ] **Li+2025** — *Implicit Reasoning in Large Language Models: A Comprehensive Survey* — the map of the field: taxonomy by execution paradigm (latent optimization, signal-guided control, layer-recurrent) and by where refinement happens (token / trajectory / internal-state level) — [arXiv](https://arxiv.org/abs/2509.02350)
- [ ] **Su+2025** — *Token Assorted: Mixing Latent and Text Tokens for Improved Language Model Reasoning* — the concrete "reasoning-token abstraction" I was pointed to: abstracts early reasoning steps into latent discrete tokens (VQ-VAE), shortening traces while keeping accuracy — [arXiv](https://arxiv.org/abs/2502.03275)

## P2 — this semester

- [ ] **Chen+2025** — *Reasoning Beyond Language: A Comprehensive Survey on Latent Chain-of-Thought Reasoning* — broader survey of latent CoT; splits reasoning tokens into discrete (symbolic control cues) vs continuous (learned embeddings) — context for the token-abstraction angle — [arXiv](https://arxiv.org/abs/2505.16782)

## P3 — on the radar

_(none yet)_

## Done

_(empty)_
