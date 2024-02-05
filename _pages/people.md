---
title: "People"
layout: gridlay
excerpt: "People"
sitemap: false
permalink: /people
---
# People


<div class="row">
  {% assign people = site.data.people | sort: 'name' %}

  {% for person in people %}
  {% unless person.break %}
  <div class="col-sm-12"> 
  <p></p>
  <h2 id="{{ person.name }}">
  {{ person.name }}<i>{% if person.title %}: {{ person.title }}{% endif %}</i>
  </h2>
  <p>  
  {% if person.photo %}
  <img src="{{ site.url }}{{ site.baseurl }}/images/people/{{ person.photo }}" style="width: 250px; float: right">
  {% endif %}
  {{ person.abstract }}
  </p>
  </div>
  {% endunless %}

  {% endfor %}

</div>



## GSoC

## Outreachy

