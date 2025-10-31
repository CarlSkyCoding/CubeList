```markdown
# CubeList 🎯

一个支持在线 JSON 文件的白名单控制器

## ✨ 特性

- 📡 支持远程 JSON 白名单配置
- ⚡ 实时重载白名单数据
- 🎮 多服务器支持
- 🔄 简单易用的配置

## 📁 配置文件

在 `cubelist/config.yml` 中配置：

```yaml
URL: 'https://verify-teb.bwumc.cn/whitelist.json'
ServiceName: 'TheEntityByte'
Quest: 'mao0705/Charlotte169'
```

### 配置说明

| 字段 | 说明 | 示例 |
|------|------|------|
| `URL` | 白名单 JSON 数据地址 | `https://verify-teb.bwumc.cn/whitelist.json` |
| `ServiceName` | 服务器标识名称 | `TheEntityByte` |
| `Quest` | 问询者标识 | `mao0705/Charlotte169` |

## 🔄 重载命令

使用 `cbreload` 命令重新从 URL 获取白名单数据：

```bash
/cbreload
```

> **注意**: 目前重载不会重新读取 config.yml 中的 URL 配置，仅重新获取当前 URL 的白名单数据。

## 🚀 快速开始

1. 将插件放入 Velocity 的 plugins 文件夹
2. 重启服务器
3. 编辑 `cubelist/config.yml` 配置你的白名单源
4. 使用 `/cbreload` 加载白名单

## 📄 JSON 格式要求

你的在线 JSON 文件应该包含玩家白名单数据，例如：

```json
[
  "player1",
  "player2",
  "player3"
]
```

---

⭐ 如果这个插件对你有帮助，请给我们一个 Star！
```
