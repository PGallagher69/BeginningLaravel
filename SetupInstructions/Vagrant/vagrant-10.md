# Setup for a Vagrant based installation (Step 10):

## Create the Laravel Project:

  1. SSH Into the Vagrant Box by using the following command;

```
vagrant ssh
```

  2. Navigate to your code directory using the following command;

```
cd code
```

  3. Create your Laravel project by using the following command, replacing [**_ProjectName_**] with the name of the Project you chose at [Step 7](vagrant-7.md);

```
laravel new [ProjectName]
```

  4. Test that the website is running by navigating to, replacing [**_ProjectName_**] with the name of the Project you chose at [Step 7](vagrant-7.md);

```
http://www.[ProjectName].local
```

| Previous | Next |
| -------- | ---- |
| [< Step 9 - Launch the Vagrant Box](vagrant-9.md) | [Step 11 -	Open Project in VS Code >](vagrant-11.md) |