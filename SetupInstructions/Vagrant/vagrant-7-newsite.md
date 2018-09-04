# Setup for a Vagrant based installation (Step 7):

## Modify homestead.yaml for a new Laravel Website

1. Open the following file, replacing the [**_LaravelDirectory_**] with the directory you chose to create at [Step 5](vagrant-5.md);
  
```
[LaravelDirectory]\Homestead\Homestead.yaml
```

2. Set the "_sites:_" mapping to the name of your Project by adding the following lines to the end of the "_sites:_" section, replacing [**_ProjectName_**] with the name of your Project;

```
    - map: www.[ProjectName].local
      to: /home/vagrant/code/[ProjectName]/public
```

3. Note the use of lowercase for the drive numbers and forward slashes for paths.
4. Save the file and close your text editor.
5. Open the Command Prompt.
6. Navigate to the following directory, replacing the [**_LaravelDirectory_**] with the directory you chose to create at [Step 5](vagrant-5.md);
  
```
[LaravelDirectory]\Homestead
```
7. execute the following command;

```
vagrant reload
```

| Previous | Next |
| -------- | ---- |
| [< Vagrant Introduction](vagrant-intro.md) | [Step 8 - Configure the Hosts File >](vagrant-8.md) |