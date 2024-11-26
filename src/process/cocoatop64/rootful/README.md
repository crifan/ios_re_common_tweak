# rootful的CocoaTop64

此处介绍，**rootful**的越狱iPhone中，如何安装：`CocoaTop`/`CocoaTop64`

* `CocoaTop64`
  * 安装
    * Mac中：下载deb
      * http://apt.thebigboss.org/repofiles/cydia/debs2.0/cocoatop64_2.2.3.deb
        * 注：另外一个，或许可用的，deb地址
          * https://github.com/D0m0/CocoaTop/releases/download/2.2.3/ru.domo.cocoatop64_2.2.3_iphoneos-arm.deb
    * Mac中：下载到iPhone中
      ```bash
      scp cocoatop64_2.2.3.deb root@192.168.2.37:/var/root/
      ```
    * iPhone中：安装deb
      * 2种方式
        * 用Filza安装
          * 点击deb-》安装-》动作-》`注销`=`Respring`=`重启桌面`
        * 用dpkg安装
          ```bash
          dpkg -i cocoatop64_2.2.3.deb
          ```
  * 常见问题
    * 安装后看不到CocoaTop的桌面图标？
      * 去清除UI缓存
        * Filza重新安装一遍deb，最后点击`uicache`
        * 或者自己去ssh命令行中运行：`uicache`
