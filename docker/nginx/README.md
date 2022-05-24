docker run -dit -p 80:80 -e hostip=host.docker.internal -v /root/development/pmsExten/docker/nginx/volume/conf:/etc/nginx
-v /root/development/pmsExten/docker/nginx/volume/www:/www -v/root/development/pmsExten/docker/nginx/volume/logs:/var/log/nginx ui
