# QA Verifier

[English](README.md) | **Português (Brasil)**

Skill de agente para **verificação funcional e QA cético**: confirma com evidência que uma mudança realmente funciona.

Descobre os comandos de lint/typecheck/teste/build do projeto (instruções, CI, scripts), executa, desenha casos de teste e entrega um relatório com veredito.

A skill prioriza verificar e reportar; só faz correções mínimas quando o bloqueio é claro ou quando solicitado.

Segue o formato aberto de [Agent Skills](https://agentskills.io) (`SKILL.md` com frontmatter `name` e `description`) e funciona no Claude Code, Cursor e outros agentes compatíveis.

## Instalação

A pasta de destino deve se chamar `qa-verifier` (o nome da skill), não o nome do repositório.

### Claude Code

```bash
# Para todos os projetos
git clone https://github.com/jrcarls/skill-qa-verifier.git ~/.claude/skills/qa-verifier

# Apenas para um projeto
git clone https://github.com/jrcarls/skill-qa-verifier.git .claude/skills/qa-verifier
```

### Cursor

```bash
git clone https://github.com/jrcarls/skill-qa-verifier.git .cursor/skills/qa-verifier
```

## Uso

O agente carrega a skill automaticamente quando a tarefa combina com a descrição. Para chamar explicitamente no Claude Code:

```text
/qa-verifier
```

## Skills relacionadas

Esta skill faz parte de um conjunto que se complementa:

- `skill-owasp-security-reviewer` — OWASP Top 10
- `skill-llm-security-reviewer` — OWASP LLM Top 10
- `skill-tenant-isolation-reviewer` — IDOR / ownership
- `skill-lgpd-compliance-advisor` — conformidade LGPD
- `skill-qa-verifier` — verificação funcional
- `skill-vue-reviewer` — revisão de frontend Vue

## Licença

[MIT](LICENSE)
