`注意：此教程不能发送信息到服务器，只能接收来自服务器的数据`
总操作流程：
- 1、[下载固件](#ESP8266-01)
- 2、[修改文件](#ESP8266-02)
- 3、[烧写测试](#ESP8266-03)

***
# <a name="ESP8266-01" href="#" >下载固件</a>
[![](https://img.shields.io/badge/官网-最新SDK发布-red.svg "官网 最新SDK发布")](http://wiki.ai-thinker.com/esp8266/sdk)
[![](https://img.shields.io/badge/esp8266_nonos_sdk_tcpclient-2.2.0-green.svg "esp8266_nonos_sdk_tcpclient_2.2.0")](https://pan.baidu.com/s/1ASkiU3OLdq_YgJl94CGY_w)


![](image/1-1.png)

# <a name="ESP8266-02" href="#" >修改文件</a>
- user_tcpclient.h
修改成路由WiFi和密码，作用：加入到路由器

![](image/1-2.png)

- user_tcpclient.c
修改成要链接的TCP服务器

![](image/1-3.png)

# <a name="ESP8266-03" href="#" >烧写测试</a>
我的WiFi模块是：esp8266-01

- 烧写

![](image/1-4.png)

- 测试

![](image/1-6.gif)
