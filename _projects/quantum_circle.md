---
layout: page
title: Quantum states
description: 
img: assets/img/quantum.png
importance: 1
---


The image below shows the probability distributions of the first 25 eigenstates of a particle trapped in a circular potential well. These distributions are the squared modulus of the quantum wavefunction $$\psi_n(x,y)$$ which is the solution to the time-independent Schrödinger equation: 

$$
\left(\frac{-1}{2m}\nabla^2 + V(x,y)\right)\psi_n(x) = E_n\psi_n(x).
$$

$$V(x,y)$$ describes a circular potential well: the potential is zero inside the radius of the circule and very large outside. I solve this by first projecting into the basis of 2D harmonic oscillator states, diagonalizing in that basis, then projecting back into position space. As you step up the ladder of energy values, the probability distribution gains more structure corresponding to the greater kinetic energy of the particle.

<div class="row">
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.html path="assets/img/quantum.png" title="Quantum states" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<br>

The animation below shows the first 70 states one at a time. Animations are rendered by rotating between two consecutive state vectors in the hyperplace spanned by the two states. Some consecutive states are degenerate (having equal energy/eigenvalue). The transitions between these states appear as simple rotations of the probability density. 

<blockquote class="reddit-embed-bq" style="height:500px" data-embed-height="728"><a href="https://www.reddit.com/r/Physics/comments/mfov6m/first_70_states_of_a_particle_trapped_in_a/">First 70 states of a particle trapped in a circular well</a><br> by<a href="https://www.reddit.com/user/hudsmith/">u/hudsmith</a> in<a href="https://www.reddit.com/r/Physics/">Physics</a></blockquote><script async="" src="https://embed.reddit.com/widgets.js" charset="UTF-8"></script>


