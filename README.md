# Drupal Libraries -- make easy Drupal libraries management with Composer

This is a custom Composer repository built with [satis](https://github.com/composer/satis) for 3rd party libraries used by Drupal contributed projects
(modules/themes/distributions)

### How to use?

Add the following lines to your project's root `composer.json` file
```
{
  "repositories": [{
    "type": "composer",
    "url": "https://drulibs.com"
  }]
}
```

After adding the above lines, your root `composer.json` file may look like:

```
{
    ...
    "type": "project",
    "repositories": [
        {
            "type": "composer",
            "url": "https://packages.drupal.org/8"
        },
        {
            "type": "composer",
            "url": "https://drulibs.com"
        }
    ],
    "require": {
    ...
```

That's all.

Next, just add the library/libraries by Composer as normal. For
example:

```bash
composer require drulibs-enyo/dropzone
```

or

```bash
composer require drulibs-enyo/dropzone:5.7.1
```

However, as you can see, `drulibs-` needs to be prepended to the package/library
name. That's the naming convention.

### Index

<table>
    <tr><td>Package/Library</td><th>Version</th><th>Relate Project(s)</th></tr>
    <tr><td>drulibs-colorlibhq/adminlte</td><td>2.4.10, 3.0.5</td><td></td></tr>
    <tr><td>drulibs-desandro/masonry</td><td>3.3.2</td><td><a href="https://drupal.org/project/content_browser">Content Browser</a></td></tr>
    <tr><td>drulibs-enyo/dropzone</td><td>5.7.1</td><td><a href="https://drupal.org/project/dropzonejs">DropzoneJS</a></td></tr>
    <tr><td>drulibs-fontawesome/fontawesome</td><td>5.15.1</td><td><a href="https://drupal.org/project/fontawesome">Font Awesome Icons</a></td></tr>
    <tr><td>drulibs-itsjavi/fontawesome-iconpicker</td><td>3.2.0</td><td><a href="https://drupal.org/project/fontawesome_menu_icons">Font Awesome Menu Icons</a></td></tr>
    <tr><td>drulibs-krambuhl/custom-event-polyfill</td><td>1.0.0, 1.0.7</td><td></td></tr>
    <tr><td>drulibs-select2/select2</td><td>4.0.12, 4.0.13</td><td><a href="https://drupal.org/project/select2">Select2</a></td></tr>
    <tr><td>drulibs-zenorocha/clipboard.js</td><td>2.0.6</td><td><a href="https://drupal.org/project/clipboardjs">Clipboard.js</a></td></tr>
</table>