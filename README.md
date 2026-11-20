# QA Verifier

**English** | [Português (Brasil)](README.pt-BR.md)

An agent skill for **skeptical functional verification and QA**: it confirms, with evidence, that a change actually works.

It discovers the project's lint/typecheck/test/build commands (instructions, CI, scripts), runs them, designs test cases and delivers a report with a verdict.

It prioritizes verifying and reporting; it only makes minimal fixes when a blocker is clear or when asked.

It follows the open [Agent Skills](https://agentskills.io) format (`SKILL.md` with `name` and `description` frontmatter) and works with Claude Code, Cursor and other compatible agents. The skill instructions are written in Brazilian Portuguese.

## Installation

The target folder must be named `qa-verifier` (the skill name), not the repository name.

### Claude Code

```bash
# All projects
git clone https://github.com/jrcarls/skill-qa-verifier.git ~/.claude/skills/qa-verifier

# A single project
git clone https://github.com/jrcarls/skill-qa-verifier.git .claude/skills/qa-verifier
```

### Cursor

```bash
git clone https://github.com/jrcarls/skill-qa-verifier.git .cursor/skills/qa-verifier
```

## Usage

The agent loads the skill automatically when the task matches its description. To invoke it explicitly in Claude Code:

```text
/qa-verifier
```

## Related skills

This skill is part of a complementary set:

- `skill-owasp-security-reviewer` — OWASP Top 10
- `skill-llm-security-reviewer` — OWASP LLM Top 10
- `skill-tenant-isolation-reviewer` — IDOR / ownership
- `skill-lgpd-compliance-advisor` — LGPD compliance
- `skill-qa-verifier` — functional verification
- `skill-vue-reviewer` — Vue frontend review

## License

[MIT](LICENSE)
