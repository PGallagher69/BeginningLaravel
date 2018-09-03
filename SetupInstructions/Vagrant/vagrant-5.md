# Setup for a Vagrant based installation (Step 5):

## Install Laravel Homestead

  1. Docs: [https://laravel.com/docs/5.6/homestead](https://laravel.com/docs/5.6/homestead)
  2. Open Command Prompt.
  3. Run the following command;

```
vagrant box add laravel/homestead
```

  4. Make a directory somewhere on your hard drive, e.g. "c:\\[**_LaravelDirectory_**]", replacing [**_LaravelDirectory_**] with a directory name of your choice.
  5. In the Command Prompt, navigate to the new directory.
  6. Clone the Laravel/Homestead git repository using the following command;

```
git clone https://github.com/laravel/homestead.git Homestead
```

  7. In the Command Prompt, create your SSH Keys using the following command, replacing the [**_EmailAddress_**] with your own email address. **Note the use of a Capital &quot;C&quot; for -C switch**

```
ssh-keygen -t rsa -b 4096 -C "[EmailAddress]"
```

  9. For &quot;_Enter passphrase&quot;, just press the Enter Key to leave this blank.
  10. In the Command Prompt, navigate to the new Homestead directory.
  11. Get the latest version of Laravel/Homestead using the following command;

```
git checkout v7.15.1
```

| Previous | Next |
| -------- | ---- |
| [< Step 4 - Install Git](vagrant-4.md) | [Step 6 - Install PHPMyAdmin >](vagrant-6.md) |