# WP REST API V2 Custom Post Fields

![Banner](https://github.com/Vatsov/wp-rest-api-v2-custom-post-fields/blob/master/assets/wp-rest-api-v2-custom-fields.png)  
[Shows Advanced Custom Field output to the WP REST API V2 for posts.](https://wordpress.org/plugins/wp-rest-api-v2-custom-post-fields/)

* **Contributors:** [Deyan Vatsov](https://wordpress.org/support/profile/vatsov)  
* **Tags:** [api](https://wordpress.org/plugins/tags/api), [json](https://wordpress.org/plugins/tags/json), [REST](https://wordpress.org/plugins/tags/rest), [rest-api](https://wordpress.org/plugins/tags/rest-api), [wp-api](https://wordpress.org/plugins/tags/wp-api), [advanced custom post fields](https://wordpress.org/plugins/tags/custom-post-types), [ACF](https://wordpress.org/plugins/tags/acf)  
* **Requires at least:** 4.3  
* **Tested up to:** 4.4.5  
* **Stable tag:** 0.2  
* **License:** [GPLv2 or later](http://www.gnu.org/licenses/gpl-2.0.html)  

<br>
- [Description](#description)
- [Installation](#installation)
- [Filters](#filters)
- [Changelog](#changelog)


Description
====

This plugin combines the two of the best WordPress plugins: [WP REST API](https://wordpress.org/plugins/rest-api/ "WP REST API") and [Advanced Custom Fields](https://wordpress.org/plugins/advanced-custom-fields/ "Advanced Custom Fields").  
Support and Requests please in [GitHub](https://github.com/Vatsov/wp-rest-api-v2-custom-post-fields).  


Installation
====

This plugin requires having [WP REST API](https://wordpress.org/plugins/rest-api/ "WP REST API") and [Advanced Custom Fields](https://wordpress.org/plugins/advanced-custom-fields/ "Advanced Custom Fields") installed and activated or it won't be of any use.  

* **Manual Installation:**  
Upload the entire /wp-rest-api-v2-custom-post-fields directory to the /wp-content/plugins/ directory.

* **Better Installation:**  
Go to Plugins > Add New in your WordPress admin and search for 'WP REST API V2 Custom Post Fields'.

Once installed, activate 'WP REST API V2 Custom Post Fields' from WordPress plugins dashboard page and you're ready to go.

This plugin works straight out of the box.


Filters
====
| Endpoint  |
|-----------|
| /wp-json/wp/v2/posts?filter[meta_key]=**{custom-field-name}**&filter[meta_value]=**{custom-field-value}** |



If you want to limit the fields you have to add the allowed meta keys in 'allowed_meta_keys' array in `plugin.php`

```PHP
$allowed_meta_keys = array( 'custom-field-name' );
```


Changelog
====
#### 0.2 - (29 April 2016) ####
* Allow filter by meta key/value.


#### 0.1 - (10 April 2016) ####
* Initial Release.

<br>
<br>
Props [Deyan Vatsov](https://github.com/Vatsov)
