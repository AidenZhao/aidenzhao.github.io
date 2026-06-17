---
permalink: /
title: "About Me"
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
.about-home {
  --ink: #253238;
  --muted: #5d6d75;
  --line: #dfe7ea;
  --blue: #226f8f;
  --teal: #14806e;
  --rose: #b34453;
  --paper: #ffffff;
  --soft: #f8fbfc;
  color: var(--ink);
}

.about-home * {
  box-sizing: border-box;
}

.about-home a {
  text-decoration: none;
  border-bottom: 1px solid rgba(34, 111, 143, 0.25);
}

.about-home a:hover {
  border-bottom-color: currentColor;
}

.profile-panel {
  margin-bottom: 1.45rem;
  padding: 1.15rem 1.25rem;
  border: 1px solid var(--line);
  border-top: 4px solid var(--blue);
  border-radius: 8px;
  background: var(--soft);
}

.profile-kicker {
  margin: 0 0 0.45rem;
  color: var(--blue);
  font-size: 0.74rem;
  font-weight: 700;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

.profile-lede {
  margin: 0 0 0.7rem;
  font-size: 1.03rem;
  line-height: 1.72;
}

.research-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.42rem;
  margin: 0.85rem 0 0.15rem;
  padding: 0;
  list-style: none;
}

.research-tags li {
  padding: 0.24rem 0.56rem;
  border: 1px solid rgba(20, 128, 110, 0.24);
  border-radius: 999px;
  background: rgba(20, 128, 110, 0.08);
  color: #185f55;
  font-size: 0.78rem;
  font-weight: 700;
  line-height: 1.25;
}

.collab-note {
  margin: 1rem 0 0;
  padding: 0.78rem 0.95rem;
  border-left: 4px solid var(--rose);
  border-radius: 0 8px 8px 0;
  background: #fff8f8;
  color: #4c3b40;
  line-height: 1.55;
}

.home-section {
  margin-top: 1.65rem;
}

.home-section h2 {
  margin: 0 0 0.78rem;
  padding-bottom: 0.3rem;
  border-bottom: 1px solid var(--line);
  color: #1f3137;
  font-size: 1.18rem;
  line-height: 1.3;
}

.news-list,
.timeline {
  display: grid;
  gap: 0.55rem;
  margin: 0;
  padding: 0;
  list-style: none;
}

.news-list li {
  display: grid;
  grid-template-columns: 5.2rem minmax(0, 1fr);
  gap: 0.75rem;
  align-items: start;
  padding: 0.62rem 0.75rem;
  border: 1px solid var(--line);
  border-radius: 8px;
  background: var(--paper);
  line-height: 1.45;
}

.news-list time {
  color: var(--rose);
  font-size: 0.85rem;
  font-weight: 700;
}

.publication-list {
  display: grid;
  gap: 0.9rem;
}

.publication-card {
  display: grid;
  grid-template-columns: 132px minmax(0, 1fr);
  gap: 1rem;
  align-items: center;
  padding: 0.8rem;
  border: 1px solid var(--line);
  border-radius: 8px;
  background: var(--paper);
}

.publication-thumb {
  display: flex;
  min-height: 96px;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  border: 1px solid #edf2f3;
  border-radius: 6px;
  background: #f8fafb;
}

.publication-thumb img {
  display: block;
  max-width: 100%;
  max-height: 112px;
  object-fit: contain;
}

.publication-card h3 {
  margin: 0 0 0.38rem;
  font-size: 1rem;
  line-height: 1.36;
}

.publication-card p {
  margin: 0.22rem 0;
  color: var(--muted);
  font-size: 0.88rem;
  line-height: 1.45;
}

.venue-badge {
  display: inline-block;
  margin-top: 0.18rem;
  padding: 0.16rem 0.46rem;
  border-radius: 4px;
  background: #eef7f5;
  color: #0d6f61;
  font-size: 0.78rem;
  font-weight: 700;
  line-height: 1.25;
}

.affiliation-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 0.75rem;
}

.affiliation-card {
  padding: 0.85rem;
  border: 1px solid var(--line);
  border-radius: 8px;
  background: var(--paper);
}

.affiliation-date {
  display: block;
  margin-bottom: 0.28rem;
  color: var(--rose);
  font-size: 0.8rem;
  font-weight: 700;
}

.affiliation-card h3 {
  margin: 0 0 0.25rem;
  color: var(--ink);
  font-size: 0.98rem;
  line-height: 1.35;
}

.affiliation-card p {
  margin: 0;
  color: var(--muted);
  font-size: 0.88rem;
  line-height: 1.45;
}

.timeline-item {
  display: grid;
  grid-template-columns: 7.2rem minmax(0, 1fr);
  gap: 1rem;
  padding: 0.75rem 0.85rem;
  border: 1px solid var(--line);
  border-left: 4px solid var(--teal);
  border-radius: 8px;
  background: var(--paper);
}

.timeline-date {
  color: #6a5860;
  font-size: 0.86rem;
  font-weight: 700;
}

.timeline-item strong {
  color: var(--ink);
}

.timeline-item p {
  margin: 0.18rem 0 0;
  color: var(--muted);
  font-size: 0.9rem;
  line-height: 1.5;
}

@media (max-width: 640px) {
  .profile-panel {
    padding: 1rem;
  }

  .news-list li,
  .timeline-item,
  .publication-card {
    grid-template-columns: 1fr;
  }

  .publication-thumb {
    min-height: 120px;
  }

  .publication-thumb img {
    max-height: 132px;
  }

  .affiliation-grid {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="about-home">

<section class="profile-panel">
  <p class="profile-kicker">Computer Graphics · Geometry Processing · 3D Vision</p>
  <p class="profile-lede">
    I am a Computer Graphics Ph.D. student in the Department of Computer Science at
    <strong>City University of Hong Kong</strong>, where I am fortunate to be advised by
    <strong>Prof. Junhui Hou</strong>. I am also a <strong>Research Scientist Intern</strong>
    at <strong>Meshy AI</strong>.
  </p>
  <p class="profile-lede">
    Before joining CityU, I received my master's degree from the School of Artificial
    Intelligence at <strong>Beijing Normal University</strong>, advised by
    <strong>Prof. Zhongke Wu</strong>.
  </p>
  <ul class="research-tags">
    <li>Generative AI</li>
    <li>Spatial Computing</li>
    <li>World Models</li>
    <li>Geometry Processing</li>
    <li>3D Vision</li>
  </ul>
  <p class="collab-note">
    I am actively looking for collaborators. If you find my research interesting,
    welcome to contact me via email.
  </p>
</section>

<section class="home-section">
  <h2>🔥 News</h2>
  <ul class="news-list">
    <li><time>2026.5</time><span><strong>PRISM</strong> is accepted by ICML 2026.</span></li>
    <li><time>2025.11</time><span><strong>FlexPara</strong> is accepted by TPAMI 2025.</span></li>
    <li><time>2024.8</time><span>One paper is accepted by Pacific Graphics 2024. Congrats to Chunhao.</span></li>
    <li><time>2024.4</time><span>A talk is given at EuroGraphics 2024.</span></li>
    <li><time>2024.2</time><span>One paper is accepted by EuroGraphics 2024.</span></li>
    <li><time>2023.5</time><span>A talk is given at ACM SIGGRAPH Symposium on Interactive 3D Graphics and Games 2023.</span></li>
    <li><time>2023.2</time><span>One paper is accepted by I3DG 2023.</span></li>
  </ul>
</section>

<section class="home-section">
  <h2>📝 Publications</h2>
  <div class="publication-list">
    <article class="publication-card">
      <a class="publication-thumb" href="https://arxiv.org/abs/2606.02268">
        <img src="{{ site.baseurl }}/images/PRSIM.png" alt="PRISM teaser">
      </a>
      <div>
        <h3><a href="https://arxiv.org/abs/2606.02268">From Extrinsic to Intrinsic: Geodesic-Guided Representation Learning for 3D Geometric Data</a></h3>
        <p><strong>Yuming Zhao</strong>, Junhui Hou, Qijian Zhang, Jia Qin, Ying He</p>
        <p><span class="venue-badge">ICML 2026</span></p>
      </div>
    </article>

    <article class="publication-card">
      <a class="publication-thumb" href="https://arxiv.org/abs/2504.19210">
        <img src="{{ site.baseurl }}/images/flexpara.png" alt="FlexPara teaser">
      </a>
      <div>
        <h3><a href="https://arxiv.org/abs/2504.19210">FlexPara: Flexible Neural Surface Parameterization</a></h3>
        <p><strong>Yuming Zhao</strong>, Qijian Zhang, Junhui Hou, Jiazhi Xia, Wenping Wang, Ying He</p>
        <p><span class="venue-badge">TPAMI 2025</span></p>
      </div>
    </article>

    <article class="publication-card">
      <a class="publication-thumb" href="https://onlinelibrary.wiley.com/doi/full/10.1111/cgf.15239">
        <img src="{{ site.baseurl }}/images/dbsc.png" alt="Disk B-spline teaser">
      </a>
      <div>
        <h3><a href="https://onlinelibrary.wiley.com/doi/full/10.1111/cgf.15239">Disk B-spline on S^2: A Skeleton-based Region Representation on 2-Sphere</a></h3>
        <p>Chunhao Zheng, <strong>Yuming Zhao</strong>, Zhongke Wu, Xingce Wang</p>
        <p><span class="venue-badge">Computer Graphics Forum, Proc. Pacific Graphics 2024</span></p>
      </div>
    </article>

    <article class="publication-card">
      <a class="publication-thumb" href="https://onlinelibrary.wiley.com/doi/full/10.1111/cgf.15021">
        <img src="{{ site.baseurl }}/images/GLS-PIA.png" alt="GLS-PIA teaser">
      </a>
      <div>
        <h3><a href="https://onlinelibrary.wiley.com/doi/full/10.1111/cgf.15021">GLS-PIA: n-Dimensional Spherical B-Spline Curve Fitting based on Geodesic Least Square with Adaptive Knot Placement</a></h3>
        <p><strong>Yuming Zhao</strong>, Zhongke Wu, Xingce Wang</p>
        <p><span class="venue-badge">Computer Graphics Forum, Proc. EuroGraphics 2024</span></p>
      </div>
    </article>

    <article class="publication-card">
      <a class="publication-thumb" href="https://dl.acm.org/doi/abs/10.1145/3585504">
        <img src="{{ site.baseurl }}/images/blending.png" alt="G2 blending teaser">
      </a>
      <div>
        <h3><a href="https://dl.acm.org/doi/abs/10.1145/3585504">G2 Blending Ball B-Spline Curve by B-Spline</a></h3>
        <p><strong>Yuming Zhao</strong>, Zhongke Wu, Xingce Wang, Xinyue Liu</p>
        <p><span class="venue-badge">ACM I3DG 2023</span></p>
      </div>
    </article>
  </div>
</section>

<section class="home-section">
  <h2>🏛️ Affiliations</h2>
  <div class="affiliation-grid">
    <article class="affiliation-card">
      <span class="affiliation-date">2025.11 - now</span>
      <h3>Meshy AI</h3>
      <p>Research Scientist Intern</p>
    </article>
    <article class="affiliation-card">
      <span class="affiliation-date">2024.9 - now</span>
      <h3>City University of Hong Kong</h3>
      <p>Ph.D. student, Department of Computer Science</p>
    </article>
    <article class="affiliation-card">
      <span class="affiliation-date">2021.9 - 2024.6</span>
      <h3>Beijing Normal University</h3>
      <p>M.S. student, School of Artificial Intelligence</p>
    </article>
    <article class="affiliation-card">
      <span class="affiliation-date">2022.10 - 2022.12</span>
      <h3>Du Xiaoman Financial</h3>
      <p>Intern, Beijing, China</p>
    </article>
  </div>
</section>

<section class="home-section">
  <h2>🎓 Education</h2>
  <div class="timeline">
    <article class="timeline-item">
      <span class="timeline-date">2024.9 - now</span>
      <div>
        <strong>Ph.D. student in Computer Science</strong>
        <p>Department of Computer Science, City University of Hong Kong, Hong Kong</p>
      </div>
    </article>
    <article class="timeline-item">
      <span class="timeline-date">2021.9 - 2024.6</span>
      <div>
        <strong>M.S. in Computer Applied Technology</strong>
        <p>School of Artificial Intelligence, Beijing Normal University, Beijing, China</p>
      </div>
    </article>
    <article class="timeline-item">
      <span class="timeline-date">2017.9 - 2021.6</span>
      <div>
        <strong>B.Sc. in Computer Science and Technology</strong>
        <p>School of Artificial Intelligence, Beijing Normal University, Beijing, China</p>
      </div>
    </article>
    <article class="timeline-item">
      <span class="timeline-date">2019.7 - 2019.8</span>
      <div>
        <strong>Summer School in Big Data and High-Performance Computing</strong>
        <p>Cardiff University, Cardiff, UK</p>
      </div>
    </article>
  </div>
</section>

<section class="home-section">
  <h2>💬 Talks</h2>
  <div class="timeline">
    <article class="timeline-item">
      <span class="timeline-date">2024.4</span>
      <div>
        <strong>Oral presentation at EuroGraphics 2024</strong>
      </div>
    </article>
    <article class="timeline-item">
      <span class="timeline-date">2023.5</span>
      <div>
        <strong><a href="https://www.youtube.com/watch?v=m8rggUd7cAQ&t=11s">Oral presentation</a> at ACM SIGGRAPH Symposium on Interactive 3D Graphics and Games 2023</strong>
      </div>
    </article>
  </div>
</section>

<section class="home-section">
  <h2>💻 Internships</h2>
  <div class="timeline">
    <article class="timeline-item">
      <span class="timeline-date">2025.11 - now</span>
      <div>
        <strong>Research Scientist Intern</strong>
        <p>Meshy AI</p>
      </div>
    </article>
    <article class="timeline-item">
      <span class="timeline-date">2022.10 - 2022.12</span>
      <div>
        <strong>Intern</strong>
        <p>Du Xiaoman Financial, Beijing, China</p>
      </div>
    </article>
  </div>
</section>

</div>
