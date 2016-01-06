---
layout: page-sidebar
title: Frequently Asked Questions
permalink: /faqs/
---

{% for faq in site.data.faqs %} * [{{ faq.question }}]({{ '/faqs/#faq' | prepend: site.baseurl }}{{ forloop.index }})
{% endfor %}

{% for faq in site.data.faqs %}

<h3 id="faq{{ forloop.index }}">{{ faq.question }}</h3>

{{ faq.answer }}

{% endfor %}
