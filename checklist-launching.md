# Final Debugging

* Ensure all test pages, Lorem Ipsum, and test images have been removed
* Ensure all watermarked stock photos have been swapped for licensed photos
* Check all pages for obvious image errors
* Run a speed test to identify potential serious issue and outliers: https://tools.pingdom.com/
* Browser testing for all unique page layouts
	* Test in Chrome
	* Test in Firefox
	* Test in Edge
	* Test in IE
* Responsive Testing for all unique page layouts
	* Test on regular desktop
	* Test on very large desktop
	* Test on netbook/tablet
	* Test on large smartphone
	* Test on small smartphone
* Ensure social network links are correct
* Credit link in the footer or on the about page


# Just before going live & while going live

* Recompile all CSS & JS so it is compressed and consolidated
* Ensure all plugins/modules/etc are up to date
* Ensure contact forms and newsletter signup forms function and are sent to the client's email address and submit complete information
* Backup site theme, database, etc
* Run a [broken link checker](https://validator.w3.org/checklink)
* If payments are taken, verify test mode is turned off and actual payments go through
* Ensure Google Analytics has been installed
* Ensure site is set to allow search engine crawling, be it settings in the CMS or removal of rel="noindex" from header or changing robots.txt
* Ensure all site generated emails are sending properly, especially emails concerning payments
* Enable user registration if applicable, like on an eCommerce website
* **Have someone else double check all major components**


# After Live

* Setup SSL Certificate (if applicable)
* If site has a SSL Certificate, ensure http forwards to https correctly
* Ensure www forwards to non-www (or vice versa)
* Ensure plugin/module/etc licenses are activated on the new domain
* Setup site backups if the host does not provide them - [Vaultpress](https://vaultpress.com/) is great for WordPress sites
* Ensure 301 redirects for all old site pages
* Give clients their login information
