---
title: Action Templates
layout: "appendix"
---

Monster attacks are supposed to be simplified versions of those that heroes utilize.
They either require an attack roll or a saving throw, but never both.

Range, damage values, attack values and difficulty class are shown on the monster stat block, as these can vary between monsters.

Monsters will also trigger these actions in different ways. For example, one monster might use Zap as a reaction while another as its Bonus action. Another still might use it as part of a Multi-attack action.

<div class="two-column-flex">
{% for template in site.data.action_templates %}
    {% capture template_name %}{{template[0]}}{% endcapture %}
    {% include action.html template=template_name %}
{% endfor %}
</div>
