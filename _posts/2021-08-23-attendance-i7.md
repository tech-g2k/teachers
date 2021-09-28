---
layout: post
title: "i7 attendance"
tags: i7 attendance
comb-att: 1RPevOdeCOYU22JiPCe2WpVwVTIMKtR_3J1WVdELQTPU
---

Attendance sheets for all the classes . . .

<div class="wrap">
  <h2>Full-Time Classes:</h2>
    <ul style="list-style: none;">
        {% for item in site.data.i7-2021.Attendance-FT %}
            <a href="{{ item.link }}" class="stitches_btn">{{ item.class }}</a>
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
<div class="wrap">
  <h2>Part-Time & Evening Classes:</h2>
  <ul style="list-style: none;">
    {% for item in site.data.i7-2021.Attendance-PT %}
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
<a href="{{ site.gdrive }}{{ page.comb-att }}" class="stitches_btn">Combined i7</a>
{% include break-line.html %}
