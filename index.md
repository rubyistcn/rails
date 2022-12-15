---
title: 首页
layout: home
nav_order: 1
---

# Ruby on Rails 指南
{: .fs-9 }

这是基于 Ruby on Rails 7 的指南。更早期版本可查看……
{: .fs-6 .fw-300 }

{% for section in site.data.documents %}
## {{ section.name }}

{% for document in section.documents %}
### [{{ document.name }}]({{ document.url }})
{% if document.work_in_progress %}
 编纂中……
 {: .label .label-yellow }
{% endif %}

{{ document.description }}

{% endfor %}

{% endfor %}
