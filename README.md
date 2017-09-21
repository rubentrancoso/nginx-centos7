# nginx-centos7

addpted from 
http://sharadchhetri.com/2014/07/29/install-nginx-source-centos-7/

Want to install NGINX in your CentOS 7 box?
JUST NEED TO EXECUTE THE LINE BELOW

```
mkdir tmp; cd tmp; yum install -y wget; \
service nginx stop; \
rm -rf nginx-install.*; \
yum -y install dos2unix; \
wget https://docs.google.com/document/d/1S0O0K6NcvlTCdj67mh_knpG7scSCvPvpseYS0fg6_PQ/export?format=txt; \
mv export\?format\=txt nginx-install.txt; \
dos2unix -n nginx-install.txt nginx-install.sh;chmod +x nginx-install.sh;\
./nginx-install.sh; rm -rf nginx-*
```
