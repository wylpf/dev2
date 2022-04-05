---
typora-root-url: C:\Users\wang\Desktop
---

# **Postman工具**



## 1、简介



Postman最早是Google浏览器的一个插件存在的，因为Google退出国内市场，现在postman主要是以一个 APP的形式存在。
Postman最初设计上就是为接口测试而设计的，对于测试人员来说主要用来做接口测试。在做接口测试的时候,Postman相当于一个客户端,它可以模拟用户发起的各类HTTP请求,将请求数据发送至服务端,获取对应的响应结果, 从而验证响应中的结果数据是否和预期值相匹配;并确保开发人员能够及时处理接口中的bug,进而保证产品上线之后的稳定性和安全性。



## **2、功能**



.postman是一款强大的网页调试、HTTP请求发送及接口测试用例运行的工具
·能够模拟各种HTTP的请求方式，比如：GET、POST、DELETE、PUT等请求方式
·请求中可以发送文件（图片、文本文件等）、额外的添加header等，实现特定的功能
·能够更高效的帮忙后台独立进行接口测试



#### 1.抓取和分析现有网站请求

这个功能需要Postman Interceptor Chrome插件和Postman结合一起使用，打开Capture开关后, Interceptor抓取请求，在Postman的History里显示详情，每个请求都会完整抓取，你可以对这些 request进行修改，过滤，以及编写测试。

![1](C:\Users\wang\Desktop\演讲图片\1.jpg)

#### 2.创建Http请求

这个功能是最基础的功能，可以在Postman插件和桌面版本上都可以使用，可以通过注册的用户同步所有的请求。
Http请求的报文每个部分，各种情况都能设置，用的过程你会觉得操作设计的很方便。Http返回的结果也能清晰查看。

![2](C:\Users\wang\Desktop\演讲图片\2.jpg)



#### 3.管理Http请求(Collections)

可以把Http请求按组管理，比如一个项目或一个模块的所有请求归到一组（Collection)。 另外很多功能都是以Collection为基础。

![3](C:\Users\wang\Desktop\演讲图片\3.jpg)



#### 4.变量

Postman有多种定义变量的方法，用于不同的作用域，详细可以参考官方文档,不管是哪种变量，都是使用{{variable}}来使用变量。
变量非常有用，在开发、测试等环境下切换或者API是可以分享给其它人的，在不同的环境下修改一下环境变量，就可以无缝使用。

![4](C:\Users\wang\Desktop\演讲图片\4.jpg)



#### 5.导出和导入

以Collection为基础可以导出为JSON格式，然后分享给其它人。也可以导入，导入支持的格式更多。

![5](C:\Users\wang\Desktop\演讲图片\5.jpg)



#### 6.生成在线API文档

这个功能非常实用，设计者定义API接口后，可以直接发布为一个在线的API文档，分享给API开发者和API使用者，API文档的模板很简洁清晰，他们基于这个API文档可以理解也可以测试。
API文档还附带了cURL脚本，JS脚本等测试代码。

![6](C:\Users\wang\Desktop\演讲图片\6.jpg)



#### 7.自动化测试

也是以Collection为基础，可以启动Postman的 Collection Runner工具，也可以批量测试所有API，可以记录所有运行日志。
（command line工具）

![7](C:\Users\wang\Desktop\演讲图片\7.jpg)



#### 8.Mock server

也是以Collection为基础，可以为一个Collection创建一个Postman提供的Mock server，额外需要为每个API请求设置一个或多个Example，设置API请求的返回Mock数据。
这个功能是收费功能

![8](C:\Users\wang\Desktop\演讲图片\8.jpg)



Postman功能特别多，以上只是一部分，即使这只是部分功能，里面细节也很多，适用于开发者和测试人员。



## 3、安装

Postman安装需要依赖 .NET 环境。
双击postman的安装文件即可安装。

（群里老师发的有）



## 4、使用

**步骤**：
1、选择请求方式
2、然后输入请求的URL
3、然后切换到Body选项，选择Content-Type，选择以后postman会自动 把Content-Type填写的headers（请求头信息）中。
4、在body中填写请求参数 （GET例外，GET请求没有请求主体）
5、断言（在Tests中编写断言）
6、点击“Send”按钮模拟发送请求

**GET请求的发送**

![g](/C:/Users/wang/Desktop/演讲图片/g.jpg)

**POST请求的发送**![p](/C:/Users/wang/Desktop/演讲图片/p.jpg)

# 5、总结

postman在做接口测试方面，发挥着越来越重大的作用，其支持多种请求方式、并可以模拟各种类型的数据请求类型，在实际开发中使用它可以极大的提高开发的效率。 