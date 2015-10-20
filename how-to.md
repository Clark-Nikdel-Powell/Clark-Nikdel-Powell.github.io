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

This site is written in Jekyll, which uses a combination of Markdown and static HTML files to display content. Start by assuming your page will be Markdown, unless you need to add a significant amount of custom markup for the specific page you're working on.
{: .panel}

### 1. Page Setup

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