# Setup for a WAMP based installation (Step 11):

## Setup the Laravel Database Connection

1. In VS Code - Open the &quot;_.env_&quot; file in the root of the project.
2. Change &quot;APP\_NAME=Laravel&quot; to the following, replacing [**_ProjectName_**] with the name of your Project;

```
APP_NAME=[ProjectName]
```

3. Find &quot;_DB\_CONNECTION=mysql_&quot; line.
4. Change &quot;_DB\_DATABASE=homestead_&quot; to the following, replacing [**_ProjectName_**] with the name of your Project;

```
DB_DATABASE=[ProjectName]
```

5. Change &quot;_DB\_USERNAME=homestead&quot; to the following, replacing [**_DatabaseUserName_**] with your Database Username from [Step 8](wamp-8.md);

```
DB_USERNAME=[DatabaseUserName]
```

6. Change &quot;DB\_PASSWORD=secret&quot; to the following, replacing [**_DatabaseUserPassword_**] with your Database Password from [Step 8](wamp-8.md);

```
DB\_PASSWORD=[DatabasePassword]
```

7. Save the File.

| Previous | Next |
| -------- | ---- |
| [< Step 10 - Open the Project in VS Code ](wamp-10.md) | [Intro to Laravel >](/Laravel/README.md) |