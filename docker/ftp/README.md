docker run -d -p 21:21 -p 81:81 -p 30000-30009:30000-30009 -e FTP_USER_NAME=gm -e FTP_USER_PASS=gmp@123 -e FTP_USER_HOME=/home/gm -v /root/development/pmsExten/docker/ftp/volume/nginx/conf:/usr/local/nginx/conf -v /root/development/pmsExten/docker/ftp/volume/ftphome:/home/gm ftp


