=== Plugin Name ===
Contributors: paddelboot
Tags: pagination
Requires at least: 3.3.2
Tested up to: 3.3.2
Stable tag: 0.1a
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Navigate to any page between 1 and 999 with no more than 3 clicks.

== Description ==

Give your visitors the ability to easily access all your site's content. This is meant for sites with high page numbers. Any page between 1 and 999 can be reached with never more than 3 clicks (see screenshots).

So far, this code has been tested on archive an category pages. Stable version will come soon.

== Installation ==

1. Upload `3pagination.php` to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Display the navigation using <?php threepagination::draw(); ?>

== Frequently Asked Questions ==


== Screenshots ==

1. Example of a pagination display


== Changelog ==

= 0.1a =
- Initial version

== Arbitrary section ==

Please leave feedback, bug reports or comments at https://github.com/paddelboot/3pagination

== A brief Markdown Example ==

<?php threepagination::draw(); ?>
<?php $string = threepagination::get(); ?>
