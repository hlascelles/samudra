---
layout: kz-page
title: Landfills and dumpsites
meta_description:
header:
  title: ""
  image_fullwidth: landingpage_image.jpg
widgets:
- url: /explore/landfill-mining/
  image: landfill-mining.jpg
  title: <a href="/explore/landfill-mining/" target="_self">Landfill mining</a>  
- url: /explore/old-landfills-uk/
  image: breached_landfill_East_Tilbury.jpg
  title: <a href="/explore/old-landfills-uk/" target="_self">Historic landfills in the UK</a>
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

