---
layout: page
title: Projects
permalink: /projects/
---

##BLUEPRINT Data Portal

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

##EpiRR

The [International Human Epigenome Consortium](http://ihec-epigenomes.org/) aims to
produce high quality reference epigenomes. Partners in the consortium release their
data to the scientific community through several data archives, including <a href="https://www.ebi.ac.uk/ega"><abbr title="European genome-phenome archive">EGA</abbr></a>, <a href="https://www.ebi.ac.uk/ena"><abbr title="European nucletoide archive">ENA</abbr></a> and <a href="http://www.ncbi.nlm.nih.gov/geo/"><abbr title="Gene expression omnibus">GEO</abbr></a>. The Epigenome Reference Registry (EpiRR)
provides a central point for consortium partners to report their contribution - accessible
epigenome data.

The registry consumes a terse dataset description - a list of experiment IDs is sufficient.
A coherent description of the epigenome is built from IHEC-compliant metadata associated wit the sample and experiment. Documents describing each dataset are served from a [Perl](https://www.perl.org/) [webserver](http://mojolicio.us/) backed by a [MySQL](https://www.mysql.com/) database.

While viewable on-line, [EpiRR](http://www.ebi.ac.uk/vg/epirr/view/all) is primarily intended for use as a REST service, to support the [IHEC data portal](http://epigenomesportal.ca/ihec/). The code is available through [GitHub](https://github.com/EMBL-EBI-GCA/EpiRR).
