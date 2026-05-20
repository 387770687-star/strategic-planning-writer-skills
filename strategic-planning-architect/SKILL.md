---
name: strategic-planning-architect
description: Design report architecture, chapter logic, word budget, strategic main line, indicator systems, and phased delivery plans for Chinese strategic planning reports. Use when the user needs an outline, chapter plan, word budget, or blueprint for a 20,000+ Chinese character strategic planning report before drafting begins.
---

# Strategic Planning Architect

Design the blueprint for a long-form Chinese strategic planning report. Produce a complete architecture that can support a 20,000+ Chinese character deliverable without repetition or filler.

## When to Use

Trigger when the user asks to:
- Design a report outline or chapter structure
- Create a word budget for a strategic report
- Build a chapter logic chain or traceability matrix
- Define a strategic main line
- Plan indicator systems and drafting sequences
- Set up the architecture before running `strategic-planning-writer`

## Workflow

### 1. Identify Report Type

Classify the report into one of:
- group-level plan (集团级总体规划)
- business-specific plan (业务专项规划)
- regional infrastructure plan (区域油气基础设施规划)
- strategic emerging industry plan (战新产业规划)
- government-facing material (省级政府汇报备参)

### 2. Define the Strategic Main Line

Write a single paragraph capturing the report's core argument. Pattern:

`以...为统领，以...为主线，以...为重点，统筹...和...，推动...，为...提供支撑。`

### 3. Build the Chapter Map

For each chapter, specify:
- chapter purpose
- key argument
- evidence needed
- expected output
- target character count

Reference `references/outline-patterns.md` for structure options by report type.

### 4. Build the Traceability Chain

Create a mapping table:

| Key Situation | Strategic Implication | Objective | Task Section | Safeguard Section |

Ensure every objective maps to at least one task, and every risk maps to a control measure.

### 5. Design the Indicator System

Cover eight dimensions: scale (规模), capability (能力), efficiency (效率), safety (安全), green (绿色), innovation (创新), market (市场), value (价值).

### 6. Produce the Word Budget

Use `references/word-budget.md` for character allocation templates. The budget must exceed 20,000 Chinese characters. A 22,800-character minimum budget or 31,300-character premium budget is available.

### 7. Produce a Phased Drafting Plan

Specify the recommended writing sequence for `strategic-planning-writer`.

## Output Format

1. Report type and stated assumptions
2. Strategic main line (one paragraph)
3. Proposed table of contents with character allocation per chapter
4. Word budget table totaling above 20,000 characters
5. Chapter logic notes (purpose, argument, evidence, output)
6. Evidence/data requirements by chapter
7. Recommended drafting sequence
8. Architecture risks and mitigation

## Architecture Rules

- The deployment section (重点任务与业务部署) must be the deepest and most practical part.
- Every objective maps to at least one task.
- Every risk maps to a control measure.
- No sections that repeat each other under different names.
- Do not place all analysis in the executive summary.
- For National PipeChina topics, maintain "全国一张网运营" and "能源安全基础设施平台" as organizing ideas.

## References

- `references/outline-patterns.md` — structure options and strategic main line examples by report type
- `references/word-budget.md` — character allocation templates (22,800 and 31,300 character budgets)

Read these when the user's report type requires a specific structure or when building the word budget.
