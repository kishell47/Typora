# Typora链接



## 参考链接

[(70条消息) Typora使用技巧 | 各种跳转 【必备】_typora链接跳转到其他文件_想要腹肌的熊的博客-CSDN博客](https://blog.csdn.net/qq_41907769/article/details/121722716)

[Typora官网：Links - Typora Support](https://support.typora.io/Links/#html-a-tag)



## 目录

​	[1. 页面链接](#1. 页内链接)

​		[1.1跳转到标题](#1.1 跳转到标题)

​		[1.2跳转到任意位置](#1.2  跳转到任意位置)

[2. 文件跳转](#2. 文件跳转)





## 1. 页内链接



### 1.1 跳转到标题



#### 1.1.1 方法一：用于目录链接跳转

* **步骤1：在需要需要跳转的地方添加链接**

  * > 语法：[文字说明]（#标题全称）

  * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305011903717.png" alt="image-20230501190327575" style="zoom: 50%;" />

* **步骤2：按`Ctrl`键+单击链接实现跳转**



#### 1.1.2 方法二：大纲直接跳转

* 标题标好，单击直接跳转

* <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305011916573.png" alt="image-20230501191611510" style="zoom: 67%;" />



### 1.2  跳转到任意位置

* **实现双链笔记**

* **模板：**

  * <font color='red'>**函数类型**</font>[点击跳转到函数类型](#函数类型)<a id = "返回正文1"></a>

  * <a href="#返回正文1">点击返回正文</a>

* **锚点：**船停在港口时，抛锚做个定点标记。`<a name="这是你的锚点"></a>` 🚩

* **步骤**

  * **描点定义**

    * ~~~html
      <a id="描点"></a>
      在typora文档中，说name属性和id属性都行
      <a name="锚点"></a>
      ~~~

    * <img src="https://img-blog.csdnimg.cn/9440fe259d1e4dfab9dc8aa70428896b.png" alt="在这里插入图片描述" style="zoom: 80%;" />

    * <img src="https://img-blog.csdnimg.cn/8dd6b4adad244e9d9b2f22b445646295.png" alt="在这里插入图片描述" style="zoom:80%;" />

  * **使用锚点：**

    * **使用 href属性：**

      * ~~~HTML
        <a href="#锚点">点击后就会跳到你定义的锚点</a>
        ~~~

* **例子**

  * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305021104714.png" alt="image-20230502110449628" style="zoom:50%;" />

  * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305021105308.png" alt="image-20230502110538245" style="zoom:50%;" />



## 2. 文件跳转

* **步骤1：在需要需要跳转的地方添加链接**

  * > 语法：[文字说明]（文件路径）

  * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305011948606.png" alt="image-20230501194803508" style="zoom: 67%;" />

* **步骤2：按`Ctrl`键+单击链接实现跳转**









