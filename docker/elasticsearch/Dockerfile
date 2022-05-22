FROM ibmjava:jre
RUN mkdir /opt/app
ADD elasticsearch-5.5.1/ /opt/app/elasticsearch-5.5.1
RUN groupadd chana && useradd chana -g chana &&echo chana:chana|chpasswd&&chown -R chana:chana /opt/app/elasticsearch-5.5.1
RUN sysctl -w vm.max_map_count=262144
CMD ["su","chana","-c"," /opt/app/elasticsearch-5.5.1/bin/elasticsearch"]
