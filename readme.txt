=== Plugin Name ===
Contributors: paddelboot
Tags: pagination
Requires at least: 3.3.2
Tested up to: 3.4
Stable tag: 1.0
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Navigate to any page between 1 and 999 with no more than 3 clicks.

== Description ==

Give your visitors the ability to easily access all your site's content. This is meant for sites with high page numbers. Any page between 1 and 999 can be accessed with a maximum of 3 clicks (see screenshots).

So far, this code has been tested on index, archive and category pages of some of the most popular WordPress themes.

Please leave feedback, bug reports or comments at https://github.com/paddelboot/3pagination/issues

== Installation ==

<h4>Installation</h4>
1. Upload `3pagination.php` to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Display the pagination using `<?php if ( class_exists( 'threepagination' ) ) : threepagination::draw(); endif; ?>`

<h4>Functions</h4>
draw() : Display the pagination
`draw ( $pretty = TRUE, $max_num_pages = FALSE, $labels = TRUE, $css = 'classic' )`
<ul>
<li>$pretty | Are you using pretty permalinks?</li>
<li>$max_num_pages | Limit to a maximum number of pages</li>
<li>$labels | Display or not the navigation arrows</li>
<li>$css | CSS class name that will be appended to the main div container</li>
</ul>

get() : Return the pagination as a HTML string
`get ( $pretty = TRUE, $num_items = FALSE, $per_page = FALSE, $labels = TRUE, $css = 'classic' )`

<h4>Example usages</h4>
`threepagination::draw ( TRUE, FALSE, FALSE, 'my_custom_class' )`
Displays the pagination on a website that uses pretty urls, takes the standard page count, hides the navigation arrows and uses a CSS class 'my_custom_class'

`$string = threepagination::get ()`
Save the pagination in the `$string` var.

== Screenshots ==

1. Example of a pagination display


== Changelog ==

= 0.1a =
- Initial version

= 0.2a =
- Improved arrow navigation
- replaced $num_items and $per_page with $max_num_pages
- Slightly changed CSS colors

= 1.0 =
- Stable version

== A brief Markdown Example ==

`<?php if ( class_exists( 'threepagination' ) ) : threepagination::draw(); endif; ?>`
`<?php if ( class_exists( 'threepagination' ) ) : threepagination::get(); endif; ?>`
