---
lang: en
lang-ref: home
# klass: home # this line adds a css class to the entire landing page and so applies the styling in main.scss
layout: home
preTitle: Welcome to ZooMu
title: Biodiversity including Zoos, Aquariums, and other living animal collections.
description: |
  <div class="mt-6">
    <form action="/occurrence/search" type="get">
      <div class="field" style="display: flex;">
        <input type="text" placeholder="Full text record search" name="q" class="input" />
        <button type="submit" class="button is-primary ml-4">Search</button>
      </div>
    </form>
  </div>
background: "{{images/1789480859154-016f294f-8793-4b0b-bec3-744acc884958_1.jpg}}"
imageLicense: "{{Jennifer D'Agostino, DVM, DACZM}}"
height: 75vh
cta:
  # - text: Search
  #   href: occurrence/search
  #   isPrimary: true
#  - text: Learn more
#    href: /about
#  - text: ZooMu Classic
#    href: zooaquariumportal.org/search
permalink: /
composition:
  - type: heroImage # the block type
  - data: home.stats
    type: stats
  # - type: pageMarkdown # there is currently no text on the page so just ignore this part
  - type: split
    data: home.about
  - type: split
    data: home.explorer
  - type: split
    data: home.resources
  - type: latestPosts
    data: we_do_not_want_any_header # weird hack as the block layout looks for a data element and falls back to the page if none is present
---
