---
layout: page
title: How To Use This Site
slug: how-to-use-this-site
permalink: /how-to-use-this-site/
status: draft
revisioncount: 1
lastedit: 10/20/15
initial: JHN
---

This site is written in Jekyll, which uses a combination of Markdown and static HTML files to display content. Start by assuming your page will be Markdown, unless you need to add a significant amount of custom markup for the specific page you're working on.
{: .panel}

### 1. Page Setup

Every page needs a configuration block:

###### Markdown

	---
	layout: page
	title: How To Use This Site
	slug: how-to-use-this-site
	permalink: /how-to-use-this-site/
	status: draft
	revisioncount: 1
	lastedit: 10/20/15
	initial: JHN
	---

#### Notes

1. **Layout:** the current layouts are "default" and "page"
1. **Title:** the page title, used in the head and in the `.post-header`
1. **Slug:** slug for the `body` class.
1. **Permalink:** be sure to end it with a slash, or else Jekyll will try to download the file instead of display it.
1. **Status:** draft, revision, resolved. Draft for the initial write-up, revision for after we review it, resolved after we agree on it.
1. **Revision info:** every time you update a page past the initial draft, update the revision count, last edit date, and initial it.

When creating a new page, keep it grouped with other pages if necessary. Follow the naming convention "groupname-pagename.md;" e.g., the CSS Style Guide is titled "style-guides-css.md,"" so that it'll be grouped next to other style guide pages when you're editing the site.


### 2. Markdown

You can add classes to small bits of Markdown like this:

<div class="row">

	<div class="medium-6 columns">
		<h6>Markdown</h6>
<pre>Here's some content.
{: .class1 .class2}</pre>
	</div>
	<div class="medium-6 columns">
		<h6>Output</h6>
		<pre>&lt;p class="class1 class2"&gt;Here's some content.&lt;/p&gt;</pre>
	</div>
</div>