[toc]

# 笔记

## 语法示例

md是html的简化

| aa | bb | cc |
| -- | -- | -- |
| 1  | 2  |    |
| 3  | >  | 4  |
| 5  | 6  |    |
| ^  | 7  | 8  |

L^A^T~E~X😄

$$
\alpha+\beta=\gamma
$$

$\alpha+\beta=\gamma$
[画图在线编辑](https://mermaid-js.github.io/mermaid-live-editor/edit#eyJjb2RlIjoiZ3JhcGggVERcbkFbQ2hyaXN0bWFzXSAtLT58R2V0IG1vbmV5fCBCKEdvIHNob3BwaW5nKVxuQiAtLT4gQ3tMZXQgbWUgdGhpbmt9XG5DIC0tPnxPbmV8IERbTGFwdG9wXVxuQyAtLT58VHdvfCBFW2lQaG9uZV1cbkMgLS0-fFRocmVlfCBGW2ZhOmZhLWNhciBDYXJdXG4iLCJtZXJtYWlkIjoie1xuICBcInRoZW1lXCI6IFwiZGVmYXVsdFwiXG59IiwidXBkYXRlRWRpdG9yIjpmYWxzZSwiYXV0b1N5bmMiOnRydWUsInVwZGF0ZURpYWdyYW0iOnRydWV9)
[画图](https://www.jianshu.com/p/77cc07f47cdc)---时序图、甘特图、饼图、[流程图](https://blog.csdn.net/lis_12/article/details/80693975)
@import "C:\Users\Qilee\Pictures\Camera Roll\logo.png"

```c
void main(){
    int a,b;
    if(a>b)
        a=1;
    else
        printf();
}
```

## 网络小技能

- github镜像网站 github.com 替换为 hub.fastgit.org

## Linux常用

- 复制文件  `cp 源路径 目的路径`
- 查找
find -name / gfgfgfg* （找文件）
grep ghhj* / （查进程或文本）
- 重启网卡
 1.  `service network restart`
 2. `/etc/init.d/networking restart`
 3. `ifdown eth0`  `ifup eth0`
- 设置时间 `date -s "20210831 19:31:22"`
- 关闭防火墙
 1. `service stop firewalld` (临时关闭)
 2. `systemctl disable firewalld` (永久关闭，需重启)

## 网络问题

- 网卡是否识别
- 网线
- IP配置，网关等
- 防火墙状态
- 交换机路由特殊配置(转换模块是否正常)

## 远程或FTP

- 传文件

  `pscp hmi@192.168.2.169:/home/hmi/Desktop/a.png C:\Users\Qilee\Desktop`
- window网络映射

  `start \\ip `

## other

