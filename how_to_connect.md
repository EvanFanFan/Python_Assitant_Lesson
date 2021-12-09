# 如何连接安卓设备

安卓设备需要打开USB调试

电脑需要下载ADB调试工具

[ADB Tools 下载地址](https://developer.android.google.cn/studio/releases/platform-tools?hl=zh_cn)



`adb devices`



![image-20211209230400193](C:\Users\freel\AppData\Roaming\Typora\typora-user-images\image-20211209230400193.png)

如果 List of devices 有设备显示 那么安卓设备已经连接成功

如果没有就再研究一下



切换网络连接的方式 

`adb tcpip 5555`

`adb connect  安卓设备IP:5555`



5555是默认的tcpip端口，你可以改成自己想要的
