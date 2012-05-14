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

Give your visitors the ability to easily access all your site's content. This is meant for sites with high page numbers. Any page between 1 and 999 can be accessed with a maximum of 3 clicks (see screenshots).

So far, this code has been tested on archive an category pages. Stable version will come soon.

Please leave feedback, bug reports or comments at https://github.com/paddelboot/3pagination/issues

== Installation ==

<h4>Installation</h4>
1. Upload `3pagination.php` to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Display the navigation using `<?php threepagination::draw(); ?>`

</h4>Functions</h4>
`draw ( $pretty = TRUE, $max_num_pages = FALSE, $labels = TRUE, $css = 'classic' )`
Display the navigation
<ul>
<li>$pretty | Are you using pretty permalinks?</li>
<li>$max_num_pages | Limit to a maximum number of pages</li>
<li>$labels | Display or not the navigation arrows</li>
<li>$css | CSS class name that will be appended to the main div container</li>
</ul>

`get ( $pretty = TRUE, $num_items = FALSE, $per_page = FALSE, $labels = TRUE, $css = 'classic' )`
Return the navigation as a HTML string

<h4>Example usages</h4>
`threepagination::draw ( TRUE, FALSE, FALSE, 'my_custom_class' )`
Displays the navigation on a website that uses pretty urls, takes the standard page count, hides the navigation arrows and uses a CSS class 'my_custom_class'


== Screenshots ==

1. Example of a pagination display


== Changelog ==

= 0.1a =
- Initial version

== A brief Markdown Example ==

`<?php threepagination::draw(); ?>`
`<?php $string = threepagination::get(); ?>`
