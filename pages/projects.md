---
layout: kz-page
title: "This is what we do"
permalink: /projects/
teaser: Our goals are to reduce the environmental pollution and greenhouse gas emissions associated with waste, and to minimise the impact of waste on human health. We aim to design projects with the highest estimated impact. In depth research guides everything we do. Learn more about our current and upcoming projects below.
header:
  title: ""
  image_fullwidth: landingpage_image.jpg
widgets:
- url: /projects/increasing-waste-collection-in-indonesia/
  image: indonesia_unsafe_landfill_by_thejakartapost_dot_com.png
  title: '<a href="/projects/increasing-waste-collection-in-indonesia/" target="_self">Current project: Improving the coverage of waste collection services in Indonesia</a>'
  text: Only 32% of municipal solid waste is currently collected in Indonesia. Uncollected waste is either openly burnt (leading to adverse effects on air quality) or dumped (facilitating the spread of disease vectors and contagious diseases). Dumped waste is likely to end up in our oceans. The aim of this project is to increase the proportion of municipal solid waste that is collected and to ensure that it is properly dispossed of.
  anchor: increasing-waste-collection-in-indonesia
  button: true
  cols: 6
- url: /projects/future-projects/
  image: world_wall_by_Karina_Zile.jpg
  title: <a href="/projects/future-projects/" target="_self">What we plan to do next</a>
  text: In the near future we plan to initiate projects focussed on different stages of the waste management process - from informing the design of products that will eventually become waste to new recycling techniques and international waste trade. These projects will be guided by the in depth research we do. Many waste management challenges are similar in different countries all across the globe; therefore we will increase our impact by sharing what we've learnt and actively learning from others.
  anchor: future-projects
  button: true
  cols: 6
---

<hr style="height:1px; visibility:hidden;" />
<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 2 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>
