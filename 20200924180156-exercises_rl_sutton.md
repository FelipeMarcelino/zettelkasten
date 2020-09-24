---
title: Exercises Sutton
date: 2020-09-24 18:01
tags: :exercises:reinforcement-learning:practice:
type: note
---

# RL Sutton - Exercises # 

## Chapter 1

### Exercise 1 

* It would learn a different policy than playing a fixed opponent since the opponent would also changing its behavior
through the time.
* However, they would not converges to a optimal solution, as both players changing constantly. 

### Exercise 2

* It is possible to update value function(for symmetrical sides) using symmetry of the board and make the agent learn faster as state space is
  smaller.
* No, because in that case the states will be different and the opponent is a part of the environment. Making a state
  symmetric might occasionally leads to suboptimal solution space.

### Exercise 3

* Might have a suboptimal solution, because *greedy* algorithms always leads to suboptimal solution. 
* Only works if the estimate for value function is perfect

### Exercise 4

* If the agent learns only for non-exploratory moves, or in the same words, only from optimal moves, the agent going to
  converge to a winning agent. 
* Using exploratory moves, might occasionally leads to a slow converge and maybe into a training agent that has
  probability to win smaller than the first version cited above. 
* The first one will results in a better policy, since it is the real agent behavior in real game. 

### Exercise 5

* Maybe adding intermediary rewards and not only win and lose reward. 
    - Assuming some actions will lead in a better *value function* 
    - Not sparsity reward, but a dense one
* Testing steps for update. Like, using update in the middle of the game(faster update) or after some games(Better estimate)





Backlink: 
----
