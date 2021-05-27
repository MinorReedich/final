# Final Project: The Big Bang

Explosion of planets 

## How to build

*macOS*

Open terminal to the directory containing this repository.

```
final $ mkdir build
final $ cd build
final/build $ cmake ..
final/build $ make
```

To run the program from build, you would type

```
final/build $ ../bin/confetti
```

## Algorithms etc...

In order to achieve the implosion-singularity-explosion effects, 
I created an explosion of particles, which I did not render, and after some time
(I created a counter and made it run 300 times), I took the negation of 
the velocities of all the particles to simulate a gravitational pull toward the origin. 
(Note: this is the reason for which the first few seconds are a black screen).
After the particles reached the sigularity, I simply allowed them to keep going in the 
same direction (opposite to the initial hidden explosion). This caused the particles 
to explode in other directions than that of which they were pulled in (in fact, the 
opposite direction). 

To test when the particles reached this singular point, I tested to see if the first particle
in mParticles was between -0.001 and 0.001. However, the particles technically starting at the origin
to begin with, I used a boolean change to determine that it was in the implosion stage as well as 
very near to the origin. When this was the case, I changed the texture to planets and randomized the colors 
to represent the diversity in the universe after the Big Bang. 

To cause the particles to explode in different directions, I mulitplied each component of the velocity by 
-1 to the power of a random integer. The result of this was not only randomizing the magnitude of each component, 
but also the direction (positive or negative). 

## Results

![](bb.gif)

As seen in the gif above, all features were implemented.
