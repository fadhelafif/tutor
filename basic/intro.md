## Prelude

test 1

![](../img/screenshot.jpg)

add code at `functions.php`

```php
add_theme_support('calibrefx-wraps', array('header', 'subnav', 'inner', 'footer', 'footer-widget'));
```

add code at `app/hooks/childfx_header_hook.php`

```php
<?php
$cfxgenerator->remove('calibrefx_after_header', 'calibrefx_do_nav');
$cfxgenerator->add('calibrefx_header_right_widget', 'calibrefx_do_nav');
?>
```