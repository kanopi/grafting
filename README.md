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

## Module Information

> The following is a list of this recipe's modules and what they do.

### Migrate File Entities to Media Entities

This module allows you to migrate Drupal 8.0 file entities to Drupal 8.5 media entities using the migrate module. See the [project page](https://www.drupal.org/project/migrate_file_to_media) for more information.

### Migrate Manifest

Provides a Drush command for running migrations using a manifest format. This is very handy when you want to run migrations in groups usually due to circular references, etc. View [this simple example](https://www.drupal.org/node/2350651#s-running-specific-migrations-using-migrate-manifest) to learn more. See the [project page](https://www.drupal.org/project/migrate_manifest) for more information.

### Migrate Plus

Provides APIs for grouping migrations as well as a facility to manipulate incoming source data in migrations as well as code examples to build custom migrations. Required by Migrate Upgrade. See the [project page](https://www.drupal.org/project/migrate_plus) for more information.

### Migrate Process Markdown to HTML

A process plugin to convert Markdown to HTML. See the [project page](https://www.drupal.org/project/migrate_process_markdown_to_html) for more information.

### Migrate Scanner

Provides a recursive directory scanner for migrations files, which helps to organize migrations into sub-directories. See the [project page](https://www.drupal.org/project/migrate_scanner) for more information.

### Migrate: Skip on 404

Allows core migrations, using either Migrate Drupal or Migrate Upgrade, to stop the normal file migration from failing if it comes across a file that cannot be located. See the [project page](https://www.drupal.org/project/migrate_skip_on_404) for more information.

### Migrate Source UI

User interface for importing data from JSON, CSV or XML sources. Work with migrate tools and other migrate modules to allow someone to upload the source file. See the [project page](https://www.drupal.org/project/migrate_source_ui) for more information.

### Migrate Tools

Since Drush 10.4, most Migrate Tools commands such as migrate:status, migrate:import, and migrate:stop are are included in Drush, except for the migrate:tree command which shows a tree of migration dependencies, which you can get by installing the module. The code-base that made its way into Drush was from an earlier and simpler fork of the Migrate Tools code. For example, Drush does not support migrate plus config entities or provide a progress bar. Over time, the Drush team continues to add features and some of this might become incorporated upstream.
See Upgrade using Drush. See the [project page](https://www.drupal.org/project/migrate_tools) for more information.

### Migrate Upgrade

Provides the migrate:upgrade a Drush command for generating the migrations from a Drupal source site. See the [project page](https://www.drupal.org/project/migrate_upgrade) for more information.

### Migrate: URL2Link

Provides a migration path for the URL module on Drupal 7 to the Link module in Drupal 8 & 9. See the [project page](https://www.drupal.org/project/migrate_url2link) for more information.

### Migrate: Views

Provides a migration path for the Views (for Drupal 7) module on Drupal 7 to the Core module - Views in Drupal 9. See the [project page](https://www.drupal.org/project/views_migration) for more information.

### Migration Tools

Adds classes and methods that help simplify a number of migration tasks including parsing source HTML, processing strings, extracting selected source content, debugging and troubleshooting, and more. See the [project page](https://www.drupal.org/project/migration_tools) for more information.

### WordPress Migrate

Can work with WordPress blog exports (WXR formats) and Drush to mass migrate from WordPress to Drupal 7 or Drupal 9 or later. See the [project page](https://www.drupal.org/project/wordpress_migrate) for more information.
