# 思想社区介绍

## 1.作品主题及形式
我们希望创建一个平台，让大家畅所欲言，分享其所见所闻所想。所以我们开发这样一个**网站**，实现<u>发帖</u>、<u>浏览</u>、<u>回复</u>等功能；我们将它取名为 ***思想社区*** ，计划使用的logo[^1]:
![logo](https://github.com/404245452/homework_2.1/blob/master/logo.png)
[^1]:logo：计划使用艺术字加图片背景形式，背景未决定好，字体也可能变动。

## 2.网站具体内容策划
为使用户更方便的浏览自己需要的内容，我们大致将网站分为以下几个主题模块[^2]：
* 学习
* 科技
* 社会
* 历史

并且将热点文章[^3]以排行榜的形式展现，方便大家浏览网站热门话题。

[^2]:主题模块：前期划分，不代表最终内容。
[^3]:热点：暂定以点击数排行；

## 3.代码模块
本网站使用<b style="color:blue">*html*</b>、<b style="color:blue">*javascript*</b>、<b style="color:blue">*css*</b>、<b style="color:blue">*php*</b>编写，并且涉及数据库的设计及使用；  
具体实现以下几个方面：
1. 网站各个页面的编写：
   * ~~index页面~~网站首页
   * 账号注册、登录界面
   * 用户信息管理界面
   * 文章浏览界面
   * 文章编写界面
2. 数据库的创建及使用
   * 用户账号密码及其他信息数据库
   * 文章信息数据库
   * 评论回复数据库
3. 文件管理
   * 用户的头像等图片存储及使用
   * 文章中的图片、音乐、视频、其他文件的存储及使用

下面是数据库连接的代码样例:
```php
$conn=mysqli_connect($mysql_server_name,$mysql_username,$mysql_password,$mysql_database); //连接数据库，面向过程！！！

mysqli_query($conn,"set names utf8");//设为中文！！！

// 检测连接
if (!$conn) {
    die("连接SQL失败...");// mysqli_connect_error()
} 
```

## 4.其他说明
现在网络上有许多与本站性质类似的大型网站，如[百度贴吧](https://tieba.baidu.com/index.html)、[微博](https://weibo.com/)、[知乎](https://www.zhihu.com)，作为初学者，我们参考借鉴了其中的一些方面，比如*网页布局*、*色彩搭配*，这些对我们启发很大。





