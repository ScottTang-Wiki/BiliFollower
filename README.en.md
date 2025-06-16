# BiliFollower

A MediaWiki extension that displays follower stats for Bilibili users.

## 📦 Installation

1. Clone this repository into your `extensions/` folder:

   ```bash
   git clone https://github.com/YourUsername/BiliFollower.git
   ```

2. Enable the extension in `LocalSettings.php`:

   ```php
   wfLoadExtension( 'BiliFollower' );
   ```

## 📘 Usage

Replace `YourUID` with a Bilibili user ID.

```wikitext
{{#bili_fan:YourUID}}          → Current follower count  
{{#bili_fan_percent:YourUID}}  → Progress toward 1 million  
{{#bili_fan_remain:YourUID}}   → Remaining to 1 million
```

## 🧩 Parser Functions

| Function                      | Description                  |
|------------------------------|------------------------------|
| `{{#bili_fan:UID}}`          | Returns follower count       |
| `{{#bili_fan_percent:UID}}`  | Percent toward 1M followers  |
| `{{#bili_fan_remain:UID}}`   | Followers needed to hit 1M   |

## 📄 License

GPL-2.0-or-later. See [LICENSE](./LICENSE).
