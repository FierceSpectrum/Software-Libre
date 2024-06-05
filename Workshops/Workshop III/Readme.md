Maquina Afritiona
```sh
vagrant shh


```

Maquina virtual
```sh
sudo apachectl -S


```
Maquina Afritiona
```sh
mkdir database
cd database
vagrant init debian/bookworm64
code Vagrantfile
vagrant up

```

Maquina web
```sh



```

Maquina database
```sh
sudo nano /etc/hosts
database*
sudo hostnamectl set-hostname database
exit

```

Maquina Afritiona
```sh
vagrant ssh


```

Maquina web
```sh
sudo hostnamectl set-hostname webserver
sudo nano /etc/hosts
webserver
exit


```

Maquina database
```sh



```

Maquina Afritiona
```sh
vagrant ssh


```

Maquina web
```sh



```

Maquina database
```sh
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install mariadb-
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install mariadb-server mariadb-client
mysql --version

sudo mysql

"IN SQL"

show databases;
desc mysql.user;
Select Host, User, Password from mysql.user;
Create user laravel;

Create user laravel2@'localhost';
Drop user laravel2@'localhost';
Drop user laravel;

Create user laravel identified by 'secret';
Set password for laravel = password('secret2');
Set password for laravel = password('secret');

Create database lfts;

Grant all privileges on lfts.* to laravel;
show grants for laravel;

Flush privileges;

exit

"End SQL"

mysql -u laravel -p
secret

Show databases;




```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh
sudo apt-get install mariadb-client
mysql --version
mysql -h 192.168.56.11 -u laravel -p
secret


```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh
exit
sudo nano /etc/mysql/mariadb.conf.d/50-server.cnf
    Command: Control-W
        bind
        #bind--adress             =127.0.0.1
    Command: Control-O
    Command: Control-X

sudo systemctl restart mysql


```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh
mysql -h 192.168.56.11 -u laravel -p
secret

"IN SQL"
exit
"END SQL"


sudo apt-get install php8.2 php8.2-mysql php8.2-mcrypt php8.2-memcache php8.2-bcmath php8.2-zip php8.2-curl php8.2-xml

php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('sha384', 'composer-setup.php') === 'dac665fdc30fdd8ec78b38b9800061b4150413ff2e3b6f88543c636f7cd84f6db9189d43a81e5503cda447da73c7e5b6') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"

sudo mkdir -p /opt/composer
sudo mv composer.phar /opt/composer/
sudo ln -s /opt/composer/composer.phar /usr/local/bin

env $PATH

ls -la /usr/local/bin/c*
sudo ln -s /opt/composer/composer.phar /usr/local/bin/composer
sudo rm /user/local/bin/composer.phar

sudo apt-get install curl
curl ifconfig.me

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
exit


```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh
vagrant ssh


```

Maquina web
```sh
nvm ls-remote
nvm install --lts
node -v
npm -v

cd
cd /vagrant/sites

composer create-poject laravel/laravel=8.6.12 lfts.isw811.xyz

ls



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh
Creamos una nueva carpeta para la pagina el config y lo modificamos 

"
<VirtualHost *:80>
ServerAdmin webmaster@lfts.isw811.xyz
ServerName lfts.isw811.xyz

# Indexes + Directory Root.
DirectoryIndex index.php index.html
DocumentRoot /home/vagrant/sites/lfts.isw811.xyz/public

<Directory /home/vagrant/sites/lfts.isw811.xyz/public>
    DirectoryIndex index.php index.html
    AllowOverride All
    Require all granted
</Directory>

ErrorLog ${APACHE_LOG_DIR}/lfts.isw811.xyz.error.log
LogLevel warn
CustomLog ${APACHE_LOG_DIR}/lfts.isw811.xyz.access.log combined
</VirtualHos

"


```

Maquina web
```sh
ls -la
sudo cp lfts.isw811.xyz.conf /etc/apache2/sites-avaliable/
sudo apache2ctl -t
sudo a2ensite lfts.isw811.xyz.conf
sudo apache2ctl -t
sudo systemctl reload apache2

cd
cd /vagrant/sites




```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh

ver telegram para configurar el .env de laravel

```

Maquina web
```sh

cd /vagrant/sites/lfts-isw811.xyz
php artisan migrate


```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```


Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```

Maquina Afritiona en Webserver
```sh



```

Maquina web
```sh



```

Maquina Afritiona en Database
```sh



```

Maquina database
```sh



```
