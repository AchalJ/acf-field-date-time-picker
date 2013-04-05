=== Advanced Custom Fields: Date and Time Picker Field ===
Contributors: PerS
Tags: 
Requires at least: 3.4
Tested up to: 3.5.1
Stable tag: trunk
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Date and Time Picker field for Advanced Custom Fields

== Description ==

This is an add-on for the [Advanced Custom Fields](http://wordpress.org/extend/plugins/advanced-custom-fields/) WordPress plugin, that allows you to add a Date and Time Picker field type.

= Compatibility =

This add-on will work with:

* version 4 and up
* version 3 and bellow

== Installation ==

This add-on can be treated as both a WP plugin and a theme include.

= Plugin =
1. Copy the 'acf-date_time_picker' folder into your plugins folder
2. Activate the plugin via the Plugins admin page

= Include =

NOT SUPPORTED in 2.0.0.beta

1.	Copy the 'acf-date_time_picker' folder into your theme folder (can use sub folders). You can place the folder anywhere inside the 'wp-content' directory
2.	Edit your functions.php file and add the code below (Make sure the path is correct to include the acf-date_time_picker.php file)

`
add_action('acf/register_fields', 'my_register_fields');

function my_register_fields()
{
	include_once('acf-date_time_picker/acf-date_time_picker.php');
}
`

== Changelog ==

= 2.0.0.beta =
* Total rewrite, based on the [acf-field-type-template](https://github.com/elliotcondon/acf-field-type-template). Works with ACF v3 and ACF v4. In this beta you can only add the Date Time Picker field as a plugin (i.e. not as a template field).
= 1.2.0 = 
* Updated jquery-ui-timepicker-addon.js to the latest version (1.0.0) and added localization support.
= 1.1.1 =
* Fixed a small bug
= 1.1 =
* Change name to Date and Time Picker to reflect the new option to select between Date and Time picker or Time Picker only. Thanks to Wilfrid for point this out (not sure why I didn’t include it in 1.0)
= 1.0 =
* Initial version
