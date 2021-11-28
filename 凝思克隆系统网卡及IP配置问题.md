### 问题描述
 凝思克隆系统网卡不起作用引起的IP配置无效，ping不通等
### 解决方法
1.重新生成mac地址网卡绑定文件
```js
cd /etc/udev/rules.d/
mv 70-persistent-net.rules 70-persistent-net.rules.bak
reboot
```
2.对照mac地址表修改自动生成的70-persistent-net.rules文件
![mac地址表](C:/Users/Qilee/Desktop/1.jpg)
![rules文件](C:/Users/Qilee/Desktop/4.jpg)
按照mac地址表MAC1-eth0 ... MAC14-eth13的顺序修改70-persistent-net.rules文件中“NAME=eth8” 类似部分
修改完毕保存重启

3.配置ip
```js
cd /etc/network/
vim interface
```
配置示例（含双IP）
![rules文件](C:/Users/Qilee/Desktop/2.jpg)
![rules文件](C:/Users/Qilee/Desktop/3.jpg)
重启网卡
`service networking restart`
清理错误dns
```js
cd /etc
vim resolve.conf
```
删掉无关的dns配置
