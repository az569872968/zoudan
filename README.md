# Larval 5.2 后台实例

## 说明

基于laravel 5.2 与 zizaco/entrust 权限管理
开箱即用的后台模板.面包线,菜单栏都是基于权限来生成
集成了laravel-debugbar 超好用调试工具
带有日志解析查看模块


## 安装

- git clone 到本地
- 执行 `composer install` (如果出现数据库方面的错误提示,请将 database/seeds/rbac.sql 先导入你创建的数据库)
- 配置 **.env** 中数据库连接信息,没有.env请复制.env.example命名为.env
- 执行 `php artisan key:generate`
- 执行 `php artisan db:seed`
- 执行 `php artisan serve`
- 键入 'localhost:8000/admin'
- 默认后台账号:admin@admin.com 密码:admin


## 使用
- 用户管理中的权限管理添加顶级权限
   比如用户管理, 'admin.user' 只有两段的做左边的菜单栏, 列表页统一为'admin.XXXX.index'

   