=== Plugin Name ===
Contributors: LorenW
Donate link: 
Tags: page template, template redirect, page
Requires at least: 2.8
Tested up to: 3.3.2
Stable tag: 0.1

Assigns hierarchical templates to pages and their children giving precedence to the page-[id].php templates.

== Description ==

In WordPress each page must be intentionally assigned a template (or have a template file intentionally named for it) or WordPress applies the default page.php template.  Child pages do not inherit parent page templates.  On a large website with many child pages within a hierarchy of pages this does not make for an easy or error free way to use page templates to create a sectioned CMS.  A user can assign a template to a top level page (or a "beginning of section" page) but its descendants (child pages) will not follow with their ancestor's template.  Each page's template must be individually assigned.  For small sites with few pages and few users this is not a significant matter.  On a site with hundreds or thousands of pages and multiple editors and multiple "sections" this makes WordPress less than ideal as a CMS platform

This plugin solves that problem.  It investigates each page and assigns hierarchical templates to pages and their children giving precedence to page-[id].php templates. If no page-[id].php templates are found all the way up the ancestory tree then it will check for page-[slug].php templates back up the ancestory tree. If those are not found then it will look for a meta assigned custom.php template - first for the currently selected page and then if the page does not have a custom.php template assigned the function will look back up the ancestory tree to see if an ancestor page has been assigned a custom.php template. If all of these fail it will fall back to WP's default page.php template.

There is more description at http://www.warkensoft.net/wordpress-plugins/wordpress-hierarchical-page-template-redirect-plugin/

== Installation ==

1. Upload `wp-hptr.php` to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
There are no options or settings

== Frequently Asked Questions ==

= None yet! =

So no answers yet either.


== Screenshots ==
There are no screen shots as this plugin works behind the scenes.

== Changelog ==

= 0.1 =
This is the first version.  However it has undergone considerable testing.

== Upgrade Notice ==
Nothing here yet