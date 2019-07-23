
一个纯原生CSS实现的登录页，大家可以用来参考

下载地址:[https://github.com/kevinlu98/logepage.git](https://github.com/kevinlu98/logepage.git)

>直接贴代码

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Document</title>
<style>
* {
    padding: 0;
    margin: 0;
}
body {
    background-color: #ECFFFF;
}
.w {
    width: 70%;
    margin-left: 50%;
    transform: translateX(-50%);
}
.errorBox {
    /*width: 60%;*/
    margin-top: 10px;
    border: 1px solid #ccc;
    /*margin-left: 50%;*/
    /*transform: translateX(-50%);*/
    padding: 10px;
    border-radius: 10px;
    background-color: #FFB5B5;
    opacity: .8;
    box-shadow: 0 10px 10px #ccc;
}
.errorBox h3 {
    color: #600000;
}
.errorBox span {
    color: #AE0000;
    padding-left: 20px;
}
.formBody {
    padding: 30px;
    border: 1px solid #429be0;
    margin-top: 30px;
    width: 20%;
    margin-left: 50%;
    transform: translateX(-50%);
    border-radius: 5px;
    background-color: #fefefe;
    box-shadow: 0 10px 10px #ccc;
}
.formBody h1 {
    font-size: 22px;
    font-weight: 400;
    text-align: center;
    padding-bottom: 10px;
    color: #666;
    border-bottom: 2px solid #ccc;
}
.formBody .row {
    padding: 10px;
}
.formBody label {
    display: block;
    color: #888;
}
.formBody .row input {
    outline: none;
    border: 1px solid #429be0;
    width: 200px;
    height: 30px;
    border-radius: 15px;
    margin-top: 5px;
    margin-left: 20px;
    padding-left: 30px;
}
.formBody .row  .chexk {
    width: 20px;
    height: 20px;
    margin-right: 10px;
    border: 1px solid #000;
    vertical-align: middle;
}
.formBody .row  span {
    /*height: 20px;*/
    /*line-height: 20px;*/
    color: #666;
}
.loginBtn {
    padding-bottom: 20px;
    border-bottom: 1px solid #ccc;
    text-align: center;
}
.loginBtn input {
    outline: none;
    width: 250px;
    height: 40px;
    color: #429be0;
    font-size: 18px;
    background-color: #fefefe;
    border: 2px solid #429be0;
    margin-bottom: 5px;
    border-radius: 20px;
}
.loginBtn input:hover {
    color: #fefefe;
    background-color: #429be0;
}
.hidden {
    display: none;
}
</style>
</head>
<body>
    <div class="w">
        <div class="formBody">
            <form method="post" action="">
                <h1>用户登录</h1>
                <div class="row">
                    <label for="username">用户名</label> <input type="text" id="username"
                        name="j_username" placeholder="请输入用户名" 
                        value="" />
                </div>
                <div class="row">
                    <label for="password">密码</label> <input type="password"
                        id="password" name="j_password" placeholder="请输入密码" />
                </div>
                <div class="row">
                    <input type="checkbox" name="_spring_security_remember_me" class="chexk" /><span>记住密码</span>
                </div>
                <div class="loginBtn">
                    <input type="submit" value="登 陆" /> <input type="reset"
                        value="重 置" />
                </div>
            </form>
            <div class="errorBox hidden">
                <h3>登陆失败</h3>
                <span>登录失败才显示</span>
            </div>
        </div>
    </div>
</body>
</html>
```
>预览

![](https://raw.githubusercontent.com/kevinlu98/cloudimg/master/data/QQ20190723-190308@2x.png)

> 希望对大家有所帮助
