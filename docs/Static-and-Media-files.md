## Static and Media files

#### Static files

  Websites are need some static files, these static files are js, css, images etc. Flash Framework help us to manage these static files.

  - Set your static files directory in settings file.

```php
$setting['static'] = '/application/your_static_dir';
```

  - Use static files in templates.

```html
<!DOCTYPE>
<html>
<head>
  <title>cat image</title>
</head>
<body>
  <img src='<?php echo $this->static.'/img/cat.jpg'; ?>' alt='cat image'/>
  <!-- or -->
  <img src='<?php echo $this->uri->static('/img/cat.jpg'); ?>' alt='cat image'/>
</body>
</html>
```

  - `$this->static` variable store your static directory path.
  - `$this->uri->static()` function return full path of static directory.

#### Media files

  media directory is used to upload files like user profile image, files etc.

  - Set your media files directory in settings file.

```php
$setting['media'] = '/application/your_media_dir';
```
  - Use media files in templates.

```html
<!DOCTYPE>
<html>
<head>
  <title>cat image</title>
</head>
<body>
  <img src='<?php echo $this->media.'/img/cat.jpg'; ?>' alt='cat image'/>
  <!-- or -->
  <img src='<?php echo $this->uri->media('/img/cat.jpg'); ?>' alt='cat image'/>
</body>
</html>
```

  - `$this->media` variable store your media directory path.
  - `$this->uri->media()` function return full path of media directory.
