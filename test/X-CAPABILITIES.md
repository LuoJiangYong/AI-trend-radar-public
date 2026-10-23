# X 采集能力清单

> 版本日期：2026-10-23（Asia/Shanghai）。工具或限额变化时更新本文件。
> 来源：Grok Bot 内置公开 X 只读工具 + 用户已连接的 X 插件。仅列已知存在的工具，不臆造。

## 1. 内置公开读取（命名空间 `x`，无需用户 X 登录）

| 类别 | 工具 |
| --- | --- |
| 用户 | `get_users_by_username`、`get_users_by_usernames`（每次 ≤25）、`get_users_by_id`（`search_users` 仅在指南列出时可用） |
| 帖子 | `get_posts_by_id`、`get_posts_by_ids`、`get_users_posts`、`get_users_mentions`、`search_posts_all`、`get_posts_counts_recent`、引用/转发查询 |
| 新闻/趋势 | `search_news`、`get_news`、`get_trends_by_woeid` |

**限额**：30 次/分钟、1000 次/天/用户、每次 ≤25 条结果；窗口在整点 :00 与 UTC 00:00 重置。

**常用字段**
- `user.fields`：`id,name,username,description,public_metrics,profile_image_url,created_at`
- `tweet.fields`：`created_at,public_metrics,author_id,lang,conversation_id`
- `expansions`：`author_id,referenced_tweets.id`

## 2. 用户连接的 X 插件（`user-X`，账号范围）

- 本人资料、主页时间线、本人帖子、提及、书签
- Lists 读写、Spaces、社区搜索
- X Chat / 通话 / 直播能力存在，但**不在 AI-trend-radar 采集范围内**

## 3. 采集器当前产出

- 账号清单 CSV（14 列，含 `头像URL`、`本地头像路径`）
- 每日原始 API 文本分片（`p01.txt`…，标准 `data` + `includes`）
- `trends-YYYY-MM-DD.json`（`lead` + `trends[{t,d,refs}]`）
- 渲染后的 ai-daily HTML + MD（摘要 + 原始汇总）
- 本地头像文件（`following/avatars/`）

## 4. 不做 / 边界

- 采集时不代 Jiang 关注、取关或发帖
- 雷达仓库中不放 API key；Actions 不抓取 X、不调用 AI
- 工具**无法列出关注者/正在关注成员**，只能拿到 `public_metrics` 中的计数（关注清单靠截图人工提供）
- 已封禁/不存在的账号会 404（例：`@intern_lm`）
- 受限额约束，单日全量补抓 200+ 账号时帖子需分批

## 5. 建议的上传契约挂钩（仅供开发 agent 参考）

- 外部批次 ID、采集器 ID、覆盖时间窗（Asia/Shanghai）、缺失说明
- 区分 source（X）与 collector（Grok Bot / X趋势助手）
- 头像 = 本地文件路径 + 原始 URL
- 保留缺失字段，**绝不用 0 填充**
