---
title: Essays
layout: default
date: 2026-01-01
summary: Essays
---

# Essays

{: .lede}
These are the essays

{% assign essays = site.pages
   | where_exp: "p", "p.path contains 'essays/'"
   | where_exp: "p", "p.path != 'essays.md'" %}

{% include nav/gallery-grid.html
  items=essays
  variant="uniform"
  min-width="200px"
  show-summary=true
  class="gallery-grid--wide"
%}