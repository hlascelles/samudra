---
layout: kz-page
title: Waste disposal methods
meta_description:
permalink: "/explore/waste_disposal_methods/"
header:
  title: ""
  image_fullwidth: landingpage_image.jpg
widgets:
- url: /explore/incineration/
  image: incinerator-diagram.jpg
  title: <a href="/explore/incineration/" target="_self">Incineration (in theory)</a>
- url:
  image: waste-grabber-in-action.jpg
  title: Incineration (in practice)
- url:
  image: pyrolysis.jpg
  title: Pyrolysis
- url:
  image: gasification.jpg
  title: Gasification

---

Waste disposal methods are not substitutes for recycling, these methods are used to treat waste that cannot be used otherwise. 
Thermal treatment methods significantly reduce the volume of the waste and destroy all pathogens present in it. 
These methods allow to recover the calorific value of the waste in a form of energy, hence they are often referred to as waste-to-energy or energy-from-waste.
[Incineration][1], waste combustion in the presence of oxygen, is the only method currently widely used on an industrial scale. 
Pyrolysis, gasification and plasma arc gasification are known as advanced thermal treatment methods. 

<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>


[1]: /explore/incineration