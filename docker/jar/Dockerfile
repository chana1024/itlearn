FROM centos as addlib
RUN mkdir /var/lib/jvm && mkdir /usr/local/app
ADD jdk1.8.0_202/ /var/lib/jvm/jdk1.8.0_202 
ENV JAVA_HOME=/var/lib/jvm/jdk1.8.0_202
ENV JRE_HOME=$JAVA_HOME/jre
ENV CLASSPATH=$JAVA_HOME/lib:$JRE_HOME/lib:$CLASSPATH
ENV PATH=$JAVA_HOME/bin:$JRE_HOME/bin:$PATH
FROM addlib
WORKDIR /usr/local/app
CMD ["/bin/bash"]

