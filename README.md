# Growth Agents

Custom AI agents built for growth. Content creation, distribution, data visualization, and shipping faster.

## Agents

### writing-coach-style-preserving-finisher

An AI writing coach that helps you finish articles when you're stuck on the last 20%.

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

### chart-maker-formal-svg

Generates clean, formal SVG charts for blog posts and articles.

- Creates production-ready SVG files you can embed anywhere.
- Supports timeline charts, pie charts, bar charts, and conceptual diagrams.
- No overlapping text. Readable labels with generous padding. Visible but subtle axes.
- Less is more. No gradients, no shadows, no decorative elements.
- Outputs self-contained SVGs with no external dependencies.

**Best for:** Data visualizations in blog posts, article illustrations, presentation assets, social media graphics.

---

## Setup

Copy the agent files to your Factory droids directory:

```bash
cp *.md ~/.factory/droids/
```

Then invoke any agent:

```bash
droid writing-coach-style-preserving-finisher
droid chart-maker-formal-svg
```

Once installed, they're also available as subagents inside any other Factory session.

## What are growth agents?

These are not generic AI prompts. They are opinionated, specialized agents that preserve your voice, push you to ship, and help you build a content engine that actually drives growth.

Custom droids are reusable AI agents built on [Factory](https://docs.factory.ai). Think of them as specialized teammates you can spin up anytime. Each droid has a specific job, a defined personality, and a set of tools it can use.

The bottleneck for most founders and creators isn't ideas. It's execution. Writing the post, making the chart, publishing it everywhere, doing it consistently. These agents close that gap.

## How is this different from Claude Skills, GPTs, or Codex?

- **Claude Skills** are saved prompts inside Claude. They don't have tool access, can't create files, and live inside one product. Custom droids can read, write, search the web, run code, and interact with your filesystem and APIs.
- **OpenAI GPTs** are chatbot wrappers. They're good for Q&A but can't take real actions. Droids execute. They create files, push to GitHub, edit your drafts, generate assets.
- **Codex custom agents** are code-focused. They're great for engineering tasks but aren't built for growth workflows like writing, content distribution, or visual asset creation.
- **Custom droids** are multi-modal growth agents. They combine deep prompt engineering with real tool access. A writing droid doesn't just suggest edits. It corrects your grammar, generates HN-optimized titles, coaches you to finish, and reminds you to distribute across every channel. A chart droid doesn't just describe a chart. It creates a production-ready SVG file you can embed in your blog post.

## Contributing

Got a growth agent that helps you ship faster? Open a PR.

## License

MIT
