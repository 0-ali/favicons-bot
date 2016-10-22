Requirements: 
-------------

- PHP language, version 4.3.2 or higher.
- GD library (version 2.0.1 or higher, usually included in PHP by default) supports images in formats GIF and PNG.

Usage:
------

```php
<?php
   require_once('src/favicons.class.php');

    $favicon = new favicon('http://www.controlstyle.ru/', 0);
    $fv = $favicon->get_output_data();

    if ($fv!=='')
    {
        header('Content-type: image/png');
        echo $fv;
    }
?>
```

Created By:
-----------
[ControlStyle](http://www.controlstyle.com/articles/programming/text/php-favicon/)




