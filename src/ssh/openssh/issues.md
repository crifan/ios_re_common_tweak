# 常见问题

## ssh connect to host port 22 Connection refused

* 现象

```bash
➜  altsys make install
swift-driver version: 1.26.9 ==> Installing…
ssh: connect to host 192.168.31.43 port 22: Connection refused
...
```

或：

```bash
➜  ~ ssh root@192.168.2.28
ssh: connect to host 192.168.2.28 port 22: Connection refused
```

* 原因和解决办法
  * 可能1：iPhone没越狱
    * 解决办法：先去给iPhone越狱
  * 可能2：没有安装OpenSSH插件
    * 解决办法：已越狱的iPhone中，安装OpenSSH插件
  * 可能3：越狱已丢失=iPhone已失去越狱
    * 解决办法：给iPhone恢复越狱
