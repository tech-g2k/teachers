---
layout: post
title: "i4 attendance"
tags: i4 attendance
comb-att: 1N_v-XKYwk8Bj5vrUn0ZfD0ikf282xLxG1b53e0vxELg
---

Attendance sheets for i4, 2022 classes ...

<div class="wrap">
  <h2>Full-Time Classes:</h2>
  <ul style="list-style: none;">
    {% for item in site.data.Y2022-i3.Attnd-FT-i4 %}
      <a href="{{ site.gdrive }}{{ item.link }}" class="stitches_btn">{{ item.class }}</a>
      &nbsp; &nbsp; &nbsp; &nbsp;
      {% assign remainder = forloop.index | modulo: 3 %}
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
    {% for item in site.data.Y2022-i3.Attnd-PT %}
      <a href="{{ site.gdrive }}{{ item.link }}" class="stitches_btn">{{ item.class }}</a>
      &nbsp; &nbsp; &nbsp; &nbsp;
      {% assign remainder = forloop.index | modulo: 3 %}
      {% if remainder == 0 %} 
        </ul>
        <ul style="list-style: none;">
      {% endif %}
    {% endfor %}
  </ul>
</div>
{% include break-line.html %}
<a href="{{ site.gdrive }}{{ page.comb-att }}" class="stitches_btn">Combined i3 & i4</a>
{% include break-line.html %}
