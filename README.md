# 登录注册demo 前端代码

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
