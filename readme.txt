=== MU Post to Multiple Blogs ===
Contributors: bdombro, donncha, imwebgefunden, wpmuguru
Tags: wordpressmu
Tested up to: 3.8
Stable tag: 1.0
Requires at least: 3.0

Allows the posting to multiple blogs at a time, bubble-out style.

== Description ==

Creates a metabox on post edit pages, which allows you to select other blogs to post to within a Wordpress multisite.

* Must be logged in as an network admin to see the box.

For performance reasons the number of posts is limited to a user configurable amount, and the blog itself can be made indexable by search engines or not.

This plugin was based on another WP plugin:  http://wordpress.org/plugins/wordpress-mu-sitewide-tags/

== Install ==
1. Install in your plugins directory in the usual way and network activate the plugin. There is no need to put it in mu-plugins.
2. Login as a site administrator and go to Super Admin->Sitewide Tags.
	3. "Max posts" defaults to 5000. Older posts will be deleted if this threshold is broken.
	4. Check "Include Pages" to include both posts and pages, handy for making a sitewide search.
	5. "Privacy" defaults to public, pages can be indexed by search engines.
	6. When "Privacy" is not public, check "Non-Public Blogs" to include blogs not indexed by search engines.
	7. Add "Post Meta" custom fields to be copied with posts/pages.

== Changelog ==

= 1.0 =
* First checkin with the post-to-multiple-blogs purpose.
* Added metabox to post edit pages, which allows users to select which other blogs to post the post to.
* Modified the save and delete hooks so that posts get posted to the blogs selected in the metabox, and get deleted when either removed from the selection or when the post is deleted.


= 0.4.2 =
* Last update before bdombro modified it for new purpose
* duplicate category fix
* page permalink fix
* thumbnail size filter

= 0.4.1.1 =
* Run populate feature in source blog context.
* Added resource warning for populate feature.
* Fixed PHP warnings.
* Only insert categories for published posts.

= 0.4.1 =
* Move SWT admin to its own screen.
* Added thumbnail support.
* Added custom taxonomy (including post formats) support.
* Update admin screens for WordPress 3.1.

= 0.4.0.1 =
* Bug fix - only push published content to the tags blog

= 0.4 =
* Added option to include pages in tags blog.
* Added option to include non search engine indexed blogs if tags blog not indexed.
* Added option for post meta to be copied with post.
