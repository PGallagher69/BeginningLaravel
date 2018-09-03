# Laravel Instructions (Step 29):

## Add the Edit Functionality:

1. Open the following file, replacing [**_ControllerName_**] with the Controller Name you chose in [Step 10](laravel-10.md);

```
\resources\views\[ControllerName]\index.blade.php
```

2. Find the following line;

```HTML
@foreach($[modelname]s as $[modelname])
```

3. Find the first spare TD;

```HTML
<td></td>
```

4. Insert code to add an Edit Link, replacing [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md), and replacing [**_modelname_**] with the lowercase Model Name you create at [Step 2](laravel-2.md);

```HTML
<td><a href="/[controllername]/{{$[modelname]->id}}/edit" class="btn btn-primary">Edit</a></td>
```

5. Open the following file, replacing [**_ControllerName_**] with the Controller Name you chose in [Step 10](laravel-10.md);

```
\app\http\controllers\[ControllerName]Controller.php
```

6. Add the following code to the "_edit_" function, replacing the following; 
    - [**_modelname_**] with the lowercase Model Name you created at [Step 2](laravel-2.md)
    - [**_ModelName_**] with the Pascal Case Model Name you created at [Step 2](laravel-2.md);
    - [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md);

```PHP
$[modelname] = [ModelName]::find($id);

return view('[controllername]/edit')->with('[modelname]', $[modelname]);
```

7. Add the following code to the "_update_" function, replacing the following;
    - [**_modelname_**] with the lowercase Model Name you created at [Step 2](laravel-2.md)
    - [**_ModelName_**] with the Pascal Case Model Name you created at [Step 2](laravel-2.md);
    - [**_columnname_**] with the lowercase Column Names;
    - [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md);

```PHP
$this->validate($request, [
    '[columnname]' => 'required',
    '[columnname]' => 'required',
    '[columnname]' => 'required',
    
]);

$[modelname] = [ModelName]::find($id);
$[modelname]->[columnname] = $request->input('[columnname]');
$[modelname]->[columnname] = $request->input('[columnname]');
$[modelname]->[columnname] = $request->input('[columnname]');
$[modelname]->save();
return redirect('/[controllername]')->with('result', 'Updated');
```

8. Save the File.
9. Open your browser and navigate to the following address, replacing [**_ProjectName_**] with the Project Name you chose, and replacing [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md);

```
http://www.[ProjectName].local/[controllername]
```

10. Click the "_Edit_" button next to any item.
11. Verify that the correct page is shown and that the data is there.
12. Change a field value.
13. Press the Submit Button.
14. Verify that you are redirected back to the View Page, and that the data is updated.

| Previous | Next |
| -------- | ---- |
| [< Step 28 - Add the Edit Page](laravel-28.md) | [Step 30 - Add the Delete Functionality: >](laravel-30.md) |