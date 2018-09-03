# Laravel Instructions (Step 30):

## Add the Delete Functionality:

Open the following file, replacing [**_ControllerName_**] with the Controller Name you chose in [Step 10](laravel-10.md);

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

4. Insert code to add a Delete Button, replacing [**_ControllerName_**] with the Pascal Case Controller Name you chose in [Step 10](laravel-10.md), and replacing [**_modelname_**] with the lowercase Model Name you created at [Step 2](laravel-2.md);

```HTML
{!! Form::open(['action' => ['[ControllerName]Controller@destroy', $[modelname]->id], 'method' => 'POST']) !!}
    <div>
        {{Form::submit('Delete', ['class' => 'btn btn-danger'])}}
    </div>
    {{ Form::hidden('_method', 'DELETE') }}
{!! Form::close() !!}
```

5. Open the following file, replacing [**_ControllerName_**] with the Controller Name you chose in [Step 10](laravel-10.md);

```
\app\http\controllers\[ControllerName]Controller.php
```

6. Add the following to the "_destroy_" function, replacing the following;
    - [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md)
    - [**_modelname_**] with the lowercase Model Name you created at [Step 2](laravel-2.md)
    - [**_ModelName_**] with the Pascal Case Model Name you created at [Step 2](laravel-2.md)

```PHP
$[modelname] = Car::find($id);
        $car->delete();
        return redirect('/[controllername]')->with('result', 'Deleted');
```

7. Save the file.
8. Open your browser and navigate to the following address, replacing [**_ProjectName_**] with the Project Name you chose, and replacing [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md);

```
http://www.[ProjectName].local/[controllername]
```

9. Click the "_Delete_" button next to any item.
10. Verify that the correct page is shown and that the row has been deleted.

| Previous | Next |
| -------- | ---- |
| [< Step 29 - Add the Edit Functionality](laravel-29.md) | [Wrap Up >](laravel-wrapup.md) |