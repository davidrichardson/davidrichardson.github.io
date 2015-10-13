---
layout: page
title: Projects
permalink: /projects/
---

##Blueprint Data Portal

The [BLUEPRINT epigenome](http://www.blueprint-epigenome.eu/) project has made a
large amount of data available through an <a href="http://ftp.ebi.ac.uk/pub/databases/blueprint"><abbr title="File transfer protocol">FTP
</abbr> site</a>, and the <a href="https://www.ebi.ac.uk/ega/dacs/EGAC00001000135"><abbr title="European genome-phenome archive">EGA</abbr></a>. I created the project [data
portal](http://dcc.blueprint-epigenome.eu/) to help scientists find data relevant to their interests.

The site was developed during summer 2014, starting from an initial prototype based on [facetedsearch.js](https://eikes.github.io/facetedsearch/), to a fully functional
site over a few weeks. Server-side engineering was kept to minimum, with the data
served as static <a href="https://en.wikipedia.org/wiki/JSON"><abbr title="JavaScript Object Notation">JSON</abbr></a> files from an [Apache](http://www.apache.org/) server.
The client-side code is based on [AngularJS](https://angularjs.org/), and the
styling based on [bootstrap CSS](http://getbootstrap.com/).

The design has been built upon further for the [HipSci](http://www.hipsci.org/)
project, by my colleague Ian Streeter. The HipSci portal uses [ElasticSearch](https://www.elastic.co/products/elasticsearch) to provide sophisticated document search features. 
