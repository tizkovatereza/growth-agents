# Growth Agents

Custom AI agents for content creation, data visualization, and shipping faster. Built on [Factory](https://factory.ai).

Not generic prompts. Opinionated, specialized agents that preserve your voice and have access to [real tools](https://docs.factory.ai/cli/configuration/custom-droids.md) -- they create files, search the web, edit drafts, and generate assets.

## Agents

### [Writing Coach](Writing-Feedback-And-Coaching-Agent.md)
Helps you finish articles when you're stuck on the last 20%. Studies your writing style, gives honest feedback, suggests what to add, generates HN-optimized titles, and coaches you hard to ship. Never overwrites your voice.

### [Chart Maker](chart-maker-formal-svg.md)
Generates clean, formal SVG charts for blog posts. Timeline charts, pie charts, bar charts, conceptual diagrams. No overlapping text, no gradients, no decorative noise. Production-ready, self-contained SVGs.

<img width="980" height="620" alt="chart2-paradox-of-choice" src="https://github.com/user-attachments/assets/00246997-23f3-49d6-a303-a09c3472dd8d" />

### [Visual Designer](tereza-tizkova-visual-designer.md)
Creates production-ready visual assets matching a minimal, editorial brand identity. Blog headers, social media graphics, data visualizations, infographics. Dark theme, typographic hierarchy, restrained accents.

### [Focus Coach](focus-coach-no-excuses.md)
Brutally honest accountability coach. Breaks tasks into steps, detects excuses, sets time limits, calls out scope creep. Funny but relentless. Won't let you quit at 80%.

## Getting Started

> **Never used a terminal?** [Read the beginner walkthrough](Getting-started-for-beginners.md).

1. Sign up at [factory.ai](https://factory.ai) and install the CLI:
   ```bash
   curl -fsSL https://app.factory.ai/install.sh | sh
   ```
2. Clone and install:
   ```bash
   git clone https://github.com/tizkovatereza/growth-agents.git
   cp growth-agents/*.md ~/.factory/droids/
   ```
3. Use them:
   ```bash
   droid writing-coach-style-preserving-finisher
   droid chart-maker-formal-svg
   droid focus-coach-no-excuses
   ```

They also work as subagents inside any Factory session. Extend with [MCP integrations](https://docs.factory.ai/cli/configuration/mcp.md), [BYOK](https://docs.factory.ai/cli/byok/overview.md), or [build your own](https://docs.factory.ai/cli/configuration/custom-droids.md).

## Contributing

Got a growth agent that helps you ship faster? Open a PR!

## License

MIT
