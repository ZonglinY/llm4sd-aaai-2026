---
layout: page
use-site-title: false
---

<h1 style="font-size: 60px; text-align: center;">Symbolic Regression: Towards Interpretability and Automated Scientific Discovery</h1>


<div class="venue" style="font-size: 24px; display: block; font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif; font-weight: 300; color: #404040; text-align: center;">
  <span style="font-size: 23px; font-weight: 300;">
    <a target="_blank" href="https://drive.google.com/file/d/1xMh5_p7oQ_OJfNJn49Y--KQnY1lzjHBL/view?usp=sharing">[Slides]</a>
  </span>
</div>



<div class="sharethis-inline-share-buttons"></div>
<meta name="thumbnail" content="./img/aaai-logo.png" />

<div class="container" style="margin-bottom: 10px;"></div>


<div class="container" style="margin-top: 25px;margin-bottom: 40px;">
  <!-- <br> 
  <div class="row"> -->
  <div class="row">
    {% for p in site.data.organizers %}
    {% if forloop.index<=4 %}
    {% capture id %}{{ p[0] }}{% endcapture %}
    {% include profile.html p=p %}
    {% endif %}
    {% endfor %}
  </div>
  <div class="row">
    {% for p in site.data.organizers %}
    {% capture id %}{{ p[0] }}{% endcapture %}
    {% if forloop.index>4 and forloop.index<=8%}
    {% include profile.html p=p %}
    {% endif %}
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


# Taxonomy

![Taxonomy-viz](./img/taxonomy.jpg)


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


### Benchmarks
- [Contemporary Symbolic Regression Methods and their Relative Performance (NeurIPS'21)](https://datasets-benchmarks-proceedings.neurips.cc/paper/2021/hash/c0c7c76d30bd3dcaefc96f40275bdc0a-Abstract-round1.html) [[Github](https://github.com/cavalab/srbench/)]
- [Rethinking Symbolic Regression Datasets and Benchmarks for Scientific Discovery (DMLR'24)](https://openreview.net/forum?id=i2e2wqt0nAI) [[Github](https://github.com/omron-sinicx/srsd-benchmark)]
