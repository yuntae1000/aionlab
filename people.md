---
layout: page
title: People
permalink: /people/
body_class: people-page
description: Researchers and students of AION Lab, led by Prof. Yoontae (Jake) Jung (정윤태) at Kyung Hee University.
---

<section class="people-directory-section" id="professor">
  <div class="directory-heading">
    <span class="directory-index">01</span>
    <div><p class="eyebrow">FACULTY</p><h2>Professor</h2></div>
  </div>
  <article class="faculty-entry">
    <img src="{{ '/assets/people/jake.jpg' | relative_url }}" alt="Professor Yoontae (Jake) Jung, 정윤태" loading="lazy">
    <div>
      <h3>Yoontae (Jake) Jung</h3>
      <p class="person-name-ko" lang="ko">정윤태</p>
      <p class="faculty-role">Assistant Professor · School of Electronic Engineering</p>
      <p>Principal Investigator, AION Lab<br>Kyung Hee University</p>
      <p>Analog and mixed-signal ICs · Neural interfaces · Intelligent sensing</p>
      <a class="directory-link" href="{{ '/people/professor/' | relative_url }}">Profile and research background <span aria-hidden="true">→</span></a>
    </div>
  </article>
</section>

<section class="people-directory-section" id="students">
  <div class="directory-heading">
    <span class="directory-index">02</span>
    <div><p class="eyebrow">LAB MEMBERS</p><h2>Students</h2></div>
  </div>
  <p class="directory-intro">AION Lab welcomes students interested in integrated circuit design and its applications to real-world sensing and intelligence.</p>
  {% include student-groups.html %}
</section>
