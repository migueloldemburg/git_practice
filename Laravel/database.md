#Database and Migrations

> php artisan make:migration create_table_tasks --create=tasks

Creates a new migration file where we can add fields through a Schema Class. We name the migration with explicit names such as *create_table_tasks*

> php artisan migrate

Now our recently made new table will added to our DB

> php artisan migrate:refresh

In case we did changes to our migration file, we can run this command to roll back changes