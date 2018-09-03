# Laravel Instructions (Step 23):

## Add Controller Code to Validate the Form Data:

1. Open the following file, replacing [**_ControllerName_**] with the Controller Name you chose in [Step 10](laravel-10.md);

```
\app\http\controllers\[ControllerName]Controller.php
```

2. Remove the following line from above from the "_store_" function;

```PHP
return $request->input('[columnname]');
```

3. Add the following code to the "_store_" function to validate your form fields, and make them required, replacing [**_columnname_**] with the lowercase name of your columns;

```PHP
$this->validate($request, [
    '[columnname]' => 'required',
    '[columnname]' => 'required',
    '[columnname]' => 'required',
]);

return "Ok";
```

4. Save the File.

| Previous | Next |
| -------- | ---- |
| [< Step 22 - Add Controller Code to test return Submitted Form Data](laravel-22.md) | [Step 24 - Add code to display Form Errors to Main App Template >](laravel-24.md) |