# Hi, I'm Gregg Chen

I help teams get from knowing about AI to using it in real work: agentic workflows, MCP connectors and agent skills, built in the open. Twenty-plus years in enterprise software, including SAP SuccessFactors.

Notes, demos and the portfolio: [gcartifacts.com](https://gcartifacts.com) · [LinkedIn](https://www.linkedin.com/in/greggchen)

## Three things I've built

**Yahoo Mail into my AI chief of staff**
Problem: Yahoo was the one inbox my agent couldn't see, so a changed meeting or a request for a decision stayed invisible until I opened the mailbox myself.
Build: n8n on a small home server reads Yahoo over IMAP, exposes search, preview and save-draft tools over MCP, and sends alerts to my agent chat. Designed and verified by me, built with ChatGPT's help.
Outcome: in a failure drill, seven reconnect attempts failed and the two messages that arrived meanwhile were each stored exactly once on recovery. A live test email was flagged in my chat within about a quarter hour, and all 18 messages checked matched one stored record each. [Write-up](https://gist.github.com/greggchen308/568f30fb3e7ea81f24d9ec2a8a4d9226)

**A safer way for an agent to use my notes**
Problem: an agent with a full-scope notes token can overwrite or corrupt a vault.
Build: [`siyuan-mcp`](https://github.com/greggchen308/workbuddy), a local MCP server for Tencent WorkBuddy. Reads are open, writes are limited to a reviewed allowlist, protected areas are hard-blocked.
Outcome: every write is read back and verified, and a write that returns corrupted is reported as a failure, not a success.

**A shared toolkit of agent skills**
Problem: the same media and reporting tasks kept getting re-explained to each agent.
Build: [`gc-skills`](https://github.com/greggchen308/gc-skills), five skills (image generation, video generation, video trim, speech-to-text, a WorkBuddy usage retrospective), each a SKILL.md runbook plus standard-library Python helpers.
Outcome: written for Claude Code, WorkBuddy and OpenClaw; the usage retrospective labels every claim as data, rule or judgement so the report shows its evidence.

## Sharing

- [AI governance briefing](https://github.com/greggchen308/AI_Governance): a slide deck on responsible AI, regulation, security and privacy for enterprise teams.
- [Community AI session, May 2026](https://github.com/greggchen308/AI-At-HV-Cuppa-2605): slides on privacy controls across AI tools and building your own Gemini Gem.

## Working with

Claude Code · ChatGPT Codex · MCP · n8n · agent skills (SKILL.md) · WorkBuddy · OpenClaw · Python · Node.js
