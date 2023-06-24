# Clash for Windows 使用教程

<img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202304100933346.png" alt="image-20230410093325206" style="zoom:33%;" />





# Clash for Android -- download

* 下载地址：https://github.com/Kr328/ClashForAndroid/releases
* 下载版本选择：https://www.zeelis.com/t/472.html

  * 【adb】 win11 配置 adb环境 史上最详细：[(81条消息) 【adb】 win11 配置 adb环境 史上最详细_win11安装adb_秋知叶i的博客-CSDN博客](https://blog.csdn.net/weixin_44205779/article/details/128215134)
  * 解决‘ADB‘ 不是内部或外部命令，也不是可运行的程序 或批处理文件：[(81条消息) 解决‘ADB‘ 不是内部或外部命令，也不是可运行的程序 或批处理文件_adb' 不是内部或外部命令,也不是可运行的程序_HaveFun_Wine的博客-CSDN博客](https://blog.csdn.net/HaveFun_Wine/article/details/126955851)

  * 打开手机**开发者模式**和**USB调试**功能，并用数据线连接电脑：[安卓手机开启USB调试 连接电脑 (360doc.com)](http://www.360doc.com/content/12/0121/07/32208585_1065757416.shtml)
* 通过USB调试使用adb工具进行查询显示cpu架构类型：[(81条消息) adb shell 查看CPU架构_adb查看cpu架构_小龙在山东的博客-CSDN博客](https://blog.csdn.net/lilongsy/article/details/120043158)
  * 小新Pad 2022系统架构：arm64-v8a
* [Clash for Android 使用教程 – BosLife Support (wikibos.com)](https://wikibos.com/index.php/kb/clash-for-android/)
  * 从GitHub下载apk安装的用户请注意：**foss** 为开源内核版，**premium** 为闭源内核版，比前者功能更强一些，推荐下载 **premium** 版。



# 进入adb环境

* D:\software\platform-tools>
* [oppo手机usb调试开关在哪-百度经验 (baidu.com)](https://jingyan.baidu.com/article/a3f121e49d9c90bd9052bbc8.html)
* [(81条消息) adb导出手机应用到电脑_adb导出apk_寒风_007的博客-CSDN博客](https://blog.csdn.net/hanfeng_linglie/article/details/126509817)
* [(81条消息) adb导出手机已安装程序到电脑.apk_adb 把手机app下载到电脑_SheaJi~的博客-CSDN博客](https://blog.csdn.net/u013452460/article/details/108124990?spm=1001.2101.3001.6650.1&utm_medium=distribute.pc_relevant.none-task-blog-2~default~CTRLIST~Rate-1-108124990-blog-126509817.235^v38^pc_relevant_default_base&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2~default~CTRLIST~Rate-1-108124990-blog-126509817.235^v38^pc_relevant_default_base&utm_relevant_index=2)

* 配置完环境变量要重启！！！！

* **查看应用列表：**
  查看所有应用列表：adb shell pm list packages
  查看系统应用列表：adb shell pm list packages -s
  查看第三方应用列表：adb shell pm list packages -3：
