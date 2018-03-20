ubuntu xenial apache + php7.0
dev enviroment setup.
php error reporting enabled on E_ERROR | E_WARNING | E_PARSE/

installed modules:

php7.0-mysql
libapache2-mod-php7.0
php7.0-curl
php7.0-cli
php7.0-json
php7.0-sqlite3
php7.0-intl
php7.0-dev
php7.0-gd
php7.0-mbstring
php7.0-mcrypt
php7.0-zip

volumes:

/var/www/html
/var/log/apache2
/etc/apache2/sites-enabled
/etc/apache2/
/etc/php/7.0/apache2/

apache-user: webmgr uid 1000
expose port: 80
start: apache2ctl (not supervisord)
