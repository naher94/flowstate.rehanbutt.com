---
layout: page
title: Flow Types
permalink: /flow-types/
---

<div class="grid-x cell explore-flow-type-item-wrapper">
  {% for flow-type in site.flow-types %}
    <a href="{{flow-type.url}}" class="cell grid-x medium-4 flow-tile-link-wrapper">
      <div class="cell grid-x spacer">
        <div class="flow-tile cell grid-x">
          <div class="icon-container cell grid-x align-center align-middle">
            {{ flow-type.icon }}
          </div>
          <div class="text-section cell grid-x align-middle align-justify">
            <span class="cell auto name">{{ flow-type.name }}</span>
            {% assign flow-count-array = site.workflows | where:"flow-type", flow-type.name %}
            {% assign flow-count = flow-count-array | size %}
            <span class="cell shrink number-of">{{flow-count}} flows</span>
          </div>
        </div>
      </div>
    </a>
  {%- endfor -%}
</div>