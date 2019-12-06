---
layout: post
title: Spherical navigation, part 2
---
I tried searching for tutorials on spherical gravity, however majority of them are for Unity3D.
The basic idea is that you:

- Deactivate game engine's downward gravity force
- In every simulation step, for every RigidBody affected by gravity
  - Align the vertical axis of the object towards the planet
  - Apply a radial force of gravity

However I stumbled upon my lack of knowledge on vector map.
What is required for the align is a quaternion rotation over minimum arc.
I knew that the axis of such rotation is the cross product between the vertical normalized axis (Y, in Godot and OpenGL conventions) of the affected object, and the normalized distance from the object to the planet.
I was still unable to complete the rotation.

This is the screen recording of what I did.

{% include youtube-player.html id="wrigG6e801c" %}
