# Laravel Instructions (Step 8):

## Change "Home" to "Dashboard" - Middleware:

### Middleware:

Middleware is a way of filtering HTTP requests, allowing the programmer to redirect traffic to certain locations based on some logic.

Laravel for instance, will use middleware to determine if a User is Authenticated, and if required, redirect that user to a login page.

You can find more information on Middleware here;

https://laravel.com/docs/5.6/middleware

---

1. Open the following file;

```
\app\Http\Controllers\middleware\RedirectIfAuthenticated.php
```

2. Find the "_handle_" function around line 18;

```PHP
public function handle($request, Closure $next, $guard = null)
```

3. Find the following line which redirects a logged in user to their dashboard, around line 21;

```PHP
return redirect('/home');
```

4. Change the above line to;

```PHP
return redirect('/dashboard');
```

5. Save the "_RedirectIfAuthenticated.php" file.

| Previous | Next |
| -------- | ---- |
| [< Step 7 - Change "Home" to "Dashboard" - Routes >](laravel-7.md) | [Step 9 - Change "Home" to "Dashboard" - Views >](laravel-9.md) |