---
layout: page
permalink: /publications/
title: publications
description:
preyears: [2020]
jyears: [2013]
cyears: [2020, 2019, 2016, 2013]
wyears: [2019, 2018]
nav: true
---

<h2>Preprints</h2> 
<div class="publications">  
{% for y in page.preyears %}   
   <h2 class="year">{{y}}</h2>   
   {% bibliography -f preprint -q @*[year={{y}}]* %} 
{% endfor %}  

</div>

<h2>Journals</h2> 
<div class="publications">  
{% for y in page.jyears %}   
   <h2 class="year">{{y}}</h2>   
   {% bibliography -f journals -q @*[year={{y}}]* %} 
{% endfor %}  

</div>

<h2>Conferences</h2> 
<div class="publications">  
{% for y in page.cyears %}   
   <h2 class="year">{{y}}</h2>   
   {% bibliography -f conferences -q @*[year={{y}}]* %} 
{% endfor %}  

</div>

<h2>Workshops</h2> 
<div class="publications">  
{% for y in page.wyears %}   
   <h2 class="year">{{y}}</h2>   
   {% bibliography -f workshops -q @*[year={{y}}]* %} 
{% endfor %}  

</div>






