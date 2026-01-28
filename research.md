---
layout: page
title: "Research"
permalink: /Research/
---

<style>
  /* Page wrapper */
  .research-page{max-width:980px;margin:0 auto;padding:0.5rem 0;}

  /* Top tagline */
  .research-tagline{margin:0 0 0.45rem 0;font-size:0.85rem;line-height:1.5}

  /* Quick nav */
  .research-nav{display:flex;flex-wrap:wrap;gap:.5rem;margin:.25rem 0 1.25rem 0}
  .research-nav a{
    display:inline-block;
    padding:.35rem .6rem;
    border:1px solid rgba(0,0,0,.15);
    border-radius:999px;
    text-decoration:none;
    font-size:.75rem;
    color: rgba(255,95,5,.92);          /* text color */
    background: rgba(255,255,255,.04);     /* optional */
    border-color: rgba(255,255,255,.18);   /* optional */
  }
.research-nav a:hover{
  color: #fff;
  border-color: rgba(255,255,255,.35);
  border:1.5px;
}
.research-nav a:visited{ color: rgba(255,95,5,.92); } /* avoid purple */
  /* Section titles */
  .research-section{margin:1.25rem 0}
  .research-section h1,
  .research-section h2{color: rgba(255,95,5,.92)},
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
  .paper-title{margin:0;font-size:.9rem;font-weight:500;line-height:1.35}
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
    font-size:.95rem;
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

  /* icons */
  .icon-link + .icon-link{display:inline-flex;align-items:center;gap:.4rem;margin-left:1.1rem;}
  .icon{width:1em;height:1em;vertical-align:-.12em}

  /* Small screens */
  @media (max-width:600px){
    .paper-card{padding:.8rem}
  }
</style>

<div class="research-page">

<p class="research-tagline"><strong>Statistical Learning, Reinforcement Learning, Reproducing Kernel Hilbert Spaces, Non-parametric Statistics, Machine Learning and Statistics Applications</strong></p>
<a class="icon-link" href="https://github.com/mehrdadmhmdi" target="_blank" rel="noopener">
  <svg class="icon" aria-hidden="true">
    <use href="{{ '/assets/fontawesome/icons.svg#github' | relative_url }}"></use>
  </svg>
  GitHub
</a>
<a class="icon-link"
   href="https://scholar.google.com/citations?user=ALnHM1oAAAAJ&hl=en"
   target="_blank" rel="noopener">
    <svg class="icon" aria-hidden="true">
      <use href="{{  '/assets/fontawesome/icons.svg#google-scholar'   | relative_url }}"></use>
    </svg>
  Google Scholar
</a>

<nav class="research-nav">
  <a href="#work-in-progress">Under Review</a>
  <a href="#theory-and-methods">Theory and Methods</a>
  <a href="#medical-sciences">Medical Science Collaborations</a>
  <a href="#business-analytics">Business Analytic Collaborations</a>
</nav>
<section id="work-in-progress" class="research-section">
  <h1>Under Review</h1>
  {% bibliography -f publications -q @*[status=under-review] -T pub_card %}
</section>

<hr class="research-divider" />

<section id="publications" class="research-section">
  <h1>Publications</h1>

  <h2 id="theory-and-methods">Theory and Methods</h2>
  {% bibliography -f publications -q @*[topic=theory-and-methods && status!=under-review] -T pub_card %}

  <h3 id="medical-sciences">Medical Sciences</h3>
  {% bibliography -f publications -q @*[topic=medical-sciences] -T pub_card %}

  <h3 id="business-analytics">Business Analytics</h3>
  {% bibliography -f publications -q @*[topic=business-analytics] -T pub_card %}
</section>

</div>
