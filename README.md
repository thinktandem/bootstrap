# Bootstrap 4.3.1

The built assets with popper.js for Drupal 8 composer install

To use in your theme, add this into your libraries yml

```yaml
bootstrap:
  version: 4.3.1
  css:
    component:
      ../../../libraries/bootstrap/css/bootstrap.min.css: {}
  js:
    ../../../libraries/bootstrap/js/bootstrap.min.js: {}
  dependencies:
    - core/jquery
    - your_theme/popper

popper:
  version: 1.14.7
  js:
    ../../../libraries/bootstrap/js/popper.min.js: {}
  dependencies:
    - core/jquery
```

In your theme.info.yml

```yaml
libraries:
- your_theme/popper
- your_theme/bootstrap
```
