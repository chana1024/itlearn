#docker 通过挂载和动态CMD，实现动态运行jar
 docker run -dit -p 8080:8080  -v /root/development/tool/docker/jar/app:/usr/local/app jar java -jar -Dspring.profile.active=test pms-framework.jar
