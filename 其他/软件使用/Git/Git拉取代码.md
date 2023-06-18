## 从远程Git仓库将代码拉取到本地

* 登录VPN
  * 服务器地址：https://wjvpn.opple.com
  * 账号：w3账号密码
* 登录
  * 10.10.10.167
* 配置ssh key
  * 在你C盘的个人账户中有个.ssh文件，里面的红框中的文件可以用vscode打开，复制里面的内容粘贴到167 ssh key 中
    * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202304271010360.png" alt="企业微信截图_16819544919339" style="zoom: 67%;" />
    * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202304271011863.png" alt="企业微信截图_16819544919339" style="zoom: 67%;" />
* **clone with ssh**
  * `git clone git@10.10.10.167:app/app-control-panel.git`
  * <img src="https://cvp.oss-cn-shanghai.aliyuncs.com/picgo/202304271013028.png" alt="image-20230427101310985" style="zoom:67%;" />

