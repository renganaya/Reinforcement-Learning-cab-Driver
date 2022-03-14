# Reinforcement-Learning-cab-Driver

The goal of the project is to build an RL-based algorithm which can help the cab drivers to maximise their profits by improving their decision-making process on the field.

Problem Statement:

The need for choosing the “Right “requests most drivers get a healthy number of ride requests from customers throughout the day. But with the recent hikes in electricity prices (all cabs are electric), many drivers complain that although their revenues are gradually increasing, their profits are almost flat. Thus,it is important that drivers choose the “Right”rides.

i.e.choose the rides which are likely to maximise the total profit earned by the driver that day.

In this project, Env.py is to create the environment and RL agent that learns to choose the best request. Env.py is a “environment class-each method (function)of the class has a specific purpose.

RL agent learns to pick the best request using DQN. The model has been trained with the hyperparameter (Epsilon (decay rate), Learning rate, discount factor etc.) Training depends purely on the epsilon-function. If the decay fast, it will not let the model explore much and Q-values converge early but to suboptimal values. If the decay slowly, the model converges slowly.

In the Agent file, we’ve provided the code skeleton. Using this structure is not necessary though.

   You have to submit your final DQN model as a pickle file as well.
Convergence- You need to converge your results. The Q-values may be suboptimal since the agent won't be able to explore much in 5-6 hours of simulation. But it is important that your Q-values converge.

There are two ways to check the convergence of the DQN model:

Sample a few state-action pairs and plot their Q-values along episodes

Check whether the total rewards earned per episode are showing stability

  Showing one of these convergence plots will suffice.
Important points to consider while training:

Choose ? -decay function carefully. Make sure that the decay rate allows the agent to explore the state space maximally at the start, and then to settle down to a fixed exploration rate (the results will converge as soon as e becomes 0, though results may not be optimal if the agent doesn’t explore much).

List down all the metrics (such as total rewards for n episodes, loss values, q-values, etc.) you want to track for checking the convergence and save them after every few episodes. It is recommended that you store and check your results after every ~1000 episodes.

Don’t forget to save your model (weights) after every few iterations.

Make sure to debug your code before running for a large number of episodes. Run for 3-4 steps in an episode, and check whether the reward, next state computations etc. are correct. Only when the code is debugged, run it for a larger number of episodes.

For a Windows 64-bit system, and with an 8GB RAM, it takes around 1 hour to train for 1000 episodes with the average length of episodes 100.

About
No description, website, or topics provided.
Resources
 Readme
Stars
 0 stars
Watchers
 1 watching
Forks
 0 forks
Releases
No releases published
Packages
No packages published
Languages
Jupyter Notebook
89.9%
 
Python
10.1%
© 2022 GitHub, Inc.
Terms
Privacy
Security
Status
Docs
