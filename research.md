---
layout: page
title: "Research"
permalink: /Research/
---

<style>
  /* Page wrapper */
  .research-page{max-width:980px;margin:0 auto;padding:0.5rem 0;}

  /* Top tagline */
  .research-tagline{margin:0 0 0.45rem 0;font-size:0.8rem;line-height:1.5}

  /* Quick nav */
  .research-nav{display:flex;flex-wrap:wrap;gap:.5rem;margin:.25rem 0 1.25rem 0}
  .research-nav a{
    display:inline-block;
    padding:.35rem .6rem;
    border:1px solid rgba(0,0,0,.15);
    border-radius:999px;
    text-decoration:none;
    font-size:.85rem;
    color: rgba(255,95,5,.92);          /* text color */
    background: rgba(255,255,255,.04);     /* optional */
    border-color: rgba(255,255,255,.18);   /* optional */
  }
.research-nav a:hover{
  color: #fff;
  border-color: rgba(255,255,255,.35);
}
.research-nav a:visited{ color: rgba(255,95,5,.92); } /* avoid purple */
  /* Section titles */
  .research-section{margin:1.25rem 0}
  .research-section h1,
  .research-section h2,
  .research-section h3{margin:.3rem 0 .6rem 0}

  /* Divider */
  .research-divider{margin:1.25rem 0;border:none;border-top:1px solid rgba(0,0,0,.15)}

  /* Lists -> cards */
  .paper-list{list-style:none;padding:0;margin:0;display:grid;gap:.45rem}
  .paper-card{
    border:0.8px solid rgba(0,0,0,.15);
    border-radius:11px;
    padding:.85rem .9rem;
    background:rgba(0,0,0,.01);
    font-size:.8rem;
  }
  .paper-title{margin:0;font-weight:500;line-height:1.35}
  .paper-meta{margin:.25rem 0 0 0;opacity:.85;line-height:1.35}
  .paper-links{margin:.55rem 0 0 0;display:flex;flex-wrap:wrap;gap:.45rem}
  .pill{
    display:inline-block;
    padding:.25rem .55rem;
    border:1px solid rgba(0,0,0,.18);
    border-radius:999px;
    text-decoration:none;
    font-size:.9rem;
  }
  .pill:hover{border:1.5px solid rgba(0,0,0,.35)}

  /* Abstract button (details/summary) */
  details.paper-details{margin-top:.55rem}
  details.paper-details > summary{
    list-style:none;
    cursor:pointer;
    display:inline-flex;
    align-items:center;
    gap:.45rem;
    padding:.28rem .6rem;
    border:1px solid rgba(0,0,0,.18);
    border-radius:10px;
    user-select:none;
    font-size:.85rem;
  }
  details.paper-details > summary::-webkit-details-marker{display:none}
  details.paper-details[open] > summary{border-color:rgba(0,0,0,.35)}
  .paper-abstract{
    margin:.55rem 0 0 0;
    font-size: 0.85rem;   /* change this */
    line-height: 1.3;
    padding:.65rem .5rem;
    border-left:3px solid rgba(0,0,0,.18);
    background:rgba(0,0,0,.03);
    border-radius:10px;
    font-style: normal
  }

  /* Small screens */
  @media (max-width:600px){
    .paper-card{padding:.8rem}
  }
</style>

<div class="research-page">

<p class="research-tagline"><strong>Statistical Learning, Reinforcement Learning, Non-parametric Statistics, Machine Learning and Statistics Applications</strong></p>

<nav class="research-nav">
  <a href="#work-in-progress">Work in Progress</a>
  <a href="#theory-and-methods">Theory and Methods</a>
  <a href="#medical-sciences">Medical Science Collaborations</a>
  <a href="#business-analytics">Business Analytic Collaborations</a>
</nav>

<section id="work-in-progress" class="research-section">
  <h1>Work in Progress/Review</h1>

  <ul class="paper-list">
    <li class="paper-card">
      <p class="paper-title">Off-policy Distributional Reinforcement Learning, M. Mohammadi, Q. Zheng, and R.Zhu</p>
      <details class="paper-details">
        <summary>Abstract</summary>
        <div class="paper-abstract">
          We propose an (offline) multi-dimensional distributional reinforcement learning framework (KE-DRL) that leverages Hilbert space mappings to estimate the kernel mean embedding of the multi-dimensional value distribution under a proposed target policy. In our setting the state-action are multi-dimensional and continuous. By mapping probability measures into a reproducing kernel Hilbert space via kernel mean embeddings, our method replaces Wasserstein metrics with a integral probability metric. This enables efficient estimation in multi-dimensional state–action spaces and reward settings, where direct computation of Wasserstein distances is computationally challenging. Theoretically, we establish contraction properties of the distributional Bellman operator under our proposed metric involving the Matérn family of kernels and provide uniform convergence guarantees. Simulations and empirical results demonstrate robust off-policy evaluation and recovery of kernel mean embedding under mild assumptions, namely, Lipschitz continuity and boundedness for the kernels, highlighting the potential of our embedding-based approaches in complex, real-world decision-making scenarios and risk evaluations.
        </div>
      </details>
    </li>

    <li class="paper-card">
      <p class="paper-title">A Wasserstein-Equivalent Metric for the Space of Probability Distributions, M. Mohammadi</p>
      <details class="paper-details">
        <summary>Abstract</summary>
        <div class="paper-abstract">
          Viewing the space of probability measures on \(\mathcal{X}\) as a metric space endowed with a Wasserstein distance, we speak of a Wasserstein Space. The Wasserstein distance suffers from high computational complexity, leaving numerous virtually intriguing problems outside of the compass of available algorithms. In this paper, we introduce Toscani–Fourier distance \(T_{s,p}\) a new metric on a dense subspace of probability measures with p-finite moments along with the topological properties of the space induced by this metric, such as convergence, completeness, etc as well as the analysis of its behavior in a high dimensional space. Under suitable moment and tail decay conditions, we prove that this metric is equivalent to the $p-$Wasserstein distance on this subspace. The Toscani–Fourier distance $T_{s,p}$ offers significant computational advantages over Wasserstein distances on this suitably restricted, but dense, subspace. Its simplicity, parallelism, and sensitivity to distributional features make it a promising alternative for a wide range of applications where exact optimal transport is infeasible or unnecessary. Image processing demonstration shows empirical advantages and the equivalence with $p-$Wasserstein.
        </div>
      </details>
    </li>

    <li class="paper-card">
      <p class="paper-title">Semiparametric Time to Event Analysis with Dating Errors, M. Mohammadi</p>
      <details class="paper-details">
        <summary>Abstract</summary>
        <div class="paper-abstract">
          Add abstract here.
        </div>
      </details>
    </li>
  </ul>
</section>

<hr class="research-divider" />

<section id="publications" class="research-section">
  <h1>Publications</h1>

  <h2 id="theory-and-methods">Theory and Methods</h2>
  <p class="paper-meta"><em>(Add items here.)</em></p>

  <h2 id="interdisciplinary-collaborations">Interdisciplinary Collaborations</h2>

  <h3 id="medical-sciences">Medical Sciences</h3>

  <ul class="paper-list">
    <li class="paper-card">
      <p class="paper-title">
        Michelle Villegas-Downs, Mehrdad Mohammadi, Aiguo Han,, William D. O'Brien Jr., Douglas G. Simpson, Tara A. Peters,Judith M. Schlaeger, and McFarlin, Barbara L.
        "Trajectory of Postpartum Cervical Remodeling in Women Delivering Full-term and Spontaneous Preterm: Sensitivity to Quantitative Ultrasound Biomarkers",
        <i> Ultrasound in Medicine &amp; Biology,</i>(2024)
      </p>
      <div class="paper-links">
        <a class="pill" href="https://www.sciencedirect.com/science/article/pii/S0301562924002618" target="_blank">pdf</a>
      </div>
    </li>

    <li class="paper-card">
      <p class="paper-title">
        McFarlin, Barbara L., Michelle Villegas-Downs, Mehrdad Mohammadi, Aiguo Han, Douglas G. Simpson, and William D. O'Brien Jr.
        "Enhanced identification of women at risk for preterm birth via quantitative ultrasound: a prospective cohort study."
        <i>American Journal of Obstetrics &amp; Gynecology MFM</i> 6, no. 5 (2024): 101250
      </p>
      <div class="paper-links">
        <a class="pill" href="https://www.sciencedirect.com/science/article/abs/pii/S2589933323003920" target="_blank">pdf</a>
      </div>
    </li>

    <li class="paper-card">
      <p class="paper-title">
        McFarlin, Barbara L., Yuxuan Liu, Michelle Villegas-Downs, Mehrdad Mohammadi, Douglas G. Simpson, Aiguo Han, and William D. O'Brien Jr.
        "Predicting Spontaneous Pre-term Birth Risk Is Improved When Quantitative Ultrasound Data Are Included With Historical Clinical Data."
        <i>Ultrasound in Medicine &amp; Biology,</i> 49, no. 5 (2023)
      </p>
      <div class="paper-links">
        <a class="pill" href="https://www.sciencedirect.com/science/article/abs/pii/S0301562922006834" target="_blank">pdf</a>
      </div>
    </li>
  </ul>

  <h3 id="business-analytics">Business Analytics</h3>
  <p class="paper-meta"><em>(Add items here.)</em></p>
</section>

</div>
