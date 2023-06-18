# Android Studio



## 1. 安装和使用教程



### 1. 1 链接

* [全网最全最细Android Studio 安装和使用教程 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/528196912)
* [(70条消息) 【android】超级详细Android Studio下载安装教程（附：JDK1.8安装教程）_智商三岁半i的博客-CSDN博客](https://blog.csdn.net/weixin_46081857/article/details/122204682)



### 1.2 步骤



1. **安装JDK（Java开发工具包）并配置好其中的环境**
   * 系统是win11
   * 具体安装的方法可以参照
     * [安装JDK并配置好其中的环境](#1.2.1 安装JDK（Java开发工具包）并配置好其中的环境)



2. **Android Studio 下载地址及版本说明**

   * Android 开发者官网：

     * [全球，需科学上网](https://developer.android.com/?hl=zh-cn)
     * [国内，可直接访问](https://developer.android.google.cn/index.html) 

   * Andriod Studio下载地址

     * https://developer.android.com/studio
     * 长时间无法下载的时候，请将下载地址复制出来，然后将https改为http即可[http&https](D:\Typora笔记\软件使用\Android Studio\Knowledge\http&https.md)

     * [下载地址](http://r4---sn-ni57rn7d.gvt1.com/edgedl/android/studio/install/2022.2.1.19/android-studio-2022.2.1.19-windows.exe?cms_redirect=yes&mh=xB&mip=36.113.101.174&mm=28&mn=sn-ni57rn7d&ms=nvh&mt=1682988503&mv=m&mvi=4&pl=19&rmhost=r3---sn-ni57rn7d.gvt1.com&shardbypass=sd&smhost=r3---sn-ni57rn7y.gvt1.com)



3. **安装步骤图解**

   * **首先在安装目录下创建SDK和Studio文件夹**

     * SDK文件夹：存放SDK文件

     * Studio文件夹：安装Android Studio

     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305020847940.png" alt="image-20230502084738874" style="zoom: 50%;" />

   * **手动双击已下载的Android Studio安装包**
     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305021020810.png" alt="image-20230502102059729" style="zoom: 67%;" />

   * **进入欢迎向导，直接点击下一步继续：**
     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305021022782.png" alt="image-20230502102237688" style="zoom:50%;" />

   * **选择要安装的组件，默认下一步即可（如果不需要模拟器也可以取消 Android Virtual Device 勾选）：**
     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305021024759.png" alt="image-20230502102407643" style="zoom:50%;" />

   * **选择 Android Studio 的安装位置（第1步创建的Studio文件夹），然后下一步：**
     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305021025980.png" alt="image-20230502102523901" style="zoom:50%;" />

   * **选择开始菜单，默认下一步即可：**
     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305021026625.png" alt="image-20230502102618509" style="zoom:50%;" />

   * **Android Studio 正在安装中：**
     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305021026912.png" alt="image-20230502102653821" style="zoom:50%;" />

   * **安装完成页面，直接下一步即可：**
     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305021027699.png" alt="image-20230502102737627" style="zoom:50%;" />

   * **点击Finish并开启 Android Studio：点击finish就安装结束了**
     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305021028797.png" alt="image-20230502102820688" style="zoom:50%;" />



4. **配置**

   * 点击`Cancel`
     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305021340305.png" alt="image-20230502134038173" style="zoom: 50%;" />

   * 点击`next`
     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305021341150.png" alt="image-20230502134144043" style="zoom: 50%;" />

   * 点击选中`Standard`
     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305021342667.png" alt="image-20230502134259540" style="zoom:50%;" />

   * 选择开发的主题颜色，然后点击`Next`
     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305021344486.png" alt="image-20230502134412380" style="zoom:50%;" />

   * 





#### 1.2.1 安装JDK（Java开发工具包）并配置好其中的环境



##### 1.2.1.1 找到JDK官网进行下载安装



1. **官方的网址**[Download the Latest Java LTS Free](https://link.zhihu.com/?target=https%3A//www.oracle.com/java/technologies/downloads/%23jdk18-windows)

   

2. **查看电脑是几位的**

   * 设置--系统--系统信息--系统类型

   * 系统类型：64位操作系统 基于x64的处理器
     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305012107180.png" alt="image-20230501210745081" style="zoom: 50%;" />



3. **进行对应的版本下载**
   * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305020810971.png" alt="image-20230502081019836" style="zoom: 50%;" />



4. **点击**
   * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305020812357.png" alt="image-20230502081227278" style="zoom:50%;" />



5. **点击下一步**
   * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305020813278.png" alt="image-20230502081357203" style="zoom:50%;" />



6. **选择相应的位置，建议放在除c盘以外的盘中，然后点击下一步**
   * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305020816581.png" alt="image-20230502081629512" style="zoom:50%;" />



7. **安装完成**
   * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305020818837.png" alt="image-20230502081846737" style="zoom: 67%;" />



##### 1.2.1.2 是否配置成功

* 一般点击安装成功以后会自动给你电脑配置好
* 打开命令窗口win+R，输入cmd回车
* 输入Java，显示以下内容表明你自动配置成功了
  * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305020822560.png" alt="image-20230502082213436" style="zoom: 50%;" />

* 再输入javac，查看你的Java工具是否路径正确
  * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305020823222.png" alt="image-20230502082354137" style="zoom: 50%;" />

* 输入Java -version

  * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305020825373.png" alt="image-20230502082559311" style="zoom:50%;" />

    * 说明你的Java环境设置好了

    * 这里的电脑是win11和jdk为20版本

    * 点击安装自动配置省去了很多步骤







## 2. 小知识



### 2.1 <font color='red'>**SDK**</font>

* <font color='red'>**SDK**</font>是Software Development Kit的缩写，指的是软件开发工具包。
* 它是一组软件开发工具和资源的集合，可以帮助开发人员创建特定类型的应用程序、软件框架、操作系统等。
* SDK通常包括一组<font color='red'>**API（应用程序接口）**</font>、示例代码、库文件、调试工具、文档和教程等内容，以方便开发人员进行开发和调试工作。
* SDK可用于开发多种不同类型的应用程序，例如游戏、移动应用程序、桌面应用程序、网站等等。

