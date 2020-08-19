---
tags: python,numpy,neural-network,reinforcement learning
mathjax: true
---
# Temporal Difference Learning (TD)

- state value or state-action value update after each temporal step (temporal difference)

## The Bellman Equation

- state value V(s) or state-action value Q(s, a) bootstrap equation
- can be understood as a recursive policy evaluation rule to calculate the value of states or state-action values
- can also be adapted to work as a policy optimization rule

## The Q Learning Algorithm

- model free algorithm
- samples reward based on policy and adds maximum Q value of new state, which may not be equal to the Q value related to the action chosen following the current behavior policy
- because of this discrepancy, Q learning is called an off-policy algorithm

## The SARSA Algorithm

- model free algorithm
- similar to Q learning algorithm, but samples reward based on policy and adds policy related Q value of new state
- SARSA algorithms are called on-policy, because the experiance used for learning is aquired following the current policy

## The Expected SARSA Algorithm

- model free algorithm
- same as SARSA algorithm, but in addition, takes action sampling probabilities into account

## The Dyna-Q Algorithm

- model based temporal difference algorithm which uses real and simulated experiance
  - the model implements a (state, action) to (new state, reward) mapping
  - real experiance is sampled from the environment
  - simulated experiance is generated using already collected real experiance
  - both real and simulated experiance are used to optimize the value function and policy of the agent
