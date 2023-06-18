# UART串口通信协议详解

* [UART串口通信协议详解](https://blog.csdn.net/qq_43533553/article/details/123255990?app_version=5.11.1&code=app_1562916241&csdn_share_tail=%7B%22type%22%3A%22blog%22%2C%22rType%22%3A%22article%22%2C%22rId%22%3A%22123255990%22%2C%22source%22%3A%22qq_44754285%22%7D&uLinkId=usr1mkqgl919blen&utm_source=app)

* <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305261408577.png" alt="image-20230526140801512" style="zoom: 80%;" />

* 数据位：5-8位数据（**先发低位，后发高位**）。例如：发送数据为0x55（01010101），则发送的数据为(10101010)
* <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305261414168.png" alt="image-20230526141412054" style="zoom:67%;" />

* <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305261428279.png" alt="image-20230526142809085" style="zoom:50%;" />





# 波特率

* 波特率的值为115200表示每秒传输115200个比特
* 传输一个比特（bit）所需的时间是1 / 115200 秒，约为 8.68 微秒。



# 透传

* 传什么是什么