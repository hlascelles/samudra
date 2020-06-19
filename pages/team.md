---
layout: kz-page
title: "Our team"
permalink: "/team/"
header:
    image_fullwidth: "homepage_image.jpg"
widget1:
  url: 'https://www.linkedin.com/in/karina-zile/'
  image: homepage_image.jpg
  title: "Karina Zile"
  text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.'
widget2:
  image: homepage_image.jpg
  title: "Andu"
  text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.'
widget3:
  image: homepage_image.jpg
  title: "Afsona"
  text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.'
widget4:
  image: homepage_image.jpg
  title: "Would you like to join us?"
  text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.'
---

{% include _frontpage-widget.html widget=page.widget1 %}
{% include _frontpage-widget.html widget=page.widget2 %}
{% include _frontpage-widget.html widget=page.widget3 %}
<br/>
{% include _frontpage-widget.html widget=page.widget4 %}
