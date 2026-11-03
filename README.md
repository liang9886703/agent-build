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

[`configs/pstack`](./configs/pstack) 是 Lauren Tan 的 Cursor marketplace 插件 **pstack v0.15.36** 的 MIT 原样副本：58 个 skill，以及 `plugin.json`、docs、agents、automations、assets、`LICENSE`、`NOTICE.md`。

上游：<https://github.com/cursor/plugins/tree/main/pstack>

这套配置是可并行的严谨 agent 工作流，用来写出更少、但质量更高的代码。Cursor、Grok Bot 这类能加载 skill 的 coding agent 可以直接用。
