# Laravel Instructions (Step 11):

## Add the Routes for the new Controller:

1. Open VS Code.
2. Open the following file;

```
\routes\web.php
```

3. Find the following line;

```PHP
Auth::routes()
```

4. Below the above line add the following line, replacing [**_controllername_**] with the lower case Controller Name you chose in [Step 10](laravel-10.md), and replace [**_ControllerName_**] which the Pascal Case (first letters of each word capitalised) Controller Name you chose in [Step 10](laravel-10.md);

```PHP
Route::resource('/[controllername]', '[ControllerName]Controller');
```

5. Return to your Command Prompt.
6. Enter the following command;

```
php artisan route:list
```

7. You should be shown a list of all of the available routes in your Project. Verify that your new Controller Routes are shown in the list.


| Previous | Next |
| -------- | ---- |
| [< Step 10 - Create a new Controller >](laravel-10.md) | [Step 12 - Create a Database Model: >](laravel-12.md) |