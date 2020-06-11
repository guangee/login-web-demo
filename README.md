# 登录注册demo 前端代码

# 在线demo [https://api-login-web.guanweiming.com/](https://api-login-web.guanweiming.com/)

# 后端接口 [https://api-login-demo.guanweiming.com/swagger-ui.html](https://api-login-demo.guanweiming.com/swagger-ui.html)

```javascript

$.ajax({
            url: host + "/api/user/login",
            method: "POST",
            data: {
                username: username,
                password: password
            },
            success: function (res) {
                if (res.status === 0) {
                    alert(res.data.username + "登录成功");
                } else {
                    alert(res.msg)
                }
            }
        })
```
