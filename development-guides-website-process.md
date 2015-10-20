---
layout: page
title: Website Building Process
permalink: /development-guides/website-building-process/
status: draft
revisioncount: 1
lastedit: 10/20/15
initial: JHN
---

1. **Development Preview**
    1. Go over the site wireframes and information architecture before the client gets the final quote.
    1. Make a [development plan](/development-guides/making-a-development-plan/).
2. **CMS Setup**
    1. Get all plugins installed and set up post types, taxonomies, and custom post meta.
    1. Content entry.
    1. *See [WordPress Tips](/tips/wordpress/) for more details.*
3. **Theme Setup**
    1. Markup
        1. Use the Zurb Foundation Framework for grid and other components.
        1. *See [Foundation Tips](/tips/foundation/) for more details.*
    2. CSS
        1. Start with Setup items: site colors, site fonts, style guide page.
        1. According to the [CSS Style Guide](/style-guides/css/), group CSS by universal styles first, then mobile-only, then tablet-small and up, etc.
    3. JavaScript & UX detail
        1. Check and see if there’s a component in Foundation first. If not, build out a component that we can re-use.
4. **Browser-Testing**
    1. Test for IE via VMware Fusion.
    2. Test for iOS via Xcode Simulator and/or native devices.
    3. Make sure nothing breaks based on viewport widths from 320 to the max row-width.
    4. Don’t forget about super sized screens either.
5. **Launch**
    1. Follow the Site Launch Checklist.
    2. Don’t forget about Google Analytics or the Reading Settings.
6. **Post-Launch**
    1. Refactor components that will make maintenance easier.
    2. Add documentation for any unexplained pieces.
    3. Save out any reusable components to the SOP site
        1. If it’s a PHP component, save out just the PHP. But if the component has markup, styles, and some interaction to it, you could conceivably save out HTML markup and PHP, CSS, and JavaScript.
    4. Do a code review of the site with the team.