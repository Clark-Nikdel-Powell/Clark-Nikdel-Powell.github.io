---
layout: page
title: Modules Style Guide
permalink: /style-guides/modules/
status: draft
revisioncount: 1
lastedit: 11/02/15
initial: JHN
---

Modules are PHP functions that we include in our theme via Bower. A good module should be useful, focused, and (in some circumstances) easy to modify. Here are some guidelines to writing a good module:

1. **Filters, then functions**: if you can do what you need to by using WordPress filters, build your module around that. Adding a new function name runs the risk of fatal errors, whereas filters do not.

2. **Consistent Names**: Put it on Github, and follow the `WP-Module-$name` naming convention.

3. **Good docs**: Include a Readme.md that follows the WordPress function documentation format: **Description**, **Usage**, **Parameters** & **Return Values**.

4. **Filter if you need to**: Include a filter to modify parts of the output that make sense, and include the filter in your documentation.

5. **Install it on the theme**: If it is essential to the Foundation Theme, update the theme's `bower.json` file.

6. **Keep an eye open**: If you notice unexpected behavior, open an issue on the module's Github repo.

