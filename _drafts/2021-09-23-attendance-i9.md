---
layout: post
title: "i9 attendance"
type: Attendance
---

Attendance sheets for i9 classes . . .

<div class="wrap">
  <ul style="list-style: none;">
    {% for item in site.data.i9-2021[page.type] %}
      <a href="{{ item.link }}" class="stitches_btn">{{ item.class }}</a>
      &nbsp; &nbsp; &nbsp; &nbsp;
      {% assign remainder = forloop.index | modulo: 2 %}
      {% if remainder == 0 %} 
        j</ul>
        <ul style="list-style: none;">
      {% endif %}
    {% endfor %}
  </ul>
</div>
<br>
{% include break-line.html %}
