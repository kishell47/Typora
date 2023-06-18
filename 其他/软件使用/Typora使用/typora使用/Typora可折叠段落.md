# Typora可折叠段落



## 目录

1. 注意
2. 步骤
3. 折叠代码



## <font color='red'>**1.注意**</font>

* typora里面需要在<font color='red'>**源码模式下**</font>编辑以下内容，如果直接通过插入代码的方式输入以上内容，不能识别折叠功能，代码块会将整个内容误认为代码。

  

## 2.步骤

* 在源代码模式下输入

  * ~~~html
    <details>
    <summary>可折叠标签</summary>
    <p>具体数据，可以使用HTML标签<kbd>Ctrl</kbd>，但是不能使用传统的markdown语法。
    </p>    
    </details>
    ~~~

* 效果
<details>
<summary>可折叠标签</summary>
<p>具体数据，可以使用HTML标签<kbd>Ctrl</kbd>，但是不能使用传统的markdown语法。
</p>    
</details>


## 3.折叠代码

* 在代码块里面头部和尾部分别添加如下内容，但是代码块内部不能有空行

* ~~~html
  <details><summary>代码名称</summary>
  代码内容
  </details>
  ~~~

<details>
<summary>代码名称</summary>
代码内容
</details>


