---
layout: post
title: Spherical navigation, part 4
---
After failure, perseverance can produce success.
I created a global registry of gravity attracting objects, that also allows to query for the nearest.
Also I limited the gravitational attraction of celestial bodies under a specific radius.
After checking that planetary gravity was working, I tried to fix the third person controller.
Figured out what was the error.
It was trying to transform the movement vector with the whole player transform, in practice adding to it the distance from player to origin.
So I transformed it with only the transform basis, to align movement vector with the current player orientation.
To visualize more easily planetary surface movement, I added textures to the planets.
Also, I allowed gamepad input for player movement.

Those are the screen recordings of today.

{% include youtube-player.html id="Qbu-QkaEKeI" %}

{% include youtube-player.html id="4DrwiUVfkkE" %}
