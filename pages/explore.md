---
layout: kz-page
title: "What we've learnt so far"
permalink: "/explore/"
subheadline: Waste management for our planet and people, not profit
meta_description:
header:
  title: ""
  image_fullwidth: landingpage_image.jpg
widgets:
- url: /explore/urgent/
  image: waste_and_climate.jpg
  title: <a href="/explore/urgent/" target="_self">Waste management challenges are urgent</a>
- url:
  image: plastic_recycling.jpg
  title: Plastics and processing of plastic waste
- url:
  image: other_recycling.jpg
  title: Processing other types of waste
- url: /explore/waste_disposal_methods/
  image: waste_disposal_methods.jpg
  title: <a href="/explore/waste_disposal_methods/" target="_self">Waste disposal methods</a> 
- url:
  image: funding.jpg
  title: Funding waste management projects
- url:
  image: waste_trade.jpg
  title: International waste trade
- url:
  image: waste_management.jpg
  title: Components of waste management system
- url:
  image: policy.jpg
  title: Waste related policies

---

In depth research guides everything we do.
Whatever we discover on our journey, we want to share it with everyone.
During our research we come across a lot of information that is not true.
To avoid spreading misinformation, we check the primary sources of all the information we publish.
However, we don't want to use this as an excuse to delay sharing our findings.
Instead, we publish drafts of our articles and keep updating them as our research progresses. 
These drafts, marked with an appropriate warning sign, might be missing important information and might contain statements that have not yet been fact checked properly.
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
