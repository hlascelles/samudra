---
layout: kz-page
title: "This is what we are working on"
permalink: "/projects/"
header:
    image_fullwidth: "homepage_image.jpg"
widget1:
  url: 'https://stopplasticpollution.io/projects/waste-management-in-indonesia'
  image: homepage_image.jpg
  title: "Expanding waste collection services in Indonesia"
  text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.'
  cols: 6
  button: true
  
widget2:
  url: 'https://stopplasticpollution.io/projects/future-projects'
  image: homepage_image.jpg
  title: "Future projects"
  text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.'
  cols: 6
  button: true
---

{% include _frontpage-widget.html widget=page.widget1 %}
{% include _frontpage-widget.html widget=page.widget2 %}

{% comment %}
When adding another one here, if it "floats off to the right" then you may have to make sure the title
is shorter!
{% endcomment %}
