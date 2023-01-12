# Unity_template_for_RL_environments

A Unity game that has the basic code with which to build Reinforcement Learning (RL) environments.

For a full explanation on what the game is about, and how to use the code as a template to create different RL environments within Unity [read the docs ](https://unity-template-for-rl-environments.readthedocs.io/en/latest/).

For a summary keep reading.


This repository is designed to be two things at once. 

First it is a Unity project that creates a few environments that an (RL) agent can interact with.
Secondly, it is a project that acts as baseline code from which one can built their own, bespoke, 3D, RL environments.


Although the idea is very similar to Unity's own [ml-agents](https://github.com/Unity-Technologies/ml-agents), this
project is build with a very different premise. The Unity_template_for_RL_environments is meant to build only an RL
environment without embedding in it the code that represents the agent learning the environment. It, on the other hand,
allows for easy communication between the process that is the Unity game (environment) and whatever process the agent 
is running in (probably a Python one using some common ML or RL framework). The project also offers some example python
code showing how an agent running in Python would interact with the environment.
