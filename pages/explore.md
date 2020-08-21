---
layout: kz-page
title: "What we've learnt so far"
permalink: "/explore/"
meta_description:
header:
  title: ""
  image_fullwidth: landingpage_image.jpg
widgets:
- url: /explore/why-is-this-urgent/
  image: plastic-pollution-beach-by-Jennifer-Lavers.jpg
  title: <a href="/explore/why-is-this-urgent/" target="_self">Why is this urgent?</a>
  text: The World Bank estimated that 1.6 billion tonnes of CO2-equivalent greenhouse gas emissions (about 5 percent of global emissions) were generated from solid waste treatment and disposal in 2016. Diseases related to mismanaged waste result in 700,000 deaths each year. This is why changing waste management practices is an urgent matter.
  anchor: why-is-this-urgent
  button: true
- url: /explore/waste-management-in-indonesia/
  image: indonesia-plastic-pollution-java-cordonpress-dot-com.jpg
  title: <a href="/explore/waste-management-in-indonesia/" target="_self">Waste management in Indonesia</a>
  text: Indonesia is home to 3.4% of the world's population; and it is estimated that 10% of the global ocean plastic pollution originates there. The Indonesia National Plastic Action Partnership mapped out this challenge.
  anchor: waste-management-in-indonesia
  button: true

---

Our aim is to solve global waste management challenges, and the research we do provides us stepping stones along the way. Below we will be sharing what we've learnt on our journey so far. This will include research about the different types of waste, waste management systems in different countries, international waste trade, waste disposal and recycling technologies. Since a growing proportion of waste is plastic, we will cover everything from plastic production and current recycling methods to proposed long-term strategies and new technologies for the whole life-cycle of plastic and its alternatives.


During our research we came across a lot of information that is not true. To avoid spreading misinformation, we check primary sources of all the information we publish. The articles which have not yet been rigorously fact checked, will be published with an appropriate warning sign. Note that all the waste-related numbers are point estimates, all of them have large margins of error as it is impossible to obtain precise data about waste. We only use the word "about" in front of the numbers to indicate that we've not yet found the data or we suspect it doesn't exist. If you spot any mistakes, please do <a href="mailto:hello@samudra.world" target="_blank">get in touch</a>, we will much appreciate that.


<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>






