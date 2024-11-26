# 注意事项

## 从`Cydia`中从`BigBoss`中搜出来的CocoaTop安装失败

* 从`Cydia`的
  * `BigBoss`的源中搜出来的
    * ![cydia_search_cocoatop](../../../assets/img/cydia_search_cocoatop.png)
      * `2.0.1`的`CocoaTop`
        * ![cydia_cocoatop_201](../../../assets/img/cydia_cocoatop_201.png)
        * ![cydia_cocoatop_confirm](../../../assets/img/cydia_cocoatop_confirm.png)
      * `2.2.3`的`CocoaTop64`
        * ![cydia_cocoatop64_223](../../../assets/img/cydia_cocoatop64_223.png)
        * ![cydia_cocoatop64_install](../../../assets/img/cydia_cocoatop64_install.png)
  * 安装结果会失败
    * HTTP/1.1 503 Service Unavailable
      * ![cydia_cocoatop64_fail_503](../../../assets/img/cydia_cocoatop64_fail_503.png)
  * -> 所以后续才改用：直接下载deb，去安装的
