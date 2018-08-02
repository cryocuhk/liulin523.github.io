---
title: "Cryosphere Lab - Photos"
layout: piclay
excerpt: "Cryosphere Lab -- Photos"
permalink: /photos/
---

# Field Pictures
(Right-click *'view image'* to see a larger image.)
## Rock glaciers in the Alps, 2018
By Yan Hu
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/field/yan_alps1.jpg" width="60%">
</figure>

## Old photos
{% assign number_printed = 0 %}
{% for pic in site.data.field_pictures %}

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
