使用postman进行post刷线配置请求时，http://localhost:2001/refresh 该接口可以刷新git配置

可能会报错，如下
{
    "timestamp": 1602545750559,
    "status": 401,
    "error": "Unauthorized",
    "message": "Full authentication is required to access this resource.",
    "path": "/refresh"
}

需要添加如下配置项：
management.security.enabled=false
