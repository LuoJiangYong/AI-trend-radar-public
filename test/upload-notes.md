# 上传说明（给开发 agent）

## 当前非正式流程
X趋势助手（Grok Bot）在其工作区调用 X 公开接口 → 将响应原样存为 `raw/<日期>/pNN.txt` → 人工/脚本提炼 `trends-<日期>.json` → 模板渲染 `ai-daily-<日期>.html/.md`。无批次 ID、无 schema、无校验，靠人工交付。

## 目标流程
外部采集器生成提交包 → 向生产仓开 PR → CI（schema 校验、重复批次识别、路径约束，不联网抓取）→ Jiang 批准后合并 → 后续阶段再单向发布到公开仓。

## 样本 → 未来 schema 对应
| 样本文件 | 未来对应 |
| --- | --- |
| `samples/*/raw/pNN.txt` | `submission.schema` 的条目原始载荷（转换为 `item.schema`） |
| `samples/2026-10-22/raw/users-check.json` | 账号核验/作者补全的附带数据 |
| `samples/*/trends.json` | 下游报告的中间产物（P3），非原始提交 |
| `samples/*/ai-daily.md/html` | 渲染产品（P3 输出参考），**不是原始提交** |
| `accounts/*.csv` + `avatars/` | 来源配置/作者元数据 + 本地素材清单 |

## 注意
- raw 文本可能较大，也可能是部分结果（分页未取全、空响应 `result_count:0`）；不要假设完整。
- 缺失字段需显式保留缺失，不得补 0。
- 当前时间为 UTC（`created_at` 以 Z 结尾），报告按 Asia/Shanghai 呈现，契约需明确两者。
- 缺：外部批次 ID、采集器 ID、覆盖窗口、缺失说明、素材哈希——均需在 schema 中补齐。
