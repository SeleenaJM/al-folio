---
layout: page
permalink: /publications/
title: publications
description:
cyears: [2020, 2019, 2018, 2016, 2013]
nav: true
---


<div class="publications">  
{% for y in page.cyears %}   
   <h2 class="year">{{y}}</h2>   
   {% bibliography -f conferences -q @*[year={{y}}]* %} 
{% endfor %}  

</div>


