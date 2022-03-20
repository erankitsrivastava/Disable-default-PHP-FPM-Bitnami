# Disable-default-PHP-FPM-Bitnami

`test ! -f "/opt/bitnami/common/bin/openssl" && echo "Approach A: Using system packages." || echo "Approach B: Self-contained installation."`

`sudo mv /etc/monit/conf.d/php-fpm.conf /etc/monit/conf.d/php-fpm.conf.disabled`

`sudo gonit reload`

`sudo /opt/bitnami/ctlscript.sh restart apache`

`sudo /opt/bitnami/ctlscript.sh stop php-fpm`


Refrence URL: https://docs.bitnami.com/aws/apps/wordpress/administration/disable-phpfpm/
