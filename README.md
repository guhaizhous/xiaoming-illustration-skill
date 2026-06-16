# xiaoming-illustration-skill

> 🇨🇳 中文文档 | [English Documentation](README.en.md)

为中文内容生成极简线条正文配图的 AI Agent Skill。适用于文章观点生图、绘本内容生图、知识点拆解生图、教学内容生图。

## 核心特点

- **小明 IP**：黑色实心小怪物，蓝色圆点眼，作为每张图的动作主体
- **极简风格**：白底、细线、蓝色点缀、大量留白
- **四种场景**：文章观点、绘本内容、知识点拆解、教学内容
- **Shot List 策略**：先分析内容输出配图策略，再生成图片

## 视觉风格

| 要素 | 规范 |
|------|------|
| 线条 | 细黑墨线，手绘微抖 |
| 背景 | 纯白，大量留白 |
| 点缀色 | 唯一蓝色 `#3B82F6` |
| 人物 | 极小，与物体形成戏剧性对比 |
| 批注 | 少量蓝/红色中文手写批注 |

## 安装

```bash
# 克隆仓库
git clone https://github.com/your-username/xiaoming-illustration-skill.git

# 复制到 Agent skills 目录
mkdir -p ~/.trae/skills/xiaoming-illustration-skill
cp -R xiaoming-illustration-skill/* ~/.trae/skills/xiaoming-illustration-skill/
```

## 使用方法

### 文章观点生图

```
用article-illustration为这篇文章生成4张观点配图
---
<粘贴文章内容>
```

### 绘本内容生图

```
用article-illustration为这个故事生成5张绘本插图
场景风格：怪诞但清爽，小明是主角。
---
<粘贴故事>
```

### 知识点拆解生图

```
用xiaoming-illustration-skill把这个知识点拆解成3张图
每张图只讲一个核心概念，用小明作为动作主体。
---
<粘贴知识点>
```

### 教学内容生图

```
用article-illustration为这个教学场景生成配图
风格：简洁清爽、怪诞有创意、适合教学展示。
---
<粘贴教学内容>
```

## 工作流

1. **分析内容**：提炼核心观点、认知转折、适合可视化的段落
2. **输出 Shot List**：确定每张图的主题、结构类型、小明动作
3. **生成图片**：使用 AI 图像模型单独生成每张图
4. **检查迭代**：对照 QA 清单检查，必要时重生成
5. **保存交付**：保存到 `assets/<article-slug>-illustrations/`

## 目录结构

```
xiaoming-illustration-skill/
├── SKILL.md              # 主规范文件（中文）
├── SKILL.en.md           # Main specification (English)
├── README.md             # 项目说明（中文）
├── README.en.md          # Project documentation (English)
├── LICENSE               # 许可证
└── references/
    ├── xiaoming-ip.md    # 小明IP定义
    ├── style-guide.md     # 风格规范
    ├── composition-types.md # 构图类型参考
    ├── prompt-template.md # 生图提示词模板
    └── qa-checklist.md    # 检查清单
```

## 示例

### 输入

```
溯源动机 — 区分"改变"和"焦虑"，学习动机必须具体可操作
打破幻觉 — 输入≠输出，收藏≠掌握，纠正三个常见认知偏差
路径执行 — 一次只吃透一件事：拉出来→费曼理解→做成知识卡片
触发条件 — 不靠意志力靠系统，设计固定/事件/环境三重触发器
```

### 输出 Shot List

| 序号 | 主题 | 结构类型 | 小明动作 |
|------|------|----------|----------|
| 1 | 溯源动机 | 分拣归类 | 小明站在岔路口，左手拉火焰(焦虑)，右手拉阶梯(改变) |
| 2 | 打破幻觉 | 概念隐喻 | 小明站在漏斗前，上方堆满书本收藏，下方只有几颗种子 |
| 3 | 路径执行 | 方法分层 | 小明弯腰只盯着一件事深挖 |
| 4 | 三重触发器 | 系统局部 | 小明同时拉下三个开关 |

## 支持的 Agent

- Trae Agent
- Cola
- Claude Code
- Codex

## 许可证

MIT License - 详见 [LICENSE](LICENSE)

## 贡献

欢迎提交 Issue 和 Pull Request！

## 作者

你的名字 / GitHub 用户名
