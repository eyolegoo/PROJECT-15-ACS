#!/bin/bash
yum install -y nginx
systemctl start nginx
systemctl enable nginx
https://github.com/eyolegoo/PROJECT-15-ACS.git
mv /PROJECT-15-ACS/reverse.conf /etc/nginx/
mv /etc/nginx/nginx.conf /etc/nginx/nginx.conf-distro
cd /etc/nginx/
touch nginx.conf
sed -n 'w nginx.conf' reverse.conf
systemctl restart nginx
rm -rf reverse.conf
rm -rf /PROJECT-15-ACS


