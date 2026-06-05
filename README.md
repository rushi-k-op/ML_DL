# Reinforcement Learning & Deep Learning — Self-Study Project

A structured learning notebook built during my internship at TU Dortmund,
exploring Reinforcement Learning from mathematical foundations to a working
Deep Q-Network implementation.

## What this covers

The notebook follows a progressive structure, where each chapter builds on the last:

1. **MDP Framework** — Formalising the RL problem using the MDP tuple, applied to CartPole
2. **Value Functions & Bellman Equation** — Defining Q-values and the optimality equation; baseline random agent
3. **Tabular Q-Learning** — TD learning on a discretised state space; observing why it fails on continuous problems
4. **Deep Q-Networks (DQN)** — Neural function approximation, Experience Replay, and Target Networks
5. **Training & Results** — Full DQN training loop with Double DQN, gradient clipping, and reward shaping

## Environment

- **Task:** CartPole-v1 (OpenAI Gymnasium)
- **Goal:** Keep a pole balanced on a cart for 500 consecutive steps

## Key results

| Method | Avg reward | Notes |
|---|---|---|
| Random agent | ~15 | No learning |
| Tabular Q-Learning | Unstable | Discretisation loses precision |
| DQN (improved) | ~224 at ep 400 | Still converging |

## Stack

Python · PyTorch · Gymnasium · Matplotlib · Google Colab
