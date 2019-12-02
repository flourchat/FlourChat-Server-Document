# Server Packet

## 0x01 ServerHello
- 包体结构： String
- 功能： 在客户端[ClientHello](https://github.com/flourchat/FlourChat-Server-Document/blob/master/ClientPacket/README.md#0x01-clienthello)后发包，核对版本号，如果不正确则Websocket关闭

## 0xfe Result
- 包体结构： Int16(状态码：正数或0为成功，负数为失败), String(状态描述)
- 功能： 返回一些操作的状态
