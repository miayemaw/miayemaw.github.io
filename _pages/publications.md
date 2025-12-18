---
layout: page
permalink: /publications/
title: publications
description: 
years: [2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015]
nav: true
nav_order: 4
---
<!-- _pages/publications.md -->

<div class="publications">

<!-- Table of Contents -->
<ol>
  <li><a href="#sciscie-journals">SCI/SCIE Indexed Journals</a></li>
  <!-- <li><a href="#other-journals">Other Peer-Reviewed Journals</a></li> -->
  <li><a href="#patents">Patents</a></li>
  <li><a href="#conferences">Conferences</a></li>
</ol>

<hr>

<!-- SCI/SCIE Journals Section -->
<h2 id="sciscie-journals">SCI/SCIE Journals</h2>
<p style="color: #b71c1c;">International Peer-Reviewed Journals (SCI/SCIE Indexed)</p>

{%- for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @article[year={{y}}]* %}
{% endfor %}

<hr>

<!-- Patents Section -->
<h2 id="patents">Patents</h2>

<h3 class="year">2022</h3>
{% bibliography -f papers -q @patent* %}

<hr>

<!-- Conferences Section -->
<h2 id="conferences">Conferences</h2>
<p style="color: #b71c1c;"> International and Domestics</p>

{%- for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @inproceedings[year={{y}}]* %}
{% endfor %}

</div>
