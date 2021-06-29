# alexamaster-auto Ubuntu/windows

注册网址：[点我](https://www.alexamaster.net/sec/join.php?id=163416)

(直连即可，一切操作不需要魔法)

注册邮箱选择163邮箱等，千万不要用QQ邮箱，QQ邮箱已经被禁。

注册后有需要你验证邮箱地址，需要```Withdraw Money```中的```REQUEST```页面点击第二个打了红色×的帖子，去绑定邮箱和寄送地址，才能满足提现条件。

(或者开启浏览器自动翻译，找到提现页面自行解决提现未满足的条件)

提现方式是paypal，国内卡直接注册即可，相关操作自行搜索。(CSDN或者知乎都有教程)

下面是具体操作

# 前提：Windows系统

得不偿失，有更好的挂机项目别挂这个，吃内存资源。

只需要下载火狐浏览器，将类似我的

https://www.alexamaster.net/ads/autosurf/163416

这样子的链接粘贴到地址栏访问即可挂机。

# 前提：Ubuntu系统

### step1：初始化

终端窗口逐行输入

国内机子：
```
sudo -i

wget xiaofd.github.io/vncam.sh 

bash vncam.sh -p 'https://gitee.com/spiritlhl/Alexamaster-onkey-start/attach_files/757322/download/passwd-d10086' -u 'https://www.alexamaster.net/ads/autosurf/163416'
```
国外机子：
```
sudo -i

wget xiaofd.github.io/vncam.sh 

bash vncam.sh -p 'https://github.com/spiritLHL/Alexamaster/releases/download/%E8%84%9A%E6%9C%AC/passwd-d10086' -u 'https://www.alexamaster.net/ads/autosurf/163416'
```
#### 说明：

 注意-p和-u参数都是必要的

-p参数后面指定的是vnc登陆密码下载链接：使用我默认的这个密码为：d10086

-u参数后面放你自己的挂机链接

这里的

https://www.alexamaster.net/ads/autosurf/163416

是我的挂机链接，有需要请自行挂网站里自己的auto surf链接

#### 非必须：

当安装完毕后可以通过命令 vncpasswd 直接修改vnc登陆密码（最长8位）

可以自己导出自己的密码文件，替换上面的-p参数，文件为 ~/.vnc/passwd

已知：

完美适用于Ubuntu16.04

运行完脚本后即可开始挂机，已经安装火狐插件和关闭屏蔽弹窗，无需进入vnc配置 vnc登陆端口5901，默认vnc登陆密码d10086

### step2：启动挂机

启动vnc桌面环境(逐行输入)

export DISPLAY=localhost:1

firefox --profile ~/.alexa/alexa --new-tab 'https://www.alexamaster.net/ads/autosurf/163416' &

tightvncserver :1

说明：

这里的

https://www.alexamaster.net/ads/autosurf/163416

是我的挂机链接，有需要请自行挂网站里自己的auto surf链接

### step3：设置定时重启避免卡住

前提：宝塔面板

在宝塔中打开计划任务

设置shell脚本

#### 第一个：

任务名称：定时关闭

执行周期：N小时 8 时 0 分

脚本内容
```
sudo -i
export DISPLAY=localhost:1
firefox --profile ~/.alexa/alexa --new-tab 'https://www.alexamaster.net/ads/autosurf/163416' &
pkill firefox
```
#### 第二个：

任务名称：定时启动

执行周期：N小时 8 时 5 分

脚本内容
```
sudo -i
export DISPLAY=localhost:1
firefox --profile ~/.alexa/alexa --new-tab 'https://www.alexamaster.net/ads/autosurf/163416' &
tightvncserver :1
```
上面中启动的是我的链接，自己的自行替换

实际测试占用还行，大概800M内存，18%的2核英特尔i5CPU和7.5G硬盘空间。

如果不是2核4G的云服务器，建议把周期从8小时改得更短。

最低配置要求：1核1G内存10G硬盘

收入大概一天好的0.2美元，坏的0.1美元。

# 提现注意事项：

不要攒到一起提现，每到1美元就进行提现，提现到账周期大概为1周，一次最多申请2~3个，申请额度高或次数过多，到账周期将以月计算。

