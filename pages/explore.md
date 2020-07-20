---
layout: kz-page
title: "What we've learnt so far"
permalink: "/explore/"
teaser: My aim is to make a difference, doing research is just stepping stones on the way. Checking primary sources! Point estimates! We use "about" when it is a guess and we've not yet found the data or suspect it doesn't exist. "the article has not yet been thoroughly fact checked"
header:
  title: ""
  image_fullwidth: landingpage_image.jpg
widgets:
- url: /explore/why-is-this-urgent/
  image: plastic-pollution-beach-by-Jennifer-Lavers.jpg
  title: <a href="/explore/why-is-this-urgent/" target="_self">Why is this urgent?</a>
  text: ...
  anchor: why-is-this-urgent
  button: true
- url: /explore/waste-management-in-indonesia/
  image: indonesia-plastic-pollution-java-cordonpress-dot-com.jpg
  title: <a href="/explore/waste-management-in-indonesia/" target="_self">Waste management in Indonesia</a>
  text: ...
  anchor: waste-management-in-indonesia
  button: true

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
