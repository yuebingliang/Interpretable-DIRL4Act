# Interpretable-DIRL4Act
This repository provides the code accompanying the paper:
“Analyzing Sequential Activity and Travel Decisions with Interpretable Deep Inverse Reinforcement Learning.”

The framework applies Adversarial Inverse Reinforcement Learning (AIRL) to model daily activity–travel sequences conditioned on individual sociodemographic features. It further introduces interpretable modules that connect the learned deep policy and reward functions to behavioral and demographic insights.

**Repository Structure**
**1. AIRL4Act_model_training_and_evaluation.ipynb**

This notebook provides the code for training an AIRL model that generates daily sequential activity and travel decisions conditioned on individual sociodemographic features.
It also includes evaluation procedures for comparing the generated and real trajectories using quantitative performance metrics.

**2. AIRL4Act_policy_interpretation.ipynb**

This notebook conducts policy interpretation.
It loads a pre-trained AIRL model and trains a surrogate logit model to approximate and interpret the DNN-based policy function learned in AIRL.
This allows users to link model behavior back to traditional discrete choice modeling concepts.

**3. AIRL4Act_reward_interpretation.ipynb**

This notebook focuses on reward interpretation.
It: (1) computes reward sequences for both real and generated activity trajectories, (2) visualizes trajectories and their corresponding reward evolution, (3) clusters individuals into different types of activity planners based on reward patterns, (4) calculates long-term returns for each trajectory, and (5) links the learned reward profiles to individual sociodemographic attributes.
