# CocoaTop64

* `CocoaTop`/`CocoaTop64`
  * 用途：查看进程详情
    * 举例
      * 查看进程参数`Raw Process Flags` -》 可以得知进程是否可调试
        * 具体详见：
          * [底层机制 · iOS逆向调试：Xcode+iOSOpenDev](https://book.crifan.org/books/ios_re_debug_xcode_iosopendev/website/app_debuggable/internal_logic.html)
          * [进程csflags定义 · iOS逆向调试：Xcode+iOSOpenDev](https://book.crifan.org/books/ios_re_debug_xcode_iosopendev/website/appendix/process_csflags.html)
        * 举例
          * ![debuggable_process_flag_whatsapp_04004004](../../assets/img/debuggable_process_flag_whatsapp_04004004.png)
            * `0x00000004` = `CS_GET_TASK_ALLOW`
              * 表示：可调试
