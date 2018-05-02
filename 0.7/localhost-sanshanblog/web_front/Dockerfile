# sanshanblog  前端  跑在nginx上
# VERSION   1.0.Beta 
 FROM nginx:1.13.3

LABEL maintainer="85432173@qq.com"

COPY nginx.conf /etc/nginx

ADD dist.tar.gz  /etc/nginx/html 

EXPOSE 4000
 

HEALTHCHECK  --interval=20s --timeout=5s \
CMD curl -fs http://127.0.0.1:4000/ ||exit 1