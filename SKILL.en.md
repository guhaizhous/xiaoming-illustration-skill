---
name: "xiaoming-illustration-skill"
description: "Generate minimalist line illustrations for articles, picture books, knowledge breakdowns, and teaching content. Invoke when users request illustrations for article viewpoints, picture book content, knowledge points, teaching scenarios, or mention 'illustration', 'image generation', 'Xiao Ming style'."
---

# Article Illustration · Article Illustration

Generate minimalist line illustrations for Chinese content. Suitable for article viewpoints, picture book content, knowledge breakdowns, and teaching scenarios. Core style: white background, thin lines, blue accents, Xiao Ming as action subject, whimsical but clean.

## Positioning

Not commercial illustration, not PPT infographics, not cute cartoons. Transform judgments, processes, structures, states, or metaphors in articles into clean, whimsical, creative, readable hand-drawn explanatory diagrams that aren't instruction manuals.

## Use Cases

| Scenario | Description | Example |
|----------|-------------|---------|
| Article Viewpoint Illustrations | Create illustrations for core article viewpoints | "Knowledge compound interest" with Xiao Ming working on an accumulation pyramid |
| Picture Book Content Illustrations | Generate scene illustrations for story picture books | Protagonist Xiao Ming walks into a knowledge forest |
| Knowledge Breakdown Illustrations | Break down complex concepts into visual diagrams | Break down "compound interest" into time × return physical metaphor |
| Teaching Content Illustrations | Teaching scenarios, knowledge explanation illustrations | Xiao Ming observes knowledge crystals through a magnifying glass |

## Style Guidelines

### Core Elements

- **Lines**: Thin black ink lines, hand-drawn with slight tremor, not mechanical
- **Background**: Pure white, no paper texture, gradients, or shadows
- **Accent Color**: Single blue `#3B82F6`, placed on the most meaningful element
- **Characters**: Very small. Objects are grand, characters are tiny, dramatic contrast
- **Whitespace**: Generous whitespace, subjects occupy 40%-60% of the image
- **Annotations**: Few blue/red Chinese handwritten annotations

### Xiao Ming IP

Xiao Ming is the fixed character in every illustration, not decoration, but an absurd worker seriously participating in system operations.

**Appearance**:
- Small solid black creature
- Blue dot eyes (echoing the accent color)
- Thin legs, occasionally thin arms
- Body can be a black bean, black box, funnel, shadow
- Expression: empty,呆, calm, serious

**Personality**:
- Very serious, but does somewhat absurd things
- Like a low-key system operator
- Dry humor, not cute
- Like truly responsible for some work in a whiteboard sketch

**Common Actions**:
- Carrying materials to pile up
- Pulling lines to converge information sources
- Stuck in breakpoints
- Operating "judgment" levers
- Becoming a screening funnel
- Cutting "materials"
- Stamping to accept phrases
- Leading paths
- Holding warning signs to look at pits
- Reaching out from holes but failing to catch
- Moving bricks, building bridges, opening doors, sorting on the side

**Prohibited**:
- Don't draw as a cute mascot
- Don't give Xiao Ming complex clothing or emoji expressions
- Don't let Xiao Ming just stand by watching
- If removing Xiao Ming still leaves the core metaphor intact, Xiao Ming is too decorative

## Workflow

### Step 1: Analyze Content

First read the user's content (articles, links, notes, screenshots), extract:
- What is the core viewpoint
- Which paragraphs carry cognitive turning points
- Which content is suitable for visual explanation
- Which places only need text, no illustrations

### Step 2: Output Shot List

If the user just asks "how to illustrate" or "analyze", provide a shot list first. For each illustration, clarify:
- Where it appears (after which paragraph)
- Illustration theme
- Core meaning
- Structure type (comic strip/system component/before-after/character state/conceptual metaphor/method layering/map route)
- What Xiao Ming does in the illustration
- Suggested elements
- Suggested Chinese annotation words

**Quantity Recommendation**: 4-8 illustrations, short articles 1-3, long articles no more than 9.

### Step 3: Generate Images

If the user explicitly requests "generate/create images/output", use the built-in image_gen to generate each illustration separately.

**Prompts must include**:
- 16:9 horizontal Chinese body illustration
- Pure white background
- Black hand-drawn line art, thin lines with slight tremor
- Single blue accent `#3B82F6`
- Xiao Ming as core action subject
- Generous whitespace
- Few blue/red Chinese handwritten annotations
- Prohibit PPT, commercial illustration, childish cuteness, complex architecture

**Single Image Principle**: Each illustration tells only one core structure, don't combine multiple illustrations into one image.

### Step 4: Check & Iterate

After generation, check:
- Is Xiao Ming just decoration
- Is the image too crowded
- Does it look like a flowchart/PPT
- Are there too many Chinese annotations or typos
- Is the background clean white
- Is it too cute/childish/rigid

Regenerate or locally edit if there are issues.

### Step 5: Save & Deliver

Save to: `assets/<article-slug>-illustrations/`
Naming: `01-topic-name.png`, `02-topic-name.png`

## Scenario Templates

### Article Viewpoint Illustrations

```
Use article-illustration to generate 4 viewpoint illustrations for this article.
Requirements: 16:9 horizontal, pure white background, black hand-drawn line art, blue accents, Xiao Ming as action subject.
---
<Paste article>
```

### Picture Book Content Illustrations

```
Use article-illustration to generate picture book illustrations for this story, 5 images.
Scene style: Whimsical but clean, Xiao Ming is the protagonist.
---
<Paste story>
```

### Knowledge Breakdown Illustrations

```
Use article-illustration to break down this knowledge point into 3 illustrations.
Each illustration focuses on one core concept, with Xiao Ming as action subject.
---
<Paste knowledge point>
```

### Teaching Content Illustrations

```
Use article-illustration to generate illustrations for this teaching scenario.
Style: Clean and fresh, whimsical and creative, suitable for teaching display.
---
<Paste teaching content>
```

## Composition Types Reference

| Type | Use Case | Xiao Ming Action |
|------|----------|------------------|
| Comic Strip | Before-after comparison, turning points | Xiao Ming experiences change |
| System Component | Input → Process → Output | Xiao Ming operates inside a machine |
| Before-After | Before/After comparison | Xiao Ming pulls a switch |
| Character State | Emotion/state changes | Xiao Ming's expression/action changes |
| Conceptual Metaphor | Abstract concept visualization | Xiao Ming interacts with metaphor objects |
| Method Layering | Progressive layers | Xiao Ming climbs/digs |
| Map Route | Path selection | Xiao Ming walks/gets lost |
| Sorting & Classification | Information organization | Xiao Ming sorts/carries |

## Judgment Criteria

Each illustration must satisfy:
1. Xiao Ming is the core action subject, not decoration
2. Generous whitespace in the image
3. Blue accents only on the most meaningful elements
4. Few Chinese annotations with handwritten feel
5. Very small characters, grand objects, dramatic contrast

## Directory Structure

```
article-illustration/
├── SKILL.md
└── references/
    ├── xiaoming-ip.md      # Xiao Ming IP definition
    ├── style-guide.md      # Detailed style guidelines
    ├── composition-types.md # Composition types reference
    ├── prompt-template.md   # Image generation prompt templates
    └── qa-checklist.md     # Quality assurance checklist
```
