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
Thermal treatment methods significantly reduce the volume of the waste and allow to recover the calorific value of the waste in a form of energy. 
Due to this second property, these methods are often referred to as waste-to-energy or energy-from-waste.
[Incineration][1], waste combustion in the presence of oxygen, is the only method currently widely used on an industrial scale. 
Other methods, gasification and pyrolysis, are known as advanced thermal treatment methods. 
Thermal treatment methods, similarly to landfilling, are not a substitute for recycling, composting or anaerobic digestion; these methods are used to treat waste that cannot be used otherwise. 


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