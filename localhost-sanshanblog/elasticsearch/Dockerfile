# es相关
# VERSION 1.0.BETA
FROM elasticsearch:2.4.0

LABEL maintainer="www.85432173@qq.com"

#COPY 配置文件
COPY elasticsearch.yml /usr/share/elasticsearch/config

#加入IK分词器
ADD ik.tar.gz  /usr/share/elasticsearch/config
ADD analysis-ik.tar.gz  /usr/share/elasticsearch/plugins

# 健康检查
HEALTHCHECK  --interval=5s --timeout=3s \
CMD curl -fs http://127.0.0.1:9200 ||exit 1





