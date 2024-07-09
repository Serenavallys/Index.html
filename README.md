httpd.con
f
/storage/emulated/0/ksweb/conf/
<VirtualHost *:8080>
    ServerAdmin webmaster@localhost
    DocumentRoot "/storage/emulated/0/htdocs/mywebsite"
    ServerName mywebsite.local
    ErrorLog "/storage/emulated/0/htdocs/mywebsite/error.log"
    CustomLog "/storage/emulated/0/htdocs/mywebsite/access.log" combined

    <Directory "/storage/emulated/0/htdocs/mywebsite">
        Options Indexes FollowSymLinks
        AllowOverride All
        Require all granted
    </Directory>
</VirtualHost>
127.0.0.1 mywebsite.local
http://mywebsite.local:8080http://mywebsite.local:8080
