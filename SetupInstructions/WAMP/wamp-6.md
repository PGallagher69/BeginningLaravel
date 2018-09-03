# Setup for a WAMP based installation (Step 6):

## Add WAMP Virtual Server:

1. Start WAMP Server.
2. Wait for green icon.
3. Left Click WAMP Tray icon.
4. Go to &quot;Your Virtual Hosts&quot; > &quot;Virtual Host Management&quot;.
5. In the &quot;Name of the Virtual Host&quot; box enter: &quot;www. **ProjectName**.local
6. In the &quot;Complete absolute box&quot; enter the following, replacing [**_WAMP Directory_**]_ with the location of your WAMP Installation Directory, and replacing [**_ProjectName_**] with the Name of your Project;

```
[WAMP Directory]\www\[ProjectName]\public
```

7. Leave the &quot;_If you want to use virtual host by IP_&quot; blank.
8. Press the &quot;_Start the creation of the VirtualHost_&quot; button.
9. Once complete, right click on WAMP Tray Icon.
10. Go to &quot;Tools&quot; > &quot;Restart DNS&quot;.

| Previous | Next |
| -------- | ---- |
| [< Step 5 - Create Project ](wamp-5.md) | [Step 7 - Check Website is Running >](wamp-7.md) |