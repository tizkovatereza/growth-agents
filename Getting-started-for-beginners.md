# Getting Started (for beginners)

Don't worry if you've never used a terminal before. This guide walks you through everything step by step. Nothing here can break your computer.

## What is this?

These are AI assistants that live on your computer. You talk to them by typing, and they do real work for you: write article drafts, create charts, give you feedback on your writing.

Think of it like ChatGPT, but instead of just talking, these agents can actually create files, edit your documents, and save things to your computer.

## What you need

- A Mac, Windows, or Linux computer
- An internet connection
- A Factory account (starts at $20/month)
- About 10 minutes

## Step 1: Open the Terminal

The terminal is just a text-based way to talk to your computer. It looks scary but it's just a blank screen where you type commands.

**On Mac:**
- Press `Cmd + Space` to open Spotlight
- Type `Terminal`
- Press Enter

You'll see something like this:

```
terezas-macbook ~ %
```

That blinking cursor is waiting for you to type something. That's it. You're in.

**On Windows:**
- Press `Win + R`
- Type `cmd`
- Press Enter

## Step 2: Create a Factory account

1. Open your browser and go to [factory.ai](https://factory.ai)
2. Click "Sign up" and create an account
3. Pick the Pro plan ($20/month) -- this gives you access to all the AI models

## Step 3: Install Factory on your computer

Go back to your terminal and paste this line:

```bash
curl -fsSL https://app.factory.ai/install.sh | sh
```

Press Enter. Wait about 30 seconds. You'll see some text scroll by. When it's done, you'll see your cursor again.

To check it worked, type:

```bash
droid --version
```

You should see a version number. If you do, it worked.

## Step 4: Log in

Type this in the terminal:

```bash
droid
```

It will ask you to log in. Follow the instructions on screen -- it will open your browser and ask you to confirm.

## Step 5: Install the growth agents

Now we need to download the agents and put them in the right folder. Type these commands one at a time:

```bash
git clone https://github.com/tizkovatereza/growth-agents.git
```

This downloads the agents to your computer.

```bash
mkdir -p ~/.factory/droids
```

This creates the folder where Factory looks for custom agents. (If it already exists, nothing happens. No harm done.)

```bash
cp growth-agents/*.md ~/.factory/droids/
```

This copies the agent files into that folder.

## Step 6: Use an agent

To start the writing coach:

```bash
droid writing-coach-style-preserving-finisher
```

A chat session will open. Just paste your article draft and start talking to it. It will give you feedback, fix your grammar, suggest titles, and push you to finish.

To start the chart maker:

```bash
droid chart-maker-formal-svg
```

Tell it what kind of chart you want (e.g., "make a pie chart showing 70% blue and 30% red with labels") and it will create an SVG file on your computer.

## Common questions

**"I got an error. What do I do?"**

Copy the error message, open a new `droid` session, and paste it. Ask "what does this error mean and how do I fix it?" The AI will help you debug it.

**"Where do my files go?"**

By default, charts and other files are saved to your Desktop or wherever you tell the agent to save them.

**"Can I use the desktop app instead of the terminal?"**

Yes. Factory has a desktop app. Download it from [factory.ai](https://factory.ai). The agents work the same way in both.

**"What if I mess something up?"**

You can't break anything. The agents only create and edit files you ask them to. They don't touch anything else on your computer.

**"Do I need to know how to code?"**

No. You just type in plain English. The agents handle everything else.

## Still stuck?

Join the [Factory Discord](https://discord.gg/zuudFXxg69) and ask for help. The community is friendly.
