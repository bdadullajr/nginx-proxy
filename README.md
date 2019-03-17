# nginx-proxy
NGINX proxy using certbot

#### NGINX SSL PROXY CONFIGURATION ####

- Install tomcat
- deploy war file
- install nginx (amazon-linux-extras install nginx1.12)
- service nginx start, restart, status stop etc...
- Generate certificate from certbot (https://certbot.eff.org/ - selecting CentOS/RHEL7 for nginx)
- Install "amazon-linux-extras install epel" before "yum install certbot python2-certbot-nginx" if error occur
- Then proceed for "certbot --nginx" 
- Create nginx config (vi /etc/nginx/conf.d/iot.bdadullajr.com.conf)
- create "/etc/ssl/private" folder
- run "openssl dhparam -out /etc/ssl/private/dhparams.pem 4096"
- Then "nginx -t && service nginx reload" if above configuration are completed

