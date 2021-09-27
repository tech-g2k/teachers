---
layout: post
title: "i9 attendance"
tags: i9 attendance
all-att: 1TpS6kArOiGSWMPBZ078ZHYdeUULInIMTnExmMaFaayI
---

Attendance sheets for i9 classes . . .

<div class="wrap">
  <ul style="list-style: none;">
    {% for item in site.data.i9-2021.Attendance %}
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
<br>
{% include break-line.html %}

<a href="{{ site.gdrive }}{{ page.all-att }}" class="stitches_btn">Combined i9</a>
