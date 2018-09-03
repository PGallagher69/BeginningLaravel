# Laravel Instructions (Step 20):

## Add the Create Page Controller Logic:

1. Open VS Code
2. Open the following file, replacing [**_ControllerName_**] with the Controller Name you chose in [Step 10](laravel-10.md);

```
\app\http\controllers\[ControllerName]Controller.php" file.
```

3. Find the "_create_" function;

```PHP
public function create() {
```

4. Add the following line to the "_create_" function, replacing [**_ControllerName_**] with the Controller Name you chose in [Step 10](laravel-10.md);

```PHP
return view('[ControllerName]/create');
```

5. Save the file.
6. Open your browser and navigate to the following address, replacing [**_ProjectName_**] with the Project Name you chose, and replacing [**_controllername_**] with the lowercase Controller Name you chose in [Step 10](laravel-10.md);

```
http://www.[ProjectName].local/[controllername]/create
```

| Previous | Next |
| -------- | ---- |
| [< Step 19 - Create the Create Page Skeleton](laravel-19.md) | [Step 21 - Add the Submit Route and Test Controller Logic >](laravel-21.md) |