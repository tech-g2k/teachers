---
layout: post
title: "i6 attendance"
tags: i6 attendance
comb-att: 1BSxC8jq47vkHZlqglbhsawaxQAogIvb9IAvuY-qTthA
---

Attendance sheets for i6, 2022 classes ...

<div class="wrap">
  <h2>Full-Time, CS & KS Classes:</h2>
  <ul style="list-style: none;">
    {% for item in site.data.Y2022-i5.Attnd-FT-i6 %}
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
    {% for item in site.data.Y2022-i5.Attnd-PT %}
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
<a href="{{ site.gdrive }}{{ page.comb-att }}" class="stitches_btn">Combined i5 & i6</a>
{% include break-line.html %}
