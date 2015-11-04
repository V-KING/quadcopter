# 多端口配置


### 1.保证httpd.conf下 


```
    LoadModule php5_module "D:/E/php/wamp/bin/php/php5.5.12/php5apache2_4.dll"
```
```
    ~~PHPIniDir D:/E/php/wamp/bin/php/php5.5.12~~
```

`很多网站上都用到PHPIniDir 配置，但是我不用这个的时候Apache才能起来
这两个没被注释掉`



### 2.打开多站点配置：


`httpd.conf`下面：`Include conf/extra/httpd-vhosts.conf` 去掉前面注释


### 3.httpd.conf下监听端口（这个好像原来老版本不是这样配置的。所以模仿第一个80的端口，可以写出8080的端口）





### 4.http-vhosts.conf配置（注意 Require all granted，不要写成什么allow from all什么的。可以参考httpd.conf中的写法。）




```
Listen 0.0.0.0:80
Listen [::0]:80

#listen to 8080
Listen 0.0.0.0:8080
Listen [::0]:8080

<VirtualHost *:80>
    ServerAdmin webmaster@dummy-host2.example.com
    DocumentRoot "D:/E/php/wamp/think"
    ServerName localhost
    ServerAlias localhost
    ErrorLog "logs/dummy-host2.example.com-error.log"
    CustomLog "logs/dummy-host2.example.com-access.log" common
    <Directory "D:/E/php/wamp/think">
    Options Indexes FollowSymLinks
    AllowOverride all
    Require all granted
    </Directory>
</VirtualHost>

<VirtualHost *:8080>
    ServerAdmin webmaster@dummy-host2.example.com
    DocumentRoot "D:/E/php/wamp/www"
    ServerName localhost
    ServerAlias localhost
    ErrorLog "logs/dummy-host2.example.com-error.log"
    CustomLog "logs/dummy-host2.example.com-access.log" common
    <Directory "D:/E/php/wamp/www">
    Options Indexes FollowSymLinks
    AllowOverride all
    Require all granted
    </Directory>
</VirtualHost>
```

注意修改正确的项目根目录

D:/E/php/wamp/www 和 D:/E/php/wamp/think