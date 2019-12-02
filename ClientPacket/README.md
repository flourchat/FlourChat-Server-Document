# Client Packet

# 0x01 ClientHello
- 包体结构： String
- 功能： 在建立连接后发包，验证服务器版本号，正确则服务器发回[ServerHello](https://github.com/flourchat/FlourChat-Server-Document/blob/master/ServerPacket/README.md#0x01-serverhello)，错误则服务器关闭Websocket
