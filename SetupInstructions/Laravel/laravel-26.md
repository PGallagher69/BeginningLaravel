# Laravel Instructions (Step 26):

## Add a Success Message to the Layout:

1. Open the following file;

```
\resources\views\layouts\app.blade.php
```

2. Find the following line;

```HTML
_yield('content')
```

3. Add the following code to show the Success Messages, directly above the above line;

```HTML
@if(session('result'))
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-8 alert alert-success">
                {{session('result')}}
            </div>     
        </div>                   
    </div>                
@endif
```

4. Save the file.
5. Open your browser and navigate to the following address, replacing [**_ProjectName_**] with the Project Name you chose, and replacing [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md);

```
http://www.[ProjectName].local/[controllername]/create
```

6. Add some data to the fields.
7. Press the Submit Button.
8. Verify that the data and the message are shown.

| Previous | Next |
| -------- | ---- |
| [< Step 25 - Save the Form Data to the Database](laravel-25.md) | [Step 27 - Add some Menu Items >](laravel-27.md) |