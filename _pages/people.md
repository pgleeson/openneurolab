---
title: "People"
layout: gridlay
excerpt: "People"
sitemap: false
permalink: /people
---
# People


<div class="row">
  {% assign people = site.data.people %}

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


# Outreach

## Google Summer of Code

Members of the lab have been actively involved in the [Google Summer of Code](https://summerofcode.withgoogle.com/) program, through the [INCF](https://incf.org) organisation.

## Outreachy

Members of the lab have been mentors in the [Outreachy](https://www.outreachy.org/) program as part of <a href="https://modeci.org">ModECI - the Model Exchange and Convergence Initiative</a>.


<br/>Please <a href="/contact">get in contact</a> if you would like to discuss working with the lab in any of these ways.<br/><br/><br/>