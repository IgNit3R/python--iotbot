# 配置

在项目根目录下创建 `.iotbot.json`文件用于配置，目前支持的配置如下几项：

```json
{
  "host": "127.0.0.1",
  "port": 8888,
  "webhook": true,
  "webhook_post_url": "http://localhost:5000",
  "webhook_timeout": 10
}
```

说明：

1. `host`: iotbot 端 ip
2. `port`: iotbot 端端口
3. `webhook`: webhook 功能开关
4. `webhook_post_url`: webhook 推送的地址，需要包含 http
5. `webhook_timeout`: webhook 推送到 url 请求的响应时间

如果你的 iotbot 配置跟默认的不符，设置`host`和`port`会很必要，否则每次调用`Action`有关方法时你都需要指定参数, 这样会方便许多，使代码简洁
