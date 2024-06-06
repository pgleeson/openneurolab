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
  <i> {% if pub.url %}<b><a href="{{ pub.url }}">{{ pub.title }}</a></b> {% else %}{{ pub.title }} {% endif %} </i><br/>{{ pub.authors }}<br/><b>{{ pub.reference }} ({{ pub.year }})</b> {% if pub.extra %}<br/>{{ pub.extra }}{% endif %}
  </p>
  </div>
  {% endunless %}

  {% endfor %}

</div>
