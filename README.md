Source:
https://github.com/munafio/chatify

1.laravel new laravel_7_with_chatify

2.
composer reqire munafio/chatify

3.
fill the needed Pusher API credentials in .env
PUSHER_APP_ID=
PUSHER_APP_KEY=
PUSHER_APP_SECRET=
PUSHER_APP_CLUSTER=eu

4.
must
php artisan vendor:publish --tag=chatify-config
php artisan vendor:publish --tag=chatify-assets
php artisan vendor:publish --tag=chatify-migrations

optional
php artisan vendor:publish --tag=chatify-controllers
php artisan vendor:publish --tag=chatify-view

NOTE: Publishing assets means (e.g. config) that creating a copy of the package's config file into the config folder of your Laravel applications and like so with the other assets (Package's Views, controllers, migrations ...).

5.
php artisan migrate

Migrating: 2014_10_12_000000_create_users_table
Migrated: 2014_10_12_000000_create_users_table (0.07 seconds)
Migrating: 2014_10_12_100000_create_password_resets_table
Migrated: 2014_10_12_100000_create_password_resets_table (0.08 seconds)
Migrating: 2019_08_19_000000_create_failed_jobs_table
Migrated: 2019_08_19_000000_create_failed_jobs_table (0.06 seconds)
Migrating: 2019_09_22_192348_create_messages_table
Migrated: 2019_09_22_192348_create_messages_table (0.12 seconds)
Migrating: 2019_10_16_211433_create_favorites_table
Migrated: 2019_10_16_211433_create_favorites_table (0.11 seconds)
Migrating: 2019_10_18_223259_add_avatar_to_users
Migrated: 2019_10_18_223259_add_avatar_to_users (0.07 seconds)
Migrating: 2019_10_20_211056_add_messenger_color_to_users
Migrated: 2019_10_20_211056_add_messenger_color_to_users (0.07 seconds)
Migrating: 2019_10_22_000539_add_dark_mode_to_users
Migrated: 2019_10_22_000539_add_dark_mode_to_users (0.06 seconds)
Migrating: 2019_10_25_214038_add_active_status_to_users
Migrated: 2019_10_25_214038_add_active_status_to_users (0.08 seconds)

6.
php artisan storage:link

The [/home/bazs/code/chatify_clone_laravel_7_25_0/public/storage] link has been connected to [/home/bazs/code/chatify_clone_laravel_7_25_0/storage/app/public].
The links have been created.

7.

After installing the package, you can access the messeneger by the default path(route path) which is /chatify

8.
composer require laravel/ui

php artisan ui vue --auth

php artisan serve

login

go:
/chatify

done.

Some other stuff:

The reason you’d want to do this with the href of a link is that normally, a javascript: URL will redirect the browser to a plain text version of the result of evaluating that JavaScript. But if the result is undefined, then the browser stays on the same page. void(0) is just a short and simple script that evaluates to undefined.
