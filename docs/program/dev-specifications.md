## 命名规范
请理解并尽量遵循以下命名规范，可以减少在开发过程中出现不必要的错误。

ThinkPHP6.0 遵循`PSR-2`命名规范和`PSR-4`自动加载规范，并且注意如下规范：

### 目录和文件
目录使用小写+下划线；

### 类库、函数文件统一以.php为后缀；
类的文件名均以命名空间定义，并且命名空间的路径和类库文件所在路径一致；
类（包含接口和Trait）文件采用驼峰法命名（首字母大写），其它文件采用小写+下划线命名；
类名（包括接口和Trait）和文件名保持一致，统一采用驼峰法命名（首字母大写）；

### 函数和类、属性命名
类的命名采用驼峰法（首字母大写），例如 User、UserType；
函数的命名使用小写字母和下划线（小写字母开头）的方式，例如 get_client_ip；
方法的命名使用驼峰法（首字母小写），例如 `getUserName`；
属性的命名使用驼峰法（首字母小写），例如 `tableName`、`instance`；
特例：以双下划线__打头的函数或方法作为魔术方法，例如 `__call` 和 `__autoload`；

### 常量和配置
常量以大写字母和下划线命名，例如 `APP_PATH`；
配置参数以小写字母和下划线命名，例如 `url_route_on` 和 `url_convert`；
环境变量定义使用大写字母和下划线命名，例如 `APP_DEBUG`；

### 数据表和字段
数据表和字段采用小写加下划线方式命名，并注意字段名不要以下划线开头，例如 `think_user` 表和 `user_name` 字段，不建议使用驼峰和中文作为数据表及字段命名。