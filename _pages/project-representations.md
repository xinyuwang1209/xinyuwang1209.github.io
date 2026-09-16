---
layout: prose
title: Learning representations beyond the surface
kicker: Representation learning / SIGMA
permalink: /projects/representations/
intro: Teaching a sequence model that different strings can describe the same underlying molecule.
---
<div class="result-band"><strong>6 of 6 benchmarks</strong><p>Improved mean performance across six molecular property-prediction benchmarks.</p></div>

## The problem

The same molecule can be written as different valid strings. A sequence model that focuses too heavily on the particular spelling can treat equivalent inputs inconsistently.

## My contribution

I developed **SIGMA**, a token-level training objective that aligns different strings representing the same molecule. The method changes training without adding inference cost.

<ol class="steps"><li>Equivalent molecular strings</li><li>Token-level semantic alignment</li><li>Generation & prediction</li></ol>

## Results

- Reduced generation-distribution error, measured by FCD, by **9.9% and 19.4%** versus the strongest baselines across two QM9 encodings.
- Improved mean prediction performance on **all six molecular benchmarks**.
- Reduced sensitivity to equivalent input strings by **up to 44.9%**.

The experiments are in molecular modeling. The broader research interest is how to learn meaning that remains stable when the representation changes.

## Paper

**SIGMA: Semantic Identifier Grouping for Molecular Autoregression**
X. Wang, F. Dou, J. Bi, M. Song.
Submitted to AAAI 2027.

[arXiv](https://arxiv.org/abs/2603.25062) · [All publications](/publications/)
