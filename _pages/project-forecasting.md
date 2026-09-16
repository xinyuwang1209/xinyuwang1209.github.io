---
layout: prose
title: Building reliable outage-forecasting workflows
kicker: UConn Outage Prediction Model
permalink: /projects/forecasting/
intro: Making a university-based weather-to-outage workflow faster, more reliable, and easier to operate.
---
<div class="result-band"><strong>≈59% faster processing</strong><p>Development-pipeline improvement through task parallelism and MPI tuning.</p></div>

## The problem

A useful forecast depends on more than prediction accuracy. Inputs must arrive, data must be prepared, forecasts must reach downstream users, and failures must be recoverable without relying on someone to watch every step.

## My contribution

As a **Machine Learning Systems Engineer (Graduate Technician) at the University of Connecticut**, I help develop and maintain an operational weather-to-outage forecasting workflow. My work connects data readiness, feature preparation, model execution, automated delivery, monitoring, and recovery logic.

<ol class="steps"><li>Validate inputs</li><li>Prepare data</li><li>Run forecasting workflow</li><li>Deliver, monitor &amp; recover</li></ol>

## Performance engineering

I accelerated the workflow’s development pipeline through task parallelism and MPI tuning, reducing combined processing time by approximately **59%**, from about **4.5 hours to under two hours**.

This is a development-stage processing comparison, not a claim about production end-to-end latency or a deployed customer-facing service.

## Reliability by design

I implemented readiness checks, duplicate-job protection, retry/resume behavior, monitoring, and alerts so routine data delays or failed jobs can be handled more consistently. I translate requirements from researchers and engineers into changes that make the workflow more dependable during severe-weather events.

[Back to selected work](/projects/)
