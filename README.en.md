# xiaoming-illustration-skill

> 🇺🇸 English Documentation | [中文文档](README.md)

An AI Agent Skill for generating minimalist line illustrations for Chinese content. Suitable for article viewpoints, picture books, knowledge breakdowns, and teaching scenarios.

## Core Features

- **Xiao Ming IP**: A small black creature with blue dot eyes, serving as the action subject in every illustration
- **Minimalist Style**: White background, thin lines, blue accents, generous whitespace
- **Four Scenarios**: Article viewpoints, picture book content, knowledge breakdowns, teaching content
- **Shot List Strategy**: Analyze content first to output illustration strategy, then generate images

## Visual Style

| Element | Specification |
|---------|---------------|
| Lines | Thin black ink lines, hand-drawn with slight tremor |
| Background | Pure white, generous whitespace |
| Accent Color | Single blue `#3B82F6` |
| Characters | Very small, dramatic contrast with objects |
| Annotations | Few blue/red Chinese handwritten annotations |

## Installation

```bash
# Clone repository
git clone https://github.com/your-username/xiaoming-illustration-skill.git

# Copy to Agent skills directory
mkdir -p ~/.trae/skills/xiaoming-illustration-skill
cp -R xiaoming-illustration-skill/* ~/.trae/skills/xiaoming-illustration-skill/
```

## Usage

### Article Viewpoint Illustrations

```
Use xiaoming-illustration-skill to generate 4 viewpoint illustrations for this article
---
<Paste article content>
```

### Picture Book Illustrations

```
Use xiaoming-illustration-skill to generate 5 picture book illustrations for this story
Style: Whimsical but clean, Xiao Ming is the protagonist.
---
<Paste story>
```

### Knowledge Breakdown Illustrations

```
Use xiaoming-illustration-skill to break down this knowledge into 3 illustrations
Each illustration focuses on one core concept, with Xiao Ming as the action subject.
---
<Paste knowledge content>
```

### Teaching Scenario Illustrations

```
Use xiaoming-illustration-skill to generate illustrations for this teaching scenario
Style: Clean and fresh, whimsical and creative, suitable for teaching display.
---
<Paste teaching content>
```
### 示例效果

| 溯源动机 | 打破幻觉 |
|----------|----------|
| ![溯源动机](https://platform-outputs.agnes-ai.space/images/text-to-image/2026/06/243e9aaf6fb6458ca397f84cf42e7b91.png) | ![打破幻觉](https://platform-outputs.agnes-ai.space/images/text-to-image/2026/06/9400a0e82ef04fca97c128492a535c1f.png) |

| 路径执行 | 三重触发器 |
|----------|------------|
| ![路径执行](https://platform-outputs.agnes-ai.space/images/text-to-image/2026/06/9b1d10bdc2d347b5bebeda05133eae2b.png) | ![三重触发器](https://platform-outputs.agnes-ai.space/images/text-to-image/2026/06/8a4398e32d09443d8b5df47df0b612a3.png) |

## Workflow

1. **Analyze Content**: Extract core viewpoints, cognitive turning points, paragraphs suitable for visualization
2. **Output Shot List**: Determine theme, structure type, and Xiao Ming's actions for each illustration
3. **Generate Images**: Use AI image models to generate each illustration separately
4. **Check & Iterate**: Review against QA checklist, regenerate if necessary
5. **Save & Deliver**: Save to `assets/<article-slug>-illustrations/`

## Directory Structure

```
xiaoming-illustration-skill/
├── SKILL.md              # Main specification (Chinese)
├── SKILL.en.md           # Main specification (English)
├── README.md             # Project documentation (Chinese)
├── README.en.md          # Project documentation (English)
├── LICENSE               # License
└── references/
    ├── xiaoming-ip.md    # Xiao Ming IP definition
    ├── style-guide.md    # Style guide
    ├── composition-types.md # Composition types reference
    ├── prompt-template.md # Image generation prompt templates
    └── qa-checklist.md   # Quality assurance checklist
```

## Example

### Input

```
Trace motivation — Distinguish "change" from "anxiety", learning motivation must be specific and actionable
Break illusions — Input ≠ Output, collecting ≠ mastering, correct three common cognitive biases
Execute path — Master one thing at a time: extract → Feynman understanding → create knowledge card
Trigger conditions — Don't rely on willpower, design fixed/event/environmental triple triggers
```

### Output Shot List

| # | Theme | Structure Type | Xiao Ming's Action |
|---|-------|----------------|-------------------|
| 1 | Trace Motivation | Sorting & Classification | Xiao Ming stands at a fork, pulling flame (anxiety) with left hand, stairs (change) with right |
| 2 | Break Illusions | Conceptual Metaphor | Xiao Ming stands before a funnel, books piled above, only a few seeds below |
| 3 | Path Execution | Layered Method | Xiao Ming bends down to dig deep into one thing |
| 4 | Triple Triggers | System Component | Xiao Ming pulls down three switches simultaneously |

## Supported Agents

- Trae Agent
- Cola
- Claude Code
- Codex
- hermes 
- pi

## License

MIT License - See [LICENSE](LICENSE) for details

## Contributing

Issues and Pull Requests are welcome!

## Author

guhaizhous(谷子熟了)
