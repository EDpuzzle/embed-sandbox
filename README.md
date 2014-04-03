### Sandbox to test the Embed code

##### Instructions to set up the development environment

Open the hosts file in your Mac or Unix computer:

```
sudo subl /etc/hosts
```

Create alias for localhost:

```
127.0.0.1 embed.dev
```

Open Apache configuration file:

```
sudo /etc/apache2/httpd.conf
```

Add the corresponding virtual hosts lines to the Apache configuration file:

```
NameVirtualHost *:80
<VirtualHost *:80>
	ServerName embed.dev
	DocumentRoot “/Users/path-to-your-projects/embed-sandbox”
</VirtualHost>
```

Restart the Apache server
```
sudo apachectl restart
```
