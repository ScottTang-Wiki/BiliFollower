# BiliFollower

👥 A MediaWiki extension that displays follower stats for Bilibili users.

👥 一个用于显示 B 站用户粉丝数量的 MediaWiki 扩展。

---------

## 📦 Installation 安装方法

1. Clone this repository into your MediaWiki `extensions/` folder:

   将本仓库克隆到你的 MediaWiki `extensions/` 目录下：

   ```bash
   git clone https://github.com/YourUsername/BiliFollower.git


Enable the extension in your LocalSettings.php:
在 LocalSettings.php 中启用扩展：
wfLoadExtension( 'BiliFollower' );

---------

📘 Usage 用法
Replace YourUID with a valid Bilibili user ID.
将 YourUID 替换为你想查询的 B 站 UID。

Current follower count: {{#bili_fan:YourUID}}
当前粉丝数：{{#bili_fan:YourUID}}

Bilibili follower progress: {{#bili_fan_percent:YourUID}}% ({{#bili_fan:YourUID}} / 1,000,000)
B站粉丝进度：{{#bili_fan_percent:YourUID}}% ({{#bili_fan:YourUID}}/1,000,000) 

Remaining to 1 million: {{#bili_fan_remain:YourUID}}
距离100万还需：{{#bili_fan_remain:YourUID}}

---------

🧩 Parser Functions 解析器函数一览
      Function	                      Description	                   说明
{{#bili_fan:UID}}	              Returns follower count	        返回粉丝数
{{#bili_fan_percent:UID}}	      Progress toward 1 million	      距百万粉丝的百分比
{{#bili_fan_remain:UID}}	      Remaining to 1 million	        距离百万粉丝的差值

---------

📄 License 许可证
GPL-2.0-or-later
本扩展遵循 GNU 通用公共许可证第 2 版或更高版本。
See LICENSE for details.
