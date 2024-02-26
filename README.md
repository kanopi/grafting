## Grafting Drupal Recipe

A simple Drupal Recipe for installing and configuring the migration supporting base modules.

### Configuring Drupal for Recipes

See https://www.drupal.org/files/issues/2023-10-01/Configuring%20Drupal%20to%20Apply%20Recipes.md

### Installing this Recipe

`composer require kanopi/grafting`

### Applying this Recipe

From your webroot run `php core/scripts/drupal recipe recipes/contrib/grafting` and `drush cr`

If you have our Docksal command in your project, `fin recipe-apply grafting`

### Unpacking this Recipe

To unpack this recipe's dependencies to your site's composer.json, in the root of your project run:

`composer unpack kanopi/grafting`

If you have our Docksal command in your project, `fin recipe-unpack kanopi/grafting`

### Known Issues

- TBD
