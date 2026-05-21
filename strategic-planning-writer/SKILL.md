---
name: strategic-planning-writer
description: Draft, expand, revise, or finalize Chinese strategic planning reports for large state-owned energy infrastructure enterprises. Use when the user needs a 20,000+ Chinese character strategic plan, five-year plan, business plan, regional infrastructure plan, new energy plan, or formal SOE planning document with evidence, policy alignment, and delivery-quality review.
---

# Strategic Planning Writer

Write formal Chinese strategic planning reports for central SOE strategy departments. Default output standard: at least 20,000 Chinese characters for full reports unless a shorter brief is explicitly requested. 在满足最低字数要求的基础上，能多写就多写、能写详细就写详细，不以任何上限为约束。宁可字数超标后由用户自行删减，不可因顾虑篇幅而牺牲论证深度。

## Operating Stance

Write as a strategy department professional drafting for senior decision makers. The report must be policy-aligned, evidence-based, operationally grounded, and usable for internal review.

Core audience: 国家管网集团战略部 or equivalent central SOE strategic planning function. Readers: group leadership, strategy/planning leaders, business-line leaders, provincial coordination stakeholders.

Do not invent current facts, internal data, project lists, investment numbers, or leadership statements. Mark unavailable facts as `[待补充：说明需要的数据]`.

## Workflow

### 1. Clarify Planning Type

Select the closest type:
- **Group-level strategic plan** (集团总体战略规划): 25,000-35,000 chars
- **Business-specific plan** (业务专项规划): 22,000-30,000 chars
- **Regional infrastructure plan** (区域油气基础设施规划): 20,000-28,000 chars
- **Strategic emerging industry plan** (新能源/战新产业规划): 22,000-30,000 chars
- **Government-facing material** (省级政府汇报备参): 8,000-12,000 chars

### 2. Load References Based on Task

| When | Read |
|---|---|
| Starting any National PipeChina report | `references/national-pipeline-context.md` |
| Choosing report structure and word budget | `references/report-architecture.md` |
| Need detailed chapter outlines | `references/planning-templates.md` |
| Drafting chapters | `references/chapter-writing-patterns.md` |
| Language/style questions | `references/style-and-language.md` |
| Terminology questions | `references/domain-lexicon.md` |
| Evidence/citation questions | `references/evidence-and-citation.md` |
| Before final delivery | `references/quality-gate.md` |

### 3. Set the Word Budget

2万字是底线，不是上限。在底线之上，能多写就多写。以下为各章节最低字数分配，而非目标区间：

| Section | 最低字数 | 说明 |
|---|---|---|
| Executive summary | 1,200 | 可根据报告复杂度上浮至2,500+ |
| Development foundation | 3,000 | 数据越丰富越应展开 |
| Situation and environment | 3,500 | 政策环境分析应尽可能详尽 |
| Overall thinking and objectives | 2,500 | 战略逻辑必须完整展开 |
| Business deployment | 7,000 | 核心章节，无上限，越详细越好 |
| Investment/value/risk | 2,000 | 有数据支撑时可大幅扩展 |
| Safeguards | 2,000 | 每项保障措施独立成节展开 |
| Outlook | 800 | 远景展望适度展开 |

如需压缩，由用户在审阅时指定删减位置，而非初稿自行压缩。

### 4. Draft Chapter by Chapter

For long reports, use a phased output plan rather than compressing all chapters into one response.

### 5. Route Through Citer

初稿完成后，将文本交给 `strategic-planning-citer` 进行以下处理：
- 对每个事实性论断进行来源审核，正文中标注 【1】【2】【3】 序号
- 生成文末「参考文献」汇总（区分知识库来源、WebSearch 检索来源、用户提供来源）
- 对 WebSearch 检索到的来源，文末附标题超链接方便溯源
- 将无法验证的断言标记为 `[待补充引用]`
- 确保每个数字、政策引用、战略判断都有可追溯的来源

Citer 确保引用可溯源（traceability）和引用真实性（authenticity），然后报告进入 reviewer 审查。

### 6. Apply Quality Gates

Before final delivery, run through `references/quality-gate.md` checklist.

## Required Report Logic

Every report must answer five questions:

1. **Why now**: national strategy, policy evolution, energy security, market change, internal reform need
2. **Where we stand**: current foundation, capabilities, achievements, constraints
3. **Where to go**: strategic positioning, objectives, stage goals, indicators
4. **How to get there**: business deployment, projects, mechanisms, resources, coordination
5. **How to guarantee delivery**: organization, investment, talent, policy, digital, compliance, risk controls

Use the closed loop: `strategic situation -> problem/opportunity -> strategic choice -> objective -> deployment task -> resource allocation -> safeguard -> risk response`

## National PipeChina Adaptation

When relevant, address: national energy security, unified pipeline network platform, "X+1+X" market reform, fair open access, national one-network connectivity/storage/peak-shaving/emergency capability, coordination of natural gas/crude oil/product oil/LNG/storage/digitalization/hydrogen/new energy/carbon/strategic emerging industries, and balance of public utility attributes with market-oriented operation.

Use neutral official language for unconfirmed internal expressions; mark them as pending confirmation.

## Drafting Standards

- Formal Chinese SOE planning style: objective, restrained, policy-aware, decision-ready
- No casual phrasing, no promotional exaggeration, no unsupported absolutes
- Use active governance verbs: 构建、完善、推进、优化、提升、健全、强化、统筹、服务、支撑
- Distinguish confirmed facts, assumptions, forecasts, and recommendations
- Use judgment language: 分析显示、综合研判、从中长期看

## Evidence Discipline

Source priority: 用户提供材料 > 已上传知识库 > 国家管网集团官网/年报/公告 > 国务院/发改委/能源局/国资委/国家统计局 > IEA/行业报告。

**缺失数据处理流程**：

1. **先检索知识库**：检查已上传的知识库中是否有相关数据
2. **其次 WebSearch 检索官方网站**：按 .gov.cn → 央企官网 → IEA 等国际组织官网 的优先级检索
3. **检索到则直接使用**：将数据填入正文，消除 [待补充] 标记
4. **检索不到再留空**：仅当知识库和官方网站均无法找到时，才使用 [待补充] 标记

**[待补充] 标记格式**：

使用 Markdown 高亮语法包裹（Typora、部分飞书编辑器等支持，显示为带背景色的高亮文本）：
```
==[待补充：需提供...内部数据]==
```

不支持高亮的输出环境退化为纯文本 `[待补充：...]` 格式。绝不允许用华丽措辞掩盖数据缺口。

**引用格式**：正文使用 【1】【2】【3】 上标编号，文末附参考文献汇总，区分知识库来源和 WebSearch 检索来源。详细格式参见 `strategic-planning-citer`。

After drafting, forward to `strategic-planning-citer` for systematic citation audit, ledger generation, and authenticity verification.

## Output Modes

- **Full report mode**: deliver complete 20,000+ char report in stages if needed
- **Chapter mode**: write or revise a specific chapter with connections to the whole
- **Expansion mode**: expand an existing draft past 20,000 chars without repetition
- **Polish mode**: improve style, logic, terminology, and leadership-readiness
- **Review-fix mode**: diagnose gaps and rewrite weak sections

## Completion Checklist

- [ ] 全报告字数达到20,000字底线，能超则超，无上限约束
- [ ] 每个战略判断有证据、假设或 [待补充] 标记支撑
- [ ] 目标链接到前面的分析和后面的任务
- [ ] 无重复段落、政策堆砌或纯粹口号语言
- [ ] 术语、日期、单位和章节编号标准化
- [ ] [待补充] 标记使用 ==[待补充：...]== Markdown 高亮语法包裹
- [ ] 缺失数据已先尝试知识库检索和 WebSearch 官方网站检索，实在找不到才留空
- [ ] 正文中引用使用 【1】【2】【3】 序号标注
- [ ] 未解决的数据占位符在文末参考文献汇总中列出

## References

- `references/national-pipeline-context.md` — enterprise positioning, strategic themes, sensitive boundaries
- `references/report-architecture.md` — report structures and word budget discipline
- `references/planning-templates.md` — six detailed report templates with full chapter outlines
- `references/chapter-writing-patterns.md` — paragraph formulas for each chapter type
- `references/style-and-language.md` — SOE formal style, verb lists, banned expressions
- `references/domain-lexicon.md` — standard energy/pipeline terminology and units
- `references/evidence-and-citation.md` — source priority, citation style, placeholder format
- `references/quality-gate.md` — pre-delivery structural, logic, data, style, and leadership-readiness checks
