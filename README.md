# City Vein

云计算期末项目

项目成员：李云帆、于天启、张嘉睿

基于https://github.com/ttcqaq/city-vein

部署ip:106.75.233.222

数据来源：8684、高德api

地图来源：百度地图api

效果展示：

![](/10195501416/city-vein/raw/branch/master/README_PIC/pic1.png)

# 网页部署方式：

1. 安装apache2
```
sudo apt install apache2
```

2. 将所有文件放至/var/www/html中

3. 访问云主机ip

# 公交线路数据更新方式：

本地更新方式：

1. 申请高德api，修改/scrpit/main.py中的key（默认已经填上申请好的key了）

2. 运行/script/main.py

分布式更新方式：

1. 需要配置四台云主机环境，安装sshpass（可以配好一台然后通过镜像创建）

2. 修改代码中对应主云主机的内网ip、用户名和密码并分别运行main1.py, main2.py, main3.py, main4.py

主云主机镜像名：MASTER

子云主机镜像名：PART

云主机账号：lyf_liyunfan@sina.com

云主机密码：l1i2y2u3nfan

![](/10195501416/city-vein/raw/branch/master/README_PIC/pic3.png)