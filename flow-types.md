---
layout: page
title: Flow Types
permalink: /flow-types/
---

<div class="grid-x cell explore-flow-type-item-wrapper">
  {% for flow-type in site.data.flow-type %}
    <a href="#" class="cell grid-x medium-4 flow-tile-link-wrapper">
      <div class="cell grid-x spacer">
        <div class="flow-tile cell grid-x">
          <div class="icon-container cell grid-x align-center align-middle">
            {{ flow-type[1].icon }}
          </div>
          <div class="text-section cell grid-x align-middle align-justify">
            <span class="cell auto name">{{ flow-type[1].name }}</span>
            <span class="cell shrink number-of">12 flows</span>
          </div>
        </div>
      </div>
    </a>
  {%- endfor -%}
</div>