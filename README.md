# agent-build

这个仓库集中存放各种 agent 配置，按目录取用。

会收录的内容包括：

- Grok Bot 各机器配置
- OpenCode 配置
- Cursor / marketplace skill packs

## 浏览

根目录 [`catalog.json`](./catalog.json) 是索引。`configs` 数组里每一项至少有：

| 字段 | 含义 |
| --- | --- |
| `name` | 配置名 |
| `folder` | 相对仓库根目录的路径 |
| `description` | 这份配置做什么 |
| `agents` | 可以使用它的 agent |

部分条目还会带 `version` 和 `license`。

## 已收录

### pstack

[`configs/pstack`](./configs/pstack) 是 Lauren Tan 的 Cursor marketplace 插件 **pstack v0.15.48** 的 MIT 原样副本：59 个 skill，以及 `plugin.json`、docs、agents、automations、assets、`LICENSE`。同目录的 `NOTICE.md` 是本仓库额外的来源说明，不属于上游目录。

上游固定版本：<https://github.com/cursor/plugins/tree/ca782ed8b3c2c521cead8e1720d55c3a5dbf2347/pstack>（commit `ca782ed8b3c2c521cead8e1720d55c3a5dbf2347`，tree `971573532de6714a4ddff8ec39b52d021ebf161a`）。该快照已包含 pstack 最近变更 `9e278fe4d4ecd8bfe98b1b79bf4be662efb338cc`。

这套配置是可并行的严谨 agent 工作流，用来写出更少、但质量更高的代码。Cursor、Grok Bot 这类能加载 skill 的 coding agent 可以直接用。
