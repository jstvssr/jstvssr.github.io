---
layout: page
permalink: /publications/
title: publications
description: Publications by year in reversed chronological order.
years: [2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2010, 2009, 2008, 2007, 2006, 2005, 2004, 2003, 2002, 2001, 2000, 1999, 1998, 1997]
---

See also my profile on [Google Scholar](https://scholar.google.com/citations?user=M9bfYFYAAAAJ).

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
