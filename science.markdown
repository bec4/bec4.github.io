---
title: Science
# feature_text: |
#     ## <span style="color:#f2f2f2">BEC4</span>
#     <span style="color:#f2f2f2">The rubidium lattice lab at MIT</span>
feature_image: /assets/img/spin-dependent-lattice.png
---

<script src="/assets/d3.min.js"></script>
<script src='https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-svg.js'></script>

<style>
.wannier {
    cursor: grab;
}

.feature {
    background-position: bottom;
}

.feature .container {
    min-height: 20vh;

}
</style>


Recently, we've been studying the mapping between the Bose--Hubbard model with a spin degree of freedom and the $S = 1$ Heisenberg model. 
Have a look at our [MIT wiki page](https://wikis.mit.edu/confluence/display/bec4/Publications) for a complete list of previous publications.


- [Preparation of the Spin-Mott State: A Spinful Mott Insulator of Repulsively Bound Pairs](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.128.093401), Phys. Rev. Lett. **129**, 093401 (2022)
<!-- - [Adiabatic cooling of bosons in lattices to magnetically ordered quantum states](https://journals.aps.org/pra/abstract/10.1103/PhysRevA.92.041602), Phys. Rev. A **92**, 041602(R) (2015) -->

Particles in a sufficiently deep lattice can be described by the Bose-Hubbard model. Here we assume they tunnel around with some rate $t$, and that they have an on-site interaction $U$.
In our lab we've been studying what happens when there are two particles per site which are allowed to be in different spin states. Things get interesting when they have a tunable interparticle interaction $U_{AB}$ (typically such that $0 \leq U_{AB} \leq U$). If we tune this all the way to zero, the energetically most favorable state is to have an A and a B particle on every site, this is the spin Mott insulator, and we studied it in the paper mentioned above.

When $U_{AB} = U$, the ground state is highly degenerate: it doesn't matter what spin configuration you have anymore, because all energies are the same. On the way to that point, however, the AB state starts to 'fluctuate,' meaning it will undergo excursions to AA or BB. These fluctuations are highly correlated between neighbors - after all, they need to exchange particles - and this tate is called an XY ferromagnet. 

In the lab we implement this using a spin-dependent lattice, which gives us control over the overlap of the atomic wave functions in the lattice. It allows us to tune $U_{AB}$. Below you can try so yourself - notice the fluctuations into paired states that arise as you approach perfect overlap.

<div id = "wannier-container" style="text-align:center;position:relative;padding:20px 0;">
    <svg id = "lattice-phase">
    </svg>
    <svg id = "wannier">
    </svg>
    <p id = "latticeInfoBox" style="opacity:1;">
        <em>A cartoon of the spin Mott insulator. Drag the wave functions to change their overlap.</em>
    </p>
</div>


<script src="/assets/spin-mott.js"></script>

- [Tunable Single-Ion Anisotropy in Spin-1 Models Realized with Ultracold Atoms](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.126.163203), Phys. Rev. Lett. **126**, 163203 (2021)

<div id = "two-site-container"></div>
<p style="text-align:center">
  <em>A toy model for our work on the spin-1 model out of equilibrium.</em>
</p>

<script src="/assets/animate-twosite.js"></script>

<!-- - [Coherence Times of Bose-Einstein Condensates beyond the Shot-Noise Limit via Superfluid Shielding](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.117.275301), Phys. Rev. Lett. **117**, 275301 (2016)
 -->
