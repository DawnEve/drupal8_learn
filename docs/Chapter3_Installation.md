# chapter 3

安装所需服务器配置和运行核心软件。
https://www.drupal.org/docs/user_guide/en/install-tools.html




## 3.1. 概念: 服务器必须标准
 - 硬盘：至少15M。如果有很多模块和主题需要60M。数据库、用户上传文件、媒体、备份等需要更多空间。
 - web服务器：
   - Apache(推荐)需要开启mod_rewrite模块。
   - Nginx是常用的高并发、高性能、低内存web服务器，必须安装和开启ngx_http_rewrite_module模块。
   - Hiawatha 是很注重安全的web服务器。也注意易用和轻量级。独立研究人员证实Hiawatha在常规条件下提供了与其他服务器类似的性能，但是遭到攻击时性能要好很多。必须安装URL Toolkit，设置重写URL。
   - Microsoft IIS 是Microsoft Windows下一个web服务器及一套扩展模块。如果php配置正确，核心程序可以工作在IIS 5, IIS 6, 或者 IIS 7下。如果需要干净的URL，就需要第三方产品了。IIS 7需要Microsoft URL Rewrite module或者第三方解决方案。
 - 数据库：使用下列数据库
   - MySQL - 5.5.3 (MariaDB 5.5.20, Percona 5.5.8) 或者更高版本，带innoDB兼容的主存储引擎。
   - PostgreSQL - 9.1.2 或更高版本。
   - SQLite - 3.4.2或更高版本。
 - PHP 5.5.9 或更高版本。




## 3.2. 概念: 额外工具

建站所需工具
1. Drush 见下文。
2. git 版本控制工具。已经成为标准网站开发工具。
3.devel Devel模块协助完成排错、检查代码、分析数据库查询、产生dummy内容等开发任务。

### Drush的特别之处

Drush是一个命令行工具，建立、维护站点用，在使用管理员界面做操作之外提供了另一个选择。很多建站或者维护者如果可能，都用Drush，并认为安装和学习Drush所花的时间是值得的。使用Drush的理由：
   - Drush提供了很多命令，用于安装基础软件、模块、主题；升级软件；做数据库操作，包括复制、查询；重设密码；清理缓存。一些第三方模块和主题页顶一楼Drush命令。
   - 使用Drush做管理任务更快、更简练。
   - 因为Drush是一个命令行界面，你可以使用Drush命令以及其他服务器命令写脚本，自动做更多复杂任务。
   - Drush提供了管理界面做不了的功能；比如，运行数据库查询。

如果想使用Drush，你需要有网站所在服务器的终端访问权限，并在该服务器上安装了兼容的Drush工具。查看[Drush website](http://www.drush.org/)获得安装建议和版本兼容信息，以及Drush命令文档。




### 模块和主题开发者需要什么工具？

除了以上提到的建站工具，以下工具对于开发模块和主题也很有用。

#### Drupal 控制台
 [Drupal 控制台](https://drupalconsole.com/)是一个命令行工具，用于产生样板代码，以及与Drupal站点交互。它可以产生块、表单代码，安装模块和主题，创建虚构内容。Drupal控制台使用了Symfony控制台。

#### Coder
[Coder](https://www.drupal.org/project/coder)是一个命令行工具，用于检查模块和主题是否符合编码标准以及其他最佳实践。它也可以修正不符合编码标准的部分。

#### Firebug
firebug是火狐插件，Drupal的[Firebug module](https://www.drupal.org/project/drupalforfirebug)可以再Firebug窗口中展示debug和SQL查询的信息。




## 3.3. 准备安装

目标：选择合适的方法安装核心程序，解决必须的前提。

如果想使用Drush安装核心软件，必须先安装Drush。

### 步骤
1 选择一个方法安装核心软件。
 - 尝试一个免费在线demo（20分钟内安装）
 - 使用你的网络供应商的一键安装包
 - 使用Drush
 - 使用web installer手工安装。

2 如果使用Drush或者web installer安装，设置URL和网站站点，或者在外部服务商或者你自己的电脑上。在网站根目录root目录放一个简单的HTML文件，确定服务器正常，访问你站点的URL。

3 如果安装Drush或者web install，创建数据库，包含一个全部权限的数据库用户账号。

4 如果使用Drush安装，在Drush命令行输入如下命令，这个例子中example 是核心软件下载的目录名字，DB_NAME, DB_USER and DB_PASS 是数据库的认证信息:
```
  drush dl drupal --drupal-project-rename=example
  cd example
  drush site-install standard --db-url='mysql://DB_USER:DB_PASS@localhost/DB_NAME' --site- name=example
```

5 如果使用web installer安装，手工上传核心软件文件。你需要：
  1. 到 https://www.drupal.org ，点击等不 下载与扩展 菜单；
  2. 点击 下载Drupal 按钮；
  3. 选择推荐版本，点击下载；
  4. 下载tar.gz或者zip文件到本地的web root目录；
  5. 上传下载的文件到服务器上。登录控制面板，导航到HTML目录。保存Drupal文件到同等级新文件夹中；
  6. 解压缩。



### 加深理解

如果选择web installer来安装核心软件，运行installer。





## 3.4. 运行安装器









------
