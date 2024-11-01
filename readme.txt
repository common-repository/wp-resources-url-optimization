=== WP Resources URL Optimization ===
Contributors: litefeel  
Tags: optimization, style, script, resources, plugins, query-string  
Donate link: https://www.paypal.me/litefeel  
Requires at least: 3.0.0  
Tested up to: 4.7.3  
Stable tag: 1.6  
License: GPLv2  
License URI: http://www.gnu.org/licenses/gpl-2.0.html  

WP Resources URL Optimization is a Wordpress plugin optimized browser cache, it will greatly enhance the website page display speed and reduce the pressure of the server to handle static files.

== Description ==

WP Resources URL Optimization is a Wordpress plugin optimized browser cache,
it will greatly enhance the website page display speed and reduce the pressure of the server to handle static files.
Default wp added after the static files the query string(version number) to ensure that the static files are modified 
immediately after the performance to the browser (front-end), this way there is a drawback: 
the browser will request the server regardless of whether the file is modified,
If the file has been modified it will download the new file, 
if the file has not been modified http status code 304 is returned to inform the browser reads the local cache. 
The goal of the plugin: do not have to re-initiate the request to the server, 
and directly read the browser cache when the file has not been modified.

Related Links:

* <a href="https://www.litefeel.com/wp-resources-url-optimization/" title="WP Resources URL Optimization Plugin for WordPress">Plugin Homepage</a>
* <a href="https://www.litefeel.com/" title="Author For WP Resources URL Optimization Plugin">Author Homepage</a>
* <a href="https://github.com/litefeel/wp-resources-url-optimization" title="on GitHub">on GitHub</a>

== Installation ==

= Using the WordPress Dashboard =

1. Navigate to the 'Add New' in the plugins dashboard
2. Search for 'WP Resources URL Optimization'
3. Click 'Install Now'
4. Activate the plugin on the Plugin dashboard

= Uploading in WordPress Dashboard =

1. Download `wp-resources-url-optimization.zip` from the WordPress plugins repository.
2. Navigate to the 'Add New' in the plugins dashboard
3. Navigate to the 'Upload' area
4. Select `wp-resources-url-optimization.zip` from your computer
5. Click 'Install Now'
6. Activate the plugin in the Plugin dashboard

= Using FTP =

1. Download `wp-resources-url-optimization.zip`
2. Extract the `wp-resources-url-optimization` directory to your computer
3. Upload the `wp-resources-url-optimization` directory to the `/wp-content/plugins/` directory
4. Activate the plugin in the Plugin dashboard


== Frequently Asked Questions ==

= The plugin will affect what files? =

The plug-in will modify the css and js file url used in the css sprite technology, the picture address are also taken to modify, while ensuring css work properly.

= Why is the plugin is enabled, js and css url did not change? =

Please ensure that js and css files added by use wp_enqueue_script and wp_enqueue_style method.

= My css file has css sprite technology, the picture will load properly? =

Yes, The plug has been considered the problem of the sprite.

= When I want to modify some files, which files I need to modify? =

Please modify the original file, not automatically generated files.

= When I want to add some files, Do i need to add a version number? =

No. The plugin will automatically generate a new files when the file modified. 

== Changelog ==

= 1.6.2 =

* Join translate.wordpress.org

= 1.6 =

* Transfer ownership

= 1.5.1.2 =

* Tested up to 4.4

= 1.5.1.1 =

* Tested up to: 4.0

= 1.5.1 =

* Tested up to: 3.9.1

= 1.5.0 =

* New: add config for only remove query string.

= 1.4.3 =

* Compatibility check for 3.6, nothing new, just bump version to tell everyone this plugin still works.

= 1.4.2 =

* Fixed: Displays an warning when the resources is not file.

= 1.4 =

* Fixed: Displays an error when you first install the plugin.

= 1.3 =

* New: Automatically delete the older version of the backup file.

= 1.2.2 =

* Fixed: ignore log trace.

= 1.2.1 =

* Fixed: Fix wrong css sprite url.

= 1.2 =

* Fixed: Fix Not working when WordPress Address and Site Address are not the same.
* Modify: Move all back files to '{WordPress Address}/wp-content/wp-resources-back/' directory.

= 1.1 =

* Fixed: Fix 'File_exists' of warning  when the css sprite is relative path.

= 1.0 =

* Initial public release.



  [1.6.2]: https://github.com/litefeel/wp-resources-url-optimization/releases/tag/1.6.2
  [1.6]: https://github.com/litefeel/wp-resources-url-optimization/releases/tag/1.6
