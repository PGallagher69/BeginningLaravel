# Laravel Instructions (Step 22):

## Add Controller Code to test return Submitted Form Data:

1. Open the following file, replacing [**_ControllerName_**] with the Controller Name you chose in [Step 10](laravel-10.md);

```
\app\http\controllers\[ControllerName]Controller.php
```

2. Remove the following line from the "_store" function;

```PHP
return "Hello!";
```

3. Add the following line to check that the Form data is being submitted, replacing [**_columnname_**] with the lowercase name of one of your columns;

```PHP
return $request->input('[columnname]');
```

4. Save the file.
5. Open your browser and navigate to the following address, replacing [**_ProjectName_**] with the Project Name you chose, and replacing [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md);

```
http://www.[ProjectName].local/[controllername]/create
```

6. Enter some data into the fields.
7. Press the Submit Button.
8. Verify that the data is returned.

| Previous | Next |
| -------- | ---- |
| [< Step 21 - Add the Submit Route and Test Controller Logic](laravel-21.md) | [Step 23 - Add Controller Code to Validate the Form Data >](laravel-23.md) |