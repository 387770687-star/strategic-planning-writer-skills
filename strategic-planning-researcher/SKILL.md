---
name: strategic-planning-researcher
description: Research, verify, structure, and synthesize evidence for Chinese strategic planning reports. Use when the user needs policy research, company background, market data, project evidence, fact packs, or research notes before drafting a 20,000+ character strategic planning report.
---

# Strategic Planning Researcher

Prepare the evidence base for strategic planning reports. Run this before `strategic-planning-writer` when the report depends on current policy, company facts, market data, project lists, investment numbers, or regional conditions.

## Goal

Produce a fact pack that a strategy writer can use without inventing data. Separate confirmed facts, user-provided facts, forecasts, assumptions, and data gaps clearly.

## Workflow

### 1. Define Research Scope

Specify: planning topic, period and target year, region/business line, required report sections, key decisions to support.

### 2. Inventory Available Materials

按以下优先级检索可用材料，**禁止跳步**：

**第一优先级 — `wiki/` 目录**：
- wiki/ 是整理后的结构化知识，优先检索
- 搜索关键词匹配的 wiki 页面，直接提取相关信息

**第二优先级 — `raw/` 目录**：
- 仅当 wiki/ 中信息不足时检索 raw/
- raw/ 存放原始资料（政策文件、报告原文、数据表格等），只读
- 搜索到的原始材料需要提取和归纳后使用

**第三优先级 — WebSearch 官方网站检索**：
- 仅当 wiki/ 和 raw/ 均无法满足需求时启动
- 限定官方网站：政府 .gov.cn、部委网站、央企官网、国家统计局、IEA 等
- 检索结果标注来源 URL

Catalog: 用户提供的文件、内部笔记、wiki/raw 知识库材料、官方网站检索结果、以及缺失数据。使用 `references/source-map.md` 匹配主题到合适的来源。

### 3. Build an Evidence Table

For each fact, record: fact statement, source, date/year, statistical scope, unit, confidence level, and intended report section.

Confidence labels:
- **Confirmed** — verified from authoritative source
- **知识库** — data retrieved from the uploaded knowledge base
- **WebSearch 检索补充** — data found via official website search, with URL recorded
- **User-provided, pending final 口径** — user data awaiting formal approval
- **Forecast** — projection with stated assumptions
- **Assumption** — working assumption for planning purposes
- **Pending verification** — requires further confirmation;知识库和官方网站均未找到

### 4. Synthesize into Planning Implications

For each piece of evidence, derive:
- What the fact means
- How it affects the enterprise
- What planning response it supports

Convert policy and data into implications; do not just summarize sources.

### 5. Return the Fact Pack

Use `references/evidence-pack-template.md` for formatting.

### 6. Flag Data Gaps

列出缺失数据、为何重要、所需来源以及临时处理方式。

**数据缺口处理流程**：

1. **先检索知识库**：检查已上传的知识库中是否有相关数据
2. **其次 WebSearch 检索官方网站**：按 .gov.cn → 央企官网 → IEA 等国际组织官网 优先级检索
3. **检索到则直接使用**：将数据纳入事实包，标注来源和检索 URL
4. **检索不到再留空**：仅当知识库和官方网站均无法找到时，标记为待补充

缺失数据清单中，每条标注"已尝试检索知识库和官方网站"或"尚未检索"。

## Output Format

1. Research scope
2. Executive findings (5-8 findings, each with evidence and implication)
3. Evidence table（每条标注来源类型：知识库 / WebSearch检索 / 用户提供）
4. Policy and market implications
5. Company/business implications
6. Data gaps and questions for the user（标注是否已尝试知识库检索和 WebSearch 官方网站检索）
7. Suggested wording reusable in the final report（含 【1】【2】【3】 引用标注建议）

## Rules

- Do not write a full report unless the user explicitly asks.
- Do not invent facts to fill gaps.
- Prefer official Chinese public sources for policy and company facts.
- Mark every uncertain fact as pending verification.
- Convert every policy and data point into an implication; do not just summarize sources.

**数据缺失时的检索优先规则**（重要）：

- 第一优先：检索已上传的知识库 `wiki/` 目录（整理后的结构化知识）
- 第二优先：检索 `raw/` 目录（原始资料，只读）
- 第三优先：通过 WebSearch 检索官方网站补充（政府网站 .gov.cn、部委网站、央企官网、国家统计局、IEA等国际组织官网）
- 检索到的数据必须交叉验证，单源数据标注"单一来源，未经交叉验证"
- 仅当 wiki/、raw/ 和官方网站均无法找到时，才标记为 `==[待补充：...]==`
- **禁止跳步**：不得跳过 wiki/ 和 raw/ 直接使用 WebSearch

**时效性校验规则**（重要）：

知识库中的旧数据可能已过时。即使 wiki/raw 中已有数据，也必须进行时效性校验：

- **校验对象**：统计数据（超过2年）、政策文件（超过5年或有修订可能）、市场数据、行业指标
- **校验方法**：用关键数据词在官方网站（.gov.cn、央企官网、国家统计局等）搜索最新年份的对应数据
- **校验通过**：标注"来源：知识库，经官网校验"
- **数据已更新**：以官方最新数据为准，替换旧数据，标注"来源：知识库，已更新至 XX 年官方数据"
- **无法校验**：标注"知识库数据，时效性未经官方校验"

**数据来源限制**：

- 禁止从非官方新闻网站获取数据。以下类网站不得作为数据来源：腾讯新闻、新浪新闻、网易新闻、搜狐新闻、今日头条、百家号、微信公众号、知乎、以及其他商业门户网站和自媒体平台。政策解读和数据报道应追溯到原始出处使用。
- 搜索引擎返回的非官方来源（如商业新闻、自媒体文章）仅可用于发现原始出处的线索，不得直接引用其中的数据或判断。

## References

- `references/source-map.md` — source priorities and topic-source matching
- `references/evidence-pack-template.md` — deliverable format template
