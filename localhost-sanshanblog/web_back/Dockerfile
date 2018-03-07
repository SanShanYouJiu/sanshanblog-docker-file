# sanshanblog  后台
#需要与mongodb，mysql容器连接
# VERSION   1.0.Beta 
FROM tomcat:8.5.23
ENV CATALINA_BASE /usr/local/tomcat

LABEL maintainer="85432173@qq.com"

RUN cd $CATALINA_BASE/webapps/ROOT && rm -r *  

# COPY Tomcat配置文件 
COPY server.xml $CATALINA_BASE/conf
COPY catalina.sh $CATALINA_BASE/bin
 

# 健康检查
HEALTHCHECK  --interval=5s --timeout=3s \
CMD curl -fs http://127.0.0.1:8080/api/ ||exit 1