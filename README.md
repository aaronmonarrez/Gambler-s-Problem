Overview
This project implements the value iteration algorithm to solve the Gambler's Problem, a classic problem in the field of reinforcement learning and dynamic programming. The Gambler's Problem involves a gambler who has the opportunity to make bets on the outcome of a coin flip, aiming to reach a desired amount of capital.

Description
The Gambler's Problem is defined by the following parameters:

S: Set of states ranging from 0 to 100, where states 0 and 100 are terminal states.
V: The value function representing the expected return from each state.
π: The policy determining the optimal action to take in each state.
ph: Probability of heads in a coin flip.
The goal is to find the optimal policy π and the corresponding value function V that maximize the expected return for the gambler.

Implementation
The implementation consists of the following steps:

Initialize parameters: Set discount factor (γ), convergence tolerance (θ), and initialize value function (V) and policy (π).
Iterate until convergence:
For each non-terminal state, calculate the expected return for each possible action (bet amount).
Update the value function and policy based on the maximum expected return.
Check for convergence, break if the change in value function falls below the tolerance threshold.
Return the optimal value function and policy.
Usage
To use this implementation, follow these steps:

Define the parameters:
S: Set of states.
ph: Probability of heads.
Call the value_iteration function with initialized value function (V) and policy (π).
Retrieve the optimal value function (V) and policy (π) for the Gambler's Problem.
