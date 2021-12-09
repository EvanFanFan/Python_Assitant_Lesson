# 如何连接安卓设备

### 一、工具准备

安卓设备需要打开USB调试

电脑需要下载ADB调试工具

[ADB Tools 下载地址](https://developer.android.google.cn/studio/releases/platform-tools?hl=zh_cn)

### 二、环境配置

将下载后的文件解压放在D盘，本示例中的路径是D:\adbtools

![8c65b2a1e228b497d6f64234b97a987](https://user-images.githubusercontent.com/43714537/145423695-9f7652e4-b2bf-4da5-803f-8ab2a73fcdb8.png)


右键我的电脑属性-->高级系统设置-->环境变量-->Path 增加项D:\adbtools

![601eb9ab75531f0733ff663fd02be01](https://user-images.githubusercontent.com/43714537/145423598-51b0a078-4947-4f6d-b80a-f5d3d243c6ff.png)




### 三、确认设备连接是否成功

`adb devices`

如果 List of devices 有设备显示 那么安卓设备已经连接成功  
![1639062235(1)](https://user-images.githubusercontent.com/43714537/145422123-745967b9-dd23-4b03-ba54-b2d11d84a71c.png)


如果没有就再研究一下



切换网络连接的方式 

`adb tcpip 5555`

`adb connect  安卓设备IP:5555`



5555是默认的tcpip端口，你可以改成自己想要的
