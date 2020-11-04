---
layout: kz-page
title: Waste disposal methods
meta_description:
header:
  title: ""
  image_fullwidth: landingpage_image.jpg
widgets:
- url: /explore/incineration/
  image: waste-grabber-in-action.jpg
  title: <a href="/explore/incineration/" target="_self">Incineration</a>
  text: Incineration is one of the methods of thermal treatment of waste.
  anchor: incineration
categories:
    - explore
show_meta: false
---

There are different waste disposal methods.

<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>