---
title: "BLAST - Team"
layout: gridlay
excerpt: "BLAST: Team members"
sitemap: false
permalink: /team/
---

## Group Members


Jump to [PhD students](#phd-students), [Master students](#master-students), [Affiliates](#affiliated-student-collaborators), [Alumni](#alumni)

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

{% assign even_odd = number_printed | modulo: 6 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-xs-6 col-sm-2 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="100%" style="float: left" />
  <h4><a href="{{member.homepage}}">{{ member.name }}</a></h4>
   <p>{{ member.advised }}</p>

  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 5 %}
</div>
{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 6 %}
{% if even_odd != 0 %}
</div>
{% endif %}


### Master Students 

{% assign number_printed = 0 %}

{% for member in site.data.master %}

{% assign even_odd = number_printed | modulo: 6 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-xs-6 col-sm-2 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="100%" style="float: left" />
  <h4><a href="{{member.homepage}}">{{ member.name }}</a></h4> 

  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 5 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 6 %}
{% if even_odd != 0 %}
</div>
{% endif %}


### Affiliated Student Collaborators
- [Juan Vasquez](https://juan-vasquez.com/), CS PhD Student, University of Colorado Boulder
- [Advait Deshmukh](https://advaitdeshmukh.com/), CS PhD Student, University of Colorado Boulder
- [Zohar Naaman](https://www.linkedin.com/in/zoharnaaman/), MS Linguistics Student, University of Colorado Boulder
- [Niklas Hofstetter](https://www.linkedin.com/in/niklas-hofstetter-1662441b2/), BS Student, St. Pölten University of Applied Sciences

### Alumni 
##### *(First Position)*

#### MS Students
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



