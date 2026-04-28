## 微服务公共协议
### 使用框架 `go-zero`

### 生成RPC代码
```bash
goctl rpc protoc user/user.proto -I user --go_out=./user --go-grpc_out=./user --zrpc_out=./user

# 删除不使用的服务端代码
rm -rf ./user/user.go # 删除服务端代码
rm -rf ./user/etc # 
rm -rf ./user/internal
```