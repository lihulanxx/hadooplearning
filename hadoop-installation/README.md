# Hadoop Installation 

### 1.准备

- Ubuntu 16.04 X64

>有条件可以实机安装,也可以装在虚拟机上(建议只保留命令行界面,图形界面会卡).如果是win10系统,可以很方便
 的从应用商店安装Ubuntu,具体教程Google.
 
 
### 2.安装Docker
 
 [官方安装教程](https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/)

### 3.拉取hadoop镜像
 
使用 [kiwenlau/hadoop-cluster-docker](https://github.com/kiwenlau/hadoop-cluster-docker) 集群镜像以及其配置。国内可以替换为相应的国内源，以加快拉取速度。
 
 > 镜像没有开放9000端口,需要在 <code>start-container.sh</code>里为<code>hadoop-master</code>添加 <code>-p 9000:9000 \
 
### 4.启动hadoop
  
  Hadoop网页管理地址:
  
  - NameNode: http://192.168.99.100:50070/
  - ResourceManager: http://192.168.99.100:8088/