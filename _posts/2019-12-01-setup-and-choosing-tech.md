---
layout: post
title: Initial setup, and choosing technology
---
> I, Mizahnyx, will participate to the next Devember.
> My Devember will be the development of an anime game.
> I promise I will program for my Devember for at least an hour, every day of the next December. 
> I will also write a daily public devlog and will make the produced code publicly available on the internet. 
> No matter what, I will keep my promise.

[This will be my public repository](https://github.com/mizahnyx/mizahnyx-devember-2019)

Feel free to take anything you want.

I would like to create an anime fighting game, inspired by mecha armors and fanservice.

To cut corners, I'll use premade tools that generate publicly available anime models, in this case, [VRoid Studio](https://vroid.com/en/studio) created by Pixiv. 
Today the latest version of VRoid Studio is Beta 0.7.5, which I will use, for Windows 64-bit.
It probably can run also on Wine on a Linux distribution, but I haven't tried it yet.

![VRoid Studio Beta 0.7.5 screenshot](/assets/img/2019-12-01-vroid-studio.png)

Also to create extra shapes needed for it I'll use latest [Blender3D](https://www.blender.org/). Current version is 2.81.

![Blender 2.81 screenshot](/assets/img/2019-12-01-blender.png)

For engine, I will use [Godot 3D nightly builds](https://hugo.pro/projects/godot-builds/) specially now that it has WebRTC peer to peer capabilities.
That, in theory, can allow me to create an entirely distributed multiplayer experience.

![Godot nightly version screenshot](/assets/img/2019-12-01-godot-nightly.png)

# Inspiration

My inspiration comes mainly from 3 anime / mecha / fanservice games that I played and liked a lot.

- SEGA's Cyber Troopers Virtual On, specially Operation Moongate
- CyberStep's Cosmic Break
- gumi's Dolls Order

Fanservice-mecha animes like Infinite Stratos or Date a Live also are influences for what I want to accomplish.

## Cyber Troopers Virtual On

Originally I knew this game as an arcade at Centro Coyoacan at Mexico City at the end of last century.
The control was unusual, because it used dual sticks, each stick with a frontal trigger and an upper hat button.
Triggers activated the weapons, hat button was used to dash.
Differential or coordinated movement of the sticks allowed to move, aim-jump and crouch-guard.

{% include youtube-player.html id="S1BwvEx7-Z8" %}

## Cosmic Break

Cosmic Break is a massively multiplayer third person shooter with extreme customization of a series of robotic and humanoid characters. 
Such characters are comprised of fixed and interchangeable parts and weapons, that can be tuned to enhance stats.
There are also chareacter classes, namely:

- LND (land), excelling on terrestial mobility, weak to beam weaponry, strong against long range artillery
- AIR (aerial), excelling on aerial movement, weak to explosives and artillery, strong against land characters
- ART (artillery), excelling on long range and antiaerial attack, weak against melee, strong against flying characters
- SUP (support), healers and buffers
- ZERO (zero), a new category that has branching paths of leveling and are generally overpowered

The PvP arena gameplay is frantic. Characters can move, dash (there are different dash "cartridges" that allow different types of dashing), jump, fly consuming boost gauge, use ranged and melee weapons, or even fire all their ranged weapons at once (alpha striking).
When the power bar is full, a special ability can be deployed in the form of a "bit", kind of a helper drone, that can be a shield, a guided missile launcher, etc.
Some characters have a fixed "bit".
Support characters can equip healing bits.

{% include youtube-player.html id="dcZskn3F4oU" %}

## Dolls Order

Dolls Order is a mobile massively multiplayer third person fighting game that pits humanoid AIs with different weapon sets against each other in 2v2 arena fights.
Its service just ended at November 29.
The game had very good voice acting and even original j-pop music.
The gameplay had movement, dash, switching target and a series of special attacks plus a power bar that when full can unleash a devastating ultimate attack.

{% include youtube-player.html id="qkXX4dEPtLk" %}

In the next entry, I will try to create a cube on Godot Engine and give it basic WASD movement over a plane.
