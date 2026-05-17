---
layout: about
title: about
permalink: /
subtitle: Postdoctoral Research Associate at DCR, University of Bern

profile:
  align: right
  image: prof_pic.jpg
  image_cicular: false # crops the image to make it circular
  address: >
    <p>Medical Data Science Group</p>
    <p>Department of Clinical Research (DCR)</p>
    <p>sitem-insel</p>
    <p>Freiburgstrasse 3</p>
    <p>3010 Bern, Switzerland</p>
    <p style="margin-top:10px;display:flex;flex-direction:column;gap:6px;background:rgba(0,0,0,0.06);border-radius:8px;padding:10px 14px;">
      <a href="https://scholar.google.com/citations?hl=en&user=eR9zhxkAAAAJ" target="_blank" class="quick-link"><i class="ai ai-google-scholar"></i> Google Scholar</a>
      <a href="https://www.linkedin.com/in/rosnikv/" target="_blank" class="quick-link"><i class="fab fa-linkedin"></i> LinkedIn</a>
    </p>

news: false  # includes a list of news items
selected_papers: true # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page
---

<div style="margin-top: 0.5rem;"></div>

👋 AI Scientist building systems that read, reason over, and synthesise scientific knowledge, with a growing focus on clinical evidence and medical AI. Currently a Postdoctoral Researcher at the [Medical Data Science Group, Department of Clinical Research (DCR), University of Bern](https://dcr.unibe.ch/research/index_eng.html).

<style>
.research-tags { display: flex; flex-wrap: wrap; gap: 8px; margin: 16px 0 28px; }
.research-tag {
  background: var(--global-card-bg-color);
  border: 1px solid var(--global-divider-color);
  border-radius: 20px;
  padding: 6px 16px;
  font-family: 'Roboto', sans-serif;
  font-size: 0.8rem;
  font-weight: 500;
  letter-spacing: 0.02em;
  color: var(--global-text-color);
  transition: background 0.2s, box-shadow 0.2s;
}
.research-tag:hover { background: var(--global-divider-color); box-shadow: 0 0 8px rgba(100,140,220,0.3); }

.timeline { position: relative; padding-left: 25px; margin: 10px 0 28px; }
.timeline::before {
  content: '';
  position: absolute;
  left: 7px; top: 6px; bottom: 6px;
  width: 2px;
  background: linear-gradient(to bottom, #4a90d9, #ddd);
  border-radius: 2px;
}
.timeline-entry {
  position: relative;
  margin-bottom: 26px;
  opacity: 0;
  animation: fadeSlideIn 0.5s ease forwards;
}
.timeline-entry:nth-child(1) { animation-delay: 0.1s; }
.timeline-entry:nth-child(2) { animation-delay: 0.25s; }
.timeline-entry:nth-child(3) { animation-delay: 0.4s; }
.timeline-entry:nth-child(4) { animation-delay: 0.55s; }
.timeline-entry:nth-child(5) { animation-delay: 0.7s; }
@keyframes fadeSlideIn {
  from { opacity: 0; transform: translateX(-8px); }
  to   { opacity: 1; transform: translateX(0); }
}
.timeline-dot {
  position: absolute;
  left: -23px; top: 6px;
  width: 12px; height: 12px;
  border-radius: 50%;
  background: #4a90d9;
  border: 2px solid white;
  box-shadow: 0 0 0 2px #4a90d9;
}
.timeline-dot.current {
  background: #2ecc71;
  box-shadow: 0 0 0 2px #2ecc71;
  animation: pulse 2s ease-in-out infinite;
}
@keyframes pulse {
  0%   { box-shadow: 0 0 0 2px #2ecc71; }
  50%  { box-shadow: 0 0 0 6px rgba(46,204,113,0.25); }
  100% { box-shadow: 0 0 0 2px #2ecc71; }
}
.timeline-date {
  font-family: 'Roboto', sans-serif;
  font-size: 0.72rem;
  font-weight: 500;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--global-text-color-light);
  display: block;
  margin-bottom: 3px;
}
.timeline-role {
  font-family: 'Roboto Slab', serif;
  font-weight: 400;
  font-size: 1rem;
  color: var(--global-text-color);
  display: block;
  line-height: 1.4;
}
.timeline-detail {
  font-family: 'Roboto', sans-serif;
  font-size: 0.84rem;
  color: var(--global-text-color-light);
  line-height: 1.6;
  margin: 4px 0 0;
}

.currently-box {
  background: var(--global-card-bg-color);
  border-left: 3px solid #2ecc71;
  border-radius: 4px;
  padding: 14px 18px;
  margin: 0 0 28px;
  font-family: 'Roboto', sans-serif;
  font-size: 1.15rem;
  font-style: italic;
  color: var(--global-text-color);
  line-height: 1.7;
}
.industry-translation {
  display: block;
  margin-top: 8px;
  font-style: normal;
  font-size: 1rem;
  color: var(--global-text-color-light);
}
.contact-cta {
  display: flex;
  align-items: center;
  gap: 16px;
  flex-wrap: wrap;
  margin-top: 8px;
}
.contact-cta-text {
  font-family: 'Roboto', sans-serif;
  font-size: 1rem;
  color: var(--global-text-color-light);
}
.contact-btn {
  display: inline-block;
  padding: 8px 20px;
  background: rgba(0, 159, 6, 0.65);
  color: #fff !important;
  border-radius: 4px;
  font-family: 'Roboto', sans-serif;
  font-size: 0.85rem;
  font-weight: 500;
  text-decoration: none !important;
  transition: opacity 0.2s;
  white-space: nowrap;
}
.contact-btn:hover { opacity: 0.85; }
.quick-links { display: flex; flex-direction: column; gap: 8px; margin-top: auto; padding-top: 20px; }
.quick-link {
  display: flex;
  align-items: center;
  gap: 8px;
  font-family: 'Roboto', sans-serif;
  font-size: 0.85rem;
  color: var(--global-text-color) !important;
  text-decoration: none !important;
  transition: color 0.2s;
}
.quick-link:hover { color: var(--global-theme-color) !important; }
.quick-link i { width: 16px; text-align: center; }

.about-columns {
  display: flex;
  gap: 20px;
  align-items: stretch;
  margin-top: 48px;
  clear: both;
  width: 100%;
}
.about-col-left  { flex: 0 0 35%; }
.about-col-right { flex: 1; }
@media (max-width: 576px) {
  .about-columns { flex-direction: column; gap: 0; }
  .about-col-left { flex: none; width: 100%; }
}
.col-section-title {
  font-family: 'Roboto', sans-serif;
  font-size: 0.72rem;
  font-weight: 600;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--global-text-color-light);
  margin-bottom: 12px;
}
</style>

<p class="col-section-title" style="margin-top: 1.5rem;">🔬 Currently working on</p>
<div class="currently-box">
  Building AI systems that read clinical evidence, assess its quality, and support translational decision-making in drug development.
  <span class="industry-translation">→ enabling faster, evidence-grounded decisions across clinical pipelines.</span>
</div>

<p class="col-section-title" style="margin-top:1rem;">🧑‍🔬 Research Interests</p>
<div class="research-tags" style="margin-bottom:20px;">
  <span class="research-tag">AI for Health</span>
  <span class="research-tag">AI-assisted scientific discovery</span>
  <span class="research-tag">Knowledge distillation</span>
  <span class="research-tag">Literature-grounded reasoning</span>
  <span class="research-tag">Scientific knowledge structuring</span>
  <span class="research-tag">Human-AI collaboration</span>
</div>

<div style="display:flex; align-items:center; gap:16px; flex-wrap:nowrap; margin-bottom:28px;">
  <span class="contact-cta-text" style="white-space:nowrap;font-size:0.92rem;">Open to academic and industry research collaboration especially in AI for health and clinical evidence.</span>
  <a href="mailto:rosni.kottekulam@unibe.ch" class="contact-btn" style="white-space:nowrap;font-size:0.88rem;padding:7px 16px;">Get in touch →</a>
</div>

<div style="display:flex; gap:40px; margin-top:8px; align-items:flex-start;">

  <div style="flex:60; min-width:0;">
    <p class="col-section-title">What's new</p>
    <div style="font-size:0.85rem;">{% include selected_news.html %}</div>
  </div>

  <div style="flex:40; min-width:0;">
    <p class="col-section-title">Journey</p>
    <div class="timeline">

      <div class="timeline-entry">
        <div class="timeline-dot current"></div>
        <span class="timeline-date">Nov 2025 – present</span>
        <span class="timeline-role">Postdoctoral Researcher · <a href="https://dcr.unibe.ch/research/index_eng.html">University of Bern</a></span>
        <p class="timeline-detail">Medical Data Science Group, Department of Clinical Research</p>
      </div>

      <div class="timeline-entry">
        <div class="timeline-dot"></div>
        <span class="timeline-date">2025 (6 months)</span>
        <span class="timeline-role">Visiting Researcher · <a href="https://allenai.org/">Allen Institute for AI (AI2)</a>, Seattle</span>
        <p class="timeline-detail">Collaborating with <a href="https://bhavanadalvi.github.io/">Bhavana Dalvi</a> and <a href="https://pclark425.github.io/">Peter Clark</a> on literature-grounded hypothesis generation and ranking</p>
      </div>

      <div class="timeline-entry">
        <div class="timeline-dot"></div>
        <span class="timeline-date">2020 – 2025</span>
        <span class="timeline-role">PhD · <a href="https://www.ifi.uzh.ch/en.html">University of Zurich</a></span>
        <p class="timeline-detail">Advised by <a href="https://www.ifi.uzh.ch/en/ddis/people/bernstein.html">Prof. Abraham Bernstein</a>, Department of Informatics</p>
      </div>

      <div class="timeline-entry">
        <div class="timeline-dot"></div>
        <span class="timeline-date">2018 – Jan 2020</span>
        <span class="timeline-role">Researcher · <a href="https://www.linkedin.com/company/tata-research-development-and-design-centre-trddc/?originalSubdomain=in">TRDDC, Pune</a></span>
        <p class="timeline-detail">Cybersecurity &amp; Privacy group, with Manish Shukla &amp; <a href="https://www.linkedin.com/in/sachin-lodha-8ba2991/?originalSubdomain=in">Sachin Lodha</a></p>
      </div>

      <div class="timeline-entry">
        <div class="timeline-dot"></div>
        <span class="timeline-date">2016 – 2018</span>
        <span class="timeline-role">Masters in AI · <a href="https://scis.uohyd.ac.in/">University of Hyderabad</a></span>
        <p class="timeline-detail">Recommender systems, advised by <a href="https://scis.uohyd.ac.in/People/profile/vn_profile.php">Prof. Vineet Padmanabhan</a></p>
      </div>

    </div>
  </div>

</div>