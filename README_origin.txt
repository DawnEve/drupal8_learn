Drupal中文版（请参考docs/目录）

CONTENTS OF THIS FILE
---------------------

 * 关于About Drupal
 * 配置Configuration and features
 * 安装Installation profiles
 * 外观Appearance
 * 开发Developing for Drupal
 * 更多More information

ABOUT DRUPAL
------------

Drupal is an open source content management platform supporting a variety of
websites ranging from personal weblogs to large community-driven websites. For
more information, see the Drupal website at https://www.drupal.org, and join
the Drupal community at https://www.drupal.org/community.
支持从个人博客到大型社区驱动的网站。

法律信息Legal information about Drupal:
 * Know your rights when using Drupal:
   See LICENSE.txt in the "core" directory.
 * Learn about the Drupal trademark and logo policy:
   https://www.drupal.com/trademark

配置CONFIGURATION AND FEATURES
--------------------------

Drupal core (what you get when you download and extract a drupal-x.y.tar.gz or
drupal-x.y.zip file from https://www.drupal.org/project/drupal) has what you
need to get started with your website. It includes several modules (extensions
that add functionality) for common website features, such as managing content,
user accounts, image uploading, and search. Core comes with many options that
allow site-specific configuration. In addition to the core modules, there are
thousands of contributed modules (for functionality not included with Drupal
core) available for download.
Drupal核心包含若干网站常用module，比如内容管理，用户账号，图像上传，以及搜索。
核心高度可配置。除了核心，还有开发者贡献的成千上万的模块可以下载。

More about configuration:
 * 安装、升级、维护Install, update, and maintain Drupal:
   See INSTALL.txt and UPDATE.txt in the "core" directory.
 * 如何建站Learn about how to use Drupal to create your site:
   https://www.drupal.org/documentation
 * 最佳实践Follow best practices:
   https://www.drupal.org/best-practices
 * 下载module来扩展功能 Download contributed modules to /modules to extend Drupal's functionality:
   https://www.drupal.org/project/modules
 * See also: "Developing for Drupal" for writing your own modules, below.


INSTALLATION PROFILES安装
---------------------

Installation profiles define additional steps (such as enabling modules,
defining content types, etc.) that run after the base installation provided
by core when Drupal is first installed. There are two basic installation
profiles provided with Drupal core.

Installation profiles from the Drupal community modify the installation process
to provide a website for a specific use case, such as a CMS for media
publishers, a web-based project tracking tool, or a full-fledged CRM for
non-profit organizations raising money and accepting donations. They can be
distributed as bare installation profiles or as "distributions". Distributions
include Drupal core, the installation profile, and all other required
extensions, such as contributed and custom modules, themes, and third-party
libraries. Bare installation profiles require you to download Drupal Core and
the required extensions separately; place the downloaded profile in the
/profiles directory before you start the installation process.
社区版修改后可以用于：媒体发布的CMS，基于web的项目跟踪工具，非盈利组织筹资的成熟的CRM。
模块modules、主题theme、第三方库lib。/profiles文件夹。

More about installation profiles and distributions:
 * profile和发行版的区别 Read about the difference between installation profiles and distributions:
   https://www.drupal.org/node/1089736
 * 下载profile和发行 Download contributed installation profiles and distributions:
   https://www.drupal.org/project/distributions
 * 开发自己的profile或者发行 Develop your own installation profile or distribution:
   https://www.drupal.org/developing/distributions


APPEARANCE外观
----------

In Drupal, the appearance of your site is set by the theme (themes are
extensions that set fonts, colors, and layout). Drupal core comes with several
themes. More themes are available for download, and you can also create your own
custom theme.
主题是设置的字体、颜色、布局，决定外观。
Drupal核心提供几套主题，也可下载，也可自定义。

More about themes:
 * 下载 Download contributed themes to /themes to modify Drupal's appearance:
   https://www.drupal.org/project/themes
 * 开发主题 Develop your own theme:
   https://www.drupal.org/documentation/theme

DEVELOPING FOR DRUPAL开发
---------------------

Drupal contains an extensive API that allows you to add to and modify the
functionality of your site. The API consists of "hooks", which allow modules to
react to system events and customize Drupal's behavior, and functions that
standardize common operations such as database queries and form generation. The
flexible hook architecture means that you should never need to directly modify
the files that come with Drupal core to achieve the functionality you want;
instead, functionality modifications take the form of modules.
有很多扩展API。由钩子组成，让module相应事件以及自定义Drupal行为，影响标准操作比如数据库查询，表单生成。
灵活的钩子，意味着你用不着直接修改核心代码，就能实现功能。相反，功能修改表现为module。

When you need new functionality for your Drupal site, search for existing
contributed modules. If you find a module that matches except for a bug or an
additional needed feature, change the module and contribute your improvements
back to the project in the form of a "patch". Create new custom modules only
when nothing existing comes close to what you need.
当你需要新功能，先搜索已有module。

More about developing:
 * 搜索已知模块 Search for existing contributed modules:
   https://www.drupal.org/project/modules
 * 贡献补丁 Contribute a patch:
   https://www.drupal.org/patch/submit
 * 开发自己的模块 Develop your own module:
   https://www.drupal.org/developing/modules
 * 最佳实践 Follow programming best practices:
   https://www.drupal.org/developing/best-practices
 * API文档 Refer to the API documentation:
   https://api.drupal.org/api/drupal/8
 * 从例子学习API | Learn from documented Drupal API examples:
   https://www.drupal.org/project/examples

MORE INFORMATION更多
----------------

 * 在线文档 See the Drupal.org online documentation:
   https://www.drupal.org/documentation

 * 安全问题 For a list of security announcements, see the "Security advisories" page at
   https://www.drupal.org/security (available as an RSS feed). This page also
   describes how to subscribe to these announcements via email.

 * 安全继承 For information about the Drupal security process, or to find out how to
   report a potential security issue to the Drupal security team, see the
   "Security team" page at https://www.drupal.org/security-team

 * 支持信息 For information about the wide range of available support options, visit
   https://www.drupal.org and click on Community and Support in the top or
   bottom navigation.

   
更多在线文档翻译
----------------

 * 请查看docs/目录。
   