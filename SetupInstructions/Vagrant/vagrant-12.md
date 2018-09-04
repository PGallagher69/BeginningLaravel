# Setup for a Vagrant based installation (Step 12):

## Modify the Laravel .env file:

1. Open VS Code
2. Open the following file in the root of your project;

```
\.env
```

2. Find the following line, around line 1;

```
APP_NAME=Laravel
```

3. Change above line to the following, replacing [**_ProjectName_**] with the name of your Project;

```
APP_NAME=[ProjectName]
```

4. Find the following line, around line 5;

```
APP_URL=http://localhost
```

5. Change above line to the following, replacing [**_ProjectName_**] with the name of your Project;

```
APP_URL=http://www.[ProjectName].local
```

6. Find the following line, around line 12;

```
DB_DATABASE=homestead
```

7. Change the above line to the following, replacing [**_databasename_**] with the name of your Database;

```
DB_DATABASE=[databasename]
```

8. Save the File.

| Previous | Next |
| -------- | ---- |
| [< Step 11 - Open the Project in VS Code](vagrant-11.md) | [Intro to Laravel >](/SetupInstructions/Laravel/README.md) |