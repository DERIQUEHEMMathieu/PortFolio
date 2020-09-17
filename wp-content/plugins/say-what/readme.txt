=== Say what? ===
Contributors: leewillis77
Donate link: http://plugins.leewillis.co.uk/downloads/say-what-pro?utm_source=wordpress&utm_medium=www&utm_campaign=say-what
Tags: string, change, translation
Requires at least: 4.3
Tested up to: 5.5
Stable tag: 1.9.6

== Description ==
An easy-to-use plugin that allows you to alter strings on your site without editing WordPress core, or plugin code. Simply enter the current string, and what you want to replace it with and the plugin will automatically do the rest!

The plugin's available for forking and contribution over on [GitHub](https://github.com/leewillis77/say-what)

Check out [Say What Pro](https://plugins.leewillis.co.uk/downloads/say-what-pro/) for:

* **String discovery** - Don't have the time/expertise to find strings in the code, set up replacements easily with easy-to-use autocomplete features
* **Wildcard string replacements** - replace individual words, or fragments across your whole site
* **Multi-lingual support** - set different replacements for different languages on multi-lingual sites
* **Import/export features** - Easy import/export of replacements through the user interface

## Treeware

You're free to use this package for free, but if it makes it to your production environment please [buy the world some trees](https://ecologi.com/ademtisoftware?gift-trees).

== Installation ==

* Install it as you would any other plugin
* Activate it
* Head over to Tools &raquo; Text changes and configure some string replacements

== Frequently Asked Questions ==

= Can I use it to change any string? =
You can only use the plugin to translate strings which are marked for translation.

= How do I find the string to translate? =
You can either have a guess, or checkout the plugin in question's source code, translatable strings are generally wrapped in __(), _e(), _n(), or _x(), for example:

`$foo = __('This is a translatable string', 'plugin-domain');`

The article [here](https://plugins.leewillis.co.uk/doc_post/replacing-wordpress-strings-context/) shows some examples of what you're looking for. Alternatively, the [Pro version of the plugin](https://plugins.leewillis.co.uk/downloads/say-what-pro/) provides a String Discovery mode which means you can search for strings on your site via autocomplete suggestions.

= Is there any support for importing replacements? =
"Say What?" has preliminary support for exporting, and importing replacements via [http://wp-cli.org/](WP-CLI). The following commands are currently
supported:

* export - Export all current string replacements.
* import - Import string replacements from a CSV file.
* list - Export all current string replacements. Synonym for 'export'.
* update - update string replacements from a CSV file.

See the [GitHub homepage](https://github.com/leewillis77/say-what) for examples.

= Can I set different replacements for different languages? =
Not in the free plugin, however this is available in the [Pro version of the plugin](https://plugins.leewillis.co.uk/downloads/say-what-pro/)

== Screenshots ==

1. Finding a string to replace
2. The admin screen - setting up a replacement
3. The result


== Changelog ==

= 1.9.6 =
* Fix link in documentation

= 1.9.5 = 
* WordPress 5.5 compatibility
* Changes to Treeware links

= 1.9.4 =
* Ensure help links open in new windows

= 1.9.3 =
* Fix link target in Treeware content

= 1.9.2 =
* Suggest Treeware donations

= 1.9.1 =
* Update information about Pro features

= 1.9.0 =
* Fix issue adding more strings after downgrade from Pro
* Update text domain of plugin to match wordpress.org guidelines to aid translations

= 1.8.2 =
* Documentation updates only

= 1.8.1 =
* Update plugin links, include settings and upgrade link
* Update documentation about pro features
* Admin styling fixes

= 1.8.0 =
* Fix issues where entities could be double encoded on admin screens.

= 1.7.1 =
* Update to admin marketing message. No functional changes.

= 1.7 =
* Support for _n() and _nx()
* Support for multi-line strings

= 1.6 =
Introduce filters that allows back compatibility for plugins that change their text-domain. Props Pippin Williamson

= 1.5 =
Avoid warnings on initial activation.
Avoid issues where strings contain HTML / entities

= 1.4 =
Add info box about Pro version

= 1.3 =
Support for WP-CLI import and export.

= 1.2 =
Swap database to UTF-8 to fix problems entering non-ASCII strings.

= 1.1 =
Fix incorrect escaping on the admin screens.

= 1.0.1 =
Fix initial DB table creation
Fix translations for strings with no domain

= 1.0 =
Allow strings with context to be replaced

= 0.9.3 =
Documentation improvements

= 0.9.2 =
Avoid wpdb->prepare warning
Minor admin fixes, don't double translate strings

= 0.9.1 =
Fix issue with fields being swapped when first entered

= 0.9 =
Beta ready for testing and feedback
