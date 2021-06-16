---
layout: kz-page
subheadline:
title: Types of plastic
meta_description:
header: no
widgets:
- url: /explore/pp/
  image: pp.jpg
  title: <a href="/explore/pp/" target="_self">Polypropylene (PP), 75 million tonnes</a>
- url: /explore/pe/
  image: missing_image.jpg
  title: <a href="/explore/pe/" target="_self">Polyethylene (PE) <br> 103 million tonnes</a>
- url: 
  image: missing_image.jpg
  title: <a href="/explore/pvc/" target="_self">PVC</a>
- url: /explore/pet/
  image: pet.jpg
  title: <a href="/explore/pet/" target="_self">Polyethylene terephthalate (PET), 30-45 million tonnes</a>
categories:
    - explore

---

About [368 million tonnes][1] of plastic wete produced in 2019. 


<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>

[1]: https://www.plasticseurope.org/en/resources/publications/4312-plastics-facts-2020
