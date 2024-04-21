---
layout: ko
---
# 역사

{% for item in site.data.history %}
{% assign title=item.year | append: " Combinatorics Workshop" %}
{% assign titleko=item.year | append: "년 조합론 학술대회" %}

## {{ item.n }}회: [{{ item.titleko | default: titleko}}]({{item.url}})
- English name: {{ item.title | default: title}}
- 날짜: {{ item.dates }}, {{item.year}}
- 장소: {{ item.venue }}, {{ item.city}}
- Host: {{item.host}}
{% endfor %}