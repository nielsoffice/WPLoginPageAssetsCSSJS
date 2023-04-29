# WPLoginPageAssetsCSSJS
WP Login page add CSS and JS


```PHP
// Admin page CSS
function myplugin_enqueue_style_login() {

  $src = plugin_dir_url( __FILE__ ) .'admin/css/example-admin.css';

  wp_enqueue_style( 'myplugin-login', $src, array(), null, 'all' );

}
add_action( 'login_enqueue_scripts', 'myplugin_enqueue_style_login' );
```

```PHP
// Admin page JS
function myplugin_enqueue_script_login() {

  $src = plugin_dir_url( __FILE__ ) .'admin/js/example-admin.js';

  wp_enqueue_script( 'myplugin-login', $src, array(), null, false );

}
add_action( 'login_enqueue_scripts', 'myplugin_enqueue_script_login' );
``
