---
layout: page
title: How To Use This Site
excerpt: Best practices and tutorials.
permalink: /how-to-use-this-site/
status: draft
revisioncount: 1
lastedit: 10/20/15
initial: JHN
---

### 0. Tone Guide

When writing updates for this site, **keep your contributions brief, plain, and to-the-point**.

At some point, somebody will be looking to this site for assistance, and it'll be easier to find help if we keep our writing sparse. A little cheekiness is okay now and then, but **this site should be defined by its helpfulness**, not by its humor.

**Keep your message clear and easy-to-understand**. Too many developers let advanced vocabulary go unexplained. If you need to use an ambiguous term, like "<span data-tooltip aria-haspopup="true" class="has-tip" title="The endpoint is the URL where your service (website) can be accessed by a client application (browser)." markdown="span">endpoint</span>," give a definition for it with a tooltip.

##### Updating the Site

Every time you update the site, please do the following:

1. If you created a new page, set the status to `draft`. Otherwise, change the page status to `revised`.
1. Wrap your updates in a `.diff` div, so that the team can review it faster.
1. Update the revision info in the page block.
1. Update the header.html file if you've added a new page / changed the location of an existing page.
1. Notify the rest of the team about your update (could set up a notification in Slack for this).
1. After the team reviews your update and gives it the +1, change the status to `resolved` and remove the `.diff` div.

<div class="diff" markdown="block">
What a `.diff` div may look like. Be sure to set `markdown="block"` if you're in a Markdown file so that the HTML [doesn't throw off your Markdown](#markdown-1).
</div>

### 1. Local Setup

To begin, you'll need to install these things:

1. Jekyll: run the command `gem install jekyll` from Terminal
1. Node.js and npm: [download Node.js](https://nodejs.org/en/) first, and check to [make sure npm is up-to-date](https://docs.npmjs.com/getting-started/installing-node).
1. Install Bower locally by running the command: `npm install -g bower`.

We install Bower so that we can keep the Foundation framework updated, and Jekyll so that you can preview your edits locally. Next:

1. Download the site repo from [Github](https://github.com/Clark-Nikdel-Powell/Clark-Nikdel-Powell.github.io)
1. cd into the local repo, and run `jekyll serve` to compile updates locally before committing.

### 2. Page Setup

This site is written in Jekyll, which uses a combination of Markdown and static HTML files to display content. Start by assuming your page will be Markdown, unless you need to add a significant amount of custom markup for the specific page you're working on.
{: .panel}

Every page needs a configuration block:

###### Markdown

    ---
    layout: page
    title: How To Use This Site
    permalink: /how-to-use-this-site/
    status: draft
    revisioncount: 1
    lastedit: 10/20/15
    initial: JHN
    ---

#### Notes

1. **Layout:** the current layouts are "default" and "page"
1. **Title:** the page title, used in the head and in the `.post-header`
1. **Permalink:** be sure to end it with a slash, or else Jekyll will try to download the file instead of display it.
1. **Status:** draft, revision, resolved. Draft for the initial write-up, revision for after we review it, resolved after we agree on it.
1. **Revision info:** every time you update a page past the initial draft, update the revision count, last edit date, and initial it.

When creating a new page, keep it grouped with other pages if necessary. Follow the naming convention "groupname-pagename.md;" e.g., the CSS Style Guide is titled "style-guides-css.md,"" so that it'll be grouped next to other style guide pages when you're editing the site.


### 2. Markdown

##### Add Classes to Markdown

<div class="row">

<div class="medium-6 columns" markdown="block">

###### Markdown
~~~
Here's some content.
{: .class1 .class2}
~~~

</div>

<div class="medium-6 columns" markdown="block">

###### Output

{% highlight html %}
<p class="class1 class2">Here's some content.</p>
{% endhighlight %}

</div>

</div>

##### Column Classes and Code Blocks

See the Kramdown syntax on [HTML Blocks](http://kramdown.gettalong.org/syntax.html#html-blocks){:target="_blank"} -- HTML tags wrapped around Mardown content should have either a `markdown="block"` attribute, or a `markdown="span"` attribute.

Add syntax highlighting via a Pygments highlighting block.

<div class="row">

<div class="medium-6 columns" markdown="block">
###### Markup
{% highlight html %}
<div class="row">
  <div class="medium-6 columns" markdown="block">
    ##### Left Column
    ~~~ html
    Fenced Code Block
    ~~~
  </div>
  <div class="medium-6 columns" markdown="block">
    ##### Right Column
    {% raw %}{% highlight html %}{% endraw %}
    <div>Highlighted Block</div>
    {% raw %}{% endhighlight %}{% endraw %}
  </div>
</div>
{% endhighlight %}
</div>

<div class="medium-6 columns" markdown="block">
###### Output
{% highlight html %}
<div class="row">
  <div class="medium-6 columns" markdown="block">
    <h5>Left Column</h5>
    <pre><code class="language-html">
    Fenced Code Block
    </code></pre>
  </div>
  <div class="medium-6 columns" markdown="block">
    <h5>Right Column</h5>
    <pre><code class="language-html" data-lang="html">
    <span class="nt">&lt;div</span><span class="nt">&gt;</span>
      Highlighted Block
    <span class="nt">&lt;/div</span><span class="nt">&gt;</span>
    </code>
    </pre>
  </div>
</div>
{% endhighlight %}
</div>

</div>

Watch your tabs! Tab-indented markup might accidentally be converted to a code block. The easiest way to avoid this is to write code with a highlight tag.
{: .alert-box .alert}

##### Gists vs Code Blocks

Code blocks with the Pygments highlighting look better and laod faster than Gists, but Gists are a bit easier to share. Use your best judgement.

