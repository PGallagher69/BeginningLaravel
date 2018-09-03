# Laravel Instructions (Step 9):

## Change "Home" to "Dashboard" - Views:

### Views:

Views contain the HTML which is rendered by the user's browser and are typically stored in the "_\resources\views_" directory.

You can find more information on Views here;

https://laravel.com/docs/5.6/views

Views use Laravel's "_Blade Templates_", and can contain logic which affects how the output is rendered, including basic Logic, Sections and the insertion of data from the Controller.

You can find more information on the "_Blade Templates_" here;

https://laravel.com/docs/5.6/blade

---

1. Find the following file;

```
\resources\views\Home.blade.php
```

2. Rename the file to;

```
dashboard.blade.php
```

---

We can now test out all of our changes to make sure they all work...

---

3. Open a Browser.
4. Navigate to the following address assuming you're logged in, replacing [**_ProjectName_**] with the name of the Project you chose;

```
http://www.[ProjectName].local/dashboard
```

5. If the page loads then click "_Logout_" Link.
6. Click the Register Link.
7. Register a New User.
8. Check that you are redirected to the Dashboard page.

| Previous | Next |
| -------- | ---- |
| [< Step 8 - Change "Home" to "Dashboard" - Middleware >](laravel-8.md) | [Step 10 - Create a New Controller >](laravel-10.md) |