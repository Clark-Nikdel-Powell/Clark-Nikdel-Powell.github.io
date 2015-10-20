---
layout: page
title: Snippets
excerpt: Reusable chunks of code.
permalink: /snippets/
status: draft
revisioncount: 1
lastedit: 10/20/15
initial: JHN
---

### WordPress Snippets

##### Remove Default Image Sizes
<script src="https://gist.github.com/jhned/f08a50a46e3ca4e1e7f8.js"></script>
>Removing the default image sizes is a good idea if all images on the site are going to be the same aspect ratio. We could probably add this as a option to Client-Core. — JHN

### Composite Snippets

###### Dateblock Style 1

### Sublime Snippets

To install Sublime Snippets, create a `filename.sublime-snippet`, and put it in `Packages / User` (which you can find by using the "Browse Packages" command in Sublime).

##### Comments

{% highlight css %}
/*——————————————————————————————————————————
/  Small Comment Line
——————————————————————————————————————————*/

/*——————————————————————————————————————————————————————————
/  Medium Comment Line
——————————————————————————————————————————————————————————*/

/*——————————————————————————————————————————————————————————————————————————————
/  Large Comment Line
——————————————————————————————————————————————————————————————————————————————*/
{% endhighlight %}

###### Triggers & Download
- `/1` Small Comment Line
- `/2` Medium Comment Line
- `/3` Large Comment Line
- [CommentSnippets.zip](/snippets/sublime/comments.zip)

You can use these comment snippets to break up your SCSS, PHP or JavaScript files. Please use [docblock formatting](https://make.wordpress.org/core/handbook/best-practices/inline-documentation-standards/php/#docblock-formatting) for functions in JavaScript and PHP.

#### Emmet Snippets

Emmet is a HTML and CSS code-expanding tool. It comes with a lot of handy snippets, but you can also add your own in `Preferences / Package Settings / Emmet / Settings — User`. Here are some that we use often: