---
layout: page
title: How To Use This Site
permalink: /how-to-use-this-site/
---

This site is written in Jekyll, which uses a combination of Markdown and static HTML files to display content. Start by assuming your page will be Markdown, unless you need to add a significant amount of custom markup for the specific page you're working on.

### Page Setup

Every page needs a configuration block:

	---
	layout: page
	title: How To Use This Site
	permalink: /how-to-use-this-site/
	---

Be sure to **end the permalink with a slash**; otherwise, Jekyll will try to download the file instead of display it.