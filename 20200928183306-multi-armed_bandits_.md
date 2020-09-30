---
title: Multi-Armed Bandits
date: 2020-09-28 18:33
tags: :armed-bandits:example:reinforcement-learning:action-value:
type: note
---

# Multi-Armed Bandits  #

* A multi-armed bandits is a problem in RL that widely used as example:
    - The problem is: A algorithm has to choose a one arm at step *t* and this arm will return a reward regarding
      this selection. The numerical reward chosen from a stationary probability distribution that depends on the action
      algorithm selected.
    - The objective is to maximize the expected total reward over some time period.
* Variation:
    - K-armed, with K possible arms
    - Action selected on time step *t* as $A_{t}$, and the corresponding reward as $R_{t}$.
    - $q_{*}(a) = \mathop{\mathbb{E}}[R_{t}|A_{t}= a]$  <-  Optimum Solution
    - Estimate value of action *a* at time step *t*  as $Q_{t}(a)$. We would like $Q_{t}(a)$ to be close to $q_{*}(a)$.
* [Exploration and Exploitation.](20200928183439-exploration_and_exploitation.md)
    - Greedy and non-greedy actions
    - Exploration: It happens when use *non-greedy* actions. In another word, non-optimum actions with the highest *value(reward)*
    - Exploitation: Algorithm uses the highest action's *value(reward)*.
    - Balance between exploration and exploitation
* First model:
    * [ Action-Value Methods](20200928190836-action-value_methods.md)
* Incremental variation:
    * [Value-Method Incremental Implementation](20200929172744-value-method_incremental_implementation.md)





Backlink: [Reinforcement Learning](20200924161528-reinforcement_learning_.md)
----
