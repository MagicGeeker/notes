# Centos7搭建WebVirtMgr
## 安装虚拟机相关软件
https://www.cnsre.cn/posts/211117937177/

https://blog.csdn.net/redrose2100/article/details/127636821

## 下载docker镜像并启动docker  
https://hub.docker.com/r/odivlad/webvirtmgr  
```
docker pull odivlad/webvirtmgr
```
按照网页所示，应该能打开8000对应对应网页


## webvirtmgr后续配置
https://blog.51cto.com/u_10272167/2697161  
## webvirtmgr错误排查
### /etc/libvirt/qemu.conf配置
```
user="root"  
group="kvm"  
vnc_listen = "0.0.0.0"  
```
### chmod 666 /dev/kvm  


## 其他问题
网页上interfaces打不开，暂未解决
网页上vnc打不开，应该是docker网络问题，暂未解决，本机下载vnc viewwe替代
