1. 上电闪灯、关灯：可能tof透镜有灰尘，擦一下
2. 重启问题：之前上电600次TOF会失效、268版本5000次重启限制、269没有重启限制
3. 烧录：
   * 接线：靠近丝印的是3.3V、接着是GND、还需要点一个SWDIO
   * 烧录不进去：检查硬件连接、点击开锁
     * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202305121508767.png" alt="image-20230512150828606" style="zoom:50%;" />



* 手势的具体参数数据

| 手势 | 识别条件                                                     | 退出条件                                           |
| :--: | :----------------------------------------------------------- | -------------------------------------------------- |
| 单扫 | 1. 手从传感器上方扫过，在传感器上方停留时间大于0.1s并小于2s<br />2. 手在1s内没有再次遮挡传感器<br />3. 识别单扫动作时间为1s |                                                    |
| 双扫 | 1. 两次连续单扫动作，两次单扫的时间间隔在0.5s到2s。<br />2. 时间间隔 = 第二次单扫手离开传感器识别范围的时刻 - 手第一次进入传感器识别范围的时刻 |                                                    |
| 悬停 | 1. 手进入传感器侦测范围内超过2s 并且没有超过3cm 的垂直移动距离。 | 手离开传感器识别范围或者有超过3cm 的垂直移动距离。 |
| 拉距 | 手进入传感器侦测范围内的2s内有超过3cm的垂直移动距离          | 手离开传感器识别范围                               |

* 注：传感器识别范围：0-30cm