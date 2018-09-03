# Laravel Instructions (Step 6):

## Change "Home" to "Dashboard" - Controllers:

### Controllers:

Controllers are a way of grouping together all of the Request Handling Logic for a particular Route into a single file. 

This is where you can determine which View is shown for a particular page.

When the User Authentication is scaffolded, it creates a set of routes, controllers and views named Home, which are actually the Dashboard. 

This is a little confusing... However, it affords us the opportunity to delve into how an existing logic to see how everything is hung together. We can do this by renaming the Home naming to Dashboard...

You can find out more about Laravel Controllers here;

https://laravel.com/docs/5.6/controllers

---

1. Open VS Code.
2. Find the following file;

```
\app\Http\Controllers\HomeController.php
```

3. Rename to the file to;

```
DashboardController.php
```

4. Open the following file;

```
\app\Http\Controllers\DashboardController.php
```

5. Find the Main "_HomeController_" Class line;

```PHP
class HomeController extends Controller
```

6. Change the line to;

```PHP
class DashboardController extends Controller
```

7. Find the "_index_" Function;

```PHP
public function index()
```

8. Find the "_return view_" line;

```PHP
return view("home");
```

9. Change the line to;

```PHP
return view("dashboard");
```

10. Save the "_DashboardController.php_" File

11. Open the following file;

```
\app\Http\Controllers\Auth\LoginController.php
```

12. Find the following line (around line 28);

```PHP
protected $redirectTo = '/home'
```

13. Change that line to;

```PHP
protected $redirectTo = '/dashboard'
```

14. Save the "_LoginController.php_" File.
15. Repeat items 11, 12, 13 and 14 for the following files, replacing occurrances of "_home_" with "_dashboard_";

```
\app\Http\Controllers\auth\RegisterController.php (Line 31)
\app\Http\Controllers\auth\ResetPasswordController.php (Line 28)
```

| Previous | Next |
| -------- | ---- |
| [< Step 5 - Register a New User](laravel-5.md) | [Step 7 - Change "Home" to "Dashboard" - Routes >](laravel-7.md) |