# Composer patches test

- clone drupal-composer/drupal-project
- include core patches from lightning project in composer.json
- add @danepowell PR fix  
- run composer clear-cache
- switch to git to 2.15.1 `brew switch git 2.15.1`
- run `composer install -vvv > git251-composer-patches#174.txt`