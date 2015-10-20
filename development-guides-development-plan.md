---
layout: page
title: Making a Development Plan
excerpt: Don't rush in to a project. Plan it out first.
permalink: /development-guides/making-a-development-plan/
status: draft
revisioncount: 1
lastedit: 10/20/15
initial: JHN
---

A good development plan will help you see holes in the design and your thinking before you start writing code. As you plan out a site, here are some questions to be thinking about:
{: .panel}


### CMS Setup

<div class="row" markdown="block">

<div class="column medium-7" markdown="block">
1. What are the post types?
1. What are the taxonomies, and what post types do they belong to?
    1. Do we *need* taxonomies, or would a meta item suffice? (See panel)
1. What are the custom meta items? What types of fields will they be?
1. Are there any post 2 post connections?
1. What plugins will we need for this website? (See [WordPress Tips](/tips/wordpress/) for recommended plugins.)

and, generally:

1. How can we handle this site's data efficiently?
1. How can we make this site's data easier to manage?
1. What blocks of code are you going to reuse throughout the site? Do they need to be in a plugin, or in the theme?
1. Use the WordPress PHP style guide for both writing [code](https://make.wordpress.org/core/handbook/best-practices/coding-standards/php/){:target="_blank"} and [documentation](https://make.wordpress.org/core/handbook/best-practices/inline-documentation-standards/php/){:target="_blank"}.
</div>

<div class="column medium-5" markdown="block">
<div class="panel callout" markdown="block">
Only use a taxonomy if you need to display an archive page for it. If it's just for better organization, use a custom meta item.
</div>
</div>

</div>

### Markup

Markup is usually difficult to plan for. What seems simple when you look at the design can become much more complicated as you start to code it. In general, plan for these ideas:

1. Simple is good, Simple is life.
1. Use class names frequently. It's better to style based on a class than a tag, because the tag may need to change.
1. If you're working on a complex module, try the **BEM naming convention**:

###### HTML
~~~~~~~~
<div class="person">
    <div class="person-image">
        <img src="[...]">
    </div>
    <div class="person-info">
        <h3 class="person-name"></h3>
        <p class="person-title"></p>
        <p class="person-email"></p>
    </div>
</div>
~~~~~~~~
{: .language-html}

Notice, I didn't write "person-info-name," but rather "person-name," which keeps it simpler.
{: .alert-box .info}

This way, we can nest for SCSS organizational purposes without adding more specificity to our CSS selectors:

<div class="row" markdown="block">
<div class="column medium-6" markdown="block">
###### SCSS
~~~~~~~~
.person {
    &-image {}
    &-info {}
    &-name {}
    &-title {}
    &-email {}
}
~~~~~~~~
{: .language-scss}
</div>
<div class="column medium-6" markdown="block">
###### CSS
~~~~~~~~
.person {}
.person-image {}
.person-info {}
.person-name {}
.person-title {}
.person-email {}
~~~~~~~~
{: .language-scss}
</div>
</div>

### SCSS

1. What modules does this site have? How can we reuse styles?
1. Modularize margins and padding as well. Look for how spacing works on the site as a whole, not just a single page.
1. Don't overnest your CSS. This is paramount to future site maintenance.
1. Get the initial type styles from Typecast.
1. When it comes to type scaling, using `rem` units at the module level only might work well: [CSS Tricks Article](https://css-tricks.com/rems-ems/)
1. For more specific tips, follow the [CSS Style Guide](/style-guides/css)

### JavaScript/UX

Do not underestimate JavaScript! Complex user interaction effects take a hell of a lot more testing than CSS effects, and are more prone to unusual behavior.
{: .alert-box .warning}

1. In general, follow the WordPress JavaScript style guide for writing [code](https://make.wordpress.org/core/handbook/best-practices/coding-standards/javascript/){:target="_blank"} and [documentation](https://make.wordpress.org/core/handbook/best-practices/inline-documentation-standards/javascript/){:target="_blank"}.