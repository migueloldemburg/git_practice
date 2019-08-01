> php artisan make:migration create_users_table --create=users

To create a migration, use the make:migration command. The --table and --create options may also be used to indicate the name of the table and whether the migration will be creating a new table

> php artisan migrate:reset

The migrate:reset command will roll back all of your application's migrations:

> php artisan migrate:refresh

The migrate:refresh command will roll back all of your migrations and then execute the  migrate command. This command effectively re-creates your entire database.

> php artisan tinker

> php artisan make:model Task

> php artisan make:model Task php -m

> composer dump-autoload

> php artisan make:controller TasksController

> php artisan make:controller TasksController -r

This command, in addition to creating the TaskController file, it includes the resource functions.cd 

> php artisan make:model Post -mc

This command creates a model Post, and migration and controller files.