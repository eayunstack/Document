# 故障检测工具

当EayunStack环境出现故障时，需要管理员进行故障排除，首先要对故障点进行定位，此时就需要用到一些故障检测的工具，下面列出一些常用故障检测工具：

|命令|功能|检测对象|
|----|----|----|
|eayunstack doctor|检测EayunStack基本环境状态</br>检测各OpenStack节点各组件状态</br>检测各集群状态</br>|EayunStack环境|
|ping|检测网络连通性|网络|
|tcpdump|网络流量截取分析|网络|
|ntpq|查看NTP状态|NTP|
|ps&top|查看系统进程信息|进程|
|free|查看内存使用量|内存|
|df|查看文件系统空间使用量|文件系统|

