# test/ · 上传链路设计用测试样本

- **仅为 fixtures**：用于开发 agent 定义上传路径、上传要求与 `submission.schema`，**不是正式生产发布**。
- 公开放置已获 Jiang 于 2026-10-23 确认。
- 不含任何密钥、token、cookie、`.env` 或私有路径。
- 采集方为外部（Grok Bot / X趋势助手）；本仓库**不在 CI 中抓取 X**，也不在 Actions 中调用 AI。

目录：
- `X-CAPABILITIES.md`：X 采集能力清单（可更新）
- `upload-notes.md`：当前非正式提交形态与未来 schema 的差距
- `accounts/`：账号清单 CSV（14 列）、handle 列表、变更摘要、头像（`avatars/<handle>.jpg`）
- `samples/2026-10-22/`、`samples/2026-10-23/`：原始 API 分片 `raw/`、`trends.json`、渲染后的 `ai-daily.md/html`
- `MANIFEST.md`：文件数与体积
