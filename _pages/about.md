---
permalink: /
title: "Yubo Zhang"
author_profile: true
redirect_from:
  - /about/
  - /about.html
  - /cv/
  - /cv
  - /resume
---

Yubo Zhang (张玉波) is an Associate Professor at [Minjiang University](https://www.mju.edu.cn/), in the [Minjiang Collaborative Center for Theoretical Physics](https://wdxy.mju.edu.cn/llwlxzzx/), Fuzhou, China.

He studies complex magnetic materials from first principles, and he develops density-functional theory methods.

## Education

* Ph.D. in Optics, Department of Physics, Harbin Institute of Technology, September 2008 – July 2012
* M.Sc. in Optics, Department of Physics, Harbin Institute of Technology, September 2006 – July 2008
* B.Eng. in Optical Information Science and Technology, Shandong University, September 2002 – July 2006

## Appointments

* January 2022 – present: Associate Professor, Minjiang University
* November 2018 – December 2021: Research Associate Professor, Southern University of Science and Technology
* August 2016 – September 2018: Postdoctoral researcher, University of Texas / Tulane University. Advisors: Jianwei Sun and Professor John Perdew
* December 2014 – July 2016: Postdoctoral researcher, Temple University. Advisor: Professor Xifan Wu
* July 2012 – December 2014: Postdoctoral researcher, Shanghai Institute of Ceramics, Chinese Academy of Sciences. Advisor: Professor Wenqing Zhang

## Research

* First-principles studies of complex magnetic materials
* Development of density-functional theory methods

## Honors

* 2021–2024: World's Top 2% Scientists annual list
* 2026: Fujian Province Class B Talent
* 2022: Fujian Province Class C Talent
* 2020: Shenzhen Peacock Team, Overseas Young Talent Team
* 2020: Guangdong Pearl River Talent Program, Young Talent Team
* 2019: Shenzhen Peacock Plan, Class C Talent

## Grants

* 2026: National Natural Science Foundation of China, General Program. Density-functional theory study of stripe phases in cuprates
* 2026: Fujian provincial general project. Design and physical properties of Heusler semiconductors for thermoelectric applications
* 2024: Principal investigator, Shanghai Jiao Tong University project. Phase-transition mechanism of Ca<sub>3</sub>Ru<sub>2</sub>O<sub>7</sub>
* 2021: Guangdong provincial general project. Multiscale theoretical study of carrier control in two-dimensional van der Waals magnetic materials
* 2020: National Natural Science Foundation of China, Young Scientists Fund. First-principles design and control of magnetic configurations in SrTMO<sub>3</sub> (TM = Ti/Ru/Ir) heterostructures
* 2020: Shenzhen municipal general project. Design of perpendicularly magnetized two-dimensional magnetic materials for anticancer-drug applications
* 2020: Core member (responsible for the first-principles research), Guangdong Pearl River Talent Program innovation and entrepreneurship team. Novel ultrathin low-dimensional magnetic materials and their applications
* 2020: Core member (responsible for the first-principles research), Shenzhen Peacock Team overseas young-talent team. Design and applications of ultrathin magnetic materials
* 2018: Tulane University LBGrants Program. Vibrational properties of cuprates with SCAN
* 2012: China Postdoctoral Science Foundation, 52nd batch general grant. Theoretical design and performance optimization of novel copper-based intermediate-band photovoltaic materials

## Publications

{% if site.author.googlescholar %}
You can also find my articles on [my Google Scholar profile]({{ site.author.googlescholar }}).
{% endif %}

\* corresponding author. # co-first author.

{% if site.publication_category %}
  {% for category in site.publication_category %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
<h2>{{ category[1].title }}</h2>
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}
