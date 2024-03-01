---
title: "BLAST - Publications"
layout: gridlay
excerpt: "BLAST -- Publications."
sitemap: false
permalink: /publications/
---


## Publications

Papers by BLAST members (Starting July 2022)

### Pre-prints

{% for publi in site.data.publist_preprint %}

  <b>{{ publi.title }}</b> ( {{ publi.year }} ) <br />
  {{ publi.authors }} <br />
  <a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  <a href="{{ publi.code.url }}">{{ publi.code.display }}</a>
{% endfor %}

### 2023

{% for publi in site.data.publist_2023 %}

  <b>{{ publi.title }}</b> <br />
  {{ publi.authors }} <br />
  <em>{{ publi.venue }}</em> <br />
  <a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  <a href="{{ publi.code.url }}">{{ publi.code.display }}</a>

{% endfor %}

### 2022

{% for publi in site.data.publist_2022 %}

  <b>{{ publi.title }}</b> <br />
  {{ publi.authors }} <br />
  <em>{{ publi.venue }}</em> <br />
  <a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  <a href="{{ publi.code.url }}">{{ publi.code.display }}</a>

{% endfor %}

Click [here](https://mlpacheco.github.io/publications/) for prior publications.
