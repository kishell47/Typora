# Git将指定的文件恢复到指定的提交版本

1. **查看某个文件的修改历史找到要回退到的commit的哈希值**

* ~~~bash
  git log [file-path]
  ~~~

* 例如：

  * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202304301607493.png" alt="image-20230430150645299" style="zoom: 67%;" />

2. **将该文件回退到指定的commit版本，覆盖当前的文件版本**

~~~bash
git checkout [commit-hash] -- [file-path]
~~~

* 请注意，如果你有未提交的修改，执行该命令将会丢失这些未提交的修改。如果你需要保存这些修改，请在执行该命令之前先进行提交或备份。
* 其中，`[commit-hash]`是指要回退到的commit的哈希值
* `[file-path]`是指文件路径
  * `[file-path]`既可以是绝对路径也可以是相对路径，具体取决于你当前所在的工作目录和文件所在的位置。
  * 如果文件在当前工作目录中，则可以使用相对路径，否则应该使用绝对路径。
  * 如果你不确定该使用哪种路径，请使用绝对路径以确保正确性。
* 例如：
  * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202304301519825.png" alt="image-20230430151940720" style="zoom: 67%;" />

3. **Git 会将指定的文件恢复到指定的提交版本，同时将该文件添加到暂存区。**
   * Git Graph
     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202304301537821.png" alt="image-20230430153710740" style="zoom: 67%;" />
   * Git Bash
     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202304301536252.png" alt="image-20230430153614160" style="zoom: 80%;" />



4. **比较指定文件在暂存区和某个指定提交的区别**

   * ~~~Bash
     git diff [commit-hash] -- [file-path]
     ~~~

     * `[commit-hash]`为要比较的提交版本的哈希值
     * `[file-path]`为要比较的文件的路径。
     * 如果要比较暂存区和最近的提交版本之间的区别，可以将`[commit-hash]`参数省略不写。
     * 比较结果会显示出两个版本中文件的差异，如果执行 `git diff [commit-hash] -- [file-path]` 没有任何输出，那么说明暂存区和指定提交的该文件内容完全一致，没有区别。

   * **例子**

     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202304301606535.png" alt="image-20230430160641421" style="zoom: 67%;" />
       * 执行 `git diff 08997807 -- .settings/language.settings.xml` 没有任何输出，那么说明暂存区和指定提交的该文件内容完全一致，没有区别。



# 工作目录

* 通过运行`pwd`命令来查看当前所在的工作目录。

* 在命令行中输入`pwd`并按下回车键即可显示当前目录的绝对路径。

* ~~~bash
  OP076859@WJL-SH40433618 MINGW64 ~/Desktop/app-control-panel (master)
  $ pwd
  /c/Users/OP076859/Desktop/app-control-panel
  ~~~

  

# 绝对路径

* 绝对路径是指文件或目录**在整个文件系统中的完整路径，以根目录（通常是“/”）作为起点**。
* 绝对路径可以唯一地确定文件或目录的位置，不受当前工作目录的影响。



# 相对路径

* 相对路径是**指相对于当前工作目录的路径**。
* 它是一种相对于当前位置的文件或目录的描述方式，而不是从根目录开始的完整路径。
* 在命令行或代码中，相对路径通常以`.`或`..`开头，分别代表当前目录和上一级目录。
* **例如：**
  * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202304301541920.png" alt="image-20230430154133857" style="zoom: 67%;" />