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

## Creating a nested section
1. Create a new folder in the `root` directory with the appropriate name of the section. Place the markdown files in the folder, and any further nesting in subfolders. **This template allows nesting with depth of at most 2.**

2. In the `_data` folder, add a `.yml` file with the same name as the section folder created previously. Describe the table of contents for navigation that will appear for the section as follows:

~~~~
toc:
- page: Nested
  url: /nested/
- page: Section 1
  url: /nested/section1.html
- page: Section 2
  url: /nested/section2/
  subpages:
    - page: Subsection
      url: /nested/section2/subsection.html
    - page: Subsection 2
      url: /nested/section2/subsection2.html
~~~~

(See sample `nested` directory file.)

## Adding a new research area
Add the markdown file in the `_research-areas` directory and include the necessary front matter (layout: page, title).
~~~~
---
layout: page
title:  "Research Area 2"
---
~~~~

## Adding a news post
Simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.markdown` and includes the necessary front matter (layout: post, title, date, categories).
~~~~
---
layout: post
title:  "Welcome to the web site!"
date:   2018-10-01 23:55:23 +1000
categories: jekyll update
---
~~~~
