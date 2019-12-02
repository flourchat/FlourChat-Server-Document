# Client Packet

## 0x01 ClientHello
- 包体结构： String
- 功能： 在建立连接后发包，验证服务器版本号，正确则服务器发回[ServerHello](https://github.com/flourchat/FlourChat-Server-Document/blob/v0/ServerPacket/README.md#0x01-serverhello)，错误则服务器关闭Websocket

## 0x02 Auth
- 包体结构： Int64(UID), String(password_sha256)
- 功能： [ServerHello](https://github.com/flourchat/FlourChat-Server-Document/blob/v0/ServerPacket/README.md#0x01-serverhello) 后进行验证操作，发送用户名和密码，验证登录信息，完成后服务器发回 [Result](https://github.com/flourchat/FlourChat-Server-Document/blob/v0/ServerPacket/README.md#0xfe-result) ，如果失败则关闭Websocket


