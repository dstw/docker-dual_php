# docker-dual_php
Example Apps consist of Apache Web Server with modphp &amp; modfpm on Docker

There are two Apache Web Server running php using modphp &amp; modfpm. Add your files into directory apache_fpm/htdocs and apache_php/htdocs. Run with:

```
docker up -d
```

Add this on hosts file:

```
${your-ip}      apache-modfpm.local
${your-ip}      apache-modphp.local
```

Change ${your-ip} respectively with your docker host IP.
You can access the web via:

http://apache-modfpm.local  
http://apache-modphp.local

The default page show phpinfo() page for each library used.

Inspired from [there]

[there]:http://www.inanzzz.com/index.php/post/su76/creating-apache-mysql-and-php-fpm-containers-for-a-web-application-with-docker-compose
