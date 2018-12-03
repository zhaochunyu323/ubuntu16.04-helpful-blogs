# ubuntu16.04-helpful-blogs  
从开始配置一个服务器，对于新手来说， 会遇到一系列的问题，当我们上网百度或者谷歌搜索问题时，一般会找到非常多的博客，所以会无从下手，我们希望能筛选出最有用博客，我把我平时使用并解决问题的一些博客总结下来，希望对大家有用  
## 1.安装NVIDIA显卡驱动  
https://www.jianshu.com/p/b313625fbe61  
https://blog.csdn.net/tianrolin/article/details/52830422  
## 2.安装显卡驱动出现循环登录问题    
https://blog.csdn.net/ssmixi/article/details/73483795  
## 3.安装CUDA  
安装nvidia官网上的步骤来，开始之前一定要进入文本模式，并禁用图形界面，使用命令`sudo service lightdm stop`，安装成功后重启图形界面`sudo service lightdm start`  
https://my.oschina.net/wangsifangyuan/blog/1575004  
## 4.安装cuDNN  
https://www.jianshu.com/p/e22866b72f43  
## 5.将系统自带的python3从python3.5升级到python3.6  
https://blog.csdn.net/u011254180/article/details/80905055  
## 6.在以太网内设置静态IP，方便远程连接
https://www.jianshu.com/p/ea4bca38e5d7  
其中的网卡名称，地址，网关，掩码和广播都根据自己的来写，完成后重启系统
## 7.让两台服务器共享文件夹
https://blog.csdn.net/yulijun2201/article/details/81873489  
可以把其中的ip地址改为\*，这样就可以使所有地址都可以连接，被共享的服务器中的文件夹要放在根目录下，就是以下博客说的内容  
https://blog.csdn.net/weixin_38663832/article/details/79796257
