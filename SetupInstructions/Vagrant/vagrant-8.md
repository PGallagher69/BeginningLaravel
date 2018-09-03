# Setup for a Vagrant based installation (Step 8):

## Configure the Hosts File

### Windows:

  1. Open your text editor as Administrator.
  2. Open the hosts file at "_c:\windows\sysytem32\drivers\etc_"

  3. Add your site to the bottom of the file, replacing [**_ProjectName_**] with the name of the Project you chose at [Step 7](vagrant-7.md), e.g.;

```
192.168.10.10   www.[ProjectName].local
192.168.10.10   www.phpmyadmin.local
```

  4. Save the file

### Linux/Mac:

  1. Open the hosts file at "_/etc/hosts_".

  2. Add your site to the bottom of the file, replacing [**_ProjectName_**] with the name of the Project you chose at [Step 7](vagrant-7.md), e.g.;

```
192.168.10.10   www.[ProjectName].local
192.168.10.10   www.phpmyadmin.local
```

  3. Save the file.

| Previous | Next |
| -------- | ---- |
| [< Step 7 - Setup homestead.yaml](vagrant-7.md) | [Step 9 - Launch the Vagrant Box >](vagrant-9.md) |