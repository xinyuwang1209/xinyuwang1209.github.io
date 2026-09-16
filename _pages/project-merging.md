---
layout: prose
title: Improving merged models without retraining
kicker: Foundation models / DIAL
permalink: /projects/model-merging/
intro: A training-free method that diagnoses unreliable layers and changes how model updates are combined.
---
<div class="result-band"><strong>77.6% → 82.3%</strong><p>ViT-B/16 average accuracy over the TIES merging baseline, without task examples or merge-time validation search.</p></div>

## The problem

Combining task-specific models can reuse learned capabilities without running another full training cycle. But different layers do not necessarily tolerate the same merging strength. One uniform or linear scaling rule can miss those differences.

## My contribution

I developed **DIAL**, a method that uses rank and interference diagnostics to identify unreliable layers and reweight their updates. Instead of imposing one linear rule across the network, I designed piecewise layer scaling.

<ol class="steps"><li>Inspect model updates</li><li>Diagnose layer reliability</li><li>Rescale and merge</li></ol>

## What changed

- Raised ViT-B/16 average accuracy by **4.7 percentage points** over the TIES baseline.
- Outperformed optimized linear schedules in **14 of 15 model-merger settings**.
- Extended the evaluation from vision models to **GPT-2 and Flan-T5 across seven NLP tasks**.

The central contribution is a better merging rule—not another round of fine-tuning or validation-driven parameter search.

## Paper

**Beyond Linear Depth Scaling: Diagnosing Piecewise Layer Reliability for Data-Free Model Merging (DIAL)**
X. Wang, K. Deng, F. Dou, J. Bi, J. Lu.
Submitted to NeurIPS 2026.

[All publications](/publications/) · [Back to selected work](/projects/)
