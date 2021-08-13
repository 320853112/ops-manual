# 离线安装rpm包

[返回上级](../catalog.md) 

    yum离线下载包：
        在有网的电脑上
        yum -y install --downloadonly --downloaddir=/home/Package/ 软件名

        安装
        rpm -ivh xxx.rpm
        

        上面的方法在本地已经安装目标包的情况下，会提示已安装，导致不能下载
        可使用如下方法：
            yumdownloader <package-name>

        ps:在不同的环境上，有时待安装的环境会缺少依赖，可根据缺少依赖的提示，
        反复的执行这个下载包的过程，直至完成目标软件的安装。    