# IP 全案 Codex 插件市场

插件：`ip-quanan-skil1`，版本 `1.0.0`。

## 安装

在支持插件的 Codex CLI 中执行：

```sh
codex plugin marketplace add THISLOOP/LIU-YUMO- --ref main
codex plugin add ip-quanan-skil1@ip-quanan-marketplace
codex plugin list --json
```

安装后在新的 Codex 会话中使用 `ip-quanan-skil1`，请求品牌 IP 全案策划或视觉资产制作。

本插件市场通过 GitHub 分发，不代表已上架官方插件目录。

## 内容

- `.agents/plugins/marketplace.json`：市场清单。
- `plugins/ip-quanan-skil1/.codex-plugin/plugin.json`：插件清单。
- `plugins/ip-quanan-skil1/skills/ip-quanan-skil1/SKILL.md`：完整 skill。

SKILL.md 与用户附件正文一致，仅按用户要求将 frontmatter 名称改为 `ip-quanan-skil1`。图片生成仍需所用 Codex 环境支持相应能力。
