---
layout: kz-page
title: "This is what do"
permalink: /projects/
teaser: blah
header:
  title: ""
  image_fullwidth: landingpage_image.jpg
widgets:
- url: /projects/increasing-waste-collection-in-indonesia/
  image: indonesia_unsafe_landfill_by_thejakartapost_dot_com.png
  title: <a href="/projects/increasing-waste-collection-in-indonesia/" target="_self">Improving the coverage of waste collection services in Indonesia</a>
  text: Blahhh
  anchor: increasing-waste-collection-in-indonesia
  button: true
  cols: 6
- url: /projects/future-projects/
  image: world_wall_by_Karina_Zile.jpg
  title: <a href="/projects/future-projects/" target="_self">What we plan to do next</a>
  text: ...
  anchor: future-projects
  button: true
  cols: 6
---

<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 2 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>
