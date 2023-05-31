# BodyDec

20年写的bp插件，github备份

因为工作需要数据包body加解密，许久未更新（代码惨目忍睹），借鉴logger++设计思路

BodyDec使用指南

本工具主要适用于数据包body为对称加密且已知加密算法的测试，方便测试过程中对加密的数据包进行直接查看、修改、重放。

例如正常加密数据包如下：


Config界面输入对应的请求包、响应包的算法信息、以及body中的加密字符串的前缀后缀（一般使用正则匹配规则），以及需要解密数据包的host信息，点击配置。

![](https://github.com/Yu4sue/BodyDec/assets/15160012/2a77a8b9-ce37-419a-9487-2795331d5f2e)

 
即可在Logger View界面下查看该域名下的数据包解密后的信息。

![](https://github.com/Yu4sue/BodyDec/assets/15160012/30544c0b-aa15-406c-bd16-814b244766e8)
 
如需修改重放数据包，则点击右键

![](https://github.com/Yu4sue/BodyDec/assets/15160012/16d73e75-ce32-44a4-9b68-06e03837ce99)

在新生成的repeater tag中进行修改、重放
 
![](https://github.com/Yu4sue/BodyDec/assets/15160012/4e95865c-3bf3-4b34-95be-53d9da995955)

