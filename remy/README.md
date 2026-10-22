# Remy skills for outside agents

These are the skills that ship inside the Remy Framer project (Site Settings → Skills), written for AI agents that work on Framer from outside the editor: Claude, Claude Code, ChatGPT, Codex, Cursor and others. They do the same jobs as the skills inside Framer. Inside the Framer editor, use the project's own skills instead: they link straight to Remy's pages, components and styles.

Live preview of the template: https://remytemplate.framer.website

## 1. Connect your agent to Framer

Use Framer MCP, Framer's official way to connect AI tools (https://www.framer.com/mcp/). It runs on Framer's servers, so there's nothing to install: you sign in to Framer in your browser and approve access.

- Open https://www.framer.com/mcp/ and choose the button for your app: Add to Claude, Add to Claude Code, Add to ChatGPT, Add to Codex or Add to Cursor. Sign in to Framer and approve access in the tab that opens.
- Codex can also add it from the terminal: codex mcp add framer --url https://mcp.framer.com/mcp
- Claude Code needs a new session once Framer is added.
- Any other app that supports remote MCP servers with sign-in: add the server https://mcp.framer.com/mcp.

Framer's install guide covers each app: https://www.framer.com/help/articles/getting-started-with-framer-mcp/

Then give your agent the link to your Remy project. Once it's connected, it also gets the skills saved in your Framer project. These files are the same skills for tools that read their own skill files; if the two ever differ, the one in your Framer project wins.

## 2. Add the skills

Each folder in skills/ holds one skill, as a SKILL.md file. Add all ten, so they can hand work to each other. remy-base holds the rules every other skill relies on.

- Claude Code: copy the ten folders from skills/ into ~/.claude/skills (for all your projects) or into .claude/skills inside a project folder.
- Claude (the app): the app takes one skill per upload. The claude-app folder has a ready ZIP for each skill. Turn on "Code execution and file creation" in Settings → Capabilities, then go to Customize → Skills, click +, then Create skill, then Upload a skill, and upload each ZIP.
- Codex: copy the ten folders from skills/ into ~/.agents/skills.
- ChatGPT: standalone skills work in the ChatGPT desktop app (Skills in the sidebar). Elsewhere, attach remy-base and the skill you need to your chat.
- Cursor and other tools that read SKILL.md files: add the folders wherever your tool reads skills.

## 3. Use them

Ask in plain words ("make this template mine") or call a skill by name: /remy-make-it-yours in Claude Code, $remy-make-it-yours in Codex.

| Skill | What it does |
|---|---|
| remy-base | The rules for every Remy task, and how to connect to Framer |
| remy-make-it-yours | Puts your name, details, portrait and links in place of the sample designer |
| remy-add-case-study | Adds a case study to the Work collection |
| remy-add-post | Adds a blog post to the Blog collection |
| remy-change-home-projects | Chooses how many projects Home shows (3, 4 or 5) and which ones |
| remy-design-system | Builds or changes pages and sections in Remy's style |
| remy-remove-ai-writing | Finds and fixes copy that sounds generic or machine-written |
| remy-seo-check | Checks one page's on-page SEO, without changing anything |
| remy-accessibility-check | Checks pages for accessibility, without changing anything |
| remy-launch-check | Reviews the whole site before launch, without changing anything |

## Sample content

Remy ships with sample content so the template shows how it works: five case studies (Halden, Ostra, Fieldnote, Kiln Week and Tern), six blog posts, four services, and a sample designer, Remy Varga, with a portrait. Replace or delete all of it before you launch. remy-make-it-yours, remy-add-case-study and remy-add-post do this, and remy-launch-check lists anything left.

## Good to know

- Your agent never publishes. You review the changes and publish yourself.
- Framer MCP changes your project directly. Before a big change, such as a new page or many CMS items, the agent offers to work on a branch (you review it in Framer and merge it) or on a duplicate of the project.
- If your tools can't change something, such as where the contact form sends messages, the agent tells you the steps instead.
- Framer MCP doesn't handle localization yet. Remy is English only, so this doesn't affect it.
