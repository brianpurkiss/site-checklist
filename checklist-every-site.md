# General

* 404 page
* Pick www or non-www and force a redirect
* Add [Humans.txt](http://humanstxt.org/) to site


# UI

* Favicon
* Basic elements have styles
	* `<a>`
	* `<p>`
	* `<ul>/<ol>`
	* `<blockquote>`
* Print friendly CSS
* [Check for enough color contrast](http://www.checkmycolours.com/)
* [Check for accessibility](https://achecker.ca/checker/index.php)
* Do webfonts load properly on a computer that doesn't have the font installed locally?


# SEO

* Run though a quick SEO Audit scanner for glaring issues
* Pages have SEO titles
* Alt tags on images
* Sitemap has been created
* Robots.txt file has been created
* Site is set to be crawled by the search engines
* [Social oriented Open Graph Protocal](http://ogp.me/) (included in Yoast SEO)


# Site Speed

* Images are scaled to the ideal size and run through a compressor
* CSS is compressed and consolidated
* Javascript is compressed and consolidated


# WordPress Specific

* Check the Site Title and Site Tagline
* Update the general setting's email address and Timezone
* Update WordPress permalinks
* The custom theme's [screenshot.png](https://codex.wordpress.org/Theme_Development#Screenshot) has been set
* Install the Brute Force Login Protection plugin
* Add the following to wp-config.php outside of the "# BEGIN WordPress" and "# End WordPress."
`# Block the include-only files.
RewriteEngine On
RewriteBase /
RewriteRule ^wp-admin/includes/ - [F,L]
RewriteRule !^wp-includes/ - [S=3]
RewriteRule ^wp-includes/[^/]+\.php$ - [F,L]
RewriteRule ^wp-includes/js/tinymce/langs/.+\.php - [F,L]
RewriteRule ^wp-includes/theme-compat/ - [F,L]

order allow,deny
deny from all

# Prevent WP Admin from editing theme and plugin files
define('DISALLOW_FILE_EDIT', true);`
* Set permalinks
* Set site timezone
* Install [Yoast SEO](https://yoast.com/wordpress/plugins/seo/)
