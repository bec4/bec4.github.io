---
title: Science
# feature_text: |
#     ## <span style="color:#f2f2f2">BEC4</span>
#     <span style="color:#f2f2f2">The rubidium lattice lab at MIT</span>
# feature_image: /assets/img/paper.png
---

<script src="/assets/d3.min.js"></script>
<script src='https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-svg.js'></script>

<style>
.wannier {
    cursor: grab;
}
/* #latticeInfoBox {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translateY(-50%) translateX(-50%);
    background-color: #e3e3e3b5;
    padding: 10px;
    font-family: 'DM Mono', monospace;
    text-align: center;
} */


</style>


Recently, we've been studying the mapping between the Bose--Hubbard model with a spin degree of freedom and the $S = 1$ Heisenberg model. 


- [Preparation of the Spin-Mott State: A Spinful Mott Insulator of Repulsively Bound Pairs](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.128.093401), Phys. Rev. Lett. **129**, 093401 (2022)

<!-- <div id = "lattice-container" style="pad-bottom:20px;">
    <svg id = "spin-dependent-lattice-demo">
    </svg>
</div> -->

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

- [Coherence Times of Bose-Einstein Condensates beyond the Shot-Noise Limit via Superfluid Shielding](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.117.275301), Phys. Rev. Lett. **117**, 275301 (2016)

See our [MIT wiki page](https://wikis.mit.edu/confluence/display/bec4/Publications) for a complete list of previous BEC4 publications.