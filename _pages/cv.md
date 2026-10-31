---
layout: academic
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

<header class="page-heading"><p class="eyebrow">BACKGROUND / EXPERIENCE</p><h1>Curriculum vitae.</h1><p>Third-year Ph.D. student in Computer Science · University at Buffalo, SUNY</p></header>

<div class="cv-content" markdown="1">

## Research interests
Medical AI, 3D anatomical modeling, and language-guided interaction. My long-term research aspiration is surgical robotics: embodied intelligence for autonomous manipulation and collaboration with surgeons.

## Ph.D. status
* Third-year doctoral student, advised by Prof. Mingchen Gao
* Advanced to Ph.D. candidacy in August 2025

## Education
* Ph.D. in Computer Science, University at Buffalo, SUNY, 2029 (expected)
* M.S. in Computer Science, Boston University, 2023
* B.S. in Math and Computer Science, University of California, San Diego, 2019

## Work experience
* Fall 2024: Teaching Assistant
  * Teaching assistant for CSE 574: Introduction to Machine Learning

* Dec. 2022 - Mar. 2023: Research Assistant
  * Boston College, EPFL
  * Mentor: Professor Donglai Wei, Dr. Jiancheng Yang, Dr. Siyu Huang

* Dec. 2022 - Mar. 2023: Research Assistant
  * Boston College, Harvard University
  * Mentor: Professor Donglai Wei, Dr. Siyu Huang

* Mar. 2022 - Aug. 2022: Research Assistant
  * Bio-Imaging & Informatics Lab @ Boston University
  * Mentor: Dr. Bang-Bon Koo


## Publications
{% assign papers = site.publications | sort: 'date' | reverse %}
{% for paper in papers %}{% include publication-entry.html paper=paper %}{% endfor %}
  
  
## Teaching
<ul>{% for course in site.teaching reversed %}<li><a href="{{ course.url | relative_url }}">{{ course.title }}</a> · {{ course.date | date: '%Y' }}</li>{% endfor %}</ul>

</div>
