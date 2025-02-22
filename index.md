---
layout: page
title: "Symbolic Regression: Towards Interpretability and Automated Scientific Discovery"
use-site-title: true
---

<div class="venue" style="font-size: 24px; display: block; font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif; font-weight: 300; color: #404040; text-align: center;">
  <strong>Philadelphia, 26 February 2025, 2–6 PM EST, Room 116</strong>
</div>

<div class="venue" style="font-size: 23px; display: block; font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif; font-weight: 300; color: #404040; text-align: center;">
  <a target="_blank" href="https://drive.google.com/drive/folders/1FIUAsEoTWQ6ntrUaEaO95rZMvMUsJNrU?usp=sharing">[Slides] 
 href="https://aaai.org/conference/aaai/aaai-25/tutorial-and-lab-list/#TH26">[AAAI 2025 website]</a>
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


# Schedule

<div class="container" style="margin-top: 15px; text-align: center;">
  <table style="width: 100%; max-width: 1050px; margin: auto; border-collapse: collapse; font-size: 17px; line-height: 1.5;">
    <tr style="font-weight: bold;">
      <th style="padding: 10px; text-align: left; width: 12%;">Time</th>
      <th style="padding: 10px; text-align: left; width: 58%;">Session</th>
      <th style="padding: 10px; text-align: left; width: 30%;">Presenters</th>
    </tr>
    <tr>
      <td style="padding: 10px;">14:00 - 14:15</td>
      <td style="padding: 10px;">Introduction and Motivation</td>
      <td style="padding: 10px;">Chandan Reddy</td>
    </tr>
    <tr>
      <td style="padding: 10px;">14:15 - 15:15</td>
      <td style="padding: 10px;">Symbolic Regression Foundation and Evolution </td>
      <td style="padding: 10px;">Sanjay Chawla</td>
    </tr>
    <tr>
      <td style="padding: 10px;">15:15 - 16:15</td>
      <td style="padding: 10px;">Modern AI-guided Equation Discovery (Evolutionary Search, Reinforcement Learning, Deep Learning, Transformers, and LLMs) </td>
      <td style="padding: 10px;">Parshin Shojaee</td>
    </tr>
    <tr>
      <td style="padding: 10px;">16:15 - 16:45</td>
      <td colspan="2" style="padding: 10px; font-style: italic; text-align: center;">Coffee Break</td>
    </tr>
    <tr>
      <td style="padding: 10px;">16:45 - 17:45</td>
      <td style="padding: 10px;">Evaluation and Benchmarking + Applications and Use Cases</td>
      <td style="padding: 10px;">Parshin Shojaee</td>
    </tr>
    <tr>
      <td style="padding: 10px;">17:45 - 18:00</td>
      <td style="padding: 10px;">Conclusion</td>
      <td style="padding: 10px;">Chandan Reddy</td>
    </tr>
  </table>
</div>

<hr>


# Reading List

**Introduction, Motivation, Challenges**:
- [Interpretable scientific discovery with symbolic regression: a review](https://link.springer.com/article/10.1007/s10462-023-10622-0)
- [Interpretable Machine Learning for Science with PySR and SymbolicRegression.jl](https://arxiv.org/abs/2305.01582)
- [Symbolic Regression is NP-hard (TMLR'22)](https://openreview.net/forum?id=LTiaPxqe2e)
  
**Methods**:
- [AI Feynman: A physics-inspired method for symbolic regression (Science Advances)](https://www.science.org/doi/10.1126/sciadv.aay2631) 
- [Deep symbolic regression: Recovering mathematical expressions from data via risk-seeking policy gradients (ICLR'21)](https://openreview.net/forum?id=m5Qsh0kBQG)
- [Neural Symbolic Regression that scales (ICML'21)](https://proceedings.mlr.press/v139/biggio21a.html)
- [End-to-end Symbolic Regression with Transformers (NeurIPS'22)](https://proceedings.neurips.cc/paper_files/paper/2022/hash/42eb37cdbefd7abae0835f4b67548c39-Abstract-Conference.html)
- [A Unified Framework for Deep Symbolic Regression (NeurIPS'22)](https://proceedings.neurips.cc/paper_files/paper/2022/hash/dbca58f35bddc6e4003b2dd80e42f838-Abstract-Conference.html)
- [Transformer-based Planning for Symbolic Regression (NeurIPS'23)](https://proceedings.neurips.cc/paper_files/paper/2023/hash/8ffb4e3118280a66b192b6f06e0e2596-Abstract-Conference.html)
- [SNIP: Bridging Mathematical Symbolic and Numeric Realms with Unified Pre-training (ICLR'24)](https://openreview.net/forum?id=KZSEgJGPxu)
- [In-Context Symbolic Regression: Leveraging Large Language Models for Function Discovery (ACL'24)](https://aclanthology.org/2024.acl-srw.49/)
- [LLM-SR: Scientific Equation Discovery via Programming with Large Language Models (ICLR'25)](https://openreview.net/forum?id=m2nmp8P5in)

**Benchmarks**:
- [Contemporary Symbolic Regression Methods and their Relative Performance (NeurIPS'21)](https://datasets-benchmarks-proceedings.neurips.cc/paper/2021/hash/c0c7c76d30bd3dcaefc96f40275bdc0a-Abstract-round1.html)
- [Rethinking Symbolic Regression Datasets and Benchmarks for Scientific Discovery (DMLR'24)](https://openreview.net/forum?id=i2e2wqt0nAI)

**Applications and Use Cases**:
- [Material Science](https://www.cambridge.org/core/journals/mrs-communications/article/symbolic-regression-in-materials-science/A5836F4AF5E9395A9B27541C5042A7F3)
- [Wind Speed Forecasting](https://arxiv.org/pdf/2102.10570?utm_source=chatgpt.com)
- [Behavioral Science](https://www.frontiersin.org/journals/artificial-intelligence/articles/10.3389/frai.2023.1039438/full?utm_source=chatgpt.com)
- [Clinical Models](https://www.nature.com/articles/s41746-023-00833-8)
- [Economics](https://www.tandfonline.com/doi/abs/10.1080/13504851.2016.1218419)



Contact: <ckreddy@vt.edu>.
