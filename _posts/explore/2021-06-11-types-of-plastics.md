---
layout: kz-page
subheadline:
title: Types of plastic
meta_description:
header: no
widgets:
- url: 
  image: missing_image.jpg
  title: <a href="/explore/pp/" target="_self">PP</a>
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

Text...

<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>
