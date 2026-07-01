---
layout: post
title:  "On a neat PDE"
date:   2026-06-14 1:48:23 +0900
categories: math research
---
I'm currently doing some research on the PDE $u_t - u_{xx} = u/|u|^2$ where $u \colon \mathbb R \to \mathbb R^2$. This arises from physical scenarios, whatever. The interesting bit comes when we look at stationary solutions. These are solutions for which $u_t \equiv 0$ or in other words $u_{xx} = -u/|u|^2$. This sort of ODE will arise in physical contexts and is well studied because it is a prototypical example of a system in classical mechanics (if you replace the 2 with a 3 you get gravity).

Since our ODE looks somewhat like gravity, it is not surprising that the orbits will look somewhat like orbits in gravity do. Except instead of always being elliptical they will precess. If you've read Arnold's classical mechanics, then you know that as the ODE energy of solutions tends towards the energy of the circular orbit, the angle of precession (the angle between subsequent maxima/minima of our orbit's radius) will approach $\pi \sqrt 2$ and as it goes to $\infty$ it will approach $\pi$. Thanks to [a wonderful paper by David Rojas](https://arxiv.org/abs/1710.08133v2), we know that furthermore the angle of precession is monotone. So therefore any periodic orbit other than the helix cannot have a nonzero winding number (for it to have such, the angle of precession would have to be $\pi / n$ for some $n \in \mathbb N$, which is impossible).

This might not sound like a big deal, but think about what it means practically. If you have periodic initial conditions to your ODE whose winding number (per period) is 1, then the only possible stationary solution is helices. Through some further classical mechanics we can deduce that there's only one suitable radius for a stationary helix of that period and winding number 1. Using a theorem I proved that the &ldquo;only&rdquo; &ldquo;approximately&rdquo; stationary initial conditions are &ldquo;close&rdquo; to the helix, we gain more insight further, giving us lots of information. This research has been fun, and I feel like I've managed to garner a lot of insight from relatively elementary observations. Things just coincidentally work out to be really nice, and the only thing that stands in my way of more impressive results right now is
1. knowing what i should try to prove
2. putting in the elbow grease
