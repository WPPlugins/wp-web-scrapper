=== WP Web Scraper ===
Contributors: akshay_raje, WisdmLabs
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_xclick&business=akshay.raje@gmail.com&item_name=Donation+for+WP+Web+Scraper
Tags: web scraping, curl, css selector, xpath, regex, realtime, post, sidebar, page, stock market, html, import
Requires at least: 2.8
Tested up to: 4.1
Stable tag: 3.5
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

An easy to implement web data extractor for WordPress. The plugin display realtime data from any website directly into your posts, pages or sidebar.


== Description ==

An easy to implement web data extractor for WordPress. This plugin can be used to display realtime data from any websites directly into your posts, pages or sidebar. It temporarily caches the content on your website. You can use this plugin to include realtime stock quotes, cricket or soccer scores or any other generic content from public domains.

> <strong>Important Note:</strong>
> Web scraping is a practice of extracting data from another website. When doing so, you need to ensure that you have the permissions to use the content, and you need to give due credit to the original source.
> Make sure when scraping content, you do not violate any copyright laws.

**Features include:**

1. Scraped output can be displayed through custom template tag, shortcode in page, post and sidebar (through a text widget).
2. Configurable caching of scraped data. Cache timeout can be defined in minutes for every scraped data.
3. Configurable Useragent for your scraper can be set for every scrape.
4. Configurable default settings like enabling, useragent, timeout, caching, error handling.
5. [Multiple ways to query content](http://wp-ws.net/docs/query/) - CSS Selector, XPath or Regex.
6. A wide range of [arguments for parsing](http://wp-ws.net/docs/arguments-api/) content.
7. Option to pass post arguments to a URL to be scraped.
8. Dynamic conversion of scraped content to specified character encoding to scrape data from a site using different charset.
9. Create scraped pages on the fly using [dynamic generation of URLs](http://wp-ws.net/docs/dynamic-url-headers/) to scrape or post arguments based on your page's get or post arguments.
10. [Callback function](http://wp-ws.net/docs/callback-functions/) for advanced parsing of scraped data.

Check the the official website [wp-ws.net](http://wp-ws.net/) for [documentation](http://wp-ws.net/docs/), browse through [examples](http://wp-ws.net/examples/), or try [paid support](http://wp-ws.net/support/) for crafting a perfectly optimized web scraper.

== Installation ==

1. Upload folder `wp-web-scrapper` to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. [Usage instructions for WP Web Scraper](http://wp-ws.net/faqs/how-to-use-wp-web-scraper/)

Mode details on this on the [FAQs](http://wp-ws.net/faqs/) page

== Frequently Asked Questions ==

* [What is web scraping? Why do I need it in WordPress?](http://wp-ws.net/faqs/what-is-web-scraping-needed-in-wordpress/)
* [How to use WP Web Scraper?](http://wp-ws.net/faqs/how-to-use-wp-web-scraper/)
* [How to optimize performance?](http://wp-ws.net/faqs/how-to-optimize-performance/)
* [Minimum requirements & dependencies](http://wp-ws.net/faqs/minimum-requirements-dependencies/)
* [Posting external content as Posts or Pages](http://wp-ws.net/faqs/posting-external-content-as-posts-or-pages/)

== Documentation ==

* [Arguments API](http://wp-ws.net/docs/arguments-api/)
* [Query - CSS Selectors, XPath and Regex](http://wp-ws.net/docs/query/)
* [Dynamic URL and headers](http://wp-ws.net/docs/dynamic-url-headers/)
* [Callback Functions](http://wp-ws.net/docs/callback-functions/)

== Examples ==

[Example code](http://wp-ws.net/examples/) for some common use cases of the plugin

== Changelog ==

= 3.5 =
* Bug fix: Post request
* Bug fix: gt, lt arguments

= 3.4 =
* Added scrape importer
* replace_query and replace_with now accepted specially formatted array arguments

= 3.3 =
* Basehref bug fix

= 3.2 =
* Documentation website change

= 3.1 =
* Bug fix: Minor bug fixes.

= 3.0 =
* Enhancement: Complete code rewrite, uses PHP DOM directly for faster processing
* Enhancement: Sandbox to test and debug
* Deprecation: Dropped `removetags`
* Changes: Changes in arguments

= 2.8 =
* Enhancement: Migrated caching to the Transients API.
* Enhancement: Clear and find / replace now supports selectors.
* Enhancement: Cleaner code - faster processing.
* Enhancement: More debugging data including processing time.
* Deprecation: Modules are deprecated in support of callback functions.

= 2.7 =
* Enhancement: Added `callback` for flexible as well as advanced parsing.
* Bug fix: Fixed the issue of usage within widget.

= 2.6 =
* Enhancement: Added `removetags` to remove certain tags and content from scrape.
* Bug fix: Retains http-cache and modules on upgrade.

= 2.5 =
* Bug fix: Patched a major security issue related to useragent string settings.

= 2.4 =
* Bug fix: Added xpathdecode to handle complex xpath queries in shortcode.

= 2.3 =
* Enhancement: Added support for xpaths.
* Enhancement: Uses builtin WP_HTTP classes instead of raw cURL or Fopen.
* Enhancement: Complete overhaul of code, architecture and documentation.
* Enhancement: Reversed to filebased cache instead of MySQL tables.

= 2.2 =
* Enhancement: Introduction of special variable `___QUERY_STRING___` for dynamic URLs.
* Enhancement: Upgraded the underlying phpQuery library to single file version.

= 2.1 =
* Enhancement: Option to turn off the debug information displayed as html comment.

= 2.0 =
* Milestone release: Complete overhaul of code, architecture and documentation.
* Bug fix: Multiple bug fixes addressed.

== Upgrade Notice ==

= 3.5 =
* Bug fix: Post request
* Bug fix: gt, lt arguments