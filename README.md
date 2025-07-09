# ReinforcementLearning
This repo will contain scripts and notebooks in which I explore and implement common RL algorithms on agents operating in Gym enviroments

Tabular_SARSA: got a tabular SARSA implementation working (kind of) on the Mountain Car environment

Tabular_QLearning: implemented a Vanilla tabular version of Q-Learning on the Acrobat environment; works relatively well

Function_Approximation_SARSA: implemented SARSA with function approximation on the Mountain Car environment. The function I used was a linear function and the state-action pairs were transformed into features using tile coding.

REINFORCE_with_Function-Approximated_Baseline: implemented the REINFORCE algorithm with a baseline. The baseline estimates the state value function using a linear function. The policy is structured as a neural network. The environment I used to test the algorithm was the CartPole environment. After training, the average reward over 50 episodes was 488 from a max of 500.

PPO: implelmented the Proximal Policy Optimization algorithm on the BlackJack env

Unsloth_Qwen2_5_(3B)_GRPO: In this notebook, I followed Unsloth's tutorial of fine tuning a base LLM with GRPO using the GSM8K dataset; 1 custom tweak I made is that I added a reward function that gives a .001 reward for each character in between the reasoning tags up to a maximum of 100. The rationale behind this was to incentivize longer reasoning chains of thought. In hindsight, I could have increeased the maximum quite a bit because 100 characters is not much. It was pretty interesting to see that after the default of 250 training steps that the model was pushed to reason even though in the example that was run the answer is still wrong. Also, I don't know why the notebook is not rendering properly in GitHub. 

LlamaGym_BlackJack: will be using LlamaGym library and their scaffold code to fine-tune (context is Blackjack) an LLM locally with PPO
