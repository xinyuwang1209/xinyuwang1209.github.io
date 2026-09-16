---
layout: prose
title: Helping language agents make better decisions
kicker: Language agents / Learning
permalink: /projects/agents/
intro: Learning from the situations an agent actually encounters, not just the examples collected before it starts.
---
<div class="result-band"><strong>56.1% → 78.1%</strong><p>Pass rate on 114 telecom tasks: a 22 percentage-point improvement.</p></div>

## The problem

An agent’s early choices change what it encounters later. Training only on an offline collection of states can leave gaps precisely where the deployed policy needs to make its next decision.

## My contribution

I built replay-based action scorers that learn from states reached by the language agent. The aim is to improve action selection by using experience from the agent’s own trajectory, rather than assuming that a fixed dataset covers every relevant situation.

<ol class="steps"><li>Collect reached states</li><li>Learn action scores from replay</li><li>Evaluate task completion</li></ol>

The telecom evaluation improved pass rate from **56.1% to 78.1% across 114 tasks**. These are benchmark results, not a claim about customer-facing deployment.

## Related direction: agent safety

My broader work also examines when tool-using agents should verify, act, delegate, or escalate. This includes a guard framework for coding agents that checks routes, provenance, and capabilities before high-risk actions.

The connecting question is practical: how do we improve completion while keeping the agent’s actions within the intended boundaries?

[Back to selected work](/projects/)
