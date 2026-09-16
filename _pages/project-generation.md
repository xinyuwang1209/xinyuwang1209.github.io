---
layout: prose
title: Scaling generation beyond a single inference loop
kicker: ML systems / Distributed generation
permalink: /projects/generation/
intro: Decoupling generation, scoring, and evaluation so a large molecular search does not have to run as one synchronous loop.
---
<div class="result-band"><strong>1B+ candidate samples</strong><p>Processed in six days using an asynchronous multi-GPU generation and evaluation pipeline.</p></div>

## The problem

Structured generation is more than repeatedly calling a model. Candidate sequences must also be scored and evaluated. Coupling all of those stages tightly makes it harder to scale the workflow and manage work across devices.

## My contribution

I built an asynchronous pipeline that separates **generation, token-level scoring, and evaluation**. The workflow supports distributed candidate processing rather than forcing every stage to wait inside a single inference loop.

<ol class="steps"><li>Generate candidates</li><li>Score token choices</li><li>Evaluate candidate outputs</li></ol>

## Scale, with context

The pipeline processed **more than one billion molecular candidate samples in six days on eight V100 GPUs**. This is a count of generated candidate samples, including repeated outputs.

Separating these stages made generation, scoring, and evaluation independently schedulable across the distributed workflow.

## Related modeling work

I also work on structure-aware decoding: checking molecular structure during generation and using reinforcement learning to correct token choices. That method reduced distribution error by **4.8%**, while preserving **99.5% valid outputs and 100% uniqueness over 10,000 samples**.

[Explore representation learning](/projects/representations/) · [Back to selected work](/projects/)
