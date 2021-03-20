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
  image: elmar.jpg
  title: Collaboration with ELMAR
  location: England, UK
  dates: Since Mar 2021
  text: Ecological Landfill Mining and Recycling (ELMAR) is a non-profit dedicated to tackling 1,264 landfills in the UK that have been breached and are leaking toxic pollution into the water bodies. I am helping with research on technologies for landfill mining and processing of plastic waste from legacy sites, and with identifying potential strategic partnerships.
- url:
  image: pes.jpg
  title: Collaboration with Premier Enviro Solutions
  location: Freetown, Sierra Leone
  dates: Since Feb 2021
  text: Premier Enviro Solutions is a social enterprise with a mission to provide innovative, sustainable and affordable waste management solutions. I am helping them with projects related to processing plastic waste into building blocks, and safe disposal of medical waste.
- url:
  image: lawma.jpg
  title: Collaboration with LAWMA
  location: Lagos, Nigeria
  dates: Since Jan 2021
  text: Lagos Waste Management Authority (LAWMA) is developing a new waste management strategy for Lagos, a city of more than 22 million people. I am advising them on technologies, partnerships and funding mechanisms that could be appropriate for this city.
- url:
  image: pyro-degrade.jpg
  title: Collaboration with Pyro-degrade Energy
  location: Nairobi, Kenya
  dates: Since Jan 2021
  text: Pyro-degrade Energy is a startup that developed a technology to produce pyro-diesel from plastic waste. Pyro-diesel is an environmentally friendly diesel substitute - it is almost sulphur free and has a low carbon footprint. I am helping them with fundraising for their first industrial scale plant.
- url:
  image: gikoko.jpg
  title: Consulting for Gikoko Kogyo Indonesia
  location: Jakarta, Indonesia
  dates: Jan-Feb 2021
  text: I helped with greenhouse gas emissions reduction calculations to evaluate a municipal solid waste infrastructure project involving multiple technologies. The proposed project included waste sorting and shredding machinery powered by in-house refuse-derived fuel, an anaerobic digestion system and other technologies.
- url:
  image: green-worms.jpg
  title: Collaboration with Green Worms
  location: Kerala, India
  dates: Dec 2020 - Jan 2021
  text: Green Worms introduce waste collection services in small coastal towns in India. I was helping them with developing external communications strategy. My goals were to improve their engagement with stakeholders and to assist with initiating collaborations with organisations outside India.
- url:
  image: forbi.jpg
  title: Collaboration with Forbi Perise Eyong Nyosai
  location: Buea, Cameroon
  dates: Sep-Dec 2020
  text: Forbi's goal was to kickstart a PET bottle collection scheme in schools in Buea, Cameroon to both increase the plastic recycling rate in the country and to educate kids about waste related challenges. I helped Forbi with writing the project proposal, making a budget and with the application process.
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


