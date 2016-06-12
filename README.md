# EasyUbuntu
Quick Installation Scripts For installing LNMP(Nginx stable + PHP5.6 + MySQL 5.6) and some more on ubuntu/debian.

Attention : Please use root privileges (either su or sudo ) to run all the scripts

## Install LNMP :
wget https://raw.githubusercontent.com/sunflyer/EasyUbuntu/master/lnmp.sh && sudo bash lnmp.sh

This scripts will install PHP5.6  FROM PPA SOURCE , and Nginx / MySQL from offical source 


## Quick Setup A HTTPS Site Using Nginx
wget https://raw.githubusercontent.com/sunflyer/EasyUbuntu/master/setHttps.sh && sudo bash setHttps.sh

This scripts will help you setup a website using https QUICKLY and EASILY

To Use :  
- Wget this script  
- input information promoted , the Certificate file path should be absolute path (e.g. /etc/ssl/a.crt)
- wait for a moment
- enjoy your site via https !

Note : The website configuration file will be put on /etc/nginx/conf.d , file named  ssl-<HOST NAME> will be generated for one operation which would contains both 301 jump and ssl configurations.

The configuration file generated will make the site using Forward Security and HSTS. You can always choose whether using it or not by editing ssl- files yourself.

PHP-FPM via UNIX SOCKET is configured by default.

## Install Shadowsock Server :
wget https://raw.githubusercontent.com/sunflyer/EasyUbuntu/master/shadowsock.sh && sudo bash shadowsock.sh

install shadowsock server (python edition) with chacha20

This scripts will make 3 scripts and 1 json file for shadowsock in current directory. The three scripts is used for start/stop/restart shadowsock and json file is used for configuration. 

By default ,the ecryption method is chacha20 and two port (2330 and 2333) opened with password (987654321 and 123456789).
Remember to change it!
