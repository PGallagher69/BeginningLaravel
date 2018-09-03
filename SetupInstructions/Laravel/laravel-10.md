# Laravel Instructions (Step 10):

## Create a new Controller:

1. Open Command Prompt.
2. Make sure you're in your Project Directory.
3. Run the following command, replacing  [**_ControllerName_**] with the name of your new controller, e.g. CarController;

```
php artisan make:controller [ControllerName]Controller --resource
```

4. The "_--resource_" switch instructs Artisan to create us a controller with CRUD logic already scaffolded.
5. Return to VS Code.
6. Check that the following file exists, replacing  [**_ControllerName_**] with the name of your new controller, e.g. CarController.php;  

```
\app\Http\Controllers\[ControllerName]Controller.php
```

7. Open the new Controller.
8. You should see that, as we used the "_--resource_" switch, Artisan has scaffolded a set of functions for us;
    - index,
    - create,
    - store,
    - show,
    - edit,
    - update,
    - destroy

| Previous | Next |
| -------- | ---- |
| [< Step 9 - Change "Home" to "Dashboard" - Views >](laravel-9.md) | [Step 11 - Create Routes for Controller >](laravel-11.md) |