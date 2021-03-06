# 搭建基本环境

基本环境的搭建需要按照以下流程进行：

## 检查环境资源

* 检查安装介质是否可用
* 检查服务器配置是否满足需求
* 检查网络设备配置是否满足需求
* 检查存储设备是否可用

## 网络规划

根据“网络架构”章节所描述的网络架构，规划各网络所使用的网段及交换机所需要划分的VLAN。

|网络角色|网段|子网掩码|
|----|----|----|
|Management/PXE|172.16.100.0|255.255.255.0|
|Public|||
|Storage|172.16.201.0|255.255.255.0|
|Private|10.0.0.0|255.255.255.0|
|Ceph Cluster|172.16.202.0|255.255.255.0|
  
> ###### 注意
> **Public**网络对应网段需要根据生产环境进行规划

## 服务器角色规划

根据“环境需求”中所描述的服务器配置需求，规划各物理服务器的角色。

|服务器角色|第一块网卡MAC地址|
|----|----|
|Fuel||
|Controller||
|Compute||
|Mongo||
|Ceph-osd||

## 设备上架

* 服务器及网络设备上架（建议将角色相同的服务器放置在相邻位置）。

## 连接网线

* 根据“网络架构”章节所描述的网络拓扑图，正确连接所有网线。

## 配置网络设备

* 根据网络规划配置交换机，划分VLAN。

## 存储设备配置

* 配置Dell equallogic（注意网络配置需要按照网络规划配置）。

