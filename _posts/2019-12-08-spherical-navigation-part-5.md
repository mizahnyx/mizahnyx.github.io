---
layout: post
title: Spherical navigation, part 5
---
Just after yesterday's development session, I noticed quite often the game got stuck.
It puzzled me, so I started trying to pinpoint the problem.
Seems that setting the basis of the transform of a a rigid body somewhat isn't a good practice.
Because the physics engine interprets that as a teleport and doesn't know what to do with it.

This is me, stumbling against the intricacies of Godot3D's physics engine.

{% include youtube-player.html id="tY1NvwvGmN4" %}
