# Obsidian Link Opener

粘贴任意文本 → 自动提取其中的 Obsidian 链接 → 点击直达 Obsidian。

解决手机上"想打开一条 Obsidian 链接，但一复制就带出一堆无关文字"的问题。

## 功能

- 识别完整 `obsidian://open?vault=…&file=…` URI
- 识别 `[[笔记名]]` / `[[笔记名|别名]]` wiki 双链（用默认 vault 打开，在 index.html 顶部改 `DEFAULT_VAULT`）
- 一键「粘贴并提取」（需浏览器剪贴板权限；失败时手动粘贴再点提取）
- URL 参数直跳：`?u=<urlencoded obsidian uri>`，可配合 iOS 快捷指令做分享菜单入口

## 部署

纯静态单文件，任何静态托管都能跑。Vercel：import 仓库 → Framework Preset 选 Other → 部署即可。

## License

MIT
