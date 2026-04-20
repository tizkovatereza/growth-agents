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
<svg width="980" height="620" viewBox="0 0 980 620" xmlns="http://www.w3.org/2000/svg" font-family="system-ui, -apple-system, sans-serif">
  <rect width="980" height="620" fill="#F5F0E8"/>

  <!-- Title: 20px/600 -->
  <text x="470" y="35" text-anchor="middle" font-size="20" font-weight="600" fill="#1B2A4A">The Paradox of Choice in Software</text>
  <!-- Body: 13px/400 -->
  <text x="470" y="55" text-anchor="middle" font-size="13" font-weight="400" fill="#4A5568">More options, less commitment</text>

  <defs>
    <marker id="axis-arrow" markerWidth="8" markerHeight="6" refX="8" refY="3" orient="auto" markerUnits="userSpaceOnUse">
      <polygon points="0 0, 8 3, 0 6" fill="#3D5A80"/>
    </marker>
  </defs>

  <!-- Axes with arrows -->
  <line x1="110" y1="400" x2="840" y2="400" stroke="#3D5A80" stroke-width="1.5" marker-end="url(#axis-arrow)"/>
  <line x1="110" y1="400" x2="110" y2="120" stroke="#3D5A80" stroke-width="1.5" marker-end="url(#axis-arrow)"/>

  <!-- Body: 13px/400 -->
  <text x="475" y="455" text-anchor="middle" font-size="13" font-weight="400" fill="#4A5568">Number of Alternatives</text>
  <text x="40" y="260" text-anchor="middle" font-size="13" font-weight="400" fill="#4A5568" transform="rotate(-90, 40, 260)">Satisfaction / Commitment</text>

  <!-- Ticks: Body 13px/400 -->
  <line x1="150" y1="400" x2="150" y2="406" stroke="#3D5A80" stroke-width="1.5"/>
  <text x="150" y="422" text-anchor="middle" font-size="13" font-weight="400" fill="#4A5568">1</text>
  <line x1="240" y1="400" x2="240" y2="406" stroke="#3D5A80" stroke-width="1.5"/>
  <text x="240" y="422" text-anchor="middle" font-size="13" font-weight="400" fill="#4A5568">3</text>
  <line x1="330" y1="400" x2="330" y2="406" stroke="#3D5A80" stroke-width="1.5"/>
  <text x="330" y="422" text-anchor="middle" font-size="13" font-weight="400" fill="#4A5568">5</text>
  <line x1="460" y1="400" x2="460" y2="406" stroke="#3D5A80" stroke-width="1.5"/>
  <text x="460" y="422" text-anchor="middle" font-size="13" font-weight="400" fill="#4A5568">10</text>
  <line x1="600" y1="400" x2="600" y2="406" stroke="#3D5A80" stroke-width="1.5"/>
  <text x="600" y="422" text-anchor="middle" font-size="13" font-weight="400" fill="#4A5568">20</text>
  <line x1="730" y1="400" x2="730" y2="406" stroke="#3D5A80" stroke-width="1.5"/>
  <text x="730" y="422" text-anchor="middle" font-size="13" font-weight="400" fill="#4A5568">50</text>
  <text x="820" y="422" text-anchor="middle" font-size="13" font-weight="400" fill="#4A5568">&#x221E;</text>

  <!-- Fill under curve -->
  <path d="M 150,340 C 170,300 200,175 240,168 C 280,161 340,195 420,255 C 500,310 600,350 700,368 C 760,375 800,380 820,382 L 820,400 L 150,400 Z"
        fill="#1B2A4A" fill-opacity="0.07" stroke="none"/>

  <!-- Danger zone fill -->
  <path d="M 420,255 C 500,310 600,350 700,368 C 760,375 800,380 820,382 L 820,400 L 420,400 Z"
        fill="#E8758A" fill-opacity="0.06" stroke="none"/>

  <!-- The curve -->
  <path d="M 150,340 C 170,300 200,175 240,168 C 280,161 340,195 420,255 C 500,310 600,350 700,368 C 760,375 800,380 820,382"
        fill="none" stroke="#1B2A4A" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>

  <!-- Sweet spot label inside the peak area: Label 13px/600 -->
  <text x="240" y="300" text-anchor="middle" font-size="13" font-weight="400" fill="#1B2A4A" opacity="0.3">sweet spot</text>

  <!-- ============ CHARACTER 1: HAPPY JUMPER ============ -->
  <!-- Place at x=300 where curve ≈ y=185. 
       Figure translate_y=155: head top=155-25=130, feet=155+18=173. 
       Gap from curve (185): 12px. Good.
       Bubble: bottom at 118, tail tip at 128. Head top at 130. Gap=2px... still tight.
       Move bubble up: top=68, bottom=108, tail=118. Head top=130. Gap=12px. Good. -->

  <!-- Speech bubble 1: top=68, height=50, bottom=118. 
       Text at 89, 103. Top pad: 89-8-68=13. Bottom pad: 118-103-3=12. Equal. -->
  <rect x="140" y="68" width="180" height="50" rx="12" fill="#FFFFFF" stroke="#1B2A4A" stroke-width="1.2"/>
  <polygon points="295,118 305,128 305,118" fill="#FFFFFF" stroke="#FFFFFF" stroke-width="1"/>
  <line x1="295" y1="118" x2="305" y2="128" stroke="#1B2A4A" stroke-width="1.2"/>
  <line x1="305" y1="118" x2="305" y2="128" stroke="#1B2A4A" stroke-width="1.2"/>
  <text x="230" y="89" text-anchor="middle" font-size="11" font-weight="400" font-style="italic" fill="#1B2A4A">"I didn't know a product for</text>
  <text x="230" y="103" text-anchor="middle" font-size="11" font-weight="400" font-style="italic" fill="#1B2A4A">this problem even existed!"</text>

  <!-- Figure at x=230: translate(230, 148). Head top=148-25=123. Tail tip=118. Gap=5px.
       Feet=148+18=166. Curve at x=230 ≈ 170. Gap=4px. Tight but no overlap. 
       Better: translate(230, 150). Head top=125. Gap from tail=7px. Feet=168. Curve≈170. Gap=2px.
       Even better: use x=280 where curve≈178. translate(280, 150). Feet=168. Curve=178. Gap=10px. -->
  <!-- Figure: translate(280, 160). Head top=160-25=135. Tail tip=128. Gap=7px.
       Feet=160+18=178. Curve at x=280 ≈ 178. Move to x=310 where curve ≈ 188. Gap=10px. -->
  <g transform="translate(310, 160)">
    <circle cx="0" cy="-18" r="7" fill="none" stroke="#1B2A4A" stroke-width="1.5"/>
    <line x1="0" y1="-11" x2="0" y2="8" stroke="#1B2A4A" stroke-width="1.5"/>
    <line x1="0" y1="-4" x2="-10" y2="-16" stroke="#1B2A4A" stroke-width="1.5" stroke-linecap="round"/>
    <line x1="0" y1="-4" x2="10" y2="-16" stroke="#1B2A4A" stroke-width="1.5" stroke-linecap="round"/>
    <line x1="0" y1="8" x2="-7" y2="18" stroke="#1B2A4A" stroke-width="1.5" stroke-linecap="round"/>
    <line x1="0" y1="8" x2="7" y2="18" stroke="#1B2A4A" stroke-width="1.5" stroke-linecap="round"/>
    <path d="M -3,-15 Q 0,-12 3,-15" fill="none" stroke="#1B2A4A" stroke-width="1" stroke-linecap="round"/>
  </g>

  <!-- ============ CHARACTER 2: THINKING (x=500) ============ -->
  <!-- Curve at x=500 ≈ y=310. -->

  <!-- Speech bubble 2: top=180, height=50, bottom=230.
       Text at 201, 215. Top pad: 201-8-180=13. Bottom pad: 230-215-3=12. Equal. -->
  <rect x="410" y="180" width="180" height="50" rx="12" fill="#FFFFFF" stroke="#3D5A80" stroke-width="1.2"/>
  <polygon points="495,230 500,240 505,230" fill="#FFFFFF" stroke="#FFFFFF" stroke-width="1"/>
  <line x1="495" y1="230" x2="500" y2="240" stroke="#3D5A80" stroke-width="1.2"/>
  <line x1="505" y1="230" x2="500" y2="240" stroke="#3D5A80" stroke-width="1.2"/>
  <text x="500" y="201" text-anchor="middle" font-size="11" font-weight="400" font-style="italic" fill="#3D5A80">"Let's evaluate which option</text>
  <text x="500" y="215" text-anchor="middle" font-size="11" font-weight="400" font-style="italic" fill="#3D5A80">is the best for us."</text>

  <!-- Figure: translate(500, 272). Head top=272-25=247. Tail=240. Gap=7px.
       Feet=272+18=290. Curve at x=500≈310. Gap=20px. Good. -->
  <g transform="translate(500, 272)">
    <circle cx="0" cy="-18" r="7" fill="none" stroke="#3D5A80" stroke-width="1.5"/>
    <line x1="0" y1="-11" x2="0" y2="8" stroke="#3D5A80" stroke-width="1.5"/>
    <line x1="0" y1="-2" x2="-10" y2="5" stroke="#3D5A80" stroke-width="1.5" stroke-linecap="round"/>
    <line x1="0" y1="-2" x2="8" y2="-10" stroke="#3D5A80" stroke-width="1.5" stroke-linecap="round"/>
    <line x1="0" y1="8" x2="-6" y2="20" stroke="#3D5A80" stroke-width="1.5" stroke-linecap="round"/>
    <line x1="0" y1="8" x2="6" y2="20" stroke="#3D5A80" stroke-width="1.5" stroke-linecap="round"/>
  </g>

  <!-- ============ CHARACTER 3: RUNNING AWAY (x=790) ============ -->
  <!-- Curve at x=790 ≈ y=378. -->

  <!-- Speech bubble 3: top=250, height=63, bottom=313.
       Text at 270, 284, 298. Top pad: 270-8-250=12. Bottom pad: 313-298-3=12. Equal. -->
  <rect x="635" y="250" width="220" height="63" rx="12" fill="#FFFFFF" stroke="#E8758A" stroke-width="1.2"/>
  <polygon points="770,313 775,323 780,313" fill="#FFFFFF" stroke="#FFFFFF" stroke-width="1"/>
  <line x1="770" y1="313" x2="775" y2="323" stroke="#E8758A" stroke-width="1.2"/>
  <line x1="780" y1="313" x2="775" y2="323" stroke="#E8758A" stroke-width="1.2"/>
  <text x="745" y="270" text-anchor="middle" font-size="11" font-weight="400" font-style="italic" fill="#E8758A">"I don't want to settle. Let's build</text>
  <text x="745" y="284" text-anchor="middle" font-size="11" font-weight="400" font-style="italic" fill="#E8758A">our own version in-house because</text>
  <text x="745" y="298" text-anchor="middle" font-size="11" font-weight="400" font-style="italic" fill="#E8758A">nothing fits perfectly."</text>

  <!-- Figure: translate(790, 356). Head top=356-25=331. Tail=323. Gap=8px.
       Feet=356+18=374. Curve at x=790≈378. Gap=4px. OK. -->
  <g transform="translate(790, 356)">
    <circle cx="5" cy="-18" r="7" fill="none" stroke="#E8758A" stroke-width="1.5"/>
    <line x1="5" y1="-11" x2="10" y2="8" stroke="#E8758A" stroke-width="1.5"/>
    <line x1="7" y1="-2" x2="20" y2="-8" stroke="#E8758A" stroke-width="1.5" stroke-linecap="round"/>
    <line x1="7" y1="-2" x2="-6" y2="6" stroke="#E8758A" stroke-width="1.5" stroke-linecap="round"/>
    <line x1="10" y1="8" x2="22" y2="16" stroke="#E8758A" stroke-width="1.5" stroke-linecap="round"/>
    <line x1="10" y1="8" x2="-2" y2="20" stroke="#E8758A" stroke-width="1.5" stroke-linecap="round"/>
    <line x1="-10" y1="-14" x2="-22" y2="-14" stroke="#E8758A" stroke-width="1" stroke-linecap="round" opacity="0.5"/>
    <line x1="-8" y1="-4" x2="-20" y2="-4" stroke="#E8758A" stroke-width="1" stroke-linecap="round" opacity="0.5"/>
    <line x1="-6" y1="6" x2="-18" y2="6" stroke="#E8758A" stroke-width="1" stroke-linecap="round" opacity="0.5"/>
  </g>

  <!-- ============ BEHAVIORAL ECONOMICS ANNOTATIONS ============ -->

  <line x1="60" y1="480" x2="880" y2="480" stroke="#D4CDC3" stroke-width="0.5" stroke-dasharray="4,4"/>

  <!-- Label: 13px/600. Small: 11px/400 -->
  <circle cx="80" cy="507" r="4" fill="#3D5A80"/>
  <text x="92" y="505" font-size="13" font-weight="600" fill="#1B2A4A">Decision fatigue</text>
  <text x="92" y="520" font-size="11" font-weight="400" fill="#4A5568">Baumeister (2011): willpower depletes.</text>
  <text x="92" y="535" font-size="11" font-weight="400" fill="#4A5568">After enough comparisons, people do nothing.</text>

  <circle cx="350" cy="507" r="4" fill="#1B2A4A"/>
  <text x="362" y="505" font-size="13" font-weight="600" fill="#1B2A4A">Choice overload</text>
  <text x="362" y="520" font-size="11" font-weight="400" fill="#4A5568">Iyengar &amp; Lepper (2000): shoppers shown</text>
  <text x="362" y="535" font-size="11" font-weight="400" fill="#4A5568">24 jams were 10x less likely to buy than 6.</text>

  <circle cx="620" cy="507" r="4" fill="#E8758A"/>
  <text x="632" y="505" font-size="13" font-weight="600" fill="#1B2A4A">Maximizer's dilemma</text>
  <text x="632" y="520" font-size="11" font-weight="400" fill="#4A5568">Schwartz (2002): "maximizers" who seek</text>
  <text x="632" y="535" font-size="11" font-weight="400" fill="#4A5568">the best report 40% less satisfaction.</text>

  <!-- Watermark: 9px/400 -->
  <text x="960" y="600" text-anchor="end" font-size="9" font-weight="400" fill="#4A5568" opacity="0.4">Made with github.com/tizkovatereza/growth-agents and Factory AI</text>
</svg>

<img width="980" height="620" alt="chart2-paradox-of-choice" src="https://github.com/user-attachments/assets/00246997-23f3-49d6-a303-a09c3472dd8d" />


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
