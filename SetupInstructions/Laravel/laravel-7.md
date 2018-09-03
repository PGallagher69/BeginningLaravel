# Laravel Instructions (Step 7):

## Change "Home" to "Dashboard" - Controllers:

### Routes:

Routing is a method whereby the application looks up which Controller Method is executed for a particular web page address.

In the case of Laravel, routes are stored in the routes/web.php file.

All of our routes are going to be looking for "_home_", so we're going to change those to "_dashboard_" instead.

You can find more information on Routes here;

https://laravel.com/docs/5.6/routing

---

1. Open the following file;

```
\routes\web.php
```

2. Find the following line;

```PHP
Route::get('/home', 'HomeController@index')->name('home');
```

3. Change the line to;

```PHP
Route::get('/dashboard', 'DashboardController@index');
```

4. Save the File.

| Previous | Next |
| -------- | ---- |
| [< Step 6 - Change "Home" to "Dashboard" - Controllers >](laravel-6.md) | [Step 8 - Create the Controller >](laravel-7.md) |