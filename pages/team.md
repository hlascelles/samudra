---
layout: kz-page
title: Our team
permalink: /team/
header:
  title: ""
  image_fullwidth: landingpage_image.jpg
widgets:
- url: https://www.linkedin.com/in/karina-zile/
  image: team-karina.jpg
  title: <a href="https://www.linkedin.com/in/karina-zile/" target="_blank">Karina Zile</a>
  text: I am the founder of Samudra. Mathematician at heart, I think about any situation as a system of equations. I am happiest when outdoors. After finishing my PhD, I decided to dedicate my life to tackling challenges that don't have a profitable solution.
  anchor: karina 

- image: homepage_image.jpg
  title: "Andu"
  text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.'
  anchor: andu

- image: homepage_image.jpg
  title: "Afsona"
  text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.'
  anchor: afsona

- image: team-join-us.png
  title: Would you like to join us?
  text: Waste management is a truly multidisciplinary affair. Whether you are a chemist, an engineer, a graphic designer, a lawyer, an expert in communications or finance, or simply an awesome individual, we can achieve more with your help. If you like what we are doing, <a href="mailto:hello@samudra.world" target="_blank">let's discuss how we can grow together!</a>
  anchor: you
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
