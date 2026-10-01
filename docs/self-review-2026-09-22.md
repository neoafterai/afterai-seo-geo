# AfterAI SEO/GEO 0.1.1 self-review

用户要求：检查 bug、SEO/GEO 依据、各阶段详细计划，以及能否一步步带用户完成。

## 结论与范围

审查覆盖 13 个安装文件、任务路由、计划与记录模板、计分、语言、Shopify 和月检。0.1.0 有可用的专业工作框架，但新手引导与部分技术判断存在缺口；本轮已修改为 0.1.1 候选版。不能据文档检查宣称无 bug、所有行业均实测或取得官方认证。

SEO 有公开平台要求和建议；本项目没有证据支持一套跨平台统一的 GEO 排名规则。项目自定义分数、任务顺序及问题预算与官方技术条件明确分开。实施时仍要复核当前平台规则。

## 发现与处理

| 发现 | 影响 | 修复位置与结果 |
|---|---|---|
| 有阶段路线，无固定引导与完成条件 | 新手可能收到大量待办，却不知道下一步 | USAGE 的 Guided workflow 增加 0–9 阶段的输入、操作、交付和完成条件；入口要求采用 |
| 跳阶段只提示缺项 | “执行 GEO”可能停在缺计划，或跳过准备 | 入口和使用说明要求回到必要的最早前置步骤，区分阻断事实与可缺测数据 |
| 任务表缺实际操作细节 | “优化标题”不足以指导人工实施 | 每任务卡新增具体步骤、位置、执行者、工作量、预期结果、验证和失败路径 |
| canonical 存在被写成得分条件 | 无必要标签的网站可能被错误扣分 | S02/S03 改为先验证规范化／sitemap 需求及现有信号，不当作普遍索引门槛 |
| 单个 A/B 条件不适用未定义 | 不同执行者可能给出不同分数 | 仅一个条件适用时保留整项权重，按该条件给 1／0／未测；双 N/A 才移除，模板同步 |
| robots/noindex 等只列检查名 | 常见冲突缺执行分支 | SEO 文件增加访问、抓取、索引、重复 URL、语言版本和下架处理顺序 |
| AI 平台差异过于笼统 | 容易混淆搜索、训练和 grounding 控制 | GEO 文件增加 Google、ChatGPT、Gemini 及可选豆包／DeepSeek 的区别与未知处理 |
| 浏览器采集未明确平台允许条件 | 能操作不代表可以自动查询 | Google Search／AI Overview 默认人工采集，自动方式须有平台允许依据 |
| Shopify 失败恢复不够具体 | 写入后故障可能继续扩大批次 | 停止后续写入，记录状态；已批准且仍适用的恢复可执行，否则展示具体方案 |

## 官方依据核查

2026-09-22 直接读取以下官方文档。agent-reach 的 Jina 读取失败，mcporter 和 agent-reach 命令不可用，使用宿主联网工具作后备；没有安装依赖或调用付费 API。

- [Google AI features](https://developers.google.com/search/docs/appearance/ai-features)：用于核对 Search AI 资格及基础优化；没有特殊文件或标记保证展示。
- [noindex](https://developers.google.com/search/docs/crawling-indexing/block-indexing)：用于核对抓取限制与索引指令的关系。
- [Canonicalization](https://developers.google.com/search/docs/crawling-indexing/consolidate-duplicate-urls)、[Sitemaps](https://developers.google.com/search/docs/crawling-indexing/sitemaps/overview)、[Language versions](https://developers.google.com/search/docs/specialty/international/localized-versions)：用于核对适用性、信号一致性与多语引用。
- [Spam policies](https://developers.google.com/search/docs/essentials/spam-policies)：用于核对内容操纵与自动查询边界。
- [OpenAI crawlers](https://developers.openai.com/api/docs/bots)、[Google common crawlers](https://developers.google.com/crawling/docs/crawlers-fetchers/google-common-crawlers)：用于核对各平台访问控制，不能由它们推算排名。

## 验证

- 修改前独立代理读取全部 13 文件，模拟新手、跳过前置阶段及 Shopify 已授权写入三个场景。它能给出合理响应，但指出部分引导依赖模型自行补齐；同时发现条件级 N/A 歧义。未将模拟称为真实网站测试。
- 修改后本地标准库检查退出码 0：13 个 Markdown 文件、英文文件名、所有本地文件链接、入口引导锚点、无重复二级标题、表格列数、frontmatter、无机器绝对路径。
- 实际评分表权重和条件级 N/A 算术检查通过：示例适用 20、已检查 10、已得 10，得到已检查得分 100、覆盖 50%、区间 50–100。
- 官方 quick_validate 再次尝试失败：开发 Python 环境缺 PyYAML。未给产品增加依赖，未宣称官方验证通过。
- 修订后独立行为复测结果另附于评估记录；这类模拟不能证明真实宿主每次都会遵循指令。

## 剩余验证

下一步用授权的真实站点完成一次从初评到复评的试跑；现阶段没有真实抓取、线上变更、Shopify 集成、AI 推荐提升或定时运行的验收。评分口径变更到 0.1.1，历史分数须重算或标明不可比。安装包仍仅 13 个 Markdown 文件。
