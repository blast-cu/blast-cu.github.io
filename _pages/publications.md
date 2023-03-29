---
title: "BLAST - Publications"
layout: gridlay
excerpt: "BLAST -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

Selected papers by BLAST members (Starting July 2022)

### 2022

{% for publi in site.data.publist_2022 %}

  <b>{{ publi.title }}</b> <br />
  {{ publi.authors }} <br />
  <em>{{ publi.venue }}</em> <br />
  <a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  <a href="{{ publi.code.url }}">{{ publi.code.display }}</a>

{% endfor %}

