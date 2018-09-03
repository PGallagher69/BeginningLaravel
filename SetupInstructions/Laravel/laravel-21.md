# Laravel Instructions (Step 21):

## Add the Submit Route and Test Controller Logic:

1. Open VS Code.
2. Open the following file;

```
\routes\web.php
```

3. Add the following route to the bottom of the file, to allow the Create page to receive the form Submit request, replacing [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md);

```PHP
Route::post('/[controllername]/store', '[ControllerName]Controller@store');
```

4. Save the file.
5. Open the following file, replacing [**_ControllerName_**] with the Controller Name you chose in [Step 10](laravel-10.md);

```
\app\http\controllers\[ControllerName]Controller.php
```

6. To test that our route is working, add the following line to the "_store_" function;

```PHP
return "Hello!";
```

7. Save the File.
8. Open your browser and navigate to the following address, replacing [**_ProjectName_**] with the Project Name you chose, and replacing [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md);

```
http://www.[ProjectName].local/[controllername]/create
```

9. Press the Submit Button and verify that the browser shows "_Hello!_".

| Previous | Next |
| -------- | ---- |
| [< Step 20 - Add the Create Page Controller Logic](laravel-20.md) | [Step 22 - Add Controller Code to test return Submitted Form Data >](laravel-22.md) |