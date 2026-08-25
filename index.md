---


title: History of Energy
layout: base
date: 2026-01-01
summary: A website about the History of Energy

hero:
  image: /assets/images/backgrounds/kashima-oil-east-gate-night.jpg
  alt: Kashima Oil Refinery
  kicker: A Museum
  title: History of Energy
  text: The objects profiled on this website tell history with energy at the center.
  buttons:
    - label: See the Essays
      url: /gallery
    - label: See Them on a Map
      url: /map

featured:
  - slug: buddha-head
    label: Sculpture
  - slug: bowl-with-dragons
    label: Ceramics

explore:
  - label: All Objects
    url: /objects
    text: The full grid, assembled from whatever folders exist under objects/.
  - label: Gallery
    url: /gallery
    text: The same objects as a wall of pictures, each at its own proportions.
  - label: Essays
    url: /essays
    text: Thematic threads that read across the objects rather than one at a time.
  - label: Map
    url: /map
    text: Every object that carries geo coordinates in its front matter.
  - label: Instructions
    url: /instructions
    text: How to add an object, and what each front matter field does.
  - label: Documentation
    url: /docs
    text: The whole Xanthan reference, including every component.
---

{% include layout/home-hero.html hero=page.hero %}

## The History of Energy

{: .lede}
This is the website for the History of Energy class. 

Our lives today are shaped through our consumption of energy. Access to energy mediates every single productive or recreational activity that we engage in. Our sources of energy: fossil fuels, hydroelectricity, nuclear power, renewables are as varied as the use we put them to. They heat and cool our homes and workplaces, cook our food, dispense our waste, enable our work and wars, and illuminate the device you are almost certainly using to read these very words. History of Energy takes this key fact of our modern life as the starting point and asks, how things came to be this way. Offering a range of critical frameworks, this class will introduce students to both the history of energy as well as energy as history itself. Using diverse source materials, students are invited to immerse themselves in a global history of energy and to consider how the struggle to produce, control and deploy energy shaped modern history, and the ways that social forces, in turn, determined energy systems. While our approach is historical rather than technical, the subject matter of our semester long discussion will include non-anthropocentric, environmental actors to shed light on questions of inequality, scientific and technological consensus, disasters and politics of climate change.

Each object lives in its own folder under `objects/`, with its page and its
images together. The catalogue facts — date, medium, place, coordinates, tags —
live in the front matter of that page, so they are written once and appear
wherever they are needed: on the grid, on the map, in search.

Nothing indexes objects by hand. Add a folder and it appears.

The [essays]({{ site.baseurl }}/essays) are the other half of the arrangement.
An object page describes one thing; an essay follows a motif, a material, or a
gap in the record through several of them. Objects stay independent of the
essays that cite them, so an argument can be added or withdrawn without
disturbing the collection underneath it.

{% include layout/picks.html
  items=page.featured
  collection="objects"
  variant="strip"
  columns=3
  kicker="Sample Objects"
  title="Three stand-ins, here to be replaced."
%}

{% include layout/link-index.html
  links=page.explore
  kicker="Where to go next"
  title="Start with the instructions, then delete these three."
%}
