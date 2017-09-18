# General

* 404 page


# UI

* Favicon
* Basic elements have styles
	* <a>
	* <p>
	* <ul>/<ol>
	* <blockquote>


# SEO

* Run though a quick SEO Audit scanner for glaring issues
* Pages have SEO titles
* Alt tags on images
* Sitemap has been created
* Robots.txt file has been created
* Site is set to be crawled by the search engines


# Site Speed

* Images are scaled to the ideal size and run through a compressor
* CSS is compressed and consolidated
* Javascript is compressed and consolidated


# WordPress Specific

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
