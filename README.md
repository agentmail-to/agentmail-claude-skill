# AgentMail Claude Skill

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

A [Claude Skill](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/claude-skill) that teaches Claude how to build email agents using the [AgentMail](https://agentmail.to) API.

Drop this into Claude Code, Cursor, or any Claude-powered coding tool and it instantly knows how to work with AgentMail — create inboxes, send emails, set up webhooks, build full email agent workflows.

## What's Inside

```
agentmail-claude-skill/
├── SKILL.md              # Core skill file — everything Claude needs to know
└── references/
    ├── api-reference.md  # Complete API method signatures
    ├── webhook-events.md # Webhook event types and payloads
    └── examples.md       # Advanced agent patterns and recipes
```

### SKILL.md Covers

- **Quick start** — installation, initialization, sending your first email
- **Resource hierarchy** — Organization → Pod → Inbox → Thread → Message
- **Common workflows** — send, reply, webhooks, websockets, attachments
- **Framework integration** — using agentmail-toolkit with OpenAI, Vercel AI SDK, and MCP
- **Best practices** — idempotency, deliverability, error handling
- **Critical gotchas** — things that trip up first-time users

### Reference Files

- **api-reference.md** — every API method with parameters and return types
- **webhook-events.md** — all webhook event types, payloads, and setup
- **examples.md** — production agent patterns (sales agent, support agent, multi-agent systems)

## Usage

### Claude Code

```bash
# Add to your project
cp -r agentmail-claude-skill/.claude/skills/ .claude/skills/
```

### Cursor

Add the skill content to your `.cursorrules` or project instructions.

### Manual

Copy `SKILL.md` into your system prompt or project context when working with Claude on email agent features.

## Example

Once the skill is loaded, you can ask Claude:

- *"Build me an email agent that monitors an inbox and auto-replies to support questions"*
- *"Set up webhooks to get real-time notifications when my agent receives email"*
- *"Create a sales outreach agent that sends personalized emails and tracks replies"*

Claude will generate working code using the AgentMail SDK with correct patterns and best practices.

## Links

- [AgentMail Website](https://agentmail.to)
- [API Documentation](https://docs.agentmail.to)
- [AgentMail Toolkit](https://github.com/agentmail-to/agentmail-toolkit)
- [Examples](https://github.com/agentmail-to/agentmail-examples)
- [MCP Server](https://github.com/agentmail-to/agentmail-mcp)

## License

MIT
