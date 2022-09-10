## Documentation on Wordpress database

Launcn 2 instances,create and attached volumes

`lsblk`

`gdisk /dev/xvd`

`sudo yum install lvm2`

`sudo pvcreate /dev/xvd`

`sudo mkdir -p /var/www/html`

`sudo mkdir -p /home/recovery/logs`

`sudo mount /dev/webdata-vg/apps-lv /var/www/html/`

`sudo rsync -av /home/recovery/logs/. /var/log`

`sudo vi /etc/fstab`

`sudo systemctl daemon-reload`

`sudo yum -y install wget httpd php php-mysqlnd php-fpm php-json`

`sudo mysql`

`sudo yum install mysql`

`sudo systemctl restart mysqld`

`sudo systemctl enable mysqld`