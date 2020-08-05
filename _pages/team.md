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

<div class="col-sm-7 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/people/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h3>{{ member.name }}</h3>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i> 
  <br>
  <a href="http://www.cuhk.edu.hk/sci/essc/people/liu.html"> Department Webpage </a>
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

<div class="col-sm-7 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/people/{{ member.photo }}" class="img-responsive" width="24%" style="float: left" />
  <h3>{{ member.name }}</h3>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i> {% if member.addcv == 1 %} <br><a href="{{ site.url }}{{ site.baseurl }}/assets/{{ member.cv }}"> CV </a> {% endif %}
  <p class="mb-0"> Research interests:</p>
  <ul style="overflow: hidden" padding-left="0em" margin-top="-10px">
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
  <br>
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


 **We are looking for new PhD students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/openings) **!**

## Alumni
**Graduate Students**<br />
Lingcao Huang, PhD student 2016-19, now Postdoc at CUHK <br />
Jie Chen, PhD student 2015-19, now Postdoc at Chinese Academy of Sciences <br />
Joseph Ma Ho Yin, MPhil student 2014-16, now PhD student at National University of Singapore <br />

**Postdocs**<br />
Guoyan Jiang, 2017-19, jointly supervised with Prof. T-f Wong, now Research Professor at Wuhan University <br />
Jiangjun Ran, 2018, now Assitant Professor at Southern University of Science and Technology <br />
Bao Zhang, 2017-18, now at Wuhan University <br />
Zhiwei Zhou, 2017-18, now Associate Researcher at Institute of Geodesy and Geophysics, Chinese Academy of Sciences <br />
Bo Hu, 2015, now faculty at Guangdong University of Technology <br />

**Research Assistants**<br />
Yufeng Hu, 2017-18, now Lecturer at Chang'an University <br />
Kenneth Ho Ngai Lun, 2017-18, now Research Assistant at Queen Mary Hospital <br />
Xiaowen Wang, 2016-17, now Associate Professor at Southwest Jiaotong University <br />

**Undergraduate Students (Final-year Project Advisees)**<br />
Yue Wu, 2017, now PhD student at University of Texas at Austin <br />
Michelle Yip Man Wai, 2016, now MPhil student at University of Hong Kong <br />

**Visiting Students**<br />
Linyang Xin, 2019, now master student at Wuhan University <br />
Yidan Ding and Haoran Wang, 2019, now master students at Jilin University <br />
Weifan Zhou, 2018, now master student at Jilin University <br />
Zhenming Wu, 2017, now PhD student at Reading University <br />
Jiahui Wang, 2017, now PhD student at Southern Methodist University <br />
Yongxin Liu, 2017 <br />
Wanwan Shao, Visiting PhD student 2016-17, now PhD student at Lanzhou University <br />
Weiyu Zheng, 2015, now PhD student at Southern Methodist University <br />
