# shell Learn

## 单引号变量不识别特殊语法
# bash 学习
*** 
pstree 查看进程树
### 每次调用bash都会开启子shell，子shell的变量作用域作用不到父shell，如果要打印子shell里面的变量就先source x.sh 然受输出x.sh里面的变量。

- shell 变量通过环境变量确定登陆的用户名、PATH路径和文件系统等
- 环境变量可以临时创建，如果要永久更新就要修改配置文件

***
- 用户个人配置文件~/.bash_profile 、 ~/.bashrc 远程登录用户特有文件
- 全局配置文件 /etc/profile 、 /etc/bashrc ,且系统建议最好创建在 /etc/profile.d/,而非直接修改主文件，修改全局配置文件，影响素有登陆系统系统的用户

## 检查系统环境变量 （set **输出所有文件，包括全局变量、局部变量** ，env **只显示全局变量**，declare **输出所有变量**，export “显示和设置环境变量值” ）

先输出全局配置文件中的变量

## 撤销环境变量 
- unset 变量名，删除变量或者函数

```
## 设置只读变量 readonly 
readonly name = "gzh"
name = "chaochao"
-bash:name:只读变量
```
