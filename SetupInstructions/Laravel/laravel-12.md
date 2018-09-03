# Laravel Instructions (Step 12):

## Create a Database Model:

### Migrations:

Migrations are Laravel's way of allowing you to keep track of changes to your database design.

Migration files contain code which allow for the database design to be modified. As this is done in code, then all of the database design can be kept under source control.

More information about Migrations can be found here;

https://laravel.com/docs/5.6/migrations

---

1. Return to your Command Prompt.
2. Enter the following command, replacing [**_ModelName_**] with the name of your Model, e.g. Car;

```
php artisan make:model [ModelName] -m
```

3. The "-m" switch instructs Artisan to create a Migration for our model.
4. Open VS Code.
5. Check to see if your new Migration File has been created in the following folder;

```
\database\migrations\
```

6. Open your Migration File, e.g. "_2018_09_01_071635_create_cars_table.php_".
7. Find the "_up" function, around line 14.
8.  
9. Add various Model Properties within the "_Schema::create", for example;

```PHP
$table->string('manufacturer');
$table->string('model');
$table->string('colour');
```

10. Return to your Command Prompt.
11. Run the Migration by executing the following command;

```
php artisan migrate
```

| Previous | Next |
| -------- | ---- |
| [< Step 11 - Add the Routes for the new Controller >](laravel-11.md) | [Step 13 - Create some Test Data: >](laravel-13.md) |