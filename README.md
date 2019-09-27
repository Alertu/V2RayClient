V2RayN使用教程
233boy edited this page on 22 Mar · 1 revision
V2RayN 是 PC 平台上一个对新手比较友好的 V2Ray Windows 客户端。写个简单的 V2RayN 使用教程帮助新手

备注
以下教程均以使用了本站的一键安装 V2Ray 脚本为前提：V2Ray 一键安装脚本
如果你还没有安装 V2Ray，可以参考这教程：V2Ray搭建详细图文教程

下载 V2RayN
备注：按住 Ctrl + 单击， 即可在新窗口打开链接

下载链接： https://github.com/2dust/v2rayN/releases/latest

然后选择 v2rayN-Core.zip 下载
下载好了之后，解压，然后打开解压的文件夹
目录结构大概如下图所示


获取 V2Ray 客户端配置
SSH 登录你的 VPS （如果你没登录）
输入 v2ray url

然后复制 vmess 链接 （将链接全选，然后鼠标右键，再选择复制即可）

配置 V2RayN
双击 v2rayN.exe 启动，然后在任务栏托盘找到 V2RayN 图标并双击它
添加一个 VMess 服务器


从剪贴板导入 URL


设置本地监听端口，此处我将它设置为 2333


启用系统代理
在任务栏托盘找到 V2RayN 图标并鼠标右键，然后选择 启动系统代理
并且设置 系统代理模式 》PAC 模式
之后在 V2RayN 主界面，找到 检查更新 》检查更新 PAC

测试一下
在完成上面的步骤的时候，正常来说，你已经处于翻出去的状态了
OK，此时你已经自由了，赶紧打开 Google 找部十八减的大电影喵喵吧。哈哈

备注一，如果你浏览器有使用 Proxy SwitchyOmega ，请点击它的图标然后选择 系统代理
备注二，如果你在使用 Firefox 浏览器，打开选项，找到网络代理，再选上 使用系统代理

暂停一下
默认来说，使用 V2RayN 的 启动系统代理 来管理翻墙比较简捷一些，浏览器直接就能翻出去了
说着当然，如果你想要手动来管理浏览器的代理也行，往下看
备注，如果你不是有特别的需求，不需要参考下面的 Firefox 和 Chrome 的做法。

Firefox (火狐浏览器)
(什么？没有在使用 Firefox ，那赶紧来试用吧， Firefox Quantum，更好的浏览器。 )
打开选项，找到网络代理

火狐设置代理
选择手动代理设置，输入 127.0.0.1 和 2333，勾选 使用 Socks v5 代理 DNS，然后确定即可。

设置代理信息
OK，此时你已经自由了，赶紧打开 Google 找部十八减的大电影喵喵吧。哈哈

Chrome (谷歌浏览器)
安装 Proxy SwitchyOmega （如果你已经安装，知道怎么设置代理吧。。SOCKS5 协议，2333 端口 ）
在线安装：从 Chrome 应用商店 安装

手动安装如下：
在 Chrome 地址栏输入 chrome://extensions 打开扩展程序，之后
下载 Proxy SwitchyOmega ，打开链接后，找到 SwitchyOmega_Chromium.crx 下载，将下载完后的文件拖动到刚才打开的扩展程序的标签进行安装
然后点击 添加扩展程序 即可

添加扩展程序
OK，在完成安装 Proxy SwitchyOmega 后，
浏览器会自动打开一个 SwitchyOmega 选项的窗口，选择跳过教程，

跳过教程
选择 导入/导出，在线恢复，输入： https://github.com/FelisCatus/SwitchyOmega/wiki/GFWList.bak

在线恢复
选择 GFWed，设置代理端口为 2333，然后点击 应用选项

设置代理
然后右上角找到 Proxy SwitchyOmega 图标，点击它，再点击自动切换

切换代理
OK，此时你已经自由了，赶紧打开 Google 找部十八减的大电影喵喵吧。哈哈

结束
实际上，没有特别的需求根本不需要安装 Proxy SwitchyOmega ，直接使用 V2RayN 打开 启动系统代理 就可以自动翻出去了
如果你有使用 Proxy SwitchyOmega
V2RayN 设置的那个 本地鉴听端口 可以随便修改的，如果你修改了，Proxy SwitchyOmega 那边也要设置成对应的端口就行
啊~生活如此美好
