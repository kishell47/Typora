# 变量跨.c文件传递

* 定义一个全局变量，static只在本文件中使用
  * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202306031439414.png" alt="image-20230603143913265" style="zoom:50%;" />
* 通过接口传递
  * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202306031440209.png" alt="image-20230603144034101" style="zoom: 67%;" />
* 头文件包含接口，头文件提供外部接口
  * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202306031441197.png" alt="image-20230603144108022" style="zoom:67%;" />
* 另一个.c包含头文件
  * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202306031445535.png" alt="image-20230603144512408" style="zoom:50%;" />
* 另一个.c文件中调用
  * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202306031443091.png" alt="image-20230603144355981" style="zoom:50%;" />



# 取低8位

* `&=0xFF；`



# 函数用指针传递数组

* <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202306031435539.png" alt="image-20230603143517414" style="zoom:50%;" />



# 函数三部分——声明、实现、调用

* <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202306031511258.png" alt="image-20230603151105132" style="zoom: 67%;" />



# extern关键字

* extern 是一个关键字，用于声明一个变量或函数的外部链接性。它的作用有以下两个方面：

  * 声明外部变量：当在一个源文件中使用 extern 关键字声明一个**变量**时，表示该变量是在其他源文件中定义的，可以在当前源文件中引用该变量而不需要重新定义它。这样可以在不同的源文件中共享同一个全局变量。

  * 声明外部函数：当在一个源文件中使用 extern 关键字声明一个**函数**时，表示该函数是在其他源文件中定义的，可以在当前源文件中调用该函数而不需要重新定义它。这样可以将函数的定义和声明分离，提高代码的可维护性和可重用性。

* 在你提供的代码中，extern 关键字用于声明一个函数 my_fifo_push_hci_tx_fifo，该函数可能是在其他源文件中定义的。通过使用 extern 关键字，可以在当前源文件中引用该函数而不需要重新定义它。这样可以实现函数的跨文件调用。