---
title: "Cryosphere Lab - Team"
layout: gridlay
excerpt: "Cryosphere Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Leader

{% assign number_printed = 0 %}
{% for member in site.data.team_lead %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i> 
  <br>
  <a href="http://www.cuhk.edu.hk/sci/essc/people/liu.html"> Personal Webpage </a>
  <br>
  <a href="{{ site.url }}{{ site.baseurl }}/assets/{{ member.cv }}"> CV </a> and  <a href="https://scholar.google.com.hk/citations?user=5VBaQTIAAAAJ&hl=en"> Google Scholar </a>
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

# Group Members

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <br>
  Research interests t1:
  <ul style="overflow: hidden" list-style="circle outside" margin-top="-5px"> 
  {% if member.number_intr == 1 %}
  <li> {{ member.interest1 }} </li>
  {% endif %}
  
  {% if member.number_intr == 2 %}
  <li> {{ member.interest1 }} </li>
  <li> {{ member.interest2 }} </li>
  {% endif %}
  
  {% if member.number_intr == 3 %}
  <li> {{ member.interest1 }} </li>
  <li> {{ member.interest2 }} </li>
  <li> {{ member.interest3 }} </li>
  {% endif %}
  
  {% if member.number_intr == 4 %}
  <li> {{ member.interest1 }} </li>
  <li> {{ member.interest2 }} </li>
  <li> {{ member.interest3 }} </li>
  <li> {{ member.interest4 }} </li>
  {% endif %}
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


 **We are  looking for new PhD students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/openings) **!**


## Alumni
**Graduate Students**<br />
Joseph Ma Ho Yin, MPhi student 2014-2016, now PhD student at National University of Singapore <br />

**Postdocs**<br />
Bao Zhang, Postdoc 2017-2018, now at Wuhan University <br />
Zhiwei Zhou, Postdoc 2017-2018, now at Institute of Geodesy and Geophysics, Chinese Academy of Sciences <br />

**Visitors**<br />
Yufeng Hu, Visiting PhD student 2017-2018, now at Chang'an University <br />
Zhenming Wu, Visiting master student, 2017, now PhD student at Reading University <br />
Jiahui Wang, Visiting undergraduate student, 2017, now PhD student at Southern Methodist University <br />
Yongxin Liu, Visiting undergraduate student, 2017, now Master student at Peking University <br />
Xiaowen Wang, Visiting PhD student 2016-2017, now at University of Tokyo <br />
Wanwan Shao, Visiting PhD student 2016-2017, now at Lanzhou University <br />
Weiyu Zheng, Visiting undergraduate student, 2015, now PhD student at Southern Methodist University <br />
