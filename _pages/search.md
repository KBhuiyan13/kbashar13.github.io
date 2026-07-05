---
layout: single
title: "Search"
permalink: /search/
author_profile: false
---


Search across publications, projects, blog posts, and pages.

<div id="search"></div>

<script src="{{ '/pagefind/pagefind-ui.js' | relative_url }}"></script>

<script>
window.addEventListener("DOMContentLoaded", () => {
  new PagefindUI({
    element: "#search"
  });
});
</script>
