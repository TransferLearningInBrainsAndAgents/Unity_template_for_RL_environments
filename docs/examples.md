Specific Examples
=================

The general idea (clever rats playing games)
---------------------------------------------

There are 4 different environments in this project, all based around the same idea but implementing slightly different
logic. 

All environments expect an agent which has a body, a head, and two front paws (a very cartoonish simulation of 
a rodent) which can move forwards and backwards in discrete steps, can rotate clock and anticlock wise again in discrete 
steps and can extend or retract one of its paws at a time. The cartoon rat lives in a rather small cubic arena. The 
arena has one reward port on one wall while the opposite wall has a hole in the middle and two buttons on either side
of the hole. The rat can poke its head but not the rest of its body through the hole. It can also "touch" the buttons 
if it extends a paw and it then overlaps the button.

Behind the wall with the hole there is a green 'screen' onto which appear three straight, equal in length and width 
lines. One is white (the target), one is black (the trap) and one is black and white striped (the manipulandum). 
The target and the trap form a cross while the manipulandum's center touches the crosse's center. 

The game's camera is mounted onto the rat's head producing renderings of the environment from the point of view of the 
agent.

Each one of the four environments implements a different 'task' for the rat to solve:


