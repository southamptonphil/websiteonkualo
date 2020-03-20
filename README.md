# Website on Kualo

## Install Open Social

`composer create-project goalgorilla/social_template:dev-master public_html/phil --no-interaction`

## Update

`php -d set_time_limit=3600 -d memory_limit=4096M /usr/local/bin/composer update --with-dependencies --profile`

## Development Environment

The composer update command above is really memory hungry and fails in the 512M available on the account.

Need to try having a local copy which can be updated and then just push the composer.lock file to the server and run composer install - which looks at the .lock file and makes it so.

As per https://benohead.com/blog/2014/12/07/php-composer-install-or-update-causes-a-php-fatal-error/
