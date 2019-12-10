---
layout: post
title: Spherical navigation, part 6
---
I finally solved the puzzle.
My calculations were right, however they had to be put in the `_integrate_forces` callback of the `RigidBody`.
Otherwise, the physics engine interprets them as teleports and gets confused.
Also I added a jump command, and used it to jump from planet to planet.

{% include youtube-player.html id="3Zp110MU3aA" %}
