---
layout: page
title: How To Use This Site
slug: how-to-use-this-site
permalink: /how-to-use-this-site/
---

This site is written in Jekyll, which uses a combination of Markdown and static HTML files to display content. Start by assuming your page will be Markdown, unless you need to add a significant amount of custom markup for the specific page you're working on.
{: .alert-box .info}

### 1. Page Setup

Every page needs a configuration block:

	---
	layout: page
	title: How To Use This Site
	slug: how-to-use-this-site
	permalink: /how-to-use-this-site/
	---

#### Notes

1. **Layout:** the current layouts are "default" and "page"
1. **Title:** the page title, used in the head and in the `.post-header`
1. **Slug:** slug for the `body` class.
1. **Permalink:** be sure to end it with a slash, or else Jekyll will try to download the file instead of display it.
