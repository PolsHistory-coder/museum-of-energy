---
title: Gallery
layout: default
date: 2026-01-01
summary: The whole collection seen at once — every object at its own proportions, running the full width of the page.
---

# Gallery

{: .lede}
The same essays as the [directory]({{ site.baseurl }}/essays), seen all at
once. Nothing here is cropped to a common square: a tall scroll stays tall and a
wide dish stays wide, because the proportions of a thing are part of what a
picture of it tells you. Titles and summaries wait until a tile is hovered over
or tabbed to, so the pictures have the page to themselves.

{% assign essays = site.pages
   | where_exp: "p", "p.path contains 'essays/'"
   | where_exp: "p", "p.path contains 'index.md'"
   | where_exp: "p", "p.path != 'essays.md'" %}

{% include nav/gallery-grid.html
  items=essays
  variant="masonry"
  min-width="180px"
  show-summary=true
  class="gallery-grid--bleed"
%}



