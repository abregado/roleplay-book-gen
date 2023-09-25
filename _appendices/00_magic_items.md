---
title: Known Magic Items
layout: "appendix"
columns: two
---
# Magic Item costs
Common items: 2d6 x 5 gp (10-60gp)
Uncommon items: 3d4 x 50 gp (150-1000gp)
Rare items: 6d6 x 250 gp (1500-9000gp)
Very Rare items: 6d4 x 1500 gp (9000-36000)
Legendary items: 4d6 x 12500 gp (50000-300000)

{% assign common_items = site.data.magic_items | where: "rarity","Common" %} 
{% assign uncommon_items = site.data.magic_items | where: "rarity","Uncommon" %} 
{% assign rare_items = site.data.magic_items | where: "rarity","Rare" %} 
{% assign very_rare_items = site.data.magic_items | where: "rarity","Very rare" %} 

# Common magic items
{% for item in common_items %}
{% assign itemData = item %}
{% include magic_item.html content=itemData %}
{% endfor %}

# Uncommon magic items
{% for item in uncommon_items %}
{% assign itemData = item %}
{% include magic_item.html content=itemData %}
{% endfor %}

# Rare magic items
{% for item in rare_items %}
{% assign itemData = item %}
{% include magic_item.html content=itemData %}
{% endfor %}

# Very Rare magic items
{% for item in very_rare_items %}
{% assign itemData = item %}
{% include magic_item.html content=itemData %}
{% endfor %}
