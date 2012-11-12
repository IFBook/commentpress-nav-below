CommentPress Nav Below
======================

This is a child theme for [*CommentPress Core*](https://github.com/IFBook/commentpress-core) where the toolbar has been moved to sit under the branding, closer to the content. Use it as a "starter pack" for creating your own look and feel.

Please note: this child theme only works with the *CommentPress Default Theme* supplied with the *CommentPress Core* plugin. Please make sure that *CommentPress Core* is properly installed before using it.

## Installation ##

Please install and activate the theme by doing the following:

1. Unzip the .zip file and, if needed, rename the enclosing folder so that the theme's files are located directly inside `/wp-content/themes/commentpress-nav-below`.
2. Activate the theme.
3. Visit settings pages and configure theme.

##### Important note for Multisite #####

If you want to use this theme **without network-activating *CommentPress Core*** then you will need to network-activate this theme despite it appearing in the "Broken" themes section of your Network Admin. To do so, you need to use the "Bulk Actions" dropdown. It will then appear as an available theme only on blogs that have *CommentPress Core* enabled. If you **have network-enabled *CommentPress Core***, then this theme will appear as normal.

## Notes ##

The JavaScript functionality to hide/show the branding has been disabled by hiding the relevant toolbar button. This functionality could be reinstated by replacing the JavaScript file that provides it with an amended one, but would not be for the technically faint-hearted.

To do so, you would use `wp_dequeue_script()` to remove the existing javascripts, the enqueue your own versions of them. See the function `get_javascript()` in the file `class_commentpress_display.php` included in the *CommentPress Core* plugin.