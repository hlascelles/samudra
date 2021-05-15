---
layout: kz-page
title: Environmental impact of waste
meta_description:
header:
  title: ""
  image_fullwidth: landingpage_image.jpg
widgets:
- url: /explore/old-landfills-uk/
  image: missing_image.jpg
  title: <a href="/explore/old-landfills-uk/" target="_self">Pre-1990s landfills in the UK</a>
categories:
    - explore

---

<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>
