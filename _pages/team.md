---
title: "BLAST - Team"
layout: gridlay
excerpt: "BLAST: Team members"
sitemap: false
permalink: /team/
---

## Group Members


Jump to [PhD students](#phd-students), [Master's students](#master-students), [Affiliates](#affiliated-student-collaborators), [Alumni](#alumni)


{% for member in site.data.faculty %}
<div class="row">
<div class="col-xs-6 col-sm-2">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="100%" style="float: left" />
  <h4><a href="{{member.homepage}}">{{ member.name }}</a></h4> 
  <i>{{ member.info }}</i>
  <ul style="overflow: hidden">
  </ul>
</div>
</div>
{% endfor %}

### PhD Students

<div class="row">
{% assign number_printed = 0 %}
{% for member in site.data.phd %}

<div class="col-xs-6 col-sm-2">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="100%" style="float: left" />
  <h4><a href="{{member.homepage}}">{{ member.name }}</a></h4>
   <p>{{ member.advised }}</p>

  <ul style="overflow: hidden">

  </ul>
</div>
{% assign number_printed = number_printed | plus: 1 %}

{%- comment -%}
  Break rows on XS: 2 per row (col-xs-6)
{%- endcomment -%}
{% assign xs_mod = number_printed | modulo: 2 %}
{% if xs_mod == 0 %}
  <div class="clearfix visible-xs-block"></div>
{% endif %}

{%- comment -%}
  Break rows on SM+: 6 per row (col-sm-2)
{%- endcomment -%}
{% assign sm_mod = number_printed | modulo: 6 %}
{% if sm_mod == 0 %}
  <div class="clearfix visible-sm-block visible-md-block visible-lg-block"></div>
{% endif %}

{% endfor %}
</div>

### Master's Students 

<div class="row">
{% assign number_printed = 0 %}
{% for member in site.data.master %}

<div class="col-xs-6 col-sm-2">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="100%" style="float: left" />
  <h4><a href="{{member.homepage}}">{{ member.name }}</a></h4>
  <ul style="overflow: hidden">
  </ul>
</div>
{% assign number_printed = number_printed | plus: 1 %}

{%- comment -%}
  Break rows on XS: 2 per row (col-xs-6)
{%- endcomment -%}
{% assign xs_mod = number_printed | modulo: 2 %}
{% if xs_mod == 0 %}
  <div class="clearfix visible-xs-block"></div>
{% endif %}

{%- comment -%}
  Break rows on SM+: 6 per row (col-sm-2)
{%- endcomment -%}
{% assign sm_mod = number_printed | modulo: 6 %}
{% if sm_mod == 0 %}
  <div class="clearfix visible-sm-block visible-md-block visible-lg-block"></div>
{% endif %}

{% endfor %}
</div>

### Affiliated Student Collaborators
- [Juan Vasquez](https://juan-vasquez.com/), CS PhD Student, University of Colorado Boulder
- [Advait Deshmukh](https://advaitdeshmukh.com/), CS PhD Student, University of Colorado Boulder
- [Zohar Naaman](https://www.linkedin.com/in/zoharnaaman/), MS Linguistics Student, University of Colorado Boulder
- [Niklas Hofstetter](https://www.linkedin.com/in/niklas-hofstetter-1662441b2/), BS Student, St. Pölten University of Applied Sciences

### Alumni 
##### *(First Position)*

#### Master's Students
- [Bagyasree Sudharsan](https://bagyasree.com/) (2024-2025)
- [Advait Deshmukh](https://advaitdeshmukh.com/) (2024-2025). *PhD Student at the University of Colorado Boulder.*
- [Alvin Chen](https://alvin-pc-chen.github.io/) (2024-2025)
- [Luna Peck](https://github.com/lunaria-bee) (2024-2025). *PhD Student at the University of British Columbia.*
- [Denzil Ekow Bilson](https://www.linkedin.com/in/denzilbilson/) (2023-2025). *Machine Learning Engineer at Intuit.*
- [Karthik Sairam](https://karthiksairam01.github.io/) (2025)
- [Ashwin Umadi](https://ashwinumadi.github.io/) (2024-2025). *Software Engineer at Goldman Sachs.*
- [Anirudh Maiya](https://anirudhmaiya.github.io/) (2024-2025). *Software Engineer at Commvault*.
- [Ankush Raut](https://www.linkedin.com/in/ankush-raut-3ab09b113/) (2024-2025). *Applied Scientist at Microsoft*. 
- [Daksha Singhal](https://github.com/sonofposeidon1999) (2024-2025). *Software Engineer at Aurum Data Solutions Inc.*
- [Matt Pauk](https://blast-cu.github.io/team/#phd-students) (2023-2025). *PhD Student at the University of Colorado Boulder*.
- [Aditya Chandra](https://www.linkedin.com/in/acprime96/) (2023-2024). *Software Engineer at Goldman Sachs.*
- [Rohan Das](https://www.rohandas.net/) (2023). *PhD Student at the University of Colorado Boulder*.

#### Undergraduate Students
- [Alexandra Barry](https://www.linkedin.com/in/alexandra-barry1/) (2024-2025)
- [Tavin Turner](https://www.ta.vin/) (2024-2025). *MS Student at the University of Colorado Boulder*.

#### Past Affiliates/Collaborators
- [Kyle Shi](https://www.linkedin.com/in/kyleshi/), CS Undergraduate Student (2024). *Software Engineer at Uber*.
- [Maksim Seniw](https://maksimseniw.com/), CS Undergraduate Student (2024). *Software Engineer at Spectrum.*
- [Brandon Perez](https://www.linkedin.com/in/brandon-a-perez/), CS Undergraduate Student (2024). *MLOps Engineer at Apple.*



