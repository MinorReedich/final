# Project idea: the Big Bang

Particles being sucked into a single point and exploding

## Uniqueness 

This demo will be unique from existing demos of explosions in that it 
will implode to a single point before exploding. This will not 
be a static object exploding, as in many existing demos, but rather particles 
coming together in order to explode. 

Existing demo of the Big Bang, to illustrate this point:

[![Big Bang](https://img.youtube.com/vi/LeUcjqqhNxM/0.jpg)](https://www.youtube.com/watch?v=LeUcjqqhNxM)

## Features

I plan to implement a few features, which I rank as minimum required, 
good-to-have, and stretch in the following way, respectively:

1. Implosion effect (particles being sucked in),
   Singularity point at which particles converge,
   Explosion effect (particles being scattered).

2. Color change (start off with white particles which explode into colorful ones).

3. Texture change (begin with particle texture and end up with planets at the 
   singular point onward).
   
## Implementation details (data structures, algorithms etc...)

I will be using particle systems and billboard shaders to acheive my desired result. 
Some relevant algorithms would be: simple blending particles so they do not appear as 
particles within a square billboard, and checking to see when the singularity occurs in order
to change textures from particles to planets and create diversity of color. Additionally,
randomizing whether the velocities will be positive or negative to "shoot" the particles 
in different directions will be necessary.  

