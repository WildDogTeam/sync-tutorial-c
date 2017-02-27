# sync-tutorial-c 
##远程加法器
本部分展示了借助 Wilddog C/嵌入式 SDK 实现远程加法器。在网页输入两个数，客户端对这两个数进行相加并推送到网页端。这是一个简单的远程加法器，它的输入和输出都是网页端，而控制逻辑也是简单的相加。你可以利用 Arduino 或树莓派 (可以在快速入门了解 Wilddog C/嵌入式 SDK 支持的平台 )，把各类的传感器的输出或者网上的天气等的数据作为其输入，电机驱动或者是 LCD 驱动作为其输出，制作更有实用意义的控制器。

### 克隆代码

    git clone https://github.com/WildDogTeam/sync-tutorial-c.git

### 使用
把 remote-cal.c 拷贝到 wilddog-client-c\examples\linux\ 下，点击此下载 [wilddog-client-c SDK](https://github.com/WildDogTeam/wilddog-client-c.git)

修改 "DEMO_YOUR_URL"，将 `"<Your appId>"` 改为你的应用的 appId , 若你还没有 appId ，需要先到 [wilddog](www.wilddog.com) 进行注册。

	#define DEMO_YOUR_URL "coap://<Your appId>.wilddogio.com"

编译：

	$ make
    $ make example

使用加法器

    $./bin/remote-cal

### 更多示例

这里分类汇总了 WildDog 平台上的示例程序和开源应用，　链接地址：[https://github.com/WildDogTeam/wilddog-demos](https://github.com/WildDogTeam/wilddog-demos)

### 相关文档

* [Wilddog 概览](https://docs.wilddog.com/overview/index.html)
* [c SDK快速入门](https://docs.wilddog.com/quickstart/sync/c.html)
* [c SDK API](https://docs.wilddog.com/api/sync/c/reference.html)
* [下载页面](https://www.wilddog.com/download/)

### License
MIT

http://wilddog.mit-license.org/

