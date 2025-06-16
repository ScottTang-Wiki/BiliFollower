# BiliFollower

一个用于显示 B 站用户粉丝数量的 MediaWiki 扩展。

## 📦 安装方法

1. 将本仓库克隆到你的 MediaWiki `extensions/` 目录下：

   ```bash
   git clone https://github.com/YourUsername/BiliFollower.git
   ```

2. 在 `LocalSettings.php` 中启用扩展：

   ```php
   wfLoadExtension( 'BiliFollower' );
   ```

## 📘 用法

将 `YourUID` 替换为 B 站的 UID。

```wikitext
{{#bili_fan:YourUID}}          → 当前粉丝数  
{{#bili_fan_percent:YourUID}}  → 距百万粉丝的百分比  
{{#bili_fan_remain:YourUID}}   → 距离百万还需粉丝数
```

## 🧩 解析函数一览

| 函数                             | 说明                  |
|----------------------------------|-----------------------|
| `{{#bili_fan:UID}}`              | 返回粉丝数            |
| `{{#bili_fan_percent:UID}}`      | 返回百分比进度        |
| `{{#bili_fan_remain:UID}}`       | 返回剩余粉丝数量      |

## 📄 许可证

本扩展遵循 GNU 通用公共许可证第 2 版或更高版本。详见 [LICENSE](./LICENSE)。
