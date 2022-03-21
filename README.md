# Steal Bomb

> 这是一个用Java语言写的轰炸盗号网站软件

## 启动软件

- 在终端执行 `java -jar stealbomb.jar` 即可使用()shiy
- 输出将显示在**控制台**上

### 启动参数

支持一个启动参数

| 参数 | 说明 | 例子 |
| --- | --- | --- |
| -Dfile= | 自定义文本文件名称(位置) | java -Dfile=../example.txt -jar steal.jar|

## 文本编写

> 默认使用同一文件夹下的文本文件 default.txt(需自行下载: <https://cdn.jsdelivr.net/gh/ObcbO/stealbomb/default.txt>)

一行只能有 `参数` 和 `参数值` ， 中间使用**空格**隔开(一行只允许一个空格)

不允许空行

| 参数 | 必填 | 默认值 | 说明 |
| --- | --- | --- | --- |
| 线程数 | 否 | 1 | 并行攻击的线程数量 |
| 请求方法 | 否 | POST | 支持所有的HTTP请求方法 |
| 攻击网址 | 是 | - | 发送账号密码的网址 |
| 参数 | 是 | - | 向网站发送的参数(支持变量) |

### 变量

目前支持两个变量

| 变量名 | 用途 |
| --- | --- |
| $[account] | 随机生成手机号,QQ号,QQ邮箱 |
| $[password] | 随机生成密码 |

## TODO

- [ ] 支持多个URL同时攻击
- [ ] 添加GUI
