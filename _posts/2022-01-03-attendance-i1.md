---
layout: post
title: "i1 attendance"
tags: i1 i2 attendance
comb-att: 1TpS6kArOiGSWMPBZ078ZHYdeUULInIMTnExmMaFaayI
---

Attendance sheets for i1, 2022 classes . . .

<div class="wrap">
  <h2>Full-Time Classes:</h2>
  <ul style="list-style: none;">
    {% for item in site.data.i1-2022.Attnd-FT %}
      <a href="{{ site.gdrive }}{{ item.link }}" class="stitches_btn">{{ item.class }}</a>
      &nbsp; &nbsp; &nbsp; &nbsp;
      {% assign remainder = forloop.index | modulo: 2 %}
      {% if remainder == 0 %} 
        </ul>
        <ul style="list-style: none;">
      {% endif %}
    {% endfor %}
  </ul>
</div>
{% include break-line.html %}

<div class="wrap">
  <h2>Part-Time & Evening Classes:</h2>
  <ul style="list-style: none;">
    {% for item in site.data.i1-2022.Attnd-PT %}
      <a href="{{ site.gdrive }}{{ item.link }}" class="stitches_btn">{{ item.class }}</a>
      &nbsp; &nbsp; &nbsp; &nbsp;
      {% assign remainder = forloop.index | modulo: 2 %}
      {% if remainder == 0 %} 
        </ul>
        <ul style="list-style: none;">
      {% endif %}
    {% endfor %}
  </ul>
</div>
{% include break-line.html %}
<a href="{{ site.gdrive }}{{ page.comb-att }}" class="stitches_btn">Combined i1</a>
{% include break-line.html %}
