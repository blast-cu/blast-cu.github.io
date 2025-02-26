---
title: "BLAST - Team"
layout: gridlay
excerpt: "BLAST: Team members"
sitemap: false
permalink: /team/
---

## Group Members


Jump to [PhD students](#phd-students), [Master students](#master-students), [Undergraduate students](#undergraduate-students), [Student Collaborators](#informal-student-collaborators), [Alumni](#alumni)

{% assign number_printed = 0 %}
{% for member in site.data.faculty %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4><a href="{{member.homepage}}">{{ member.name }}</a></h4> 
  <i>{{ member.info }}</i>
  <i>{{ member.dept }}</i>
  <i>{{ member.fellow }}</i>
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

### Undergraduate Students

{% assign number_printed = 0 %}
{% for member in site.data.undergrad %}

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

### Informal Student Collaborators
- [Advait Deshmukh](https://advaitdeshmukh.github.io/portfolio/), CS Master Student
- [Ankush Raut](https://www.linkedin.com/in/ankush-raut-3ab09b113/), Data Science Master Student

### Alumni

#### MS Independent Studies

- [Advait Deshmukh](https://advaitdeshmukh.github.io/portfolio/) (2024)
- [Ankush Raut](https://www.linkedin.com/in/ankush-raut-3ab09b113/) (2024) 
- [Aditya Chandra](https://www.linkedin.com/in/acprime96/) (2023-2024)


#### Informal Student Collaborators
- [Kyle Shi](https://www.linkedin.com/in/kyleshi/), CS Undergraduate Student
- [Maksim Seniw](https://maksimseniw.com/), CS Undergraduate Student
- [Brandon Perez](https://www.linkedin.com/in/brandon-a-perez/), CS Undergraduate Student




