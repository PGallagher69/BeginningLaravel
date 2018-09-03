# Laravel Instructions (Step 18):

## Install Laravel Collective:

### Laravel Collective:

Laravel Collective is a collection of Components for Laravel which, amongst other things, gives us the ability to add Forms to our Laravel Application.

More information on Laravel Collective can be found here;

https://laravelcollective.com/

---

1. Open the Command Prompt.
2. Make sure you're in your Project Directory
3. Install Laravel Collective by entering the following command;

```
composer require "laravelcollective/html":"^5.4.0"
```

4. Open VS Code
5. Open the following file;

```
\config\app.php
```

6. Find the "_providers_" section on line 122 onwards.
7. Find the following line, around line 148;

```PHP
Illuminate\View\ViewServiceProvider::class
```

8. Add the following line after the line above;

```PHP
Collective\Html\HtmlServiceProvider::class,
```

9. Find the "_aliases_" section around line 176 onwards.
10. Find the following line;

```PHP
'View' => Illuminate\Support\Facades\View::class,
```

11. Add the following lines below the line above;

```PHP
'Form' => Collective\Html\FormFacade::class,
'Html' => Collective\Html\HtmlFacade::class,
```

12. Save the File

| Previous | Next |
| -------- | ---- |
| [< Step 17 - Test the new Page](laravel-17.md) | [Step 19 - Create the Add Page Skeleton >](laravel-19.md) |