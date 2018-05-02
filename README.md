# about sanshanblog docker build file
## 0.8
> This is deployed on the cluster to the attention of the management node can't occupy port 80 or 443

you need https site.key && name for site.crt to create secrets
this sanshan-main-setting.json config to domain name
and notice you docker  must  login to registry.cn-hangzhou.aliyuncs.com to download images 

## 0.7
> this is local test docker file,ip is localhost ,notice don't take up  port 80
###  notice
please use [localhost-sanshanblog.tar](https://github.com/SanShanYouJiu/sanshanblog-docker-file/releases) (There is a problem with using the file directly)

at local system to tar-xvf decompressed [localhost-sanshanblog.tar](https://github.com/SanShanYouJiu/sanshanblog-docker-file/releases)

and Fill in some configuration in web_back/sanshanblog/sanshanblog.properties

Run the docker-compose up command in the localhost-sanshanblog folder (In the console will be to print the stack)

The deployment environment requires 2 gb of memory or 2gb swapmemory 

> It is best to multi core cpu 