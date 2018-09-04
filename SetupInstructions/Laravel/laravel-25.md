# Laravel Instructions (Step 25):

## Save the Form Data to the Database:

### Eloquent:

Eloquent is Laravel's ORM or Object Relational Mapping library.

Eloquent allows the programmer to quickly interact with the Database Model and data without having to write direct SQL queries.

Eloquent also simplifies the topic of security by handling security behind the scenes.

More information on Eloquent can be found here;

https://laravel.com/docs/5.6/eloquent

---

1. Open the following file, replacing [**_ControllerName_**] with the Controller Name you chose in [Step 10](laravel-10.md);

```
\app\http\controllers\[ControllerName]Controller.php
```

2. Find and Remove the following line from the "_submit_" function;

```PHP
return "Ok";
```

3. Add the following code at the bottom of the "_store_" function, replacing the following;
    - [**_modelname_**] - With the lowercase name of the Model you created at [Step 2](laravel-2.md).
    - [**_columnname_**] - With the lowecase name of your Column Name.
    - [**_controllername_**] - With the lowercase Controller Name you chose in [Step 10](laravel-10.md).

```PHP
$[modelname] = new [ModelName];
$[modelname]->[columnname] = $request->input('[columnname]');
$[modelname]->[columnname] = $request->input('[columnname]');
$[modelname]->[columnname] = $request->input('[columnname]');
$[modelname]->save();

return redirect('/[controllername]')->with('result', 'Saved');
```

4. Save the file.
5. Open your browser and navigate to the following address, replacing [**_ProjectName_**] with the Project Name you chose, and replacing [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md);

```
http://www.[ProjectName].local/[controllername]/create
```

6. Enter some data and press Submit.
7. Verify that you are redirected and that the data is present.

| Previous | Next |
| -------- | ---- |
| [< Step 24 - Add code to display Form Errors to Main App Template](laravel-24.md) | [Step 26 - Add a Success Message to the Layout >](laravel-26.md) |