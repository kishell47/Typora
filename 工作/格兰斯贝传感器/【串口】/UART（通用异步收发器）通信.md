# 8258或8278进行UART（通用异步收发器）通信流程

* 初始化函数`uart_drv_init()`

  * 声明
    * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305290829784.png" alt="image-20230529082931669" style="zoom:50%;" />

  * 调用
    * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305290833678.png" alt="image-20230529083356562" style="zoom: 50%;" />

  * 



`uart_drv_init()`是在特定的MCU环境（8258或8278）中进行UART（通用异步收发器）通信初始化的函数。以下是该函数的详细解析：

1. 设置UART硬件和DMA（直接内存访问）配置。
2. 初始化UART数据的接收缓冲区，并设置UART的引脚（发送和接收）。
3. 执行UART复位操作，将与UART相关的数字寄存器复位为初始状态。
4. 根据时钟频率设置UART的波特率。具体的时钟频率设置取决于MCU的类型（16MHz、24MHz、32MHz或48MHz）。
5. 启用UART的DMA传输，使UART数据能够通过DMA传输到硬件缓冲区中。

总之，该函数的作用是对UART进行初始化设置，以便在MCU中进行串口通信。



# 在特定的MCU环境（8258或8278）中进行UART通信的流程

1. 设置UART的引脚：根据具体硬件设计，设置UART的发送（TX）和接收（RX）引脚。
2. 复位UART：执行UART的复位操作，将与UART相关的寄存器复位为初始状态。
3. 初始化UART：根据特定的时钟频率和波特率要求，初始化UART的配置。根据MCU的时钟频率选择合适的波特率设置，例如115200。具体的波特率设置可以在初始化函数中进行调整。
4. 启用UART DMA传输：启用UART的DMA传输功能，允许使用DMA传输数据到UART的硬件缓冲区。
5. 中断设置：根据需要，配置UART相关的中断功能。例如，可以使能UART接收（RX）和发送（TX）的DMA中断，以便在数据接收和发送完成时触发中断。

以上是在特定的MCU环境（8258或8278）中进行UART通信的基本流程。具体的代码实现可能会有所差异，取决于具体的开发环境和需求。





1. 设置UART的引脚：通过调用函数`uart_gpio_set(UART_TX_PIN, UART_RX_PIN)`设置UART的发送（TX）和接收（RX）引脚。
2. 复位UART：通过调用函数`uart_reset()`执行UART的复位操作，将与UART相关的寄存器复位为初始状态。
3. 初始化UART：根据MCU的时钟频率选择合适的波特率设置，并调用`uart_init()`函数进行UART的初始化配置。波特率的具体设置在代码中根据不同的时钟频率进行了选择。
4. 启用UART DMA传输：通过调用函数`uart_dma_enable(1, 1)`启用UART的DMA传输功能，允许使用DMA来传输数据到UART的硬件缓冲区。

综上所述，UART硬件和DMA配置的设置发生在初始化函数中的上述步骤中。这些设置确保UART能够正常工作，并与其他设备进行异步通信。具体的硬件配置和寄存器设置可能因MCU型号而异，上述代码片段中的设置适用于特定的MCU环境（8258或8278）。