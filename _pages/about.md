---
layout: academic
permalink: /
title: "About"
description: "Kangxian Xie is a third-year Computer Science Ph.D. student at the University at Buffalo, studying medical AI and aspiring to advance surgical robotics and embodied intelligence."
redirect_from:
  - /about/
  - /about.html
---
<section class="hero" aria-labelledby="hero-title">
  <div class="hero-copy">
    <p class="eyebrow"><span class="status-dot" aria-hidden="true"></span> MEDICAL AI · EMBODIED INTELLIGENCE</p>
    <h1 id="hero-title">Kangxian Xie</h1>
    <p class="hero-role">Third-year Ph.D. student in Computer Science</p>
    <p class="hero-affiliation">University at Buffalo, SUNY <span aria-hidden="true">/</span> Buffalo, NY</p>
    <p class="hero-intro">I study how AI can understand anatomy and work with clinicians. My next ambition is to bring that understanding into <em>surgical robots that can perceive, reason, and act.</em></p>
    <div class="hero-links"><a class="button button-dark" href="mailto:{{ site.author.email }}">Get in touch <span aria-hidden="true">↗</span></a><a href="{{ site.author.googlescholar }}">Google Scholar <span aria-hidden="true">↗</span></a><a href="https://github.com/{{ site.author.github }}">GitHub <span aria-hidden="true">↗</span></a></div>
  </div>
  <figure class="portrait">
    <div class="portrait-image"><img src="{{ '/images/profile.jpeg' | relative_url }}" alt="Portrait of Kangxian Xie" width="789" height="1218" fetchpriority="high"></div>
    <figcaption><span>RESEARCHER &amp; BUILDER</span><span>BUFFALO, NY</span></figcaption>
  </figure>
</section>

<section class="about-section section-rule" aria-labelledby="about-title">
  <div class="section-label"><span class="section-number">01 /</span><h2 id="about-title">A little about me</h2></div>
  <div class="about-body">
    <p>I am a third-year Ph.D. student at the <a href="https://engineering.buffalo.edu/computer-science-engineering.html">University at Buffalo</a>, advised by <a href="https://engineering.buffalo.edu/computer-science-engineering/people/faculty-directory/full-time.host.html/content/shared/engineering/computer-science-engineering/profiles/faculty/ladder/gao-mingchen.detail.html">Prof. Mingchen Gao</a>. My work brings together medical image analysis, 3D anatomical modeling, and language-guided interaction.</p>
    <p>Before UB, I worked with <a href="https://donglaiw.github.io/">Prof. Donglai Wei</a>, <a href="https://siyuhuang.github.io/">Dr. Siyu Huang</a>, and <a href="https://jiancheng-yang.com/">Dr. Jiancheng Yang</a>, and began my medical imaging research at the <a href="https://sites.bu.edu/bil/">Bio-Imaging &amp; Informatics Lab at Boston University</a>. I hold an M.S. in Computer Science from Boston University and a B.S. in Math and Computer Science from UC San Diego. I’m originally from Zhuhai, China.</p>
    <a class="text-link" href="{{ '/cv/' | relative_url }}">More about my background <span aria-hidden="true">→</span></a>
  </div>
</section>

<section class="research-section section-rule" id="research" aria-labelledby="research-title">
  <div class="section-heading"><div><p class="eyebrow">02 / RESEARCH DIRECTION</p><h2 id="research-title">From understanding anatomy<br>to intelligent action.</h2></div><p class="section-aside">Medical imaging is where I started.<br>Surgical robotics is where I want to go.</p></div>
  <div class="aspiration">
    <div class="aspiration-copy"><p class="eyebrow">MY ASPIRATION</p><h3>Embodied intelligence<br>for surgical robotics.</h3><p>My long-term goal is to develop intelligent surgical robots that connect visual and anatomical understanding with autonomous manipulation. I want to study how robots can learn surgical skills, reason about the physical world, and collaborate with surgeons.</p><p>Building on my work in 3D medical AI and language-guided refinement, I hope to connect perception, decision-making, and action to support safer, more precise surgical care.</p></div>
    <div class="research-path" aria-label="Research aspirations: perception, reasoning, and action">
      <div class="path-step"><span class="path-index">01</span><div><h4>Perceive</h4><p>Understand 3D anatomy and surgical scenes.</p></div><span class="path-symbol" aria-hidden="true">↗</span></div>
      <div class="path-step"><span class="path-index">02</span><div><h4>Reason</h4><p>Connect anatomy, clinical intent, and physical constraints.</p></div><span class="path-symbol" aria-hidden="true">↗</span></div>
      <div class="path-step"><span class="path-index">03</span><div><h4>Act</h4><p>Learn embodied skills for autonomous surgical manipulation.</p></div><span class="path-symbol" aria-hidden="true">↗</span></div>
      <p class="path-note">A research vision connecting medical AI with robotics.</p>
    </div>
  </div>
</section>

{% assign latest_paper = site.publications | where: 'project_name', 'CoWTalk' | first %}
{% if latest_paper %}
<section class="featured-section section-rule" aria-labelledby="featured-title">
  <div class="section-heading"><div><p class="eyebrow">03 / LATEST WORK</p><h2 id="featured-title">Let clinicians guide the shape.</h2></div><span class="venue-badge">MICCAI 2026</span></div>
  <div class="featured-work">
    <a class="featured-figure" href="{{ latest_paper.url | relative_url }}" aria-label="Read about CoWTalk"><img src="{{ '/images/research/cowtalk-workflow.png' | relative_url }}" alt="CoWTalk workflow: a radiologist provides verbal instructions to iteratively refine a 3D arterial segmentation." width="1080" height="360" loading="lazy"><span>CLINICIAN IN THE LOOP <span aria-hidden="true">↗</span></span></a>
    <div class="featured-copy"><p class="eyebrow accent-text">CoWTalk</p><h3><a href="{{ latest_paper.url | relative_url }}">{{ latest_paper.title }}</a></h3><p>What if refining a 3D segmentation started with a conversation? CoWTalk pairs arterial shapes with corrective language and studies iterative refinement guided by clinicians’ instructions.</p><div class="paper-links"><a href="{{ latest_paper.paperurl }}">Read paper <span aria-hidden="true">↗</span></a><a href="{{ latest_paper.codeurl }}">Code <span aria-hidden="true">↗</span></a><a href="{{ latest_paper.dataseturl }}">Dataset <span aria-hidden="true">↗</span></a></div></div>
  </div>
</section>
{% endif %}

<section class="publications-section section-rule" aria-labelledby="publications-title">
  <div class="section-heading"><div><p class="eyebrow">04 / PUBLICATIONS</p><h2 id="publications-title">Selected research</h2></div><a class="text-link" href="{{ '/publications/' | relative_url }}">All publications <span aria-hidden="true">↗</span></a></div>
  {% assign papers = site.publications | sort: 'date' | reverse %}
  {% for paper in papers limit: 3 %}{% include publication-entry.html paper=paper %}{% endfor %}
</section>

<section class="news-section section-rule" aria-labelledby="news-title">
  <div class="section-label"><span class="section-number">05 /</span><h2 id="news-title">Recent updates</h2></div>
  <ol class="news-list">
    <li><time datetime="2026-05">MAY 2026</time><p><a href="{{ '/publication/2026-refining-3d-medical-segmentation-verbal-instruction' | relative_url }}">CoWTalk</a> received early acceptance at <strong>MICCAI 2026</strong>.</p></li>
    <li><time datetime="2025-12">DEC 2025</time><p>Our work on template-guided pulmonary segment reconstruction was accepted by <strong>Medical Image Analysis</strong>.</p></li>
    <li><time datetime="2025-08">AUG 2025</time><p>I advanced to Ph.D. candidacy at the University at Buffalo.</p></li>
    <li><time datetime="2024-10">OCT 2024</time><p>Our work on anatomical labeling of pulmonary trees was accepted by <strong>Medical Image Analysis</strong>.</p></li>
    <li><time datetime="2024-09">SEP 2024</time><p>I joined UB as a Ph.D. student and teaching assistant.</p></li>
  </ol>
</section>
