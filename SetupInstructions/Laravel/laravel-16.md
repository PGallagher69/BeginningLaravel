# Laravel Instructions (Step 16):

## Get Data From Database in the new Controller:

1. Open VS Code
2. Open the following file, replacing [**_ControllerName_**] with the name of the Controller you created at [Step 10](laravel-10.md);

```
\app\Http\Controllers\[ControllerName]Controller.php
```

3. Find the following line;

```PHP
use Illuminate\Http\Request
```

4. Unde the line above, add a Reference to the Model, replacing [**_ModelName_**] with the Pascal Case Name of the Model you created at [Step 2](laravel-2.md);

```PHP
use App\[ModelName];
```

5. Find the "_index_" function;

```PHP
public function index()
```

6. Add the following code to store all of the Model data in a variable by adding the following line to the "_index_" function, replacing [**_modelname_**] with the lowercase name of the Model you created at [Step 2](laravel-2.md), and replacing [**_ModelName_**] with the Pascal Case name of the Model you created at [Step 2](laravel-2.md);

```PHP
$[modelname] = [ModelName]::all();
```

7. Return the Model data with the View from the Controller by adding the following line to the index function, after the above line, replacing [**_ControllerName_**] with the name of the Controller you created at [Step 10](laravel-10.md), and replacing [**_modelname_**] with the lowercase name of the Model you created at [Step 2](laravel-2.md);

```PHP
return view('[ControllerName]/index')->with('[modelname]', $[modelname]);
```

| Previous | Next |
| -------- | ---- |
| [< Step 15 - Create the HTML for the new View](laravel-15.md) | [Step 17 - Test the new Page >](laravel-17.md) |