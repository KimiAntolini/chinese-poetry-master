# Chinese Poetry Master (诗词鉴赏)

> AI Skill Pack for deep literary appreciation of Chinese poetry. 11 sub-skills + 1 orchestrator. Cross-platform: Claude Code / OpenCode / GPT.
>
> AI Skills 包：11 子 Skill + 1 主编排器，为中国诗词提供 10 段式深度赏析。跨平台适用。

---

[English](#english) | [中文](#中文)

---

## English

### What Is This?

A **skill pack** that empowers AI to perform 10-section deep analysis of Chinese poetry (诗/词/曲/新诗). Built on a **6,006-poem dataset** spanning **8 dynasties** (先秦→清→当代), filtered by an S/A/B/C/D five-tier quality grading system.

Each of the 11 sub-skills brings deep domain knowledge to one dimension of poetry appreciation — from imagery dictionaries and 意境 typology to historical criticism databases and modern poetry analysis methods.

### Architecture

```
chinese-poetry-master/
├── SKILL.md                       # Main orchestrator: trigger→dispatch→synthesize
├── CLAUDE.md                      # Development conventions
├── README.md                      # This file
├── Poem.md                        # Dataset: 6,006 poems across 8 dynasties
└── skills/
    ├── poetry-author/             # 1. Author biography + style matrix
    ├── poetry-background/         # 2. Historical context + period reference
    ├── poetry-imagery/            # 3. Imagery dictionary + cultural codes
    ├── poetry-yijing/             # 4. Artistic conception typology
    ├── poetry-surface/            # 5. Surface reading + translation method
    ├── poetry-deep/               # 6. Allusion, symbol & allegory decoding
    ├── poetry-emotion/            # 7. Emotion typology + intent analysis
    ├── poetry-prosody/            # 8. Prosody, rhyme & meter analysis
    ├── poetry-criticism/          # 9. Historical criticism database
    ├── poetry-synthesis/          # 10. Multi-dimensional holistic appreciation
    └── poetry-modern/             # 11. Modern/contemporary poetry specialist
```

### Quick Demo

**Input**: "赏析李白的《静夜思》"

**Output**: Structured 10-section analysis:
```
1. Author Biography → 2. Historical Context → 3. Imagery → 4. Yijing
→ 5. Surface Reading → 6. Deep Meaning → 7. Author's Emotion/Intent
→ 8. Prosody Analysis → 9. Expert Criticism (2-3 scholars) → 10. Synthesis
```

### Installation

| Platform | Method |
|----------|--------|
| **OpenCode** | Copy to `~/.config/opencode/skills/chinese-poetry-master/` |
| **Claude Code** | Copy to `~/.claude/skills/chinese-poetry-master/` |
| **GPT / Other** | Inject `SKILL.md` as System Prompt + provide sub-skills as context |

### Dataset

| Metric | Value |
|--------|-------|
| Total poems | 6,006 |
| Dynasties | 先秦·汉·魏晋·南北朝·唐·宋·元·明·清·近现代·当代 |
| Poetry types | 诗 ~60% · 词 ~30% · 曲 ~10% |
| Quality system | S/A/B/C/D 5-tier grading (all poets, all dynasties) |
| Source | [chinese-poetry/chinese-poetry](https://github.com/chinese-poetry/chinese-poetry) (MIT) |

### License

MIT. Data sourced from [chinese-poetry/chinese-poetry](https://github.com/chinese-poetry/chinese-poetry) (MIT).

---

## 中文

### 这是什么？

一个 **Skills 包**（11 子 Skill + 1 主编排器），为 AI 提供中国诗词 10 段式深度赏析能力。基于 **6006 首**诗词数据集，覆盖**八大朝代**（先秦至当代），经 **S/A/B/C/D 五级**优先级评判体系严格筛选。

每个子 Skill 为一个赏析维度装满专业知识和分析方法——从意象辞典、意境类型学到历代诗话数据库，从近现代新诗节奏分析到当代诗意象解码。

### 架构

```
chinese-poetry-master/
├── SKILL.md                       # 主编排器：触发→调度子Skill→汇总输出
├── CLAUDE.md                      # 项目开发规范
├── README.md                      # 本文件（中英双语）
├── Poem.md                        # 诗词数据集（6006首，八朝代覆盖）
└── skills/                        # 11 子 Skill 包
    ├── poetry-author/             # 1. 作者生平（诗人数据库+风格矩阵）
    ├── poetry-background/         # 2. 创作背景（历史年表+以史证诗）
    ├── poetry-imagery/            # 3. 意象（意象辞典+文化密码+组合规律）
    ├── poetry-yijing/             # 4. 意境（类型学+王国维境界说+构成法则）
    ├── poetry-surface/            # 5. 表意（逐句解读法+语序还原+翻译策略）
    ├── poetry-deep/               # 6. 深层意（用典/象征/比兴/寄托解码）
    ├── poetry-emotion/            # 7. 作者意图感情（情感类型学+表达策略）
    ├── poetry-prosody/            # 8. 韵律分析（平仄/押韵/对仗/节奏/词牌格律）
    ├── poetry-criticism/          # 9. 名家赏析（历代诗话数据库+评注方法论）
    ├── poetry-synthesis/          # 10. 综合赏析（多维整合框架+鉴赏词汇库）
    └── poetry-modern/             # 11. 近现代&当代专项（新诗+旧体诗词+当代意象）
```

### 使用示例

```
赏析《静夜思》
分析李白的将进酒
帮我找几首边塞诗
赏析这首诗：[粘贴全文]
```

### 数据集

| 指标 | 数值 |
|------|------|
| 总诗词数 | 6,006 首 |
| 朝代覆盖 | 先秦·汉·魏晋·南北朝·唐·宋·元·明·清·近现代·当代 |
| 体裁比例 | 诗 ~60% · 词 ~30% · 曲 ~10% |
| 质量体系 | S/A/B/C/D 五级评判（所有诗人、所有朝代统一适用） |
| 数据来源 | [chinese-poetry/chinese-poetry](https://github.com/chinese-poetry/chinese-poetry)（MIT） |

### 优先级评判体系

| 等级 | 标准 | 保留策略 |
|------|------|----------|
| **S 级** | 千古名篇、教材必选、家喻户晓 | 不限数量 |
| **A 级** | 代表诗人最高成就、学界认可 | ≤50首/作者 |
| **B 级** | 有一定艺术价值、文学史提及 | ≤20首/作者 |
| **C 级** | 中等质量、偶见引用 | ≤5首/作者 |
| **D 级** | 应酬唱和、仅有文献价值 | 删除 |

### 赏析输出（10 段铁律）

```
1. 作者生平 → 2. 创作背景 → 3. 意象 → 4. 意境 → 5. 表意
→ 6. 深层意 → 7. 作者意图感情 → 8. 韵律分析 → 9. 名家赏析(2-3位) → 10. 综合赏析
```

### 开源许可

MIT。数据源自 [chinese-poetry/chinese-poetry](https://github.com/chinese-poetry/chinese-poetry)（MIT）。

---

*为中国诗词而建。Built for Chinese poetry.*
