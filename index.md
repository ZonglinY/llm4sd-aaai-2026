---
layout: page
use-site-title: false
---

<h1 style="font-size: 60px; text-align: center;">Frontiers of LLMs for Automated Scientific Discovery: A Tutorial</h1>

<style>
  /* Speakers layout: predictable, centered, wraps cleanly */
  .speakers {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 24px;               /* space between cards */
    text-align: center;
  }

  /* Neutralize Bootstrap floats in this section only */
  .speakers > [class*="col-"] {
    float: none !important;
    padding: 0;
    flex: 0 1 300px;         /* card width; tweak 280–340px if you like */
  }

  /* Card: vertical stack */
  .speaker-card {
    width: 100%;
    max-width: 320px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  /* Photo */
  .speaker-photo {
    width: 260px;            /* tweak to match your assets */
    height: 260px;
    object-fit: cover;
    border-radius: 9999px;   /* round avatar */
    display: block;
    margin-bottom: 10px;
  }

  /* Name */
  .speaker-name {
    display: block;
    font-weight: 600;
    margin: 6px 0 2px;
    line-height: 1.3;
  }

  /* Affiliation — reserve up to 3 lines so cards align */
  .speaker-affil {
    display: block;
    line-height: 1.35;
    min-height: 4.05em;      /* ≈ 3 lines; use 2.7em for 2 lines */
    word-break: break-word;
    overflow-wrap: anywhere;
    color: #555;
  }
</style>





<div class="venue" style="font-size: 24px; display: block; font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif; font-weight: 300; color: #404040; text-align: center;">
  <span style="font-size: 23px; font-weight: 300;">
    <a target="_blank" href="https://drive.google.com/file/d/1oTRnVPSqrHoJb5xcu3cQ0_Jtflpj4bqW/view?usp=sharing">[Slides]</a>
  </span>
</div>



<div class="sharethis-inline-share-buttons"></div>
<meta name="thumbnail" content="./img/aaai-logo.png" />

<div class="container" style="margin-bottom: 10px;"></div>


<!-- Speakers -->
<div class="container text-center" style="margin-top:25px;margin-bottom:40px;">
  <div class="row speakers">
    {% for p in site.data.organizers %}
      {% assign person = p[1] %}
      <div class="col-xs-12 col-sm-6 col-md-4">
        <div class="speaker-card">
          <img class="speaker-photo"
               src="{{ site.baseurl }}/img/{{ person.img }}"
               alt="{{ person.name }}"
               loading="lazy">
          <a class="speaker-name" href="{{ person.url }}" target="_blank" rel="noopener">{{ person.name }}</a>
          <small class="speaker-affil">{{ person.affiliation }}</small>
        </div>
      </div>
    {% endfor %}
  </div>
</div>
<hr>




<!-- # Program Committee
<div class="container">
  <ul class="list-group list-group-flush">
    {% for p in site.data.pc.people %}
      <li class="list-group-item col-xs-6 col-sm-4 col-md-3">{{ p }}</li>
    {% endfor %}
  </ul>
</div>
<hr> -->


<!--# Taxonomy

![Taxonomy-viz](./img/taxonomy.jpg)-->


# About this Tutorial

This tutorial provides a comprehensive exploration of Symbolic Regression, an emerging area of AI focused on discovering interpretable mathematical expressions from data. As AI systems become increasingly integrated into critical domains, the ability to uncover transparent, mathematical relationships is essential for advancing scientific understanding and developing trustworthy AI systems. 

Recent advances in AI, particularly in deep learning and LLMs, have opened new paradigms in symbolic regression, enabling more sophisticated approaches to equation discovery and interpretation. These developments raise fundamental questions about how we can harness AI techniques to advance scientific understanding while maintaining interpretability.

Our tutorial is guided by the central question:
*"How can we leverage AI to discover meaningful mathematical expressions that advance scientific understanding while ensuring interpretability and trustworthiness?"*
We will explore this question through a comprehensive journey that covers:

- **Foundations and Evolution**: How has symbolic regression evolved from traditional search-based methods to modern AI-driven approaches? What are the key principles and challenges in discovering interpretable mathematical expressions?
- **Modern Approaches**: How do different paradigms - from evolutionary algorithms to transformer models and LLMs - contribute to equation discovery? How can we effectively combine these approaches?
- **Evaluation and Benchmarking**: What constitutes meaningful evaluation in symbolic regression? How do we design benchmarks that truly capture the ability to discover interpretable mathematical relationships?
- **Impact**: How can symbolic regression advance interpretable modeling and scientific discovery across different domains? What are the practical implications?

The tutorial is designed for researchers and practitioners in machine learning, AI, and scientific domains who seek to understand and contribute to the advancement of interpretable modeling. While familiarity with basic machine learning concepts is helpful, no prior experience with symbolic regression is required.
Through this tutorial, attendees will gain both theoretical understanding and practical insights into symbolic regression, positioning them to contribute to this evolving field and its applications across science and industry.

<hr>


# Reading List

### Introduction

- [A Survey on Large Language Models for Scientific Research](https://arxiv.org/abs/2501.04306)
- [Interpretable scientific discovery with symbolic regression: a review](https://link.springer.com/article/10.1007/s10462-023-10622-0)
- [Symbolic Regression is NP-hard](https://openreview.net/forum?id=LTiaPxqe2e) 

  
### Methods

**Search SR Methods**

- [Interpretable Machine Learning for Science with PySR and SymbolicRegression.jl](https://arxiv.org/abs/2305.01582) [[Github](https://github.com/MilesCranmer/PySR)]
- [Gene-pool Optimal Mixing Evolutionary Algorithm for Genetic Programming (Evolutionary Computation'21)](https://www.science.org/doi/10.1126/sciadv.aay2631) [[Github](https://github.com/marcovirgolin/GP-GOMEA)]
- [Symbolic Regression via Neural-Guided Genetic Programming Population Seeding (NeurIPS'21)](https://arxiv.org/abs/2111.00053) [[Github](https://github.com/dso-org/deep-symbolic-optimization)]
- [Symbolic Physics Learner: Discovering governing equations via Monte Carlo tree search (ICLR'23)](https://openreview.net/forum?id=ZTK3SefE8_Z) [[Github](https://github.com/isds-neu/SymbolicPhysicsLearner)]
- [AI Feynman: A physics-inspired method for symbolic regression (Science Advances)](https://www.science.org/doi/10.1126/sciadv.aay2631) [[Github](https://github.com/SJ001/AI-Feynman)]
- [Deep symbolic regression: Recovering mathematical expressions from data via risk-seeking policy gradients (ICLR'21)](https://openreview.net/forum?id=m5Qsh0kBQG) [[Github](https://github.com/dso-org/deep-symbolic-optimization)]




**Learning SR Methods**

- [Neural Symbolic Regression that scales (ICML'21)](https://proceedings.mlr.press/v139/biggio21a.html) [[Github](https://github.com/SymposiumOrganization/NeuralSymbolicRegressionThatScales)]
- [End-to-end Symbolic Regression with Transformers (NeurIPS'22)](https://proceedings.neurips.cc/paper_files/paper/2022/hash/42eb37cdbefd7abae0835f4b67548c39-Abstract-Conference.html) [[Github](https://github.com/facebookresearch/symbolicregression)]
- [SymFormer: End-to-end symbolic regression using transformer-based architecture](https://arxiv.org/abs/2205.15764) [[Github](https://github.com/vastlik/symformer)]
- [SymbolicGPT: A Generative Transformer Model for Symbolic Regression](https://arxiv.org/abs/2106.14131) [[Github](https://github.com/mojivalipour/symbolicgpt)]
- [SNIP: Bridging Mathematical Symbolic and Numeric Realms with Unified Pre-training (ICLR'24)](https://openreview.net/forum?id=KZSEgJGPxu) [[Github](https://github.com/deep-symbolic-mathematics/Multimodal-Math-Pretraining)]


**Learning + Search SR Methods**

- [Transformer-based Planning for Symbolic Regression (NeurIPS'23)](https://proceedings.neurips.cc/paper_files/paper/2023/hash/8ffb4e3118280a66b192b6f06e0e2596-Abstract-Conference.html) [[Github](https://github.com/deep-symbolic-mathematics/TPSR)]
- [A Unified Framework for Deep Symbolic Regression (NeurIPS'22)](https://proceedings.neurips.cc/paper_files/paper/2022/hash/dbca58f35bddc6e4003b2dd80e42f838-Abstract-Conference.html) [[Github](https://github.com/dso-org/deep-symbolic-optimization)]
- [Deep Generative Symbolic Regression (ICLR'23)](https://openreview.net/forum?id=o7koEEMA1bR) [[Github](https://github.com/samholt/DeepGenerativeSymbolicRegression)]
- [Efficient Generator of Mathematical Expressions for Symbolic Regression (Machine Learning'23)](https://link.springer.com/article/10.1007/s10994-023-06400-2) [[Github](https://github.com/smeznar/HVAE)]
- [SNIP: Bridging Mathematical Symbolic and Numeric Realms with Unified Pre-training (ICLR'24)](https://openreview.net/forum?id=KZSEgJGPxu) [[Github](https://github.com/deep-symbolic-mathematics/Multimodal-Symbolic-Regression)]


**LLM-guided SR  Methods**
- [LLM-SR: Scientific Equation Discovery via Programming with Large Language Models (ICLR'25)](https://openreview.net/forum?id=m2nmp8P5in) [[Github](https://github.com/deep-symbolic-mathematics/LLM-SR)]
- [In-Context Symbolic Regression: Leveraging Large Language Models for Function Discovery (ACL'24)](https://aclanthology.org/2024.acl-srw.49/) [[Github](https://github.com/merlerm/In-Context-Symbolic-Regression)]
- [Symbolic Regression with a Learned Concept Library (NeurIPS'24)](https://aclanthology.org/2024.acl-srw.49/) [[Github](https://github.com/trishullab/LibraryAugmentedSymbolicRegression.jl)]


**SR Benchmarks**  
- [Contemporary Symbolic Regression Methods and their Relative Performance (NeurIPS'21)](https://datasets-benchmarks-proceedings.neurips.cc/paper/2021/hash/c0c7c76d30bd3dcaefc96f40275bdc0a-Abstract-round1.html) [[Github](https://github.com/cavalab/srbench/)]
- [Rethinking Symbolic Regression Datasets and Benchmarks for Scientific Discovery (DMLR'24)](https://openreview.net/forum?id=i2e2wqt0nAI) [[Github](https://github.com/omron-sinicx/srsd-benchmark)]
- [LLM-SRBench: A New Benchmark for Scientific Equation Discovery with Large Language Models (ICML'25)](https://arxiv.org/abs/2504.10415) [[Github](https://github.com/deep-symbolic-mathematics/llm-srbench)] [[Dataset](https://huggingface.co/datasets/nnheui/llm-srbench)]
