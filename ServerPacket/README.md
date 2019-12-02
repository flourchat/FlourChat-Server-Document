# Server Packet

## 0x01 ServerHello
- 包体结构： String
- 功能： 在客户端[ClientHello](https://github.com/flourchat/FlourChat-Server-Document/blob/master/ClientPacket/README.md#0x01-clienthello)后发包，核对版本号，如果不正确则Websocket关闭


