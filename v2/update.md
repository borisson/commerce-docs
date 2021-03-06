# Updating

> Note: Drupal Commerce 2 has now hit beta which supports upgrades. If you have an alpha installation, you will need to implement an upgrade path manually.

To update to the newest version of Drupal Commerce, you will need to update with Composer.

```sh
composer update drupal/commerce --with-dependencies
```

> Please note the `--with-dependencies` option. Without this option specified any needed, contributed projects and libraries will not update. Only the Drupal Commerce module will be updated.

Run your Drupal updates once all of the dependencies are updated. We recommend running them on the command line rather than the `update.php` script. See the example below.

```sh
drupal update:debug
drupal update:execute
```

For more information about using Composer with Drupal, see the (Managing Your Drupal Project with Composer)[https://glamanate.com/blog/managing-your-drupal-project-composer] blog post.
