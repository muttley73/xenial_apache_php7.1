ubuntu 7.10 apache + php7.1
dev enviroment setup.
php error reporting enabled on E_ERROR | E_WARNING | E_PARSE/

installed modules:

php7.1-mysql
libapache2-mod-php7.1
php7.1-curl
php7.1-cli
php7.1-json
php7.1-sqlite3
php7.1-intl
php7.1-dev
php7.1-gd
php7.1-mbstring
php7.1-mcrypt
php7.1-zip

volumes:

/var/www/html
/var/log/apache2
/etc/apache2/sites-enabled
/etc/apache2/
/etc/php/7.0/apache2/

apache-user: webmgr uid 1000
expose port: 80
start: apache2ctl (not supervisord)

