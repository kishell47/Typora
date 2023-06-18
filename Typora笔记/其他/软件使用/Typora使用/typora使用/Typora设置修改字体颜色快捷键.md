# Typora设置修改字体颜色快捷键



## 链接

[(70条消息) Typora设置修改字体颜色快捷键_typora改变字体颜色快捷键_耶耶LCY的博客-CSDN博客](https://blog.csdn.net/weixin_63676550/article/details/130111682)



## 目录

​	1.typora如何设置修改字体颜色快捷键[跳转到设置字体颜色](#1.typora如何设置修改字体颜色快捷键)

​	2.AutoHotKey软件安装[跳转到AutoHotKey软件安装](#2. AutoHotKey软件安装)

​	3.typora关于AutoHotKey的具体操作[跳转到typora关于AutoHotKey的具体操作](#3.typora关于AutoHotKey的具体操作)

4. 设置ahk文件开机自动启动[跳转到设置ahk文件开机自动启动](#4.设置ahk文件开机自动启动)



## 1.typora如何设置修改字体颜色快捷键

* typora本身是不能直接修改字体颜色的，不过若是想修改还是可以用一些代码去改变的，但是每次都修改一次实在麻烦。ahk全称[AutoHotKey](https://so.csdn.net/so/search?q=AutoHotKey&spm=1001.2101.3001.7020)，是一个强大的、简单易学的，Windows终极自动化脚本语言，我们可以借助这种语言来满足我们的需求

* > 借助一下AutoHotKey这个软件，可以很好的解决这个问题，软件大概10M，完全无压力，放一个蓝奏云链接：https://wwix.lanzoue.com/iaxOg0ssx0fa 密码:b6oc



## 2. AutoHotKey软件安装

* 双击该exe文件运行进行安装，你可以选择默认安装，也可以选择自定义安装，默认安装就是C盘了，我这里习惯选择的是自定义安装。
  * <img src="https://img-blog.csdnimg.cn/8797a90046cf4937b5f01fa0b60c6ce2.png" alt="img" style="zoom: 67%;" />



* 这个根据自己的电脑情况而定，我这里选择的是第二个
  * <img src="https://img-blog.csdnimg.cn/c931363274f4497bba8ec62e9ce7f5a0.png" alt="img" style="zoom: 67%;" />



*  在上面设置我们自己的安装位置
  * <img src="https://img-blog.csdnimg.cn/5abef9214e2e4967b9d6b72282479eab.png" alt="img" style="zoom: 50%;" />



* 然后安装完就可以退出了，点exit
  * <img src="https://img-blog.csdnimg.cn/d28291d1886d4e898c2d35046985a831.png" alt="img" style="zoom: 67%;" />



##  3.typora关于AutoHotKey的具体操作

* 在AutoHotKey刚刚的安装目录下，新建一个txt文件，然后将下列代码复制进去

  * ~~~json
    #IfWinActive ahk_exe Typora.exe
    {
        ; Ctrl+Alt+R 红色
        ^!r::addFontColor("red")
    }
     
    ; 快捷增加字体颜色
    addFontColor(color){
        Send {ctrl down}c{ctrl up} ; 复制
        SendInput {TEXT}<font color='%color%'>**
        SendInput {ctrl down}v{ctrl up} ; 粘贴
        If(clipboard = ""){
            SendInput {TEXT}**</font> ; Typora 在这不会自动补充
        }else{
            SendInput {TEXT}**</ ; Typora中自动补全标签
        }
    }
    ~~~

* 我一般只用红色，没有别的需求，如果你还想加其它颜色，可以在`^!r::addFontColor("red")`这句话下面继续添加。分号后面的都是注释。

* 然后将txt文件的后缀改为ahk，双击这个文件运行即可

* 然后在typora里面按下`Ctrl+Alt+R`修改字体颜色为<font color='red'>**红色**</font>



## 4.设置ahk文件开机自动启动

* 按`win+R`，输入`shell:startup`，打开启动的文件夹
  * <img src="https://img-blog.csdnimg.cn/31806e6427424c56a7192056e9059c7c.png" alt="img" style="zoom: 50%;" />
*  然后我们可以将想要开机自启动的文件放进来(复制或移动)
  * <img src="https://img-blog.csdnimg.cn/49943b9511da465f8ce9e9c254c284ee.png" alt="img" style="zoom: 50%;" />





