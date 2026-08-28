---
layout: page
title: MIRAGE
description: Misalignment and Representation Audit for Global Ethical Simulation
img:
importance: 1
category: research
related_publications: true
---

**MIRAGE** (**Mi**salignment and **R**epresentation **A**udit for **G**lobal **E**thical Simulation) is a cross-national, multi-LLM framework for auditing how faithfully persona-injected large language models represent human ethical values.

The framework couples the [World Values Survey](https://www.worldvaluessurvey.org/) (WVS) Wave 7 with LLM-generated, demographically-stratified personas across 8 countries and 3 LLMs, and measures misalignment along two axes:

- **Directional bias** — a systematic skew of LLM responses toward a particular ethical direction relative to humans.
- **Distributional diversity** — how well LLM responses preserve the spread (not just the mean) of human responses.

This work was published as {% cite choi2026auditing %} at CIKM 2026.

Full statistical results and analysis code are available on GitHub: [mirage-cikm/MIRAGE_Statistical_Full_Results](https://github.com/mirage-cikm/MIRAGE_Statistical_Full_Results).
