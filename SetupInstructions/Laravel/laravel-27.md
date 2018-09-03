# Laravel Instructions (Step 27):

## Add some Menu Items:

1. Open the follwing file;

```
\resources\views\layouts\app.blade.php
```

2. Find the following lines around line 35;

```HTML
<!-- Left Side Of Navbar -->
<ul class="navbar-nav mr-auto">
```

3. Add the following code to the above Div to show two new Menu Items, replacing [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md);

```HTML
<li class="nav-item">
    <a class="nav-link" href="/[controllername]">View</a>
</li>
<li class="nav-item">
    <a class="nav-link" href="/[controllername]/create">Create</a>
</li>
```

4. Save the file.
5. Open your browser and navigate to the following address, replacing [**_ProjectName_**] with the Project Name you chose, and replacing [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md);

```
http://www.[ProjectName].local/[controllername]
```

6. Login if necessary.
7. Verify that the new Menu Items are shown.

| Previous | Next |
| -------- | ---- |
| [< Step 26 - Add a Success Message to the Layout](laravel-26.md) | [Step 28 - Add the Edit Page >](laravel-28.md) |