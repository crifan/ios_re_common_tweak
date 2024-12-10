# OpenSSH

* OpenSSH
  * 作用：可以通过`ssh`的命令行方式去访问和操作越狱iPhone
  * 安装
    * `Cydia`/`Sileo`中搜：`openssh`，并安装，即可
      * Cydia
        * ![cydia_search_openssh](../../assets/img/cydia_search_openssh.png)
      * Sileo
        * ![sileo_search_openssh](../../assets/img/sileo_search_openssh.png)
  * 如何使用
    ```bash
    ssh root@192.168.2.28
    ```
    * 说明
      * iPhone要和电脑端（Mac）同处于一个WiFi局域网内
      * `192.168.2.28`是的iPhone的IP
        * ![iphone8_wifi_ip_28](../../assets/img/iphone8_wifi_ip_28.png)
      * 【首次=只需要初始化一次】
        * 当出现提示`Are you sure you want to continue connecting (yes/no/[fingerprint])? `
          * 输入：`yes`
      * OpenSSH的ssh的（默认）密码是：`alpine`
  * ssh免密登录
    * 概述
      * 初始化好环境后，每次只需要
        ```bash
        ssh-copy-id root@192.168.2.28
        ```

