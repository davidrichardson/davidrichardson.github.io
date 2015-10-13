---
layout: page
title: Publications
permalink: /publications/
---

<ul>
{% for pub in site.data.publications.resultList.result %}

<li>
<h5><a href="http://europepmc.org/abstract/MED/{{pub.pmid}}">{{pub.title}}</a></h5>

<p>{{pub.authorString}}</p>
<p>{{pub.journalTitle}} Volume {{pub.journalVolume}} ({{pub.pubYear}}) {{pub.pageInfo}} <a href="http://dx.doi.org/{{pub.doi}}">{{pub.doi}}</a></p>

{% endfor %}
</ul>
