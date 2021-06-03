## V2RayN客户端



#### V2Ray搭建

新的一键V2Ray脚本，经过笔者的测试，安装简单方便，自动关闭防火墙，自动安装BBR加速，因此推荐大家使用！



**安装命令：**

输入以下命令，回车执行

```bash
bash <(curl -s -L https://git.io/v2ray-setup.sh)
```

如果提示 curl: command not found ，那是因为你的 VPS 没装 Curl 

ubuntu/debian 系统安装 Curl 方法: apt-get update -y && apt-get install curl -y 

centos 系统安装 Curl 方法: yum update -y && yum install curl -y 安装好 curl 之后就能安装脚本了

##### 显示一下信息代表安装成功（可直接用以下配置进行连接）(以下配置在链接时使用)：

```
---------- V2Ray 配置信息 -------------

 地址 (IP Address) = 141.*.*.*

 端口 (Port) = 8888

 用户ID (User ID / UUID) = 38b272ba-8a91-*-*-*

 额外ID (Alter Id) = 0

 传输协议 (Network) = tcp

 伪装类型 (header type) = none

---------- END -------------

V2Ray 客户端使用教程: https://git.io/v2ray-client

提示: 输入 v2ray url 可生成 vmess URL 链接 / 输入 v2ray qr 可生成二维码链接

---------- V2Ray vmess URL / V2RayNG v0.4.1+ / V2RayN v2.1+ / 仅适合部分客户端 -------------

vmess://ewoidiI6I*****g==
```



**配置文件要注意(建议直接复制安装结果中 vmess://\**\** 地址，直接导入，避免自己填配置出错)：**

> Network(传输协议)： tcp
> type(伪装类型)：none
> 不对的话连不上！！！



好了到这里我们就搭建成功了(*^▽^*)



### 下载 V2RayN (客户端)

下载链接： https://github.com/2dust/v2rayN/releases/latest



### v2ray客户端：

**下载方式一：网盘(直接解压可用)**

【v2rayN】：

 https://cloud.degoo.com/share/f-Vljc2ZjhmcPyHbi5Pw0A 

 https://github.com/xyz690/cloudimg/blob/main/data/v2rayN-3.29.zip



### **下载方式二：GitHub**

客户端：下载[v2rayN.zip](https://github.com/2dust/v2rayN/releases/download/3.29/v2rayN.zip)

【[v2rayN.exe Github Releases](https://github.com/2dust/v2rayN/releases)】 https://github.com/2dust/v2rayN/releases/download/3.29/v2rayN.zip

内核：下载`v2ray-windows-64.zip`文件

【[v2ray-windows-64.zip Github Releases](https://github.com/v2ray/v2ray-core/releases)】 https://github.com/v2fly/v2ray-core/releases/download/v4.31.0/v2ray-windows-64.zip

对`v2ray-windows-64.zip` 和 `v2rayN`进行解压，然后将 `v2rayN` 目录下所有文件复制到`v2ray-windows-64`解压后的目录，即两个下载好的文件需要在同一目录。



### **进行配置:**

客户端的配置需要根据你的服务端进行相应的配置，因为你的服务端协议可能是vmess等。

如果你的服务端配置是协议vmess，则配置如下：

![](https://github.com/Alertu/VSNAS/blob/master/img_5ea112995ff23.png)



### Android v2ray客户端：

**下载方式一：网盘(APK直接安装)**

【APK】：https://cloud.degoo.com/share/msgcYbsWQVoz2EIbSXr5bw 或 https://github.com/xyz690/cloudimg/blob/main/data/v2rayNG_1.4.13_arm64-v8a.apk

**下载方式二：GitHub**
一般手机是arm架构，我就直接给出对应客户端了，其他架构需要你去网上找设备相应的CPU架构并进行选择下载：
【[v2rayNG Github Releases](https://github.com/2dust/v2rayNG/releases)】https://github.com/2dust/v2rayNG/releases/download/1.4.13/v2rayNG_1.4.13_arm64-v8a.apk



**使用方法:**

```javascript
(1）打开 v2rayNG APP
(2）点击右上角 + 号
(3）选择 手动输入[Vmess]
(4）别名随意，地址(填服务器外网IP地址)，端口(你设置的V2Ray端口)，用户ID，额外ID:0，加密方式:auto，其他设置默认
(5）右上角 √ 保存
(6）右下角 V图标 点击启动.
(7）打开浏览器试试吧
```



## v2ray提速之BBR

本文脚本对支持BBR加速的系统，自动安装BBR加速！

CentOS查看BBR是否运行，输入以下命令，回车执行（`shift+insert`可粘贴）：

```shell
lsmod | grep bbrCOPY
```

有返回则成功！



