# Claude Code Configuration

My Claude Code skills and MCP configs. Syncs across machines.

## Skills

- **using-superpowers** — meta-skill: 1% rule, skill discovery protocol (from [obra/superpowers](https://github.com/obra/superpowers))
- **brainstorming** — interactive requirement refinement before coding (from [obra/superpowers](https://github.com/obra/superpowers))
- **obsidian-skills** — 5 sub-skills: markdown, bases, canvas, cli, defuddle (from [kepano/obsidian-skills](https://github.com/kepano/obsidian-skills))
- **skill-creator** — create custom skills (from [anthropics/skills](https://github.com/anthropics/skills))
- **playwright-skill** — browser automation for testing (from [lackeyjb/playwright-skill](https://github.com/lackeyjb/playwright-skill))
- **markitdown** — convert documents to Markdown (from [microsoft/markitdown](https://github.com/microsoft/markitdown))

## MCP Servers

- Brave Search
- Fetch (web content)
- Screenshot
- Playwright (browser automation)

## Setup

```bash
# Clone this repo
git clone https://github.com/huang860517-cell/claude-config.git

# Copy skills
cp -r skills ~/.claude/

# Copy MCP config (edit API keys first!)
cp mcp.template.json ~/.claude/mcp.json
# Edit ~/.claude/mcp.json and add your BRAVE_API_KEY

# Install Python deps for markitdown
pip install markitdown
```
