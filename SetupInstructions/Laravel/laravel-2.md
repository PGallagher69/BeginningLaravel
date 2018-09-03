# Laravel Instructions (Step 2):

## Create Users Table in Database:

### Artisan

Artisan is a command line tool packaged with Laravel which allows for the execution of a host of different bits of logic which build parts of the web application automatically. This includes scaffolding parts of code, executing Database Migrations and a host of other useful bits of logic.

More information on Artisan can be found here:

https://laravel.com/docs/5.6/artisan

---

1. Open Cmder
2. If using Vagrant
  1. Navigate to the following directory,replacing the [**_LaravelDirectory_**] with the directory you chose;
  
  ```
  [LaravelDirectory]**\Homestead
  ```

  2. Open an SSH session by using the following command;

```
vagrant ssh
```

3. Navigate to your project directory.
4. Enter the following command;

```
php artisan migrate
```

5. Confirm that migrations completed successfully

| Previous | Next |
| -------- | ---- |
| [< Step 1 - Fix Laravel Text String Length Bug](laravel-1.md) | [Step 3 - Check that Users Table has been created >](laravel-3.md) |