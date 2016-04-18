# WP REST API V2 Custom Post Fields
====
Shows Advanced Custom Field output to the WP REST API V2 for posts.

https://wordpress.org/plugins/wp-rest-api-v2-custom-post-fields/

- [Installation](#installation)
- [Filters](#filters)

Installation
====

This plugin requires having WP API installed and activated or it won't be of any use.

*Manual Installation:
Upload the entire /wp-rest-api-v2-custom-post-fields directory to the /wp-content/plugins/ directory.

*Better Installation:
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