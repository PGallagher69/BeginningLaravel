# Laravel Instructions (Step 28):

## Add the Edit Page:

1. Make a copy of the following file, replacing [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md);

```
\resources\views\[controllername]\create.blade.php
```

2. Name the file "_edit.blade.php_".
3. Open the following file, replacing [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md);

```
\resources\views\[controllername]\edit.blade.php
```

4. Find the following line;

```HTML
{!! Form::open(['url' => '[controllername]/store']) !!}
```

5. Change the above line to the following, replacing [**_ControllerName_**] with the Pascal Case Controller Name you chose in [Step 10](laravel-10.md), and replacing [**_modelname_**] with the lowercase Model Name you created at [Step 2](laravel-2.md);

```HTML
{!! Form::open(['action' => ['[ControllerName]Controller@update', $[modelname]->id], 'method' => 'POST']) !!} 
```

6. Find each Text Entry Box line like the following, replacing [**_columnname_**] with the lowercase Column Name, and replacing [**_Column Name Label_**] with a Human Readable Column Name;

```HTML
{{Form::text('[columnname]','', ['class' => 'form-control', 'placeholder' => '[Column Name Label]'])}}
```

7. Add a default value to the Text Input boxes by changing the Text Entry Boxes to the following, replacing the following;
    - [**_columnname_**] with the lowercase Column Name.
    - [**_modelname_**] with the lowercase Model Name you created at [Step 2](laravel-2.md).
    - [**_Column Name Label_**] with a human readable Column Name.;

{{Form::text('[columnname]',$[modelname]->[columnname], ['class' => 'form-control', 'placeholder' => '[Column Name Label]'])}}

8. Find the following line;

```HTML
{!! Form::close() !!}
```

9. Add the following line directly above the above line;

```HTML
{{ Form::hidden('_method', 'PUT') }}
```

10. Save the File.

| Previous | Next |
| -------- | ---- |
| [< Step 27 - Add some Menu Items](laravel-27.md) | [Step 29 - Add the Edit Functionality >](laravel-29.md) |