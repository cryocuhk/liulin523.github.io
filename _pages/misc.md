---
title: "Cryosphere Lab - misc"
layout: textlay
excerpt: "Cryosphere Lab -- misc"
sitemap: false
permalink: /misc
---

This page is under construction.
# Miscellaneous

## Group Meetings
Fall 2018 Schedule (10-11 am, MMW 302)

August 2

August 14

## Educational materials

<a href="{{ site.url }}{{ site.baseurl }}/assets/Wahr_Geodesy.pdf">  Geodesy and Gravity</a>, a class note written by <a href="http://www.johnwahr.com"> John M. Wahr</a>.

## Field photos
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_Leiden %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/field/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>


## Useful links

