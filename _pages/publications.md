---
title: "Publications"
layout: gridlay
excerpt: "Publications"
sitemap: false
permalink: /publications
---
# Publications


<div class="row">
  {% assign publications = site.data.publications | sort: 'year' | reverse %}

  {% for pub in publications %}
  {% unless person.break %}
  <div class="col-sm-12"> 
  <p></p>
  <p id="{{ pub.title }}">
  <i> {{ pub.title }}</i><br/>{{ pub.authors }}<br/><b>{{ pub.reference }} ({{ pub.year }})</b>
  </p>
  </div>
  {% endunless %}

  {% endfor %}

</div>
