# arc-medtechai
This is a Jekyll-based website for a research group.

## Creating a new page
Add the markdown file in the `root` directory with the necessary front matter (layout: page, title, categories).

Categories may include `navi` or `browse`.
* `navi` is for adding the page to the navigation bar
* `browse` is for adding the page to the browsing topics on the home page

~~~~
---
layout: page
title: News
categories: [navi]
---
~~~~

~~~~
---
layout: page
title: About
categories: [navi, browse]
browse-description: Learn more about our organisation.
---
~~~~

## Adding a new research area
Add the markdown file in the `_research-areas directory` and include the necessary front matter (layout: page, title).
~~~~
---
layout: page
title:  "Research Area 2"
---
~~~~

## Adding a news post
Simply add a file in the `_posts directory` that follows the convention `YYYY-MM-DD-name-of-post.markdown` and includes the necessary front matter (layout: post, title, date, categories).
~~~~
---
layout: post
title:  "Welcome to ARC Medtech!"
date:   2018-07-05 23:55:23 +1000
categories: jekyll update
---
~~~~


