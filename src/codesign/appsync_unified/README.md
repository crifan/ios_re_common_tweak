# AppSync Unified

* `AppSync`=`AppSync Unified`
  * 用途：让系统不再验证签名-》app安装就不会，因为签名原因而安装失败了
  * 安装
    * 概述
      * `Cydia`
        * 添加软件源
          * 软件源-》编辑-》添加-》输入Cydia/APT地址：
            * https://cydia.akemi.ai/
        * 安装插件
          * 软件源-》`Karen/あけみ’s Repo` -》插件-》`AppSync Unified`-》安装
      * 特殊说明：截止20241210，上述源地址 https://cydia.akemi.ai/ 已失效
        * 暂时只能根据网上[介绍](https://www.reddit.com/r/LegacyJailbreak/comments/1drdgwm/help_alternate_repo_for_appsync_unified/)，去别处下载插件的deb
          * https://web.archive.org/web/20230516162851/https://cydia.akemi.ai/debs/nodelete-ai.akemi.appsyncunified.deb
        * 然后下载到iPhone中
          ```bash
          scp nodelete-ai.akemi.appsyncunified.deb root@192.168.2.28:/var/root/devRoot
          ```
        * 手动去安装
          * 方式1：`dpkg`
          ```bash
          dpkg -i nodelete-ai.akemi.appsyncunified.deb
          ```
            * 注意：安装后，要`重启桌面`=`注销`=`Respring`一下才能生效
              ```bash
              ldrestart
              ```
          * 方式2：`Filza`
            * 概述
              * `Filza`->点击deb插件（`nodelete-ai.akemi.appsyncunified.deb`）->`安装`->`动作`->`注销`=`Respring`
            * 详解
              * [Filza安装](../../codesign/appsync_unified/installing/filza_install.md)
