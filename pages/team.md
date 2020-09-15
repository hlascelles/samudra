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
  text: I am the founder of Samudra. Mathematician at heart, I think about any situation as a system of equations. I am happiest when outdoors. After finishing my PhD, I decided to dedicate my life to tackling global challenges that don't have a profitable solution.
  anchor: karina 

- url: https://www.linkedin.com/in/lawrenceyeh/
  image: team-lawrence.jpg
  title: <a href="https://www.linkedin.com/in/lawrenceyeh/" target="_blank">Lawrence Yeh</a>
  text: "I often think about how well we understand each other in a society, and how we may improve our lives if we were better at communicating. Sometimes I get a little overwhelmed when trying to convey an idea, especially given my instincts to optimize everything. One remedy I have relied on is to retreat to nature and delve into the marvellous wonders of the world."
  anchor: lawrence

- url: https://www.linkedin.com/in/afsona-bonu/
  image: team-afsona.jpg
  title: <a href="https://www.linkedin.com/in/afsona-bonu/" target="_blank">Afsona-Bonu Mansurova</a>
  text: "I was born a believer in the idea that everyone deserves a decent livelihood and that we ourselves can be the magic wand to make a change. The more I travelled around the world, the more I studied and volunteered, I realised that I want to do more to join the common efforts in making this world a better place for all."
  anchor: afsona

- image: team-join-us.jpg
  title: Would you like to join us?
  text: Waste management is a truly multidisciplinary affair. Whether you are a chemist, an engineer, a graphic designer, a lawyer, an expert in communications or finance, or simply an awesome individual, we can achieve more with your help. If you like what we do, <a href="mailto:hello@samudra.world" target="_blank">let's discuss how we can grow together!</a>
  anchor: you
---

We are a diverse bunch of people. Each of us has a strong desire to make the world a better place, this common goal makes us a strong team. If you share a similar passion, <a href="mailto:hello@samudra.world" target="_blank">let's discuss how we can grow together!</a>

<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>
