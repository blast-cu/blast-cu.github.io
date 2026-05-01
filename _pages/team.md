---
title: "BLAST - Team"
layout: gridlay
excerpt: "BLAST: Team members"
sitemap: false
permalink: /team/
---

## Group Members


Jump to [PhD students](#phd-students), [Affiliates](#affiliated-student-collaborators), [Alumni](#alumni)


{% for member in site.data.faculty %}
<div class="row">
<div class="col-xs-6 col-sm-2">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="100%" style="float: left" />
</div>
<div class="row">
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

### Affiliated Student Collaborators
{% for member in site.data.collaborators -%}
- [{{ member.name }}]({{ member.homepage }}), {{ member.position }}, {{ member.institution }}
{% endfor %}


### Alumni 
##### *(First Position)*

#### Master's Students
{% for member in site.data.alumni_ms -%}
- [{{ member.name }}]({{ member.homepage }}) ({{ member.period }}). *{{ member.position }}*
{% endfor %}

#### Undergraduate Students
{% for member in site.data.alumni_bs -%}
- [{{ member.name }}]({{ member.homepage }}) ({{ member.period }}). *{{ member.position }}*
{% endfor %}

#### Past Affiliates/Collaborators
{% for member in site.data.alumni_collaborators -%}
- [{{ member.name }}]({{ member.homepage }}), {{ member.affiliation }} ({{ member.period }}). *{{ member.position }}*
{% endfor %}



