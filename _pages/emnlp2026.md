---
layout: default
permalink: /emnlp2026/
title: EMNLP 2026 paper
description: "Do Prompts Guarantee Safety? Mitigating Toxicity from LLM Generations through Gradient Based Subspace Intervention — Findings of EMNLP 2026."
nav: false
---

<!--
  Landing page for the QR code on the EMNLP 2026 poster.
  Most visitors arrive from a phone, so the PDF button comes first: mobile
  browsers render an embedded PDF as a single static page, so the inline viewer
  is only shown on wider screens.
-->

<style>
  .paper-page {
    padding-top: 1rem;
  }
  .paper-page .venue {
    display: inline-block;
    padding: 0.15rem 0.6rem;
    border-radius: 0.25rem;
    background: var(--global-theme-color);
    color: var(--global-hover-text-color);
    font-size: 0.8rem;
    font-weight: 600;
    letter-spacing: 0.02em;
  }
  .paper-page h2.paper-title {
    margin: 0.75rem 0 0.5rem;
    font-size: 1.6rem;
    line-height: 1.3;
  }
  .paper-page .authors {
    margin: 0;
    font-size: 1.05rem;
  }
  .paper-page .authors a {
    color: inherit;
    border-bottom: 1px solid var(--global-divider-color);
  }
  .paper-page .affils {
    margin: 0.25rem 0 0;
    color: var(--global-text-color-light);
    font-size: 0.9rem;
  }
  .paper-page .actions {
    display: flex;
    flex-wrap: wrap;
    gap: 0.6rem;
    margin: 1.5rem 0;
  }
  .paper-page .actions a {
    flex: 1 1 9rem;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 0.7rem 1rem;
    border-radius: 0.4rem;
    border: 1px solid var(--global-theme-color);
    color: var(--global-theme-color);
    font-weight: 600;
    text-decoration: none;
  }
  .paper-page .actions a.primary {
    background: var(--global-theme-color);
    color: var(--global-hover-text-color);
  }
  .paper-page .actions a:hover {
    background: var(--global-hover-color);
    color: var(--global-hover-text-color);
  }
  .paper-page .warning {
    font-size: 0.85rem;
    color: var(--global-text-color-light);
    font-style: italic;
  }
  .paper-page .viewer {
    width: 100%;
    height: 85vh;
    border: 1px solid var(--global-divider-color);
    border-radius: 0.4rem;
  }
  .paper-page pre.bibtex {
    white-space: pre-wrap;
    word-break: break-word;
    font-size: 0.8rem;
    padding: 1rem;
    border-radius: 0.4rem;
    background: var(--global-code-bg-color);
  }
  @media (max-width: 768px) {
    .paper-page .viewer-section {
      display: none;
    }
  }
</style>

<div class="paper-page">

<span class="venue">Findings of EMNLP 2026 · Budapest</span>

<h2 class="paper-title">Do Prompts Guarantee Safety? Mitigating Toxicity from LLM Generations through Gradient Based Subspace Intervention</h2>

<p class="authors">
  <a href="{{ '/' | relative_url }}">Himanshu Singh</a>,
  <a href="https://home.ziwei-xu.com/">Ziwei Xu</a>,
  <a href="https://iiitd.ac.in/subramanyam">A. V. Subramanyam</a>,
  <a href="https://www.comp.nus.edu.sg/~mohan/">Mohan Kankanhalli</a>
</p>
<p class="affils">IIIT Delhi · FAR.AI · National University of Singapore</p>

<div class="actions">
  <a class="primary" href="{{ '/assets/pdf/EMNLP2026_paper.pdf' | relative_url }}" target="_blank" rel="noopener">Read the full paper (PDF)</a>
  <a href="{{ '/assets/pdf/EMNLP2026_poster.pdf' | relative_url }}" target="_blank" rel="noopener">Poster</a>
  <a href="https://arxiv.org/abs/2602.06623" target="_blank" rel="noopener">arXiv</a>
  <a href="#bibtex">Cite</a>
</div>

<h3>Abstract</h3>

<p>
Large Language Models (LLMs) are powerful text generators, yet they can produce toxic or harmful content even when given seemingly harmless prompts. This presents a serious safety challenge and can cause real-world harm. Toxicity is often subtle and context-dependent, making it difficult to detect at the token level or through coarse sentence-level signals. Moreover, efforts to mitigate toxicity often face a trade-off between safety and the coherence, or fluency, of the generated text. In this work, we present a targeted subspace intervention strategy based on gradient signals for identifying and suppressing hidden toxic patterns from underlying model representations, while preserving the overall ability to generate safe, fluent content. On the RealToxicityPrompts dataset, our method achieves strong mitigation performance compared to existing baselines while imposing minimal impact on inference complexity. Across LLMs, our approach reduces the toxicity of state-of-the-art detoxification systems by 8–20%, while maintaining comparable fluency. We further validate cross-benchmark generality on ToxiGen, where the same gains hold under adversarial, implicitly toxic prompts. Through extensive quantitative and qualitative analyses, we show that our approach achieves effective toxicity reduction without impairing generative performance, consistently outperforming existing baselines.
</p>

<p class="warning">Content warning: the paper contains examples of toxic and offensive language. Toxic words are partially masked with *.</p>

<div class="viewer-section">
  <h3>Paper</h3>
  <iframe class="viewer" src="{{ '/assets/pdf/EMNLP2026_paper.pdf' | relative_url }}#view=FitH" title="EMNLP 2026 paper PDF" loading="lazy"></iframe>
</div>

<h3 id="bibtex">Citation</h3>

<pre class="bibtex">@inproceedings{singh2026promptsguaranteesafetymitigating,
  title     = {Do Prompts Guarantee Safety? Mitigating Toxicity from LLM Generations through Gradient Based Subspace Intervention},
  author    = {Singh, Himanshu and Xu, Ziwei and Subramanyam, A. V. and Kankanhalli, Mohan},
  booktitle = {Findings of the Association for Computational Linguistics: EMNLP 2026},
  address   = {Budapest, Hungary},
  month     = {October},
  year      = {2026},
  eprint    = {2602.06623},
  archivePrefix = {arXiv}
}</pre>

</div>
