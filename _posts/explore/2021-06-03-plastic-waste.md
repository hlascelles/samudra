---
layout: kz-page
title: Plastic waste
meta_description: The main ways of processing plastic waste include recycling it back into plastic, producing new materials, and producing plastic-derived liquid fuels. 
header:
  title: ""
  image_fullwidth: landingpage_image.jpg
widgets:
- url: /explore/plastic-recycling/
  image: plastic_recycling.jpg
  title: <a href="/explore/plastic-recycling/" target="_self">Recycling plastic into plastic</a>
- url:
  image: missing_image.jpg
  title: Processing plastic waste into materials
- url:
  image: missing_image.jpg
  title: Processing plastic waste into fuels
categories:
    - explore

---

The main ways of processing plastic waste include recycling it back into plastic, producing new materials, and producing plastic-derived liquid fuels. 


<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>


