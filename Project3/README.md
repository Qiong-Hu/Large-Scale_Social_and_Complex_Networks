# Project 3: Reinforcement Learning (RL) and Inverse Reinforcement Learning (IRL) 

Main code: [Jupyter notebook](project3.ipynb)

Full report: [report.pdf](project3_report.pdf)

Coding language: Python

Python package used in implementation: numpy, matplotlib

<br>

## Objectives

In this project, we will implement the value iteration algorithm to learn the optimal policy of an agent navigating in a 2D environment. We will also explore the application of Inverse Reinforcement Learning (IRL) to extract an expert's reward function by observing the optimal policy of the expert.

## Instructions

### Reinforcement Learning (RL)

1. Model the environment of the agent by Markov Decision Process (MDP), by setting up the state-space, action set, transition probabilities, discount factor, and reward function.

    <img src="img/Q1-1.png" width="40%"> <img src="img/Q1-2.png" width="40%">

    Visualization of reward function in two layouts.

2. Implement the initialization and estimation steps of the value iteration algorithm.

    <img src="img/Q3.png" width="40%"> <img src="img/Q7.png" width="40%">

    <img src="img/Q9-heatmap_RF1_w0.6.png" width="40%"> <img src="img/Q9-heatmap_RF2_w0.6.png" width="40%">

    Visualization of optimal state values when action error probablity ![omega=0.1](https://render.githubusercontent.com/render/math?math=\omega=0.1) and ![omega=0.6](https://render.githubusercontent.com/render/math?math=\omega=0.6).

### Inverse Reinforcement Learning (IRL)

1. Implement the IRL algorithm using Linear Programming (LP) formulation.

    (Left to right: ground truth reward function, extracted reward function using IRL, optimal state value from the extracted reward function)

    <img src="img/Q13_ground_truth_RF1.png" width="30%"> <img src="img/Q13_extracted_reward_RF1.png" width="30%"> <img src="img/Q14_opt_value_extracted_RF1.png" width="30%">

    <img src="img/Q20_ground_truth_RF2.png" width="30%"> <img src="img/Q20_extracted_reward_RF2.png" width="30%"> <img src="img/Q21_opt_value_extracted_RF2.png" width="30%">

2. Evaluate the performance of IRL algorithm by comparing the extracted reward function and the ground truth reward function, and calculate the accuracy of optimal policy map.

    <img src="img/Q17_policy_cmp_RF1.png" width="40%"> <img src="img/Q24_policy_cmp_RF2.png" width="40%">

    Comparison of optimal policy map.

    The accuracy in both circumstances are 92%. After changing a set of parameters, the highest accuracy can reach up to 97%.

<br>

Full report see: [report.pdf](project3_report.pdf)
