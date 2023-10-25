Configuración
Instalación de apache
sudo apt update 
sudo apt install apache2
sudo ufw app list
Output
Available applications:
  Apache
  Apache Full
  Apache Secure
  OpenSSH

sudo systemctl status apache2

instalación de composer 
sudo apt update
sudo apt install php-cli unzip
cd ~
curl -sS https://getcomposer.org/installer -o composer-setup.php
HASH=`curl -sS https://composer.github.io/installer.sig`
echo $HASH
php -r "if (hash_file('SHA384', 'composer-setup.php') === '$HASH') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
out put 
Installer verified

configurar repositorio 
permisos 
sudo chmod -R 775 /var/www
sudo chown -R www-data:www-data
Cd /var/www/
Git clone repositorios credenciales para autenticar entregadas por bibliotech
Cd bibliotech
Permisos 
sudo find . -type d -exec chmod 755 {} \;
 sudo find . -type f -exec chmod 644 {} \;
Composer install 
Yarn install 
Yarn run build 



instalación de mysql
sudo apt update
sudo apt install mysql-ser
sudo mysql
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';
GRANT ALL PRIVILEGES ON db.* TO '$user'@'localhost' WITH GRANT OPTION;
FLUSH PRIVILEGES;
Exit
Creación de virtual Host
cd /etc/apache2/sites-available
sudo vim bibliotech.conf
<VirtualHost *:80>
    ServerName bibliotechonline.com
    DocumentRoot /var/www/bibliotech/public

    <Directory /var/www/bibliotech/public>
        AllowOverride All
        Require all granted

        FallbackResource /index.php
    </Directory>

    ErrorLog ${APACHE_LOG_DIR}/error.log
    CustomLog ${APACHE_LOG_DIR}/access.log combined
</VirtualHost>

sudo a2ensite bibliotic.conf

sudo systemctl reload apache2

instalación de php 8.1
sudo apt update
sudo apt upgrade
sudo add-apt-repository ppa:ondrej/php
sudo apt install php8.1
instalación de estaciones de php 
sudo apt-get php8.1-intl
sudo apt-get php8.1-xml
sudo apt-get php8.1-*
sudo systemctl restart apache2

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash
source ~/.bashrc
nvm –version
nvm install “version”

Nota: Para el despliegue se han instalado diferente versión la 14.21.3,
16.17.1 versión de desarrollo de bibliotech
16.20.2
18.17.1
19.9.0
20.5.1
Cada version contiene su version indicada de npm
Npm yarn install -g  

Configuración .env
DATABASE_URL="mysql://devbibliotech_desarrollo:JjxviLGO3Zc]@127.0.0.1:3306/devbibliotech_bibliotech"
Agregar base de datos creada previamente con el usuario y contraseña 
Pruebas con 
APP_ENV=dev
APP_DEBUG=1
Cambiar a  
APP_ENV=prod
APP_DEBUG=0

