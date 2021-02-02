---
layout: kz-page
title: "What we've learnt so far"
permalink: "/explore/"
meta_description:
header:
  title: ""
  image_fullwidth: landingpage_image.jpg
widgets:
- url: /explore/waste_disposal_methods/
  image: dumpsite-manila.jpg
  title: <a href="/explore/waste_disposal_methods/" target="_self">Waste disposal methods</a>
  text:
  anchor: waste_disposal_methods
- url: /explore/why-is-this-urgent/
  image: waste_and_climate.jpg
  title: <a href="/explore/why-is-this-urgent/" target="_self">Why is this urgent?</a>
  text: Today 2.6 billion people that have no access to waste collection services faced a choice of what to do with their waste. Today 32,877 tonnes of plastic waste ended up in our oceans. The damage done in the past 24 hours will have long lasting effects. The good news is that this can be changed. If we postpone implementing the necessary changes to waste management systems around the globe, they will not become any easier to implement but the benefits of doing so will be diminished by the previously accumulated irreversible damage. That is why it is important to act now.
  anchor: why-is-this-urgent
---

In depth research guides everything we do.
Whatever we discover on our journey, we want to share it with everyone.
During our research we come across a lot of information that is not true.
To avoid spreading misinformation, we check the primary sources of all the information we publish.
However, we don't want to use this as an excuse to delay sharing our findings.
Instead, we publish drafts of our articles and keep updating them as our research progresses. 
These drafts, marked with an appropriate warning sign, might be missing important information and might contain statements that have not yet been fact checked rigorously.
Note that all the waste-related numbers are point estimates, all of them have large error margins as it is impossible to obtain precise data about waste. 
We only use the word "about" in front of the numbers to indicate that we've not yet found the data or we suspect it doesn't exist. 
If you spot any mistakes, please do <a href="mailto:hello@samudra.world" target="_blank">get in touch</a>, we will much appreciate that.


<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>
