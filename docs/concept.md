Concepts
=========


What is happening here
----------------------

The [Unity_template_for_RL_environments](https://github.com/TransferLearningInBrainsAndAgents/Unity_template_for_RL_environments)
repository is designed to be two things at once. 

First it is a Unity project that creates a few environments that a Reinforcement Learning (RL) agent can interact with.
More on those in the Specific Examples page.
Secondly, it is a project that acts as baseline code from which one can built their own, bespoke, 3D, RL environments.


Although the idea is very similar to Unity's own [ml-agents](https://github.com/Unity-Technologies/ml-agents), this
project is build with a very different premise. The Unity_template_for_RL_environments is meant to build only an RL
environment without embedding in it the code that represents the agent learning the environment. It, on the other hand,
allows for easy communication between the process that is the Unity game (environment) and whatever process the agent 
is running in (probably a Python one using some common ML or RL framework). The project also offers some example python
code showing how an agent running in Python would interact with the environment.

Basic requirements
------------------
The project was born out of two requirements (see frustrations). One was the need, to create RL environments with 3D 
graphics, audio, physics and relatively complex logic in the interactions between the agents and the environmental 
components, without having to rely on other people's specific implementations 
(like [DeepMind's Lab](https://github.com/deepmind/lab)). So having the freedom the opengym (currently 
[Gymnasium](https://github.com/Farama-Foundation/Gymnasium)) is 
offering through its environment building API, but for environments a bit more nuanced than Lunar Lander. 
Obviously Unity was the go-to software for building such environments (which can also be thought of as rather simple
first person games).

The second requirement was the need to develop the agent totally separate of the environment, using a code base suited 
for the task. That meant that the agent should not only utilise the most used (i.e. trendy) methods in the field but 
should allow the use of any method the developer requires, especially new, experimental ones (just like the Gymnasium 
environments are just environments and do not force upon the  developer a pre-specified number of methodologies). 
This is the main reason Unity's ml-agents work was not good enough. 
