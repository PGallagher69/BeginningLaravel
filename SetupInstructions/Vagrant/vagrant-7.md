# Setup for a Vagrant based installation (Step 7):

## Setup homestead.yaml

1. Open the Command Prompt.
2. Navigate to the following directory, replacing the [**_LaravelDirectory_**] with the directory you chose to create at [Step 5](vagrant-5.md);
  
```
[LaravelDirectory]\Homestead
```

3. Create the Homestead.yaml Configuration File using either;

### Windows:

```
init.bat
```

### Linux Bash:

```
bash init.sh
```

4. Open "_Homestead.yaml_" in a text editor.
5. Set &quot;_authorize:_&quot; to the path to your .ssh directory, replacing [**_YourUsername_**] with the folder name of your User Directory.
  
### Windows;

```
c:/Users/[YourUsername]/.ssh/id/_rsa.pub
```

### Linux Bash;

```
~/.ssh/id_rsa.pub
```

6. Set &quot;_keys:_&quot; to the path to your .ssh directory, replacing [**_YourUsername_**] with the folder name of your User Directory.
  
### Windows;

```
c:/Users/[YourUsername]/.ssh/id/_rsa.pub
```

### Linux Bash;

```
~/.ssh/id_rsa
```

7. Set the &quot;_folders:_&quot; \&gt; &quot;- map:&quot; directory to your code directory, replacing the [**_LaravelDirectory_**] with the directory you chose to create at [Step 5](vagrant-5.md). e.g.;

```
folders:
    - map: c:/[LaravelDirectory]/
      to: /home/vagrant/code/
```

8. Add the PhpMyAdmin folder to the Homestead.yaml file by adding the following two lines under the &quot;_folders_&quot; section, replacing the [**_LaravelDirectory_**] with the directory you chose to create at [Step 5](vagrant-5.md);

```
    - map: c:/[LaravelDirectory]/phpMyAdmin
      to: /home/vagrant/code/phpMyAdmin
```

9. Add the PhpMyAdmin site to the Homestead.yaml file by adding the following two lines under the &quot;sites&quot; section;

```
sites:
    - map: www.phpmyadmin.local
      to: /home/vagrant/code/phpMyAdmin
```

10. Set the "_sites:_" mapping to the name of your Project by adding the following lines to the end of the "_sites:" section, replacing [**_ProjectName_**] with the name of your Project;

```
    - map: www.[ProjectName].local
      to: /home/vagrant/code/[ProjectName]/public
```

11. Note the use of lowercase for the drive numbers and forward slashes for paths.
12. Add a database for your project by adding the following lines to the end of the "_databases:_" section, replacing [**_databasename_**] with the name of your project's database;

```
    - [databasename]
```

13. Save the file and close your text editor.

| Previous | Next |
| -------- | ---- |
| [< Step 6 - Install PHPMyAdmin](vagrant-6.md) | [Step 8 - Configure the Hosts File >](vagrant-8.md) |