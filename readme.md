# 介绍
广东海洋大学阳江校区校园网登录软件（个人开发），练手软件

本软件仅供学习参考使用

## 实现功能
### 目前实现一下功能：
登录、登出
密码自动保存

### 未实现功能
断网自动登录

## 实现原理
更新日期 2022.01.03
你看得懂代码也就明白了
### 登录
访问抓包后可以很明显发现，登录就是get这个url请求（至于为什么不是post账号密码，或者为啥要明文传输密码，我不知道）

http://10.200.132.20:801/eportal/portal/login?user_account=[]&user_password=[]
把[]替换成登录内容



### 登出
http://10.200.132.20:801/eportal/portal/logout


## 关于校园网有线链接
经过测试，学校drcom X版本只开启了802.1x协议登录，使用pandvan之类路由器,相关配置如下
![image](https://user-images.githubusercontent.com/49276659/193325371-1c9f8877-50fb-46cb-9cab-e5eca6d94352.png)








