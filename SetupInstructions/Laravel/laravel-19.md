# Laravel Instructions (Step 19):

## Create the Create Page Skeleton:

1. Create a copy of the following file, replacing [**_ControllerName_**] with the Controller Name you chose in [Step 10](laravel-10.md);

```
\resources\views\[ControllerName]\index.blade.php
```

2. Rename the file to "_create.blade.php_"
3. Open the following file, replacing [**_ControllerName_**] with the Controller Name you chose in [Step 10](laravel-10.md);

```
\resources\views\[ControllerName]\create.blade.php
```

4. Find the following line;

```HTML
<div class="card-header">View</div>
```

5. Change the above line to, replacing [**_Model Name_**] with the human readable name of the Model you created at [Step 2](laravel-2.md);

```HTML
<div class="card-header">Create [Model Name]</div>
```

6. Find and remove everything between the following lines, replacing [**_Model Name_**] with the human readable name of the Model you created at [Step 2](laravel-2.md);

```HTML
@if(count($[ModelName]))
...
@endif
```

7. Add the following within the "_card-body_" Div section below the "_@endif_", replacing the following;
    - [**_ControllerName_**] with the Controller Name you chose in [Step 10](laravel-10.md).
    - [**_columnname_**] with the lowercase Column Name.
    - [**_Column Name Label_**] with a human readable Column Name.

```HTML
{!! Form::open(['url' => '[ControllerName]/store']) !!}

    <div class="form-group">

        {{Form::label('[columnname]', '[Column Name Label]')}}
        {{Form::text('[columnname]','', ['class' => 'form-control', 'placeholder' => 'Enter [Column Name Label]'])}}

    </div>

    <div class="form-group">

        {{Form::label('[columnname]', '[Column Name Label]')}}
        {{Form::text('[columnname]','', ['class' => 'form-control', 'placeholder' => 'Enter [Column Name Label]'])}}

    </div>

    <div class="form-group">

        {{Form::label('[columnname]', '[Column Name Label]')}}
        {{Form::text('[columnname]','', ['class' => 'form-control', 'placeholder' => 'Enter [Column Name Label]'])}}

    </div>

    <div>

        {{Form::submit('Submit', ['class' => 'btn btn-primary'])}}

    </div>

{!! Form::close() !!}
```

| Previous | Next |
| -------- | ---- |
| [< Step 18 - Test the new Page](laravel-18.md) | [Step 20 - Add the Create Page Controller Logic >](laravel-20.md) |