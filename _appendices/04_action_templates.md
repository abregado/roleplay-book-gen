---
title: Action Templates
layout: "appendix"
---



<div class="two-column-flex">
{% for template in site.data.action_templates %}
    {% capture template_name %}{{template[0]}}{% endcapture %}
    {% include action.html template=template_name %}
{% endfor %}
</div>
