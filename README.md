# 说明

_此项目只是用来熟悉gin和xorm，所以如果出现使用错误或者其他错误，还请提issue说明，看到我会及时回复！_

## 功能

由于本人前端技术比较菜，所以本项目中的模板页面是从开源项目 [Guns](https://gitee.com/naan1993/guns) 中抽离的，Guns 是个Java项目，模板引擎使用的是 `beetl` ，gin是无法渲染的，所以将 `beetl` 页面改成了HTML页面，中间难免有错误还请见谅！

本项目用到的技术栈：`gin`, `xorm`, `xormplus`，数据库是MySQL。

主要功能也是参考 Guns 项目，当然没有那么丰富，包括用户登录，用户角色管理，权限分配，部门管理等等

## 启动

> 默认登录用户名和密码： `admin/111111`, `boss/111111`

1、将sql目录下的gin.sql在MySQL中执行

2、直接执行 `main.go` 启动项目，main函数中定义了默认的端口3000，可以按照需求自己改

3、如果执行了 `go install` ，也可以通过二进制执行 `./gin-xorm-admin` , 可以在后面跟上参数 `--port` 可以修改默认端口
