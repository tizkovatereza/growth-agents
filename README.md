# Growth Agents

Custom AI agents built for growth. Content creation, distribution, data visualization, and shipping faster.

These are not generic AI prompts. They are opinionated, specialized agents built on [Factory](https://factory.ai) that preserve your voice, push you to ship, and help you build a content engine that actually drives growth. Each agent has a specific job, a defined personality, and access to [real tools](https://docs.factory.ai/cli/configuration/custom-droids.md) -- they can create files, search the web, edit your drafts, and generate assets.

## Agents

### [Writing Coach](writing-coach-style-preserving-finisher.md)

An AI writing coach that helps you finish articles when you're stuck on the last 20%.

- On first use, asks you about your writing style (sentence length, punctuation habits, forbidden words, tone, sample writing) and adapts permanently.
- Studies and preserves your exact writing style. Never overwrites your voice.
- Gives honest, no-fluff feedback. Tells you what works and what doesn't.
- Identifies gaps in your draft and suggests specific additions.
- Generates 5 title options ranked by Hacker News trending potential.
- Coaches you hard to finish. Sets time limits. Doesn't let you procrastinate.
- Corrects grammar and suggests better phrasing while keeping your tone.
- Detects and flags AI-generated filler patterns (preambles, hedges, recap closers).
- Reminds you to distribute: HN, X/Twitter, LinkedIn, personal site.
- Adapts suggestions based on the publishing platform.

**Best for:** Blog posts, technical articles, thought pieces, Substack newsletters, HN submissions.

### [Chart Maker](chart-maker-formal-svg.md)

Generates clean, formal SVG charts for blog posts and articles.

- Creates production-ready SVG files you can embed anywhere.
- Supports timeline charts, pie charts, bar charts, and conceptual diagrams.
- No overlapping text. Readable labels with generous padding. Visible but subtle axes.
- Less is more. No gradients, no shadows, no decorative elements.
- Outputs self-contained SVGs with no external dependencies.

**Best for:** Data visualizations in blog posts, article illustrations, presentation assets, social media graphics.

### [Focus Coach](focus-coach-no-excuses.md)

A brutally honest accountability coach that keeps you on task and won't let you quit at 80%.

- Breaks your task into concrete steps and tracks progress ruthlessly.
- Detects excuses in real time. Has heard them all. Not impressed.
- Sets aggressive but realistic time limits. Parkinson's Law is the enemy.
- Calls out scope creep, perfectionism, and "productive procrastination" (researching instead of doing).
- Funny, slightly sarcastic, but genuinely wants you to finish.
- Pushes hardest when you're closest to done -- the last 10% is where amateurs quit.
- Makes you define what DONE looks like before you start, then holds you to it.

**Best for:** Finishing articles, shipping features, completing any task where you keep getting distracted or quitting at "good enough."

---

## Getting Started

> **Not technical? Never used a terminal?** No problem. [Read the beginner-friendly walkthrough](GETTING-STARTED-FOR-BEGINNERS.md). It explains everything from scratch, step by step, for dummies. Don't be afraid, you don't need to write code, I promise!

### 1. Get Factory

These agents run on [Factory](https://factory.ai) -- an AI-native development platform with a [desktop app, web app, and CLI](https://docs.factory.ai/cli/getting-started/quickstart.md). You need a Factory account ([Pro plan starts at $20/mo](https://docs.factory.ai/pricing.md)).

1. Go to [factory.ai](https://factory.ai) and sign up
2. Download the desktop app or install the CLI:
   ```bash
   curl -fsSL https://app.factory.ai/install.sh | sh
   ```
3. Run `droid` and log in when prompted

### 2. Install the agents

Clone this repo and copy the agent files:

```bash
git clone https://github.com/tizkovatereza/growth-agents.git
cp growth-agents/*.md ~/.factory/droids/
```

### 3. Use them

Start a dedicated session with any agent:

```bash
droid writing-coach-style-preserving-finisher
droid chart-maker-formal-svg
droid focus-coach-no-excuses
```

Once installed, they're also available as subagents inside any other Factory session. You can also extend them with [MCP integrations](https://docs.factory.ai/cli/configuration/mcp.md), connect your own API keys via [BYOK](https://docs.factory.ai/cli/byok/overview.md), or build your own agents using the [custom droids guide](https://docs.factory.ai/cli/configuration/custom-droids.md).

## How is this different?

### Claude Skills vs Factory Droids
Claude Skills are saved prompts inside Claude. They don't have tool access, can't create files, and live inside one product. Factory droids can read, write, search the web, run code, and interact with your filesystem and APIs.

### OpenAI GPTs vs Factory Droids
GPTs are chatbot wrappers. They're good for Q&A but can't take real actions. Droids execute. They create files, push to GitHub, edit your drafts, generate assets.

### Codex Custom Agents vs Factory Droids
Codex agents are code-focused. They're great for engineering tasks but aren't built for growth workflows like writing, content distribution, or visual asset creation.

### Cursor Rules vs Factory Droids
Cursor has project rules (`.cursorrules`) that guide its AI inside the IDE. They're great for coding conventions but they're scoped to code editing. You can't use Cursor rules to write a blog post, generate a chart, or push to GitHub. Factory droids work across your whole system, not just inside an editor.

### Devin (Cognition) vs Factory Droids
Devin is an autonomous software engineer. It writes code, runs tests, and ships PRs. But it's built for engineering, not growth. You can't ask Devin to coach your writing, optimize a title for Hacker News, or create an SVG chart for your blog. Factory droids are specialized for non-engineering workflows that founders and creators need.

### Why Factory Droids?
The bottleneck for most founders and creators isn't ideas. It's execution. Writing the post, making the chart, publishing it everywhere, doing it consistently. Factory droids are multi-modal growth agents that combine deep prompt engineering with real tool access. A writing droid doesn't just suggest edits. It corrects your grammar, generates HN-optimized titles, coaches you to finish, and reminds you to distribute across every channel. A chart droid doesn't just describe a chart. It creates a production-ready SVG file you can embed in your blog post. Build your own with the [custom droids guide](https://docs.factory.ai/cli/configuration/custom-droids.md) or extend these with [skills](https://docs.factory.ai/cli/configuration/skills.md). Questions? Join the [Factory Discord](https://discord.gg/zuudFXxg69).

## Contributing

Got a growth agent that helps you ship faster? Open a PR! I will try to get to that. :) 
T

## License

MIT
