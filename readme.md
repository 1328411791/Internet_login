# 介绍
广东海洋大学阳江校区校园网登录软件（个人开发），应该兼容主校区校园网，练手软件
理论上兼容使用深澜协议的校园网，但是没有测试过，如果有兴趣可以试试

目前校园网更新，暂时不可用，等待更新

本软件仅供学习参考使用

## 实现功能
### 目前实现一下功能：
登录

## 未实现功能
1. 断网自动登录服务
2. 修改登录配置文件


## 开源相关
1. [srun](https://github.com/zu1k/srun)



# 旧版逻辑（目前废弃）
## 实现原理
更新日期 2022.01.03
你看得懂代码也就明白了

# WIFI登录

### 登录
访问抓包后可以很明显发现，登录就是get这个url请求（至于为什么不是post账号密码，或者为啥要明文传输密码，我不知道）

http://10.200.132.20:801/eportal/portal/login?user_account=[]&user_password=[]
把[]替换成登录内容



### 登出
http://10.200.132.20:801/eportal/portal/logout

# 校园网有线链接方式

经过测试，学校drcom X登录软件目前只开启了802.1x协议登录，可以使用pandvan/OpenWRT等路由器，使用锐捷（或其他软件）实现登录,我目前使用的路由器相关配置如下

登录账号和密码同上

登录协议选择：
![image](https://user-images.githubusercontent.com/49276659/193325371-1c9f8877-50fb-46cb-9cab-e5eca6d94352.png)








