# Composer patches test

- clone drupal-composer/drupal-project
- include core patches from lightning project in composer.json
- switch to cweagans/composer-patches:1.6.2
- add `"preferred-install": "source"` in composer.json
- nuke previous composer install artifacts (docroot, composer.lock, vendors)
- run composer clear-cache
- switch to git to 2.13.4 `brew switch git 2.13.4`
- lock core to 8.4.2
- run `composer install -vvv > git234-composer-patches162.txt`