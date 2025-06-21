# ReinforcementLearning
This repo will contain scripts and notebooks in which I explore and implement common RL algorithms on agents operating in Gym enviroments

Tabular_SARSA: got a tabular SARSA implementation working (kind of) on the Mountain Car environment

Tabular_QLearning: implemented a Vanilla tabular version of Q-Learning on the Acrobat environment; works relatively well

Function_Approximation_SARSA: implemented SARSA with function approximation on the Mountain Car environment. The function I used was a linear function and the state-action pairs were transformed into features using tile coding.

REINFORCE_with_Function-Approximated_Baseline: implemented the REINFORCE algorithm with a baseline. The baseline estimates the state value function using a linear function. The policy is structured as a neural network. The environment I used to test the algorithm was the CartPole environment. After training, the average reward over 50 episodes was 488 from a max of 500.
