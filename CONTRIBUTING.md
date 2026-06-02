# Contributing

Thanks for helping improve Frontend Polish.

The most useful contributions are practical:

- real prompts that should trigger the skill
- before/after screenshots from frontend polish work
- examples where the skill produced too much decoration or too little structure
- framework-specific guidance for React, Vue, Tailwind CSS, CSS modules, or plain HTML/CSS
- clearer playbook rules for dashboards, auth flows, landing pages, ecommerce, and components

## Guidelines

- Keep `skills/frontend-polish/SKILL.md` concise and operational.
- Put detailed examples in `skills/frontend-polish/references/call-examples.md`.
- Put deeper design guidance in `skills/frontend-polish/references/polish-playbook.md`.
- Preserve the core rule: keep product logic and information architecture intact unless the user explicitly asks for a deeper redesign.
- Avoid adding trend-specific styling rules that will age quickly.

## Local Validation

If you have Codex skill validation tools available, run them against:

```bash
skills/frontend-polish
```

At minimum, check that `SKILL.md` has valid YAML frontmatter with `name` and `description`.
