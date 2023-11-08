---
layout: page
title: Quantum time evolution
description: 
img: assets/img/quantum_timeevolve.png
importance: 1
---

This animation shows the dynamics of a quantum particle in a 2D square-well potential. Despite the apparent chaos that quickly ensues, the state soon revives right back to where it started.

To be a little more precise, the initial state is the ground state of a circular well potential near the top-left. It’s as if a particle was sitting in the ground state of the circular well and then the circular well was suddenly “turned off” allowing the particle to enter a 2D square well with walls on the edge of the view.

I generate this animation by solving for the ground state (the lowest energy eigenstate) of the circular well in the 2D box basis. The time-dependent wave function is then simply the superposition of the box basis states with time-dependent phase factors given by the inner product of the initial state with the eigenstates of the 2D box potential. I map from the probability density (modulus squared wave function) to the colors shown in the animation. I use Python here. Numpy to solve the Schrodinger equation and OpenCV to create the video.

<blockquote class="reddit-embed-bq" style="height:500px" data-embed-height="739"><a href="https://www.reddit.com/r/Physics/comments/m2fylo/time_evolution_of_a_quantum_particle_in_a_2d_box/">Time evolution of a quantum particle in a 2D box</a><br> by<a href="https://www.reddit.com/user/hudsmith/">u/hudsmith</a> in<a href="https://www.reddit.com/r/Physics/">Physics</a></blockquote><script async="" src="https://embed.reddit.com/widgets.js" charset="UTF-8"></script>