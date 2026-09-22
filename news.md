---
layout: page
title: "News"
permalink: /news/
---
<style>
  .news-filter {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    gap: .5rem;
    margin: .25rem 0 1.25rem 0;
  }

  .news-filter label {
    margin: .5em 0;
  }

  .news-filter select {
    display: inline-block;
    padding: .35rem .6rem;
    border: 1px solid rgba(255,255,255,.18);
    border-radius: 999px;
    color: rgba(255,95,5,.92);
    background: rgba(255,255,255,.04);
    font: inherit;
    cursor: pointer;
  }

  .news-filter select:hover,
  .news-filter select:focus {
    border-color: rgba(255,255,255,.35);
    outline: none;
  }

  .news-filter option {
    color: #fff;
    background: #212f3d;
  }
</style>

<div class="news-filter">
  <label for="news-year">Filter by year:</label>
  <select id="news-year" aria-label="Filter news by year">
    <option value="all">All years</option>
    <option value="2026">2026</option>
    <option value="2025">2025</option>
    <option value="2024">2024</option>
  </select>
</div>

<ul id="news-list">
<li data-year="2026"><strong>August 2026:</strong> Successfully defended my PhD dissertation.</li>
<li data-year="2026"><strong>August 2026:</strong> Paper <i>"SILK: Shift-Invariant Landmark Kernels for Dynamic Risk Prediction with an Unknown Time Origin"</i> Presented at The Joint Statistical Meetings- Boston, MA</li>
<li data-year="2025"><strong>November 2025:</strong> Larine Y. Cowan Make A Difference Leadership Award.<i> OVCDEI, at the U of I</i></li>
<li data-year="2025"><strong>August 2025:</strong> Paper <i>"Distributional Reinforcement Learning: A Hilbert Space Embedding Approach"</i> Presented at The Joint Statistical Meetings- Nashville, TN</li>
<li data-year="2025"><strong>April 2025:</strong> Illinois International Graduate Achievement Award. <a href="https://blogs.illinois.edu/view/6758/627615639" target="_blank"> [News Link 1]</a>  and <a href="https://international.illinois.edu/awards-funding/achievement/grad.html" target="_blank"> [News Link 2].</a> </li>
<li data-year="2025"><strong>April 2025:</strong> Presented at the Bohrer Workshop on Distributional RL at UIUC Department of Statistics. <a href="https://calendars.illinois.edu/detail/1439?eventId=33507286" target="_blank"> [News Link].</a></li>
<li data-year="2025"><strong>April 2025:</strong> Awarded 2025 Social Justice Bridge Builder Graduate Award from UIUC Diversity & Social Justice Education <a href="https://dsje.illinois.edu/events/social-justice-awards-ceremony" target="_blank"> [News Link].</a>.</li>
<li data-year="2025"><strong>March 2025:</strong> Paper accepted for presentation in <i>2025 The Joint Statistical Meetings- Nashville, TN</i></li>
<li data-year="2024"><strong>Dec 2024:</strong> Paper accepted in <i>Ultrasound in Medicine & Biology</i>, Vol. 50, Issue 12.</li>
</ul>

<script>
  document.getElementById('news-year').addEventListener('change', function () {
    var selectedYear = this.value;
    document.querySelectorAll('#news-list li').forEach(function (item) {
      item.hidden = selectedYear !== 'all' && item.dataset.year !== selectedYear;
    });
  });
</script>

