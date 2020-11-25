
### 登录接口

#### 功能
管理员通过用户名密码登录
- 已注册：返回token
- 未注册：登录失败

#### 请求地址
```text
/api/admin/login
```

#### 请求方式
POST

#### 请求参数
```json
{
  "user": "",
  "pwd": ""
}
```

#### 返回结果
1. 正常
```json
{
  "code": 0,
  "message": "successs",
  "body": {
      "xxxx" // 系统长期token
  }
}
```

2. 未注册
```json
{
  "code": 1,
  "message": "账号或密码错误"
}
```

#### curl
```text

```