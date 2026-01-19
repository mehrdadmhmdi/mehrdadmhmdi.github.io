---
layout: page
title: "Software/Packages"
permalink: /Software/
---

<style>
  /* Page wrapper */
  .software-page{max-width:980px;margin:0 auto;padding:0.5rem 0;}

  /* Top tagline */
  .software-tagline{margin:0 0 0.45rem 0;font-size:0.85rem;line-height:1.5}

  /* Quick nav */
  .software-nav{display:flex;flex-wrap:wrap;gap:.5rem;margin:.25rem 0 1.25rem 0}
  .software-nav a{
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
.software-nav a:hover{
  color: #fff;
  border-color: rgba(255,255,255,.35);
  border:1.5px;
}
.software-nav a:visited{ color: rgba(255,95,5,.92); } /* avoid purple */
  /* Section titles */
  .software-section{margin:1.25rem 0}
  .software-section h1,
  .software-section h2,
  .software-section h3{margin:.3rem 0 .6rem 0}

  /* Divider */
  .software-divider{margin:1.25rem 0;border:none;border-top:1px solid rgba(0,0,0,.15)}

  /* Lists -> cards */
  .software-list{list-style:none;padding:0;margin:0;display:grid;gap:.45rem}
  .software-card{
    border:0.8px solid rgba(0,0,0,.15);
    border-radius:11px;
    padding:.85rem .9rem;
    background:rgba(0,0,0,.01);
    font-size:.8rem;
  }
  .software-title{margin:0;font-size:.9rem;font-weight:500;line-height:1.35}
  .software-meta{margin:.25rem 0 0 0;opacity:.85;line-height:1.35}
  .software-links{margin:.55rem 0 0 0;display:flex;flex-wrap:wrap;gap:.45rem}
  .pill{
    display:inline-block;
    padding:.25rem .55rem;
    border:1px solid rgba(0,0,0,.18);
    border-radius:999px;
    text-decoration:none;
    font-size:.9rem;
  }
  .pill:hover{border:1.5px solid rgba(0,0,0,.35)}

  /* info button (details/summary) */
  details.software-details{margin-top:.55rem}
  details.software-details > summary{
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
  details.software-details > summary::-webkit-details-marker{display:none}
  details.software-details[open] > summary{border-color:rgba(0,0,0,.35)}
  .software-info{
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
    .software-card{padding:.8rem}
  }
</style>

<div class="software-page">

<a class="icon-link" href="https://github.com/mehrdadmhmdi" target="_blank" rel="noopener">
  <svg class="icon" aria-hidden="true">
    <use href="{{ '/assets/fontawesome/icons.svg#github' | relative_url }}"></use>
  </svg>
  GitHub
</a>

<section id="Software/Packages" class="software-section">
  <ul class="software-list">
    <li class="software-card">
      <p class="software-title"><b>Kernel Embedding Distributional Reinforcement Learning (KE-DRL) </b>
      <details class="software-details">
        <summary>Info</summary>
        <div class="software-info">
          <b>Offline Multi-Dimensional Distributional RL - RKHS Mean Embedding Estimation</b>
            <b>Works on Linux/macOS/Windows (requires GPU, Python ≥3.9, git, and pip).</b>
          <div class="software-links">
        <a class="pill" href="https://github.com/mehrdadmhmdi/ke-drl" target="_blank">KE-DRL Repository</a>
      </div>
        </div>
      </details>
    </li>
  </ul>
</section>
</div>
