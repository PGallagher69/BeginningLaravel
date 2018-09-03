# Laravel Instructions (Step 24):

## Add code to display Form Errors to Main App Template:

1. Open the follwing file;

```
\resources\views\layouts\app.blade.php
```

2. Find the following line, around line 75;

```HTML
_yield('content')
```

3. Add the following code to show all of the errors, directly above the above line;

```HTML
@if(count($errors) > 0)

    <div class="container">

        @foreach($errors->all() as $error)

            <div class="row justify-content-center">
                <div class="col-8 alert alert-danger">
                    {{$error}}
                </div>
            </div>

        @endforeach

    </div>

@endif
```

4. Save the file.
5. Open your browser and navigate to the following address, replacing [**_ProjectName_**] with the Project Name you chose, and replacing [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md);

```
http://www.[ProjectName].local/[controllername]/create
```

6. Leave all of the fields empty.
7. Press the Submit Button.
8. Verify that the Errors are shown.

| Previous | Next |
| -------- | ---- |
| [< Step 23 - Add Controller Code to Validate the Form Data](laravel-23.md) | [Step 25 - Save the Form Data to the Database >](laravel-25.md) |