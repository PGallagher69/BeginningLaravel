# Laravel Instructions (Step 14):

## Create the HTML for the new View:

1. Open VS Code.
2. Open the following file, replacing [**_ControllerName_**] with the name of the Controller you created at [Step 10](laravel-10.md) ;

```
\resources\views\[ControllerName]\index.blade.php
```

3. Find the following line, around line 8;

```HTML
<div class="card-header">Dashboard</div>;
```

4. Change the above line to;

```HTML
<div class="card-header">View</div>;
```

5. Find and remove the following line, around line 17;

```HTML
You are logged in!
```

6. Add the following within the "_card-body_" Div, replacing;
    - [**_modelname_**]s with the lowercase plural name the model name you chose at [Step 12](laravel-12.md), e.g. cars.
    - [**_modelname_**] with the lowercase singular of the model name you chose at [Step 12](laravel-12.md), e.g. car.
    - [**_Column Name_**] with a User Readable Column Name from the model you created at [Step 12](laravel-12.md), e.g. Manufacturer
    - [**_columnname_**] with the lowercase Column Name from the model you created at [Step 12](laravel-12.md), e.g. manufacturer

```HTML
@if(count($[modelname]s))

    <table class="table table-striped">

        <tr>
            <th>[Column Name]</th>
            <th>[Column Name]</th>
            <th>[Column Name]</th>
            <th></th>
            <th></th>
        </tr>

        @foreach($[modelname]s as $[modelname])

            <tr>
                <td>{{$[modelname]->[columnname]}}</td>
                <td>{{$[modelname]->[columnname]}}</td>
                <td>{{$[modelname]->[columnname]}}</td>
                <td></td>
                <td></td>
            </tr>

        @endforeach

    </table>

@endif
```

7. Open your Browser
8. Navigate to the following address, replacing [**_ProjectName_**] with the name of the Project you chose, and replacing [**_ControllerName_**] with the name of the Controller you created at [Step 10](laravel-10.md);

```
http://www.[ProjectName].local/[ControllerName]/
```

9. Verify that your test data is shown.

| Previous | Next |
| -------- | ---- |
| [< Step 14 - Create the View for the new Controller >](laravel-14.md) | [Step 16 - Get Data From Database in the new Controller: >](laravel-16.md) |