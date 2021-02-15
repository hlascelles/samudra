---
layout: kz-page
title: "This is what we do"
permalink: /projects/
subheadline: Waste management for our planet and people, not profit
teaser: "Our goals are to reduce the environmental pollution and greenhouse gas emissions associated with waste, and to minimise the impact of waste on human and animal health. Here is what we do to achieve these goals:"
header:
  title: ""
  image_fullwidth: landingpage_image.jpg
widgets:
- url:
  image: lawma.jpg
  title: Collaboration with LAWMA
  location: Lagos, Nigeria
  dates: Since Jan 2021
  text: LAWMA (Lagos Waste Management Authority) is developing a new waste management system for Lagos, a city of more than 22 million people. I am exploring technologies, partnerships and funding mechanisms that could be appropriate for this context.
- url:
  image: pyro-degrade.jpg
  title: Collaboration with Pyro-degrade Energy
  location: Nairobi, Kenya
  dates: Since Jan 2021
  text: Pyro-degrade Energy developed technology to process plastic waste into pyrolysis oil - an affordable fuel that can be used instead of diesel. This fuel is environmentally friendly due to its low sulfur content. I am helping them with fundraising for their first industrial scale plant.
- url:
  image: gikoko.jpg
  title: Consulting for Gikoko Kogyo Indonesia
  location: Jakarta, Indonesia
  dates: Jan-Feb 2021
  text: I helped with greenhouse gas emissions reductions calculations to evaluate a municipal solid waste infrastructure building project involving multiple technologies. The proposed project included waste sorting and shredding machinery powered by in-house refuse-derived fuel, an anaerobic digestion system and other technologies.
- url:
  image: green-worms.jpg
  title: Collaboration with Green Worms
  location: Kerala, India
  dates: Since Dec 2020 
  text: Green Worms introduce waste collection services in small coastal towns in India. I am helping them with developing external communications strategy. My goals are to improve their engagement with stakeholders and to assist with initiating collaborations with organisations outside India.
- url:
  image: forbi.jpg
  title: Collaboration with Forbi Perise Eyong Nyosai
  location: Buea, Cameroon
  dates: Sep-Dec 2020
  text: Forbi's goal was to kickstart a PET bottle collection scheme in schools in Buea, Cameroon to both increase the plastic recycling rate in the country and to educate kids about waste related challenges. I helped Forbi with writing the project proposal, making a budget and the application process.
---

<hr style="height:1px; visibility:hidden;" />
<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>


