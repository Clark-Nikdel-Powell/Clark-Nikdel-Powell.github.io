---
layout: page
title: WordPress Tips
slug: wordpress-tips
permalink: /tips/wordpress/
status: draft
revisioncount: 1
lastedit: 10/20/15
initial: JHN
---

### Recommended Plugins

> I'd like to bulk install plugins, so that we don't have to spend an hour installing plugins for every project. Some
> possibilities are [WP Quick Install](http://wp-quick-install.com/), or the [Multi Plugin Installer](https://wordpress.org/plugins/multi-plugin-installer/), or [
> Variable V's blueprints](https://github.com/bradp/vv#blueprints). I feel like we'd need these features:
>
> 1. Install from a WordPress plugin repo.
> 1. Install from a Github plugin repo.
> 1. Install from a local location.
> 1. Ability to save plugin collections so that it's a one or two-click process each time.
>
> — JHN, 10/20/15

#### Admin Setup

1. **Set Standard WP Settings:** Basic Settings (CNP, [Github](https://github.com/Clark-Nikdel-Powell/Basic-Settings))
1. **Admin Navigation:**{:id="acp"}{:download="admin-command-palette"} Admin Command Palette (CNP, [WordPress](https://wordpress.org/plugins/admin-command-palette/))
1. **Page Ordering:**{:id="page-ordering"}{:download="simple-page-ordering"} Simple Page Ordering ([WordPress](https://wordpress.org/plugins/simple-page-ordering/))
1. **Custom Post Type Menu Links:** WordPress Post Type Archive Links ([WordPress](https://wordpress.org/plugins/post-type-archive-links/))
1. **CSS Hotfixes:** Simple Custom CSS ([WordPress](https://wordpress.org/plugins/simple-custom-css/))
1. **Syntax Highlighting:** HTML Editor Syntax Highlighter ([WordPress](https://wordpress.org/plugins/html-editor-syntax-highlighter/))
1. **Manager User Role:** Mr. Manager (CNP, [Github](https://github.com/Clark-Nikdel-Powell/Mr.-Manager))
1. **More Editing Tools:** TinyMCE Advanced ([WordPress](https://wordpress.org/plugins/tinymce-advanced/))

#### CMS Setup

1. **Custom meta boxes:** Advanced Custom Fields Pro (Licensed)
1. **Post Relationships:** Posts 2 Posts ([WordPress](https://wordpress.org/plugins/posts-to-posts/) / [Github Docs](https://github.com/scribu/wp-posts-to-posts/wiki))
1. **Better Admin Column Information:** Admin Columns ([WordPress](https://wordpress.org/plugins/codepress-admin-columns/))
1. **Events Plugin:** Tzolkin (CNP, [Github](https://github.com/Clark-Nikdel-Powell/Tzolkin))
1. **Social Settings / Twitter API:** Lepidoptera (CNP, [Github](https://github.com/Clark-Nikdel-Powell/Lepidoptera))
1. **Email Forms:** Contact Form 7 ([WordPress](https://wordpress.org/plugins/contact-form-7/)), Gravity Forms (Licensed)

#### Tools

1. **Site Moves:** WP DB Pro (Licensed), WPSyncDB ([Github](https://github.com/wp-sync-db/wp-sync-db)), WPSyncDB Media Files ([Github](https://github.com/wp-sync-db/wp-sync-db-media-files))
1. **Regenerate Thumbnails:**{:id="force-regenerate-thumbnails"}{:download="force-regenerate-thumbnails"} Force Regenerate Thumbnails ([WordPress](https://wordpress.org/plugins/force-regenerate-thumbnails/))
1. **Replace Media:**{:id="enable-media-replace"}{:download="enable-media-replace"} Enable Media Replace ([WordPress](https://wordpress.org/plugins/enable-media-replace/))
1. **Better Image Thumbnails:** Theia Smart Thumbnails (Lincensed)

#### Utilities

1. **Caching:** WP-Rocket (Licensed)
1. **Site Security / Firewall:** Cloudflare ([WordPress](https://wordpress.org/plugins/cloudflare/)) / Sucuri ([WordPress](https://wordpress.org/plugins/sucuri-scanner/))
1. **Redirection:** Safe Redirect Manager ([WordPress](https://wordpress.org/plugins/safe-redirect-manager/))
1. **Google Analytics:** Google Analytics ([WordPress](https://wordpress.org/plugins/googleanalytics/)), Simple Google Analytics ([WordPress](https://wordpress.org/plugins/simple-google-analytics/)), or All-in-One SEO Pack ([WordPress](https://wordpress.org/plugins/all-in-one-seo-pack/))
1. **SEO:** All-in-One SEO Pack ([WordPress](https://wordpress.org/plugins/all-in-one-seo-pack/))
1. **HTTPS:** WordPress HTTPS ([WordPress](https://wordpress.org/plugins/wordpress-https/))
1. **Better Mail Sending:** wpMandrill ([WordPress](https://wordpress.org/plugins/wpmandrill/))
1. **Keep site de-indexed:** Get Off My Lawn (CNP, [Github](https://github.com/Clark-Nikdel-Powell/Get-Off-My-Lawn))

### CMS Setup Notes

1. Keep your custom meta field names scoped, but don't overscope them.
2. Choose image sizes **VERY** carefully. Any additional image size means there's another copy of an image on the server.