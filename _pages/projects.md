---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

These selected projects highlight the work most relevant to AI/ML research internships, applied scientist roles, and research engineering.

## LLM Agents, Agentic Control, and Safety

**Problem:** Long-horizon language agents need to decide when to ask, delegate, verify, act, or escalate, while avoiding unsafe or unauthorized actions.

**What I built:** Learning and evaluation methods for agentic control, plus a benchmark and guard framework for tool-using coding agents. The framework checks route, provenance, and capability before high-risk actions.

**Impact:** Improved audited-seed success from 6.2% to 37.8%, utility from -0.237 to 1.051, and decision regret from 0.323 to 0.109. Strong safe-family evaluations reached 6/6 task success with zero unauthorized effects and zero route misfires.

**Keywords:** LLM agents, agentic AI, safety, tool use, coding agents, evaluation, counterfactual action values.

Related engineering note: [Codex memory-fix fork](/notes/#codex-memory-fix-fork), a small Rust systems patch for large local coding-agent session files.

## Data-Free Foundation Model Adaptation

**Problem:** Model merging and adaptation methods often need task data, training, test-time tuning, or recipe-specific assumptions.

**What I built:** A data-free performance enhancer for model merging that can be applied on top of broadly used task-vector-style merging methods rather than a single merge recipe.

**Impact:** Improved average benchmark performance to 86.1 across 7 NLP tasks and 8 vision tasks without training, task data, or test-time tuning.

**Keywords:** foundation models, model merging, data-free adaptation, evaluation, NLP, vision.

## Structure-Aware Decoding and Large-Scale Search

**Problem:** Autoregressive sequence models can produce repeated outputs and hidden structural collapse in constrained generation settings.

**What I built:** Structure-aware decoding and search methods, plus a distributed asynchronous generation and evaluation framework with token-level value prediction and human-in-the-loop steering.

**Impact:** Scaled candidate generation to 1B+ samples in 6 days on 8 V100 GPUs, enabling broader exploration over large structured candidate spaces.

**Keywords:** sequence modeling, decoding, search, autoregressive models, distributed evaluation, GPU pipelines.

## Applied ML for Health and Scientific Discovery

**Problem:** Health and scientific domains require models that can integrate heterogeneous signals and support downstream prediction or candidate selection.

**What I built:** Multi-view representation learning models for MRI and multimodal health data, sequence-modeling and generative methods for structured scientific workflows, and molecular generation methods using hierarchical chemical graph representations.

**Impact:** Contributed to publications in connected health, molecular informatics, biomedical systems modeling, and depression treatment outcome prediction.

**Keywords:** multimodal learning, health AI, drug discovery, molecular generation, representation learning.
