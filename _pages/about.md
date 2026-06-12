---
layout: minimal
title: home
nav_title: Home
permalink: /
nav: true
nav_order: 1
---

<div class="home-photo" aria-label="Profile photo placeholder"></div>

<div class="intro">
  <p>
    Jae-Hong Lee is an Assistant Professor in the
    <a href="#">Division of Language &amp; AI</a> at
    <a href="#">Hankuk University of Foreign Studies</a>, Seoul, South Korea.
  </p>

  <p>
    He received the B.S. degree in electronic engineering from Hanyang University in 2017,
    and the M.S. and Ph.D. degrees in electronics engineering from Hanyang University in 2024.
  </p>

  <p>
    His research interests include <strong>signal processing and machine learning</strong>
    applications for <strong>time-varying data</strong> such as speech, audio, video, text,
    and time series, with an emphasis on <strong>dynamical systems</strong>,
    <strong>probability</strong>, and <strong>optimization</strong>.
  </p>
</div>

<p class="links">
  <a href="mailto:ljh93ljh@hufs.ac.kr">Email</a>
  <a href="#">Google Scholar</a>
  <a href="#">CV</a>
</p>

<p>
  <strong>Office</strong>: Rm 401, Faculty Building, Hankuk University of Foreign Studies,
  107, Imun-ro, Dongdaemun-gu, Seoul, Republic of Korea
</p>

## Recent News

<div class="news-list">
  {% assign news_items = site.news | sort: "date" | reverse %}
  {% for item in news_items limit: 5 %}
    <article class="news-item">
      <div class="news-date">{{ item.date | date: "%b %Y" }}</div>
      <div class="news-text">{{ item.content }}</div>
    </article>
  {% endfor %}
</div>
