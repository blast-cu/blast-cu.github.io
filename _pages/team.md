---
title: "BLAST - Team"
layout: gridlay
excerpt: "BLAST: Team members"
sitemap: false
permalink: /team/
---

## Group Members


Jump to [PhD students](#phd-students), [Master students](#master-students), [Visitors](#visitors), [Alumni](#alumni)

{% assign number_printed = 0 %}
{% for member in site.data.faculty %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="30%" style="float: left" />
  <h4><a href="{{member.homepage}}">{{ member.name }}</a></h4> 
  <i>{{ member.info }}</i>
  <i>{{ member.info2 }}</i>
  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

### PhD Students

{% assign number_printed = 0 %}
{% for member in site.data.phd %}

{% assign even_odd = number_printed | modulo: 5 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-2 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="100%" style="float: left" />
  <h4><a href="{{member.homepage}}">{{ member.name }}</a></h4>
   <p>{{ member.advised }}</p>

  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 4 %}
</div>
{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 5 %}
{% if even_odd != 0 %}
</div>
{% endif %}


### Master Students 

{% assign number_printed = 0 %}

{% for member in site.data.master %}

{% assign even_odd = number_printed | modulo: 5 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-2 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="100%" style="float: left" />
  <h4><a href="{{member.homepage}}">{{ member.name }}</a></h4> 
  <p>{{ member.info }}</p>

  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 4 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 5 %}
{% if even_odd != 0 %}
</div>
{% endif %}

### Visitors

{% assign number_printed = 0 %}

{% for member in site.data.visitors %}

{% assign even_odd = number_printed | modulo: 5 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-2 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="100%" style="float: left" />
  <h4><a href="{{member.homepage}}">{{ member.name }}</a></h4> 

  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 4 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 5 %}
{% if even_odd != 0 %}
</div>
{% endif %}

### Alumni 
##### *(First Position)*

#### BS Senior Thesis
- [Alexandra Barry](https://www.linkedin.com/in/alexandra-barry1/) (2024-2025). "Evaluating LLM Robustness to Dialectal Variation in Spanish". 
- [Tavin Turner](https://www.ta.vin/) (2024-2025). "Statutory Relational Stance Modeling". *MS Student at the University of Colorado Boulder*.

#### MS Computational Linguistics Capstone Projects
- [Alvin Chen](https://alvin-pc-chen.github.io/) (2024-2025). "Effects of Collaboration on the Performance of Interactive Theme Discovery Systems".
- [Luna Peck](https://github.com/lunaria-bee) (2024-2025). "ConEm: Learning Embedded Concept Representations from LLMs". *PhD Student at the University of British Columbia*. 

#### MS Independent Studies 
- [Denzil Ekow Bilson](https://www.linkedin.com/in/denzilbilson/) (2023-2025) *Machine Learning Engineer at Intuit.*
- [Karthik Sairam](https://karthiksairam01.github.io/) (2025)
- [Ashwin Umadi](https://ashwinumadi.github.io/) (2024-2025). *Software Engineer at Goldman Sachs.*
- [Anirudh Maiya](https://anirudhmaiya.github.io/) (2024-2025). *Software Engineer at Commvault*.
- [Ankush Raut](https://www.linkedin.com/in/ankush-raut-3ab09b113/) (2024-2025). *Applied Scientist at Microsoft*. 
- [Daksha Singhal](https://github.com/sonofposeidon1999) (2024-2025). *Software Engineer at Aurum Data Solutions Inc.*
- [Matt Pauk](https://blast-cu.github.io/team/#phd-students) (2023-2025). *PhD Student at the University of Colorado Boulder*.
- [Aditya Chandra](https://www.linkedin.com/in/acprime96/) (2023-2024). *Software Engineer at Goldman Sachs.*
- [Rohan Das](https://www.rohandas.net/) (2023). *PhD Student at the University of Colorado Boulder*.

#### Informal Student Collaborators
- [Kyle Shi](https://www.linkedin.com/in/kyleshi/), CS Undergraduate Student. *Software Engineer at Uber*.
- [Maksim Seniw](https://maksimseniw.com/), CS Undergraduate Student
- [Brandon Perez](https://www.linkedin.com/in/brandon-a-perez/), CS Undergraduate Student. *MLOps Engineer at Apple.*



