# JNDIMonitor

![](img/jndi.png)

## 简介

随着Apache Log4j被打的越来越多，常见的dnslog平台估计会被屏蔽的越来越狠，而且利用dnslog平台去做批量化，感觉也不太好判断是哪里触发的。

突然想到常用的Java jndi注入工具就有这功能，然后就删去了多余的代码，当一个`LDAP`请求监听器，摆脱`dnslog`平台。

```shell
Usage: java -jar JNDIMonitor-1.0-SNAPSHOT.jar [options]
  Options:
  * -i, --ip       Local ip address  (default: 0.0.0.0)
    -l, --ldapPort Ldap bind port (default: 1389)
    -h, --help     Show this help
```

## 参考

https://github.com/0x727/JNDIExploit/

![as](https://starchart.cc/r00tSe7en/JNDIMonitor.svg)
