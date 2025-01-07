# OpenSSH

* `OpenSSH` = `ssh`
  * 源地址
    * https://apt.bingner.com/
  * 作用：可以通过`ssh`的命令行方式去访问和操作越狱iPhone
  * 概述
    * 安装
      * `Cydia`/`Sileo`中搜：`openssh`，可以搜到多个，点击`OpenSSH`，并安装，即可
    * 登录
      * 说明
        * 对于ssh的用户名：`<ssh_username>`
          * rootful：`root`
            * 举例
              * `ssh root@192.168.2.28`
          * rootless：`mobile`
            * 举例
              * `ssh mobile@192.168.2.28`
        * 对于ssh的密码：都是`alpine`
      * 首次
        * 首次登录
          ```bash
          ssh <ssh_username>@192.168.2.28
          ```
        * 输入`yes`，保存设置
        * 输入密码: `alpine`，即可登录
      * 去设置免密登录（只需要初始化一次）
        ```bash
        ssh-copy-id <ssh_username>@192.168.2.28
        ```
      * 之后每次直接登录
        ```bash
        ssh <ssh_username>@192.168.2.28
        ```
