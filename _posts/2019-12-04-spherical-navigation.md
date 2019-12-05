---
layout: post
title: Spherical navigation
---

Sorry for the delay in posts and in the dynamics of Devember.
I had some professional and personal issues to take care of.

> A whole world to toy with.
>
> -- Syndra, League of Legends

The MMOTPS Cosmic Break simulates planet curvature with a shader.

![Cosmic Break screenshot showing planet curvature](/assets/img/2019-12-04-cosmic-break.jpg)

This allows long range artillery units to use the horizon as concealment.
I will go one step beyond and make the action take place on a fully spherical planet.

So I started Godot and created an empty project, with GLES2 renderer so it can run on almost any device.

![Godot new project screenshot](/assets/img/2019-12-04-godot-new-project.png)

![Godot project settings](/assets/img/2019-12-04-godot-project-settings.png)

Under the scene's top Spatial node, I create a hierarchy of nodes of the following classes:

- `Spatial` (top scene node)
  - `StaticBody` (with scale `10, 10, 10`)
    - `CollisionShape` (its `Shape` is a `SphereShape`)
    - `MeshInstance` (its `Mesh` is a new `SphereMesh`)
  - `Camera`

![Basic planetary sphere](/assets/img/2019-12-04-godot-planet-sphere.png)

So I will add the player, a `RigidBody` in character mode.
Under it I will create a capsule `CollisionShape` of 1 unit long and 0.5 units radius.
Also, a `MeshInstance` capsule mesh with the same dimensions as the collision shape.
Finally I'll attach the camera to the `RigidBody` and point it to the player capsule.

![Basic capsule player](/assets/img/2019-12-04-godot-capsule-player.png)

Describing in text everything its more cumbersome to me than doing it.
Maybe I should just vlog it all to some video platform and then just link the video.
