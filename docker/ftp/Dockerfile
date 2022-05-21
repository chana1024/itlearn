FROM stilliard/pure-ftpd as addlib
ADD nginx /usr/local/nginx
ADD lib/* /lib/x86_64-linux-gnu
ADD run.sh /
RUN mkdir /home/gm &&mkdir /home/gm/image && mkdir /home/gm/image/common/&&touch /home/gm/image/common/test.txt
FROM addlib
CMD ["/bin/sh","-c","/run.sh -l puredb:/etc/pure-ftpd/pureftpd.pdb -E -j -R -P $PUBLICHOST"]
