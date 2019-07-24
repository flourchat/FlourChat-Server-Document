# FlourChat-Server-Document
This document is only in Chinese.

# 连接方式
创建一个websocket长连接到服务器。

# 数据包格式 （Version 0x00）
## Header部分，占8字节
一个完整的header看起来是这样子的：
```
00 00 01 00 00 00 00 00
```
- 第一个字节：版本号：永远为0x00
- 第二个字节：连接类型：永远为0x00
- 第三个字节：包ID：根据不同的功能来定义
- 第四个字节：发送者类型：永远为0x00
- 第五个字节和第六个字节：一个Short代表包体长度
- 第七个字节和第八个字节：一个Short永远为0

# 数据包

