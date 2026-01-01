---
layout: page
title: Case Studies
permalink: /case-studies/
---

<div style="text-align: center; background-color: #f6f8fa; padding: 2rem; margin-bottom: 2rem; border-radius: 8px; border-left: 4px solid #0366d6;">
  <p style="font-size: 1.1rem; line-height: 1.8; color: #24292e; margin: 0; max-width: 800px; margin-left: auto; margin-right: auto;">
    Explore hands-on case studies designed to bridge theory and practice across modern web development technologies. Each module presents real-world scenarios that guide you through practical implementations, from foundational concepts to advanced patterns. Navigate through structured lessons within each technology stack to build comprehensive, production-ready skills.
  </p>
</div>

{% assign modules = "TypeScript,React,MongoDB,Express" | split: "," %}

{% assign module_colors = "667eea,f093fb,4facfe,43e97b" | split: "," %}
{% assign module_icons = "📘,⚛️,🍃,🚀" | split: "," %}

{% for module in modules %}
{% assign color = module_colors[forloop.index0] %}
{% assign icon = module_icons[forloop.index0] %}

<div style="margin-bottom: 2.5rem; border-radius: 12px; overflow: hidden; box-shadow: 0 4px 12px rgba(0,0,0,0.1);">
  <details style="margin: 0;">
    <summary style="cursor: pointer; font-size: 1.7rem; font-weight: bold; padding: 1.5rem 2rem; background: linear-gradient(135deg, #{{ color }}20 0%, #{{ color }}40 100%); border-left: 6px solid #{{ color }}; display: flex; align-items: center; gap: 0.75rem;">
      <span style="font-size: 2rem;">{{ icon }}</span>
      <span>{{ module }}</span>
      <span style="font-size: 0.85rem; color: #586069; font-weight: normal; margin-left: auto; background: white; padding: 0.25rem 0.75rem; border-radius: 12px;">
        {% assign module_items = site.case_studies | where: "module", module | sort: "order" %}
        {{ module_items.size }} lessons
      </span>
    </summary>
    
    <div style="padding: 2rem; background-color: white;">
      {% assign module_items = site.case_studies | where: "module", module | sort: "order" %}
      
      {% if module_items.size > 0 %}
        <div style="display: grid; gap: 1rem;">
          {% for cs in module_items %}
            <a href="{{ cs.url | relative_url }}" style="text-decoration: none; display: block; padding: 1.25rem; border: 1px solid #e1e4e8; border-radius: 8px; transition: all 0.2s; background-color: #fafbfc;">
              <div style="font-weight: 600; font-size: 1.1rem; color: #24292e; margin-bottom: 0.5rem;">
                <span style="display: inline-block; width: 2rem; height: 2rem; background: linear-gradient(135deg, #{{ color }}30, #{{ color }}50); border-radius: 50%; text-align: center; line-height: 2rem; margin-right: 0.75rem; color: #{{ color }}; font-weight: bold; font-size: 0.9rem;">{{ cs.order }}</span>
                {{ cs.title }}
              </div>
              {% if cs.summary %}<div style="color: #586069; font-size: 0.95rem; padding-left: 2.75rem;">{{ cs.summary }}</div>{% endif %}
            </a>
          {% endfor %}
        </div>
      {% else %}
        <p style="color: #888; font-style: italic;">No case studies available yet.</p>
      {% endif %}
    </div>
  </details>
</div>

{% endfor %}
