---
title: Reinforcement Learning 
date: 2020-09-24 16:15
tags: :reinforcement-learning:literature-note:introduction:book:
type: note
---

# Reinforcement Learning  # 

* The idea behind reinforcement learning is learning by interacting with the environment
* The agent interact with the environment causing and effect(Consequences of actions). (Cause and Effect)
* The objective of the agent is to maximize a numerical reward signal
    - Reward signal: It can be discrete or continuous 
    - Must discover with actions yield the most reward by trying each of them 
        * Some actions affects not only the immediate reward but also the next subsequents rewards (**Value Function**)
* Trial-and-Error search and delayed reward are the most important features of reinforcement learning methods 
* Incompletely-known *Markov Decision Process*
    - Markov decision process has three main aspects: sensation, action, and goal
* Challenges:
    - Trade-off between exploration and exploitation. 
        * The agent must explore different actions to see what are better ones for each state
        * In the same time, the agent must use the most effective action that it has tried in the past and producing a
          substantive amount of the reward
        * "The agent has to *exploit* what it has already experienced in order to obtain reward, but it also has to
          *explore* in order to make better action selections in the future." Sutton, Page 3 
* Reinforcement learning is the closest to the kind of learning that humans and animals do. It is inspired by biological
  learning systems that arise from experience with the environment. 
* Reinforcement learning use simpler fewer general principles of artificial intelligence: Learning, Search and Decision
  Making. This kind of principles were one time characterized as "weak methods", and specific knowledge as  "strong
  methods". However, today this view is changing with the new methods.
* The agent requires taking into account indirect, delayed consequences of actions, and thus may require *foresight* and
  *planning* 
* Elements of Reinforcement Learning:
    - Agent: Take actions regarding environment's state 
    - Environment: The world who the agent will interact 
    - Policy: How the agent interact with the environment at a given time. It is mapping state to a possible
      set of actions. 
    - Reward signal: A single number evaluating how good a specific taken action in a specific state at given time.
    - Value: "The value of a state is the total amount of reward an agent can expect to accumulate over the future,
      starting from that state." Sutton, Page 6
        * A specific state might yields a low immediate reward but still have a high value because it is regularly
          followed by other states  that yield high rewards. Or the reverse could be true. (*Farsighted judgment*)
        * The agent seeks actions that bring about states of highest value, not highest reward.
    - Model: Mimics the behavior of the environment, or more generally, allows inferences to be made about how the
      environment will behave.

* A state represents totally or partially an environment. Most of the times, partially is used as representation. 
* "Genetic algorithms, genetic programming, simulate annealing, and other optimization methods never estimate value
  functions." Sutton, Page 7
    - Random fixed polices are generated and evaluated over time. The best ones are carried over to the next generation
      of policies and the process repeats. 
        * They do not learning during their individual lifetimes. 
        * If the space of policies is sufficiently small, or can be structured so that good policies are common or easy to
          find - or if a lot of time is available for the search, then evolutionary methods can be effective. 
* Classical optimization methods for sequential decision problems, such as dynamic programming, can *compute* an optimal
  solution for any problem, but require as input a complete specification of that problem.
* $V(S_{t}) \leftarrow V(S_{t}) + \alpha \left[V(S_{t+1}) - V(S_{t}) \right]$
    - This update rule is an example of *temporal-difference* learning methods, so called its changes are based on a
      difference, $V(S_{t+1}) - V(S_{t})$, between estimates  at two successive times.
* Learning a value function takes advantages of information available during the course of actions.
* A good agent will interact well with the environment rely on its capabilities to generalize from past experiences. 


Backlink: 
----
