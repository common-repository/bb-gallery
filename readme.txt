=== Backbone Bootstrap Gallery ===
Contributors: Magenta Cuda
Tags: gallery, shortcode, lightbox, slideshow, responsive, plug-compatible, replacement
Requires at least: 4.4
Tested up to: 4.9
Stable tag: 1.8.2.4.5.1
Requires PHP: 5.6
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Responsive plug-compatible replacement for the built-in WordPress gallery shortcode.

== Description ==
This is a responsive, mobile-friendly, plug-compatible replacement for the built-in WordPress gallery shortcode. You can view a working sample web page using this plugin at [my portfolio website](http://magentacuda.com/demo-bbgallery/). It is implemented using a [Backbone.js](http://backbonejs.org/) Model-View-Presenter (MVP) populated via the [WordPress REST API](http://v2.wp-api.org/). It is styled by a [Twitter Bootstrap 3](http://getbootstrap.com/) stylesheet and has touch optimizations from [jQuery Mobile](https://jquerymobile.com/). Using a MVP allows you to [switch instantaneously](http://docs.magentacuda.com/#navbar) (i.e. without doing a HTTP request) between multiple views of a gallery. The default implementation supports a [gallery view](http://docs.magentacuda.com/#gallery), [Miro's Justified Gallery](http://miromannino.github.io/Justified-Gallery/) view, a [carousel view](http://docs.magentacuda.com/#carousel), a [tabs view](http://docs.magentacuda.com/#tabs) and a [dense view](http://docs.magentacuda.com/#dense) of the gallery. Using the WP REST API allows you to [dynamically load](http://docs.magentacuda.com/#alt_galleries) (i.e. without reloading the entire page) new galleries. The view is styled by a Twitter Bootstrap 3 stylesheet so it is automatically responsive. You can easily modify the Backbone templates to create your own customized views of the gallery. The homepage for this plug-in is [http://docs.magentacuda.com/](http://docs.magentacuda.com/).

== Installation ==
1. Upload the folder "bb-gallery" to the "/wp-content/plugins/" directory.
2. Activate the plugin using the "Dashboard > Plugins > Installed Plugins" page.
3. Check the "Enable BB Gallery" option on the "Dashboard > Settings > Media" page. The defaults for all other options should work reasonably well. Save the settings.
4. Visit any page which has a gallery shortcode.
5. If you are not happy simply uninstall the plugin. Your website will not be changed in anyway.

== Frequently Asked Questions ==
= Why is the page loading slowly? =
BB Gallery can preload full size images for better user interactivity. This does not work well for low bandwidth and/or slow cpus. You can set the bandwidth option to "low" to prevent the preloading of full size images.

= Where is the documentation? =
http://docs.magentacuda.com/

== Screenshots ==
1. [Multiple Views of a Gallery](http://docs.magentacuda.com/#navbar)
2. [Miro's Justified Gallery](http://docs.magentacuda.com/#view-justified)
3. [WordPress Gallery](http://docs.magentacuda.com/#view-gallery)
4. [Alternate Flexbox Gallery View](http://docs.magentacuda.com/#gallery-flexbox)
5. [Carousel](http://docs.magentacuda.com/#view-carousel)
6. [Tabbed Gallery](http://docs.magentacuda.com/#view-tabs)
7. [Dense Gallery](http://docs.magentacuda.com/#view-dense)
8. [Dynamically Loading Galleries](http://docs.magentacuda.com/#alt_galleries)
9. Dynamically Generating Galleries from Search Criteria
10. [Full-Size Image Overlay of the Selected Image](http://docs.magentacuda.com/#overlay)
11. [Image Info Overlay of the Selected Image](http://docs.magentacuda.com/#alt-overlay)
12. Mobile Portrait View
13. [User Options Pane](http://docs.magentacuda.com/#options)
14. [Admin Settings](http://docs.magentacuda.com/#installation)

== Changelog ==

= 1.8.2.4.5.1 =

* fix bad url

= 1.8.2.4.5 =

* update links to new documentation website
* add info overlay to gallery and carousel views

= 1.8.2.4.4 =

* add info overlay to Miro's gallery

= 1.8.2.4.3 =

* disable loading of unneeded hi-res thumbnails
* fix alignment bug in fullscreen landscape mode

= 1.8.2.4.2 =

* bb_tags now includes unattached images
* search now uses the bb_tags taxonomy

= 1.8.2.4.1 =

* css tweaks

= 1.8.2.4 =

* tweaks to support the 2017 theme
* css tweaks for better fit and finish

= 1.8.2.3 =

* fix compatibility bug with Yoast SEO and Jetpack

= 1.8.2.2 =

* workaround for a bug? in Chrome where navbar is hidden after the image overlay is closed.
* fix bug where search result back pager shows wrong default view.

= 1.8.2.1 =

* fix bug where search results shows in the wrong default view
* add missing Justified preferred row height setting

= 1.8.2 =

* added support for a fullscreen view
* change default to not preload full size images
* bug fixes and css tweaks

= 1.8.1.1 =

* make compatible with the new WordPress REST API released with 4.7
* fix HTML validation errors
* some small enhancements, css tweaks and bug fixes

= 1.8.1 =

* some small enhancements, css tweaks and bug fixes

= 1.8 =

* replaced &lt;picture&gt; with &lt;img srcset&gt; for better support of Retina displays
* added support for [Miro's Justified Gallery](http://miromannino.github.io/Justified-Gallery/)
* bug fixes and css tweaks

= 1.7.3.4 =

* bug fix

= 1.7.3.3 =

* bug fix

= 1.7.3.2 =

* bug fixes
* compatibility with WordPress 4.6 RC1

= 1.7.3.1 =

* add object-fit contain and fill modes to tiles view
* css tweaks and bug fixes

= 1.7.3 =

* added tiles view - show images as [butt joined square image tiles](http://docs.magentacuda.com/#gallery)
* css tweaks and bug fixes

= 1.7.1.2 =

* option to [embed carousel inside post content](http://docs.magentacuda.com/#carousel)
* option to individually specify initial view of gallery
* css tweaks to prettify carousel

= 1.7.1.1 =

* show loadable galleries as a gallery of clickable representative images in place of a list of clickable titles
* bug fixes and usability enhancements

= 1.7.1 =

* option to make the carousel as the initial view
* option to show the dynamically loadable galleries as tabs
* bug fixes, css tweaks and usability enhancements

= 1.7 =

* support for dynamically loading galleries using the WordPress REST API to populate Backbone.js collections.

= 1.5.5 =

* use the WordPress REST API if available - no new features just a more modern implementation
* css tweaks and bug fixes

= 1.5.3.1.1 =

* compatible with WordPress 4.5-RC1
* added language support
* more integration with jQuery Mobile

= 1.5.3.1 =

* replaced the Bootstrap carousel indicators with a jQuery mobile slider which is much more mobile friendly

= 1.5.3 =

* added support for mobile features: swipe, orientation change, ...
* fix overlay bug on old Internet Explorer
* add pause control to carousel

= 1.5.2.1 =
* various enhancements, bug fixes and improvements to code quality

= 1.5.2 =
* support history for multi-part search results

= 1.5.1 =
* support multi-part search results
* css tweaks

= 1.5 =
* search added
* enhancements for mobile

= 1.3.3 =
* fixes for problems with mobile (touch screen, small screen and/or low bandwidth) devices

= 1.3.2 =
* add carousel interval option
* allow front-end to set options (minimum image width, number of columns, carousel interval) and save as a cookie

= 1.3.1 =
* better support for captions
* description now supports shortcodes
* prettify UI

= 1.3 =
* The gallery view and the dense view now support displaying a full viewport overlay of a selected image

= 1.2.1 =
* implement CSS object-fit in JavaScript for Microsoft Edge which does not have the CSS object-fit
* improved tabs view

= 1.2 =
* added dense view

= 1.1 =
* improved flex gallery

= 1.0 =
* Initial release.

== Upgrade Notice ==

= 1.8.2.4.5.1 =

* fix bad url

= 1.8.2.4.5 =

* update links to new documentation website
* add info overlay to gallery and carousel views

= 1.8.2.4.4 =

* add info overlay to Miro's gallery

= 1.8.2.4.3 =

* disable loading of unneeded hi-res thumbnails
* fix alignment bug in fullscreen landscape mode

= 1.8.2.4.2 =

* bb_tags now includes unattached images
* search now uses the bb_tags taxonomy

= 1.8.2.4.1 =

* css tweaks

= 1.8.2.4 =

* tweaks to support the 2017 theme
* css tweaks for better fit and finish

= 1.8.2.3 =

* fix compatibility bug with Yoast SEO and Jetpack

= 1.8.2.2 =

* workaround for a bug? in Chrome where navbar is hidden after the image overlay is closed.
* fix bug where search result back pager shows wrong default view.

= 1.8.2.1 =

* fix bug where search results shows in the wrong default view
* add missing Justified preferred row height setting

= 1.8.2 =

* added support for a fullscreen view
* change default to not preload full size images
* bug fixes and css tweaks

= 1.8.1.1 =

* make compatible with the new WordPress REST API released with 4.7
* fix HTML validation errors
* some small enhancements, css tweaks and bug fixes

= 1.8.1 =

* some small enhancements, css tweaks and bug fixes

= 1.8 =

* replaced &lt;picture&gt; with &lt;img srcset&gt; for better support of Retina displays
* added support for [Miro's Justified Gallery](http://miromannino.github.io/Justified-Gallery/)
* bug fixes and css tweaks

= 1.7.3.4 =

* bug fix

= 1.7.3.3 =

* bug fix

= 1.7.3.2 =

* bug fixes
* compatibility with WordPress 4.6 RC1

= 1.7.3.1 =

* add object-fit contain and fill modes to tiles view
* css tweaks and bug fixes

= 1.7.3 =

* added tiles view - show images as butt joined square image tiles
* css tweaks and bug fixes

= 1.7.1.2 =

* option to embed carousel inside post content
* option to individually specify initial view of gallery
* css tweaks to prettify carousel

= 1.7.1.1 =

* show loadable galleries as a gallery of clickable representative images in place of a list of clickable titles
* bug fixes and usability enhancements

= 1.7.1 =

* option to make the carousel as the initial view
* option to show the dynamically loadable galleries as tabs
* bug fixes, css tweaks and usability enhancements

= 1.7 =

* support for dynamically loading galleries using the WordPress REST API to populate Backbone.js collections.

= 1.5.5 =

* use the WordPress REST API if available - no new features just a more modern implementation
* css tweaks and bug fixes

= 1.5.3.1.1 =

* compatible with WordPress 4.5-RC1
* added language support
* more integration with jQuery Mobile

= 1.5.3.1 =

* replaced the Bootstrap carousel indicators with a jQuery mobile slider which is much more mobile friendly

= 1.5.3 =

* added support for mobile features: swipe, orientation change, ...
* fix overlay bug on old Internet Explorer
* add pause control to carousel

= 1.5.2.1 =
* various enhancements, bug fixes and improvements to code quality

= 1.5.2 =
* support history for multi-part search results

= 1.5.1 =
* support multi-part search results
* css tweaks

= 1.5 =
* search added
* enhancements for mobile

= 1.3.3 =
* fixes for problems with mobile (touch screen, small screen and/or low bandwidth) devices

= 1.3.2 =
* add carousel interval option
* allow front-end to set options (minimum image width, number of columns, carousel interval) and save as a cookie

= 1.3.1 =
* better support for captions
* description now supports shortcodes
* prettify UI

= 1.3 =
* The gallery view and the dense view now support displaying a full viewport overlay of a selected image

= 1.2.1 =
* implement CSS object-fit in JavaScript for Microsoft Edge which does not have the CSS object-fit
* improved tabs view

= 1.2 =
* added dense view

= 1.1 =
* improved flex gallery

= 1.0 =
* Initial release.

