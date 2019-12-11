---
layout: post
title: Ground detection on jump
---
I tried to add ground detection via an `Area`.
However as I had first thought of using a `RayCast` for it, and `RayCast`'s API is very easy to understand, I preferred it to `Area`.

`RayCast` just checks the collision of a segment determined by the origin of its transform, and an arbitrary `Vector3` with other colliders and areas.

{% include youtube-player.html id="doBL197cqfU" %}
